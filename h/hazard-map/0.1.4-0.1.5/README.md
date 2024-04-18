# Comparing `tmp/hazard_map-0.1.4.tar.gz` & `tmp/hazard_map-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.1.4.tar", max compression
+gzip compressed data, was "hazard_map-0.1.5.tar", max compression
```

## Comparing `hazard_map-0.1.4.tar` & `hazard_map-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11942 2024-04-17 15:32:55.142166 hazard_map-0.1.4/hazard_map/hazard_map.py
--rw-r--r--   0        0        0     2084 2024-04-17 15:34:02.975187 hazard_map-0.1.4/hazard_map/main.py
--rw-r--r--   0        0        0      587 2024-04-17 15:34:34.064200 hazard_map-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2603 2024-04-17 14:33:44.391269 hazard_map-0.1.4/readme.md
--rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 hazard_map-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    12362 2024-04-18 09:58:22.836511 hazard_map-0.1.5/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0     2245 2024-04-18 09:57:23.395260 hazard_map-0.1.5/hazard_map/main.py
+-rw-r--r--   0        0        0      587 2024-04-18 10:06:04.289025 hazard_map-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2656 2024-04-17 15:54:42.739575 hazard_map-0.1.5/readme.md
+-rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 hazard_map-0.1.5/PKG-INFO
```

### Comparing `hazard_map-0.1.4/hazard_map/hazard_map.py` & `hazard_map-0.1.5/hazard_map/hazard_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,24 +86,24 @@
         workbook_filename = os.path.basename(workbook_path)
         workbook_name, workbook_filetype = os.path.splitext(workbook_filename)
         if workbook_filetype == '.xlsx': 
             return workbook_name
         else:
             raise Exception('Please upload an xlsx file')
 
-    def extract_sheet_mappings(self, sheets: list[Sheet]):
+    def extract_sheet_mappings(self, sheets: list[Sheet], custom_mapping_regex: str=None):
         '''Extract hazard-cause and cause-control mappings from the matrices in the workbook.'''
         for sheet in sheets:
             df = pd.read_excel(self.WORKBOOK_PATH, sheet.name, header=None, index_col=None)
 
             # transform the sheet as appropriate
             if sheet.transpose: df = df.T
             df = self._extract_clean_mappings(df, sheet)
 
-            df.apply(self._extract_individual_mappings, axis=1)
+            df.apply(self._extract_individual_mappings, axis=1, args=[custom_mapping_regex])
 
     def _extract_clean_mappings(self, df: pd.DataFrame, sheet: Sheet) -> pd.DataFrame:
         '''Extract a clean table of mappings from the raw worksheet.'''
         # find out what size the mapping table is (i.e. how many pairs are in the table)
         def find_list_length(s: pd.Series) -> int:
             for i, item in enumerate(s): 
                 if item in [0, np.nan, '']: break
@@ -124,27 +124,33 @@
         # reduce the dataframe to only the mappings on the sheet
         df = df.iloc[
             sheet.mapping_table_location[1]:sheet.mapping_table_location[1]+table_dimensions[1], 
             sheet.mapping_table_location[0]:sheet.mapping_table_location[0]+table_dimensions[0],
         ]
         return df
 
-    def _extract_individual_mappings(self, row: pd.Series):
+    def _extract_individual_mappings(self, row: pd.Series, custom_mapping_regex: str=None):
         '''Extract meaningful mappings from the clean table discerned from the worksheet.'''
         map_from = Node.from_str(row.name)
 
         row = row.dropna()
-        mapped = row[row.str.match(MAPPING_MATCHER)].index.str.strip().to_list()
+        mapped = row[row.str.match(
+            MAPPING_MATCHER if not custom_mapping_regex else custom_mapping_regex
+        )].index.str.strip().to_list()
         mapped_typed = [Node.from_str(node_str) for node_str in mapped]
         
         for map_to in mapped_typed: 
             self.graph.add_edge(map_from, map_to)
 
-    def write_to_file(self, output_directory: str, output_json: bool=False) -> str:
+    def write_to_file(self, output_directory: str, output_json: bool=False):
         '''Save the extracted mappings as a reformatted Excel workbook (and json if requested).'''
+        if nx.is_empty(self.graph):
+            print('The graph is empty - there\'s no hazard log to save.')
+            return
+        
         if not os.path.exists(output_directory): os.mkdir(output_directory)
         output_file = os.path.join(output_directory, f'{self.WORKBOOK_NAME}-hazard_log.xlsx')
 
         with pd.ExcelWriter(output_file) as writer:
             for hazard in self.filter_node_set_for_kind(
                 self.graph.nodes, 
                 Kind.HAZARD,
@@ -216,14 +222,16 @@
         '''Draw a colourful graph of network.'''
         self.fig, self.ax = plt.subplots(
             frameon=False,
             figsize=(9, 7),
             dpi=DEFAULT_RENDERING_DPI if not custom_dpi else custom_dpi,
         )
         self.ax.axis('off')
+
+        if nx.is_empty(self.graph): return
     
         nx.draw_networkx(
             self.graph,
             pos=nx.kamada_kawai_layout(self.graph),
             node_color=[
                 KIND_COLOURS.get(node.kind, '#53676c') 
                 for node in self.graph.nodes
@@ -252,29 +260,31 @@
             min([
                 size_limits[0] + add_size_per_connect*n_connections,
                 size_limits[1],
             ])
             for node, n_connections in degrees
         ]
 
-    def save_graph(self, output_directory: str, custom_dpi: int=None) -> str: 
+    def save_graph(self, output_directory: str, custom_dpi: int=None): 
         '''Save a graph of the network to a file.'''
         if not hasattr(self, 'fig'):
             self.draw_graph()
 
+        if nx.is_empty(self.graph): return
+
         if not os.path.exists(output_directory): os.mkdir(output_directory)
         output_file = os.path.join(output_directory, f'{self.WORKBOOK_NAME}-graph_rendering.png')
 
         plt.savefig(
             output_file, 
             transparent=True, 
             dpi=DEFAULT_RENDERING_DPI if not custom_dpi else custom_dpi,
         )
 
-        return os.path.basename(output_file)
+        print(f'Saved a plot of the network to "{os.path.basename(output_file)}".')
 
     def report_kind_counts(self) -> str:
         kind_count_report = 'The network consists of '
         all_kinds = [Kind.HAZARD, Kind.CAUSE, Kind.CONTROL]
 
         for i, kind in enumerate(all_kinds):
             if i < len(all_kinds) - 2:
```

### Comparing `hazard_map-0.1.4/hazard_map/main.py` & `hazard_map-0.1.5/hazard_map/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,31 +13,33 @@
     print(f'The outputs of this script will be saved in the following directory:')
     print(f'\"{arguments.output_directory}\"')
 
     print()
 
     hazard_log = HazardMap(arguments.input_workbook)
 
-    graph = hazard_log.extract_sheet_mappings([
-        Sheet('HazardCause Mapping', (0, 0), (1, 1), (2, 2), False),
-        Sheet('CauseControl Mapping', (0, 0), (1, 1), (2, 2), False),
-    ])
+    graph = hazard_log.extract_sheet_mappings(
+        [
+            Sheet('HazardCause Mapping', (0, 0), (1, 1), (2, 2), False),
+            Sheet('CauseControl Mapping', (0, 0), (1, 1), (2, 2), False),
+        ],
+        arguments.mapping_regex,
+    )
     print(f'Mappings were successfully extracted from the workbook "{arguments.input_workbook}"!')
     print(hazard_log.report_kind_counts())
 
     print()
 
     hazard_log_output_file = hazard_log.write_to_file(
         arguments.output_directory, 
         arguments.output_json,
     )
 
     hazard_log.draw_graph()
     plot_output_file = hazard_log.save_graph(arguments.output_directory, arguments.plot_dpi)
-    print(f'Saved a plot of the network to "{plot_output_file}".')
 
 def parse_arguments():
     '''Uses the argparse library to create a command-line interface for the script.'''
     parser = argparse.ArgumentParser(
         prog='hazard-map',
         description='Build and analyze a network model of hazards, causes, and controls',
     )
@@ -59,14 +61,21 @@
         help='Save a json description of the mappings alongside the hazard log',
         default=False,
         type=bool,
         action=argparse.BooleanOptionalAction,
     )
 
     parser.add_argument(
+        '-m', '--mapping-regex',
+        help='Set a custom regex for identifying mapping pairs',
+        default='',
+        type=str,
+    )
+
+    parser.add_argument(
         '-d', '--plot-dpi',
         help='Set a custom DPI (quality) for the plot output',
         default=None,
         type=int,
     )
 
     return parser.parse_args()
```

### Comparing `hazard_map-0.1.4/pyproject.toml` & `hazard_map-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hazard-map"
-version = "0.1.4"
+version = "0.1.5"
 description = "Build and analyze a network model of hazards, causes, and controls"
 authors = ["Thom Cameron <thomcm@proton.me>"]
 readme = "readme.md"
 license = "license.txt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `hazard_map-0.1.4/readme.md` & `hazard_map-0.1.5/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,27 +51,27 @@
 
 Pass an Excel workbook (xlsx) file with hazard-cause and cause-control mappings (indicated by a "Y" at the intersection of row/column pair that map onto one-another) in worksheets named "HazardCause Mapping" and "CauseControl Mapping" respectively:
 
 ``` fish
 hazard-map our_mappings.xlsx
 ```
 
-See the [test mappings](tests/test_mappings.xlsx) for an example of a compatible document.
+See the [test mappings](https://gitlab.com/thom-cameron/hazard-map/-/blob/main/tests/test_mappings.xlsx) for an example of a compatible document.
 
 Development
 -----------
 
 If you want to develop this project further or just set it up so you can modify the source code (to work with a different matrix format, for example), clone this repo:
 
 ``` fish
 git clone https://gitlab.com/thom-cameron/hazard-map
 cd hazard-map
 ```
 
-Packaging and dependency management for this project are handled with [poetry](https://python-poetry.org/). Install poetry, or, if you use [nix](https://nixos.org/), start up a shell with everything you need:
+Packaging and dependency management for this project are handled by [poetry](https://python-poetry.org/). Install poetry, or, if you use [nix](https://nixos.org/), start up a shell with everything you need:
 
 ``` fish
 nix-shell
 ```
 
 Then, get the code running:
```

### Comparing `hazard_map-0.1.4/PKG-INFO` & `hazard_map-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazard-map
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build and analyze a network model of hazards, causes, and controls
 License: license.txt
 Author: Thom Cameron
 Author-email: thomcm@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -72,27 +72,27 @@
 
 Pass an Excel workbook (xlsx) file with hazard-cause and cause-control mappings (indicated by a "Y" at the intersection of row/column pair that map onto one-another) in worksheets named "HazardCause Mapping" and "CauseControl Mapping" respectively:
 
 ``` fish
 hazard-map our_mappings.xlsx
 ```
 
-See the [test mappings](tests/test_mappings.xlsx) for an example of a compatible document.
+See the [test mappings](https://gitlab.com/thom-cameron/hazard-map/-/blob/main/tests/test_mappings.xlsx) for an example of a compatible document.
 
 Development
 -----------
 
 If you want to develop this project further or just set it up so you can modify the source code (to work with a different matrix format, for example), clone this repo:
 
 ``` fish
 git clone https://gitlab.com/thom-cameron/hazard-map
 cd hazard-map
 ```
 
-Packaging and dependency management for this project are handled with [poetry](https://python-poetry.org/). Install poetry, or, if you use [nix](https://nixos.org/), start up a shell with everything you need:
+Packaging and dependency management for this project are handled by [poetry](https://python-poetry.org/). Install poetry, or, if you use [nix](https://nixos.org/), start up a shell with everything you need:
 
 ``` fish
 nix-shell
 ```
 
 Then, get the code running:
```

