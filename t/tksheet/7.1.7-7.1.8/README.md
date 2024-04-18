# Comparing `tmp/tksheet-7.1.7.tar.gz` & `tmp/tksheet-7.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.1.7.tar", last modified: Thu Apr  4 19:00:53 2024, max compression
+gzip compressed data, was "tksheet-7.1.8.tar", last modified: Thu Apr 18 17:47:17 2024, max compression
```

## Comparing `tksheet-7.1.7.tar` & `tksheet-7.1.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.7/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-04 19:00:53.996107 tksheet-7.1.7/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.7/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-01 18:49:27.000000 tksheet-7.1.7/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-04 19:00:53.996107 tksheet-7.1.7/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     2010 2024-04-04 06:38:42.000000 tksheet-7.1.7/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    99870 2024-04-04 18:51:50.000000 tksheet-7.1.7/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    39612 2024-04-04 07:10:00.000000 tksheet-7.1.7/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      384 2024-04-04 18:57:38.000000 tksheet-7.1.7/tksheet/listbox.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   323154 2024-04-04 18:54:36.000000 tksheet-7.1.7/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13604 2024-03-30 16:31:45.000000 tksheet-7.1.7/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   105354 2024-04-04 18:51:54.000000 tksheet-7.1.7/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   256166 2024-04-04 14:40:53.000000 tksheet-7.1.7/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-04 14:40:28.000000 tksheet-7.1.7/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.7/tksheet/text_editor.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.7/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.7/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     2092 2024-03-23 14:39:32.000000 tksheet-7.1.7/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      500 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.832809 tksheet-7.1.8/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.8/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-18 17:47:17.832809 tksheet-7.1.8/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.8/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-09 11:49:17.000000 tksheet-7.1.8/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-18 17:47:17.832809 tksheet-7.1.8/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.828809 tksheet-7.1.8/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1994 2024-04-17 16:38:46.000000 tksheet-7.1.8/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   100204 2024-04-18 17:26:28.000000 tksheet-7.1.8/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    39709 2024-04-16 16:58:22.000000 tksheet-7.1.8/tksheet/functions.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   318290 2024-04-18 17:24:33.000000 tksheet-7.1.8/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-04-18 07:38:29.000000 tksheet-7.1.8/tksheet/other_classes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   105673 2024-04-18 17:25:32.000000 tksheet-7.1.8/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   257298 2024-04-18 17:34:24.000000 tksheet-7.1.8/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-04 14:40:28.000000 tksheet-7.1.8/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.8/tksheet/text_editor.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.8/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.8/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2288 2024-04-18 17:22:58.000000 tksheet-7.1.8/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.832809 tksheet-7.1.8/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.1.7/LICENSE.txt` & `tksheet-7.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/PKG-INFO` & `tksheet-7.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.7
+Version: 7.1.8
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `tksheet-7.1.7/README.md` & `tksheet-7.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/pyproject.toml` & `tksheet-7.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.1.7"
+version = "7.1.8"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.1.7/tksheet/__init__.py` & `tksheet-7.1.8/tksheet/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.1.7"
+__version__ = "7.1.8"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
@@ -31,38 +31,36 @@
     to_str,
     try_to_bool,
 )
 from .functions import (
     alpha2idx,
     alpha2num,
     consecutive_chunks,
+    consecutive_ranges,
     data_to_displayed_idxs,
     displayed_to_data_idxs,
     dropdown_search_function,
     event_dict,
     get_checkbox_dict,
     get_checkbox_kwargs,
-    rounded_box_coords,
     get_dropdown_dict,
     get_dropdown_kwargs,
     get_index_of_gap_in_sorted_integer_seq_forward,
     get_index_of_gap_in_sorted_integer_seq_reverse,
     get_n2a,
     get_new_indexes,
     get_seq_without_gaps_at_index,
     is_iterable,
     move_elements_by_mapping,
     move_elements_to,
     num2alpha,
+    rounded_box_coords,
     span_dict,
     tksheet_type_error,
 )
-from .listbox import (
-    ListBox,
-)
 from .main_table import MainTable
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DrawnItem,
     EventDataDict,
     GeneratedMouseEvent,
```

### Comparing `tksheet-7.1.7/tksheet/colors.py` & `tksheet-7.1.8/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/column_headers.py` & `tksheet-7.1.8/tksheet/column_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     color_map,
 )
 from .formatters import is_bool_like, try_to_bool
 from .functions import (
     consecutive_ranges,
     ev_stack_dict,
     event_dict,
-    rounded_box_coords,
     get_n2a,
     is_contiguous,
+    rounded_box_coords,
     try_binding,
 )
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DropdownStorage,
     TextEditorStorage,
@@ -37,14 +37,15 @@
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
     USER_OS,
     rc_binding,
     symbols_set,
+    text_editor_to_unbind,
 )
 
 
 class ColumnHeaders(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
@@ -938,15 +939,15 @@
         iid: None | int = None,
     ) -> int:
         coords = rounded_box_coords(
             x1,
             y1,
             x2,
             y2,
-            radius=9 if self.PAR.ops.rounded_boxes else 0,
+            radius=8 if self.PAR.ops.rounded_boxes else 0,
         )
         if isinstance(iid, int):
             self.coords(iid, coords)
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
         else:
             if self.hidd_boxes:
                 iid = self.hidd_boxes.pop()
@@ -1659,14 +1660,15 @@
                 text = self.extra_begin_edit_cell_func(
                     event_dict(
                         name="begin_edit_header",
                         sheet=self.PAR.name,
                         key=extra_func_key,
                         value=text,
                         loc=c,
+                        column=c,
                         boxes=self.MT.get_boxes(),
                         selected=self.MT.selected,
                     )
                 )
             except Exception:
                 return False
             if text is None:
@@ -1722,20 +1724,22 @@
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
         self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(c=c))
+        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(c=c))
         if USER_OS == "darwin":
             self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(c=c))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
         self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((c, "Tab")))
         self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((c, "Return")))
+        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((c, "Return")))
         if not dropdown:
             self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((c, "FocusOut")))
         self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((c, "Escape")))
         return True
 
     # displayed indexes                         #just here to receive text editor arg
     def text_editor_has_wrapped(self, r=0, c=0, check_lines=None):
@@ -1823,16 +1827,16 @@
                     self.MT.col_positions[c],
                     0,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
-            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
-                self.text_editor.tktext.unbind(b)
+            for binding in text_editor_to_unbind:
+                self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # c is displayed col
     def close_text_editor(
@@ -1858,14 +1862,15 @@
         event_data = event_dict(
             name="end_edit_header",
             sheet=self.PAR.name,
             cells_header={datacn: self.get_cell_data(datacn)},
             key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
             value=text_editor_value,
             loc=c,
+            column=c,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
             c=c,
@@ -1966,14 +1971,15 @@
                 lambda _x: self.dropdown_text_editor_modified(
                     self.dropdown.window,
                     event_dict(
                         name="header_dropdown_modified",
                         sheet=self.PAR.name,
                         value=self.text_editor.get(),
                         loc=c,
+                        column=c,
                         boxes=self.MT.get_boxes(),
                         selected=self.MT.selected,
                     ),
                     kwargs["modified_function"],
                 ),
             )
             self.update_idletasks()
@@ -2001,14 +2007,15 @@
             event_data = event_dict(
                 name="end_edit_header",
                 sheet=self.PAR.name,
                 cells_header={datacn: pre_edit_value},
                 key="??",
                 value=selection,
                 loc=c,
+                column=c,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             )
             if kwargs["select_function"] is not None:
                 kwargs["select_function"](event_data)
             if self.MT.edit_validation_func:
                 selection = self.MT.edit_validation_func(event_data)
@@ -2226,14 +2233,15 @@
             event_data = event_dict(
                 name="end_edit_header",
                 sheet=self.PAR.name,
                 cells_header={datacn: pre_edit_value},
                 key="??",
                 value=value,
                 loc=c,
+                column=c,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             )
             if kwargs["check_function"] is not None:
                 kwargs["check_function"](event_data)
             try_binding(self.extra_end_edit_cell_func, event_data)
         if redraw:
```

### Comparing `tksheet-7.1.7/tksheet/formatters.py` & `tksheet-7.1.8/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/functions.py` & `tksheet-7.1.8/tksheet/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     cells_header: None | dict = None,
     cells_index: None | dict = None,
     selected: None | tuple = None,
     data: object = None,
     key: None | str = None,
     value: object = None,
     loc: None | int | tuple[int] = None,
+    row: None | int = None,
+    column: None | int = None,
     resized_rows: None | dict = None,
     resized_columns: None | dict = None,
     # resized_index: None, dict] = None,
     # resized_header: None, dict] = None,
     being_selected: None | tuple = None,
     named_spans: None | dict = None,
     **kwargs,
@@ -143,14 +145,16 @@
         ),
         selected=tuple() if selected is None else selected,
         being_selected=tuple() if being_selected is None else being_selected,
         data=[] if data is None else data,
         key="" if key is None else key,
         value=None if value is None else value,
         loc=tuple() if loc is None else loc,
+        row=row,
+        column=column,
         resized=DotDict(
             rows=DotDict() if resized_rows is None else resized_rows,
             columns=DotDict() if resized_columns is None else resized_columns,
             # "header": DotDict() if resized_header is None else resized_header,
             # "index": DotDict() if resized_index is None else resized_index,
         ),
     )
@@ -399,16 +403,16 @@
         return True
     except Exception:
         return False
 
 
 def move_elements_by_mapping(
     seq: list[object],
-    new_idxs: dict,
-    old_idxs: dict,
+    new_idxs: dict[int, int],
+    old_idxs: dict[int, int],
 ) -> list[object]:
     # move elements of a list around, displacing
     # other elements based on mapping
     # of {old index: new index, ...}
 
     # create dummy list
     res = [0] * len(seq)
@@ -468,16 +472,15 @@
     new_idxs = {old: new for old, new in zip(to_move, new_idxs)}
     if get_inverse:
         return new_idxs, dict(zip(new_idxs.values(), new_idxs))
     return new_idxs
 
 
 def insert_items(seq: list | tuple, to_insert: dict, seq_len_func: Callable | None = None) -> list:
-    # faster method of inserting many items into a list
-    # using a dict of reverse sorted order of
+    # inserts many items into a list using a dict of reverse sorted order of
     # {index: value, index: value, ...}
     res = []
     extended = 0
     for i, (idx, v) in enumerate(reversed(to_insert.items())):
         # need to extend seq if it's not long enough
         if seq_len_func and idx - i > len(seq):
             seq_len_func(idx - i - 1)
```

### Comparing `tksheet-7.1.7/tksheet/main_table.py` & `tksheet-7.1.8/tksheet/main_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     partial,
 )
 from itertools import (
     accumulate,
     chain,
     cycle,
     islice,
-    product,
     repeat,
 )
 from math import (
     ceil,
     floor,
 )
 from operator import itemgetter
@@ -52,52 +51,54 @@
     consecutive_ranges,
     decompress_load,
     diff_gen,
     diff_list,
     ev_stack_dict,
     event_dict,
     gen_formatted,
-    rounded_box_coords,
     get_new_indexes,
     get_seq_without_gaps_at_index,
     index_exists,
     insert_items,
     int_x_iter,
     is_iterable,
     is_type_int,
     len_to_idx,
     mod_event_val,
     mod_span,
+    mod_span_widget,
     move_elements_by_mapping,
     pickle_obj,
+    rounded_box_coords,
     span_idxs_post_move,
-    mod_span_widget,
     try_binding,
     unpickle_obj,
 )
 from .other_classes import (
     Box_nt,
     Box_st,
     Box_t,
     DotDict,
     DropdownStorage,
     EventDataDict,
     FontTuple,
+    Loc,
     Selected,
     SelectionBox,
     TextEditorStorage,
 )
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
     USER_OS,
     ctrl_key,
     rc_binding,
     symbols_set,
+    text_editor_to_unbind,
     val_modifying_options,
 )
 
 
 class MainTable(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
@@ -671,15 +672,15 @@
             lastbox_c2,
         ) = self.selection_boxes[self.selected.fill_iid].coords
         lastbox_numrows = lastbox_r2 - lastbox_r1
         lastbox_numcols = lastbox_c2 - lastbox_c1
         if lastbox_numrows > new_data_numrows and not lastbox_numrows % new_data_numrows:
             nd = []
             for _ in range(int(lastbox_numrows / new_data_numrows)):
-                nd.extend([r.copy() for r in data])
+                nd.extend(r.copy() for r in data)
             data.extend(nd)
             new_data_numrows *= int(lastbox_numrows / new_data_numrows)
 
         if lastbox_numcols > new_data_numcols and not lastbox_numcols % new_data_numcols:
             for rn, r in enumerate(data):
                 for _ in range(int(lastbox_numcols / new_data_numcols)):
                     data[rn].extend(r.copy())
@@ -967,22 +968,22 @@
                         boxst,
                         len(self.row_positions) - 1,
                         boxend,
                         "columns",
                         run_binding=True,
                     )
         if move_data:
-            self.data[:] = [
-                move_elements_by_mapping(
-                    r,
-                    data_new_idxs,
-                    data_old_idxs,
-                )
-                for r in self.data
-            ]
+            self.data = list(
+                map(
+                    move_elements_by_mapping,
+                    self.data,
+                    repeat(data_new_idxs),
+                    repeat(data_old_idxs),
+                ),
+            )
             maxidx = len_to_idx(totalcols)
             self.CH.fix_header(maxidx)
             if isinstance(self._headers, list) and self._headers:
                 self._headers = move_elements_by_mapping(self._headers, data_new_idxs, data_old_idxs)
             maxidx = self.get_max_column_idx(maxidx)
             full_new_idxs = self.get_full_new_idxs(
                 max_idx=maxidx,
@@ -1191,15 +1192,15 @@
                         0,
                         boxend,
                         len(self.col_positions) - 1,
                         "rows",
                         run_binding=True,
                     )
         if move_data:
-            self.data[:] = move_elements_by_mapping(
+            self.data = move_elements_by_mapping(
                 self.data,
                 data_new_idxs,
                 data_old_idxs,
             )
             maxidx = len_to_idx(totalrows)
             self.RI.fix_index(maxidx)
             if isinstance(self._row_index, list) and self._row_index:
@@ -3209,47 +3210,38 @@
                 widget.MT.set_yviews(*args, move_synced=False, redraw=redraw)
             else:
                 widget.yview(*args)
             # except Exception:
             #     continue
 
     def set_xviews(self, *args, move_synced: bool = True, redraw: bool = True) -> None:
+        self.main_table_redraw_grid_and_text(setting_views=True)
+        self.update_idletasks()
         self.xview(*args)
         if self.show_header:
             self.CH.xview(*args)
         if move_synced:
             self.x_move_synced_scrolls(*args)
         self.fix_views()
-        if redraw:
-            self.main_table_redraw_grid_and_text(redraw_header=True if self.show_header else False)
+        self.PAR.set_refresh_timer(redraw)
 
     def set_yviews(self, *args, move_synced: bool = True, redraw: bool = True) -> None:
+        self.main_table_redraw_grid_and_text(setting_views=True)
+        self.update_idletasks()
         self.yview(*args)
         if self.show_index:
             self.RI.yview(*args)
         if move_synced:
             self.y_move_synced_scrolls(*args)
         self.fix_views()
-        if redraw:
-            self.main_table_redraw_grid_and_text(redraw_row_index=True if self.show_index else False)
+        self.PAR.set_refresh_timer(redraw)
 
     def set_view(self, x_args: list[str, float], y_args: list[str, float]) -> None:
-        self.xview(*x_args)
-        if self.show_header:
-            self.CH.xview(*x_args)
-        self.yview(*y_args)
-        if self.show_index:
-            self.RI.yview(*y_args)
-        self.x_move_synced_scrolls(*x_args)
-        self.y_move_synced_scrolls(*y_args)
-        self.fix_views()
-        self.main_table_redraw_grid_and_text(
-            redraw_row_index=True if self.show_index else False,
-            redraw_header=True if self.show_header else False,
-        )
+        self.set_xviews(*x_args)
+        self.set_yviews(*y_args)
 
     def mousewheel(self, event: object) -> None:
         if event.delta < 0 or event.num == 5:
             self.yview_scroll(1, "units")
             self.RI.yview_scroll(1, "units")
             self.y_move_synced_scrolls("moveto", self.yview()[0])
         elif event.delta >= 0 or event.num == 4:
@@ -4889,15 +4881,15 @@
 
     def data_dimensions(self, total_rows: int | None = None, total_columns: int | None = None):
         if total_rows is None and total_columns is None:
             return self.total_data_rows(), self.total_data_cols()
         if total_rows is not None:
             if len(self.data) < total_rows:
                 ncols = self.total_data_cols() if total_columns is None else total_columns
-                self.data.extend([self.get_empty_row_seq(r, ncols) for r in range(total_rows - len(self.data))])
+                self.data.extend(self.get_empty_row_seq(r, ncols) for r in range(total_rows - len(self.data)))
             else:
                 self.data[total_rows:] = []
         if total_columns is not None:
             for rn, r in enumerate(self.data):
                 if (lnr := len(r)) > total_columns:
                     r = r[:total_columns]
                 elif lnr < total_columns:
@@ -5189,14 +5181,15 @@
             self.disp_checkbox[t] = True
 
     def main_table_redraw_grid_and_text(
         self,
         redraw_header: bool = False,
         redraw_row_index: bool = False,
         redraw_table: bool = True,
+        setting_views: bool = False,
     ) -> bool:
         try:
             can_width = self.winfo_width()
             can_height = self.winfo_height()
         except Exception:
             return False
         row_pos_exists = self.row_positions != [0] and self.row_positions
@@ -5282,14 +5275,16 @@
             0,
             last_col_line_pos + self.PAR.ops.empty_horizontal + 2,
             last_row_line_pos + self.PAR.ops.empty_vertical + 2,
         )
         if scrollregion != self.scrollregion:
             self.configure(scrollregion=scrollregion)
             self.scrollregion = scrollregion
+        if setting_views:
+            return False
         scrollpos_bot = self.canvasy(can_height)
         end_row = bisect_right(self.row_positions, scrollpos_bot)
         if not scrollpos_bot >= self.row_positions[-1]:
             end_row += 1
         scrollpos_left = self.canvasx(0)
         scrollpos_top = self.canvasy(0)
         scrollpos_right = self.canvasx(can_width)
@@ -5761,16 +5756,16 @@
         type_: Literal["cells", "rows", "columns"],
         fill_iid: int,
         lower_selection_boxes: bool = True,
     ) -> int:
         fill, outline = self.get_selected_box_bg_fg(type_=type_)
         x1 = self.col_positions[c] + 1
         y1 = self.row_positions[r] + 1
-        x2 = self.col_positions[c + 1] if index_exists(self.col_positions, c + 1) else self.col_positions[c]
-        y2 = self.row_positions[r + 1] if index_exists(self.row_positions, r + 1) else self.row_positions[r]
+        x2 = self.col_positions[c + 1] if index_exists(self.col_positions, c + 1) else self.col_positions[c] + 1
+        y2 = self.row_positions[r + 1] if index_exists(self.row_positions, r + 1) else self.row_positions[r] + 1
         self.hide_selected()
         if self.PAR.ops.show_selected_cells_border:
             fill = ""
         else:
             fill = outline
             outline = ""
         iid = self.display_box(
@@ -5805,20 +5800,24 @@
         fill: str,
         outline: str,
         state: str,
         tags: str | tuple[str],
         width: int,
         iid: None | int = None,
     ) -> int:
+        if not self.PAR.ops.rounded_boxes or not x2 - x1 or not y2 - y1:
+            radius = 0
+        else:
+            radius = 8
         coords = rounded_box_coords(
             x1,
             y1,
             x2,
             y2,
-            radius=9 if self.PAR.ops.rounded_boxes else 0,
+            radius=radius,
         )
         if isinstance(iid, int):
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags, width=width)
             self.coords(iid, coords)
         else:
             if self.hidd_boxes:
                 iid = self.hidd_boxes.pop()
@@ -5840,15 +5839,15 @@
     def hide_box(self, item: int | None) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
 
     def hide_selection_box(self, item: int | None, set_current: bool = True) -> bool:
-        if item is None:
+        if item is None or item is True:
             return
         box = self.selection_boxes.pop(item)
         self.hide_box(box.fill_iid)
         self.hide_box(box.bd_iid)
         self.RI.hide_box(box.index)
         self.CH.hide_box(box.header)
         if self.selected.fill_iid == item:
@@ -6044,15 +6043,15 @@
                 self.PAR.ops.header_selected_columns_bg if type_ == "columns" else self.PAR.ops.header_selected_cells_bg
             ),
             outline="",
             state="normal",
             tags="cells" if type_ == "rows" else type_,
             iid=self.selection_boxes[fill_iid].header,
         )
-        if (bd_iid := self.selection_boxes[fill_iid].bd_iid):
+        if bd_iid := self.selection_boxes[fill_iid].bd_iid:
             if self.PAR.ops.show_selected_cells_border:
                 self.display_box(
                     x1,
                     y1,
                     x2,
                     y2,
                     fill="",
@@ -6143,176 +6142,70 @@
         if min_x != float("inf") and min_y != float("inf") and max_x > 0 and max_y > 0:
             return min_y, min_x, max_y, max_x
         return None, None, None, None
 
     def get_selected_rows(
         self,
         get_cells: bool = False,
-        within_range: tuple | None = None,
         get_cells_as_rows: bool = False,
     ) -> set[int] | set[tuple[int, int]]:
-        s = set()
-        if within_range is not None:
-            within_r1 = within_range[0]
-            within_r2 = within_range[1]
         if get_cells:
-            if within_range is None:
-                for item, box in self.get_selection_items(cells=False, columns=False):
-                    r1, c1, r2, c2 = box.coords
-                    s.update(set(product(range(r1, r2), range(0, len(self.col_positions) - 1))))
-                if get_cells_as_rows:
-                    s.update(self.get_selected_cells())
-            else:
-                for item, box in self.get_selection_items(cells=False, columns=False):
-                    r1, c1, r2, c2 = box.coords
-                    if r1 >= within_r1 or r2 <= within_r2:
-                        s.update(
-                            set(
-                                product(
-                                    range(r1 if r1 > within_r1 else within_r1, r2 if r2 < within_r2 else within_r2),
-                                    range(0, len(self.col_positions) - 1),
-                                )
-                            )
-                        )
-                if get_cells_as_rows:
-                    s.update(
-                        self.get_selected_cells(
-                            within_range=(
-                                within_r1,
-                                0,
-                                within_r2,
-                                len(self.col_positions) - 1,
-                            )
-                        )
-                    )
+            s = {
+                (r, c)
+                for item, box in self.get_selection_items(cells=False, columns=False)
+                for r in range(box.coords.from_r, box.coords.upto_r)
+                for c in range(0, len(self.col_positions) - 1)
+            }
+            if get_cells_as_rows:
+                return s | self.get_selected_cells()
         else:
-            if within_range is None:
-                for item, box in self.get_selection_items(cells=False, columns=False):
-                    r1, c1, r2, c2 = box.coords
-                    s.update(set(range(r1, r2)))
-                if get_cells_as_rows:
-                    s.update(set(tup[0] for tup in self.get_selected_cells()))
-            else:
-                for item, box in self.get_selection_items(cells=False, columns=False):
-                    r1, c1, r2, c2 = box.coords
-                    if r1 >= within_r1 or r2 <= within_r2:
-                        s.update(set(range(r1 if r1 > within_r1 else within_r1, r2 if r2 < within_r2 else within_r2)))
-                if get_cells_as_rows:
-                    s.update(
-                        set(
-                            tup[0]
-                            for tup in self.get_selected_cells(
-                                within_range=(
-                                    within_r1,
-                                    0,
-                                    within_r2,
-                                    len(self.col_positions) - 1,
-                                )
-                            )
-                        )
-                    )
+            s = {
+                r
+                for item, box in self.get_selection_items(cells=False, columns=False)
+                for r in range(box.coords.from_r, box.coords.upto_r)
+            }
+            if get_cells_as_rows:
+                return s | set(tup[0] for tup in self.get_selected_cells())
         return s
 
     def get_selected_cols(
         self,
         get_cells: bool = False,
-        within_range: tuple | None = None,
         get_cells_as_cols: bool = False,
     ) -> set[int] | set[tuple[int, int]]:
-        s = set()
-        if within_range is not None:
-            within_c1 = within_range[0]
-            within_c2 = within_range[1]
         if get_cells:
-            if within_range is None:
-                for item, box in self.get_selection_items(cells=False, rows=False):
-                    r1, c1, r2, c2 = box.coords
-                    s.update(set(product(range(c1, c2), range(0, len(self.row_positions) - 1))))
-                if get_cells_as_cols:
-                    s.update(self.get_selected_cells())
-            else:
-                for item, box in self.get_selection_items(cells=False, rows=False):
-                    r1, c1, r2, c2 = box.coords
-                    if c1 >= within_c1 or c2 <= within_c2:
-                        s.update(
-                            set(
-                                product(
-                                    range(c1 if c1 > within_c1 else within_c1, c2 if c2 < within_c2 else within_c2),
-                                    range(0, len(self.row_positions) - 1),
-                                )
-                            )
-                        )
-                if get_cells_as_cols:
-                    s.update(
-                        self.get_selected_cells(
-                            within_range=(
-                                0,
-                                within_c1,
-                                len(self.row_positions) - 1,
-                                within_c2,
-                            )
-                        )
-                    )
+            s = {
+                (r, c)
+                for item, box in self.get_selection_items(cells=False, rows=False)
+                for r in range(0, len(self.row_positions) - 1)
+                for c in range(box.coords.from_c, box.coords.upto_c)
+            }
+            if get_cells_as_cols:
+                return s | self.get_selected_cells()
         else:
-            if within_range is None:
-                for item, box in self.get_selection_items(cells=False, rows=False):
-                    r1, c1, r2, c2 = box.coords
-                    s.update(set(range(c1, c2)))
-                if get_cells_as_cols:
-                    s.update(set(tup[1] for tup in self.get_selected_cells()))
-            else:
-                for item in self.get_selection_items(cells=False, rows=False):
-                    r1, c1, r2, c2 = box.coords
-                    if c1 >= within_c1 or c2 <= within_c2:
-                        s.update(set(range(c1 if c1 > within_c1 else within_c1, c2 if c2 < within_c2 else within_c2)))
-                if get_cells_as_cols:
-                    s.update(
-                        set(
-                            tup[0]
-                            for tup in self.get_selected_cells(
-                                within_range=(
-                                    0,
-                                    within_c1,
-                                    len(self.row_positions) - 1,
-                                    within_c2,
-                                )
-                            )
-                        )
-                    )
+            s = {
+                c
+                for item, box in self.get_selection_items(cells=False, rows=False)
+                for c in range(box.coords.from_c, box.coords.upto_c)
+            }
+            if get_cells_as_cols:
+                return s | set(tup[1] for tup in self.get_selected_cells())
         return s
 
     def get_selected_cells(
         self,
         get_rows: bool = False,
         get_cols: bool = False,
-        within_range: bool = None,
     ) -> set[tuple[int, int]]:
-        s = set()
-        if within_range is not None:
-            within_r1 = within_range[0]
-            within_c1 = within_range[1]
-            within_r2 = within_range[2]
-            within_c2 = within_range[3]
-        if within_range is None:
-            for item, box in self.get_selection_items(rows=get_rows, columns=get_cols):
-                r1, c1, r2, c2 = box.coords
-                s.update(set(product(range(r1, r2), range(c1, c2))))
-        else:
-            for item in self.get_selection_items(rows=get_rows, columns=get_cols):
-                r1, c1, r2, c2 = box.coords
-                if r1 >= within_r1 or c1 >= within_c1 or r2 <= within_r2 or c2 <= within_c2:
-                    s.update(
-                        set(
-                            product(
-                                range(r1 if r1 > within_r1 else within_r1, r2 if r2 < within_r2 else within_r2),
-                                range(c1 if c1 > within_c1 else within_c1, c2 if c2 < within_c2 else within_c2),
-                            )
-                        )
-                    )
-        return s
+        return {
+            (r, c)
+            for item, box in self.get_selection_items(rows=get_rows, columns=get_cols)
+            for r in range(box.coords.from_r, box.coords.upto_r)
+            for c in range(box.coords.from_c, box.coords.upto_c)
+        }
 
     def get_all_selection_boxes(self) -> tuple[tuple[int, int, int, int]]:
         return tuple(box.coords for item, box in self.get_selection_items())
 
     def get_all_selection_boxes_with_types(self) -> list[tuple[tuple[int, int, int, int], str]]:
         return [Box_st(box.coords, box.type_) for item, box in self.get_selection_items()]
 
@@ -6465,15 +6358,17 @@
             try:
                 text = self.extra_begin_edit_cell_func(
                     event_dict(
                         name="begin_edit_table",
                         sheet=self.PAR.name,
                         key=extra_func_key,
                         value=text,
-                        loc=(r, c),
+                        loc=Loc(r, c),
+                        row=r,
+                        column=c,
                         boxes=self.get_boxes(),
                         selected=self.selected,
                     )
                 )
             except Exception:
                 return False
             if text is None:
@@ -6528,20 +6423,22 @@
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
         self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(r, c))
+        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(r, c))
         if USER_OS == "darwin":
             self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(r, c))
         for key, func in self.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
         self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((r, c, "Tab")))
         self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((r, c, "Return")))
+        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((r, c, "Return")))
         if not dropdown:
             self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((r, c, "FocusOut")))
         self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((r, c, "Escape")))
         return True
 
     # displayed indexes
     def text_editor_newline_binding(
@@ -6623,16 +6520,16 @@
                     self.col_positions[c],
                     self.row_positions[r],
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
-            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
-                self.text_editor.tktext.unbind(b)
+            for binding in text_editor_to_unbind:
+                self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     def close_text_editor(
         self,
@@ -6656,15 +6553,17 @@
         datarn, datacn = self.datarn(r), self.datacn(c)
         event_data = event_dict(
             name="end_edit_table",
             sheet=self.PAR.name,
             cells_table={(datarn, datacn): text_editor_value},
             key=editor_info[2],
             value=text_editor_value,
-            loc=(r, c),
+            loc=Loc(r, c),
+            row=r,
+            column=c,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
             r=r,
@@ -6907,15 +6806,17 @@
             self.text_editor.tktext.bind(
                 "<<TextModified>>",
                 lambda x: self.dropdown.window.search_and_see(
                     event_dict(
                         name="table_dropdown_modified",
                         sheet=self.PAR.name,
                         value=self.text_editor.get(),
-                        loc=(r, c),
+                        loc=Loc(r, c),
+                        row=r,
+                        column=c,
                         boxes=self.get_boxes(),
                         selected=self.selected,
                     )
                 ),
             )
             if kwargs["modified_function"] is not None:
                 self.dropdown.window.modified_function = kwargs["modified_function"]
@@ -6950,15 +6851,17 @@
             pre_edit_value = self.get_cell_data(datarn, datacn)
             event_data = event_dict(
                 name="end_edit_table",
                 sheet=self.PAR.name,
                 cells_table={(datarn, datacn): pre_edit_value},
                 key="??",
                 value=selection,
-                loc=(r, c),
+                loc=Loc(r, c),
+                row=r,
+                column=c,
                 boxes=self.get_boxes(),
                 selected=self.selected,
             )
             if kwargs["select_function"] is not None:
                 kwargs["select_function"](event_data)
             if self.edit_validation_func:
                 selection, edited = self.edit_validation_func(event_data), False
@@ -7038,15 +6941,17 @@
             )
             event_data = event_dict(
                 name="end_edit_table",
                 sheet=self.PAR.name,
                 cells_table={(datarn, datacn): pre_edit_value},
                 key="??",
                 value=value,
-                loc=(r, c),
+                loc=Loc(r, c),
+                row=r,
+                column=c,
                 boxes=self.get_boxes(),
                 selected=self.selected,
             )
             if kwargs["check_function"] is not None:
                 kwargs["check_function"](event_data)
             try_binding(self.extra_end_edit_cell_func, event_data)
         if redraw:
@@ -7157,15 +7062,15 @@
         if datarn < len(self.data):
             for datacn, v in enumerate(islice(self.data[datarn], start, end)):
                 if not self.input_valid_for_cell(datarn, datacn, v):
                     self.data[datarn][datacn] = self.get_value_for_empty_cell(datarn, datacn)
 
     def fix_data_len(self, datarn: int, datacn: int | None = None) -> int:
         ncols = self.total_data_cols() if datacn is None else datacn + 1
-        self.data.extend([self.get_empty_row_seq(rn, end=ncols, start=0) for rn in range(len(self.data), datarn + 1)])
+        self.data.extend(self.get_empty_row_seq(rn, end=ncols, start=0) for rn in range(len(self.data), datarn + 1))
         return len(self.data)
 
     def reapply_formatting(self) -> None:
         for c in gen_formatted(self.col_options):
             for r in range(len(self.data)):
                 if not (
                     (r, c) in self.cell_options
```

### Comparing `tksheet-7.1.7/tksheet/other_classes.py` & `tksheet-7.1.8/tksheet/other_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,16 @@
     "Box_nt",
     "from_r from_c upto_r upto_c",
 )
 Box_t = namedtuple(
     "Box_t",
     "from_r from_c upto_r upto_c type_",
 )
-Box_st = namedtuple(
-    "Box_st",
-    "coords type_"
-)
+Box_st = namedtuple("Box_st", "coords type_")
+Loc = namedtuple("Loc", "row column")
 
 Highlight = namedtuple(
     "Highlight",
     (
         "bg",
         "fg",
         "end",  # only used for row options highlights
@@ -468,8 +466,7 @@
         None,
         None,
         None,
         None,
         None,
     ),
 )
-
```

### Comparing `tksheet-7.1.7/tksheet/row_index.py` & `tksheet-7.1.8/tksheet/row_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     is_bool_like,
     try_to_bool,
 )
 from .functions import (
     consecutive_chunks,
     ev_stack_dict,
     event_dict,
-    rounded_box_coords,
     get_n2a,
     is_contiguous,
     num2alpha,
+    rounded_box_coords,
     try_binding,
 )
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DropdownStorage,
     Node,
@@ -47,14 +47,15 @@
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
     USER_OS,
     rc_binding,
     symbols_set,
+    text_editor_to_unbind,
 )
 
 
 class RowIndex(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
@@ -961,15 +962,15 @@
         iid: None | int = None,
     ) -> int:
         coords = rounded_box_coords(
             x1,
             y1,
             x2,
             y2,
-            radius=9 if self.PAR.ops.rounded_boxes else 0,
+            radius=8 if self.PAR.ops.rounded_boxes else 0,
         )
         if isinstance(iid, int):
             self.coords(iid, coords)
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
         else:
             if self.hidd_boxes:
                 iid = self.hidd_boxes.pop()
@@ -1751,14 +1752,15 @@
                 text = self.extra_begin_edit_cell_func(
                     event_dict(
                         name="begin_edit_index",
                         sheet=self.PAR.name,
                         key=extra_func_key,
                         value=text,
                         loc=r,
+                        row=r,
                         boxes=self.MT.get_boxes(),
                         selected=self.MT.selected,
                     )
                 )
             except Exception:
                 return False
             if text is None:
@@ -1812,20 +1814,22 @@
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
         self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(r=r))
+        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(r=r))
         if USER_OS == "darwin":
             self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(r=r))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
         self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((r, "Tab")))
         self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((r, "Return")))
+        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((r, "Return")))
         if not dropdown:
             self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((r, "FocusOut")))
         self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((r, "Escape")))
         return True
 
     def text_editor_newline_binding(self, r=0, c=0, event: object = None, check_lines=True):
         if not self.height_resizing_enabled:
@@ -1905,16 +1909,16 @@
                     0,
                     self.MT.row_positions[r],
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
-            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
-                self.text_editor.tktext.unbind(b)
+            for binding in text_editor_to_unbind:
+                self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # r is displayed row
     def close_text_editor(
@@ -1938,14 +1942,15 @@
         event_data = event_dict(
             name="end_edit_index",
             sheet=self.PAR.name,
             cells_index={datarn: self.get_cell_data(datarn)},
             key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
             value=text_editor_value,
             loc=r,
+            row=r,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
             r=r,
@@ -2060,14 +2065,15 @@
                 lambda _x: self.dropdown_text_editor_modified(
                     self.dropdown.window,
                     event_dict(
                         name="index_dropdown_modified",
                         sheet=self.PAR.name,
                         value=self.text_editor.get(),
                         loc=r,
+                        row=r,
                         boxes=self.MT.get_boxes(),
                         selected=self.MT.selected,
                     ),
                     kwargs["modified_function"],
                 ),
             )
             self.update_idletasks()
@@ -2096,14 +2102,15 @@
             event_data = event_dict(
                 name="end_edit_index",
                 sheet=self.PAR.name,
                 cells_header={datarn: pre_edit_value},
                 key="??",
                 value=selection,
                 loc=r,
+                row=r,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             )
             if kwargs["select_function"] is not None:
                 kwargs["select_function"](event_data)
             if self.MT.edit_validation_func:
                 selection = self.MT.edit_validation_func(event_data)
@@ -2318,14 +2325,15 @@
             event_data = event_dict(
                 name="end_edit_index",
                 sheet=self.PAR.name,
                 cells_index={datarn: pre_edit_value},
                 key="??",
                 value=value,
                 loc=r,
+                row=r,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             )
             if kwargs["check_function"] is not None:
                 kwargs["check_function"](event_data)
             try_binding(self.extra_end_edit_cell_func, event_data)
         if redraw:
```

### Comparing `tksheet-7.1.7/tksheet/sheet.py` & `tksheet-7.1.8/tksheet/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from bisect import bisect_left
 from collections import defaultdict, deque
 from collections.abc import Callable, Generator, Iterator, Sequence
 from itertools import accumulate, chain, islice, product
 from timeit import default_timer
 from tkinter import ttk
 from typing import Literal
-from warnings import warn as WARNING
 
 from .column_headers import ColumnHeaders
 from .functions import (
     add_highlight,
     add_to_options,
     convert_align,
     data_to_displayed_idxs,
@@ -42,16 +41,16 @@
 from .main_table import MainTable
 from .other_classes import (
     DotDict,
     EventDataDict,
     FontTuple,
     GeneratedMouseEvent,
     Node,
-    Span,
     Selected,
+    Span,
 )
 from .row_index import RowIndex
 from .sheet_options import (
     new_sheet_options,
 )
 from .themes import (
     theme_black,
@@ -268,17 +267,14 @@
             self,
             parent,
             background=frame_bg,
             highlightthickness=outline_thickness,
             highlightbackground=outline_color,
             highlightcolor=outline_color,
         )
-        WARNING(
-            "There have been many changes from tksheet version 6.x.x to version 7.x.x. Please see the changelog for more information."
-        )
         self.ops = new_sheet_options()
         if column_width is not None:
             default_column_width = column_width
         if header_height is not None:
             default_header_height = header_height
         if row_height is not None:
             default_row_height = row_height
@@ -610,15 +606,15 @@
         # e.g. [(binding, function), (binding, function), ...]
         elif is_iterable(bindings):
             iterable = bindings
 
         for b, f in iterable:
             b = b.lower()
 
-            if func is not None and b in emitted_events:
+            if f is not None and b in emitted_events:
                 self.bind(b, f)
 
             if b in (
                 "all",
                 "bind_all",
                 "unbind_all",
             ):
@@ -1353,46 +1349,42 @@
                     else:
                         res.append([quick_idata(r, get_displayed=idisp) for r in rows])
                 else:
                     res.append([quick_idata(r, get_displayed=idisp) for r in rows])
             if header:
                 if table:
                     res.extend(
-                        [
-                            [quick_hdata(c, get_displayed=hdisp)]
-                            + [quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for r in rows]
-                            for c in cols
-                        ]
+                        [quick_hdata(c, get_displayed=hdisp)]
+                        + [quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for r in rows]
+                        for c in cols
                     )
                 else:
-                    res.extend([[quick_hdata(c, get_displayed=hdisp)] for c in cols])
+                    res.extend([quick_hdata(c, get_displayed=hdisp)] for c in cols)
             elif table:
-                res.extend([[quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for r in rows] for c in cols])
+                res.extend([quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for r in rows] for c in cols)
         elif not span.transposed:
             if header:
                 if header and index:
                     if table:
                         res.append([""] + [quick_hdata(c, get_displayed=hdisp) for c in cols])
                     else:
                         res.append([quick_hdata(c, get_displayed=hdisp) for c in cols])
                 else:
                     res.append([quick_hdata(c, get_displayed=hdisp) for c in cols])
             if index:
                 if table:
                     res.extend(
-                        [
-                            [quick_idata(r, get_displayed=idisp)]
-                            + [quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for c in cols]
-                            for r in rows
-                        ]
+                        [quick_idata(r, get_displayed=idisp)]
+                        + [quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for c in cols]
+                        for r in rows
                     )
                 else:
-                    res.extend([[quick_idata(r, get_displayed=idisp)] for r in rows])
+                    res.extend([quick_idata(r, get_displayed=idisp)] for r in rows)
             elif table:
-                res.extend([[quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for c in cols] for r in rows])
+                res.extend([quick_tdata(r, c, get_displayed=tdisp, fmt_kw=fmt_kw) for c in cols] for r in rows)
         if not span.ndim:
             # it's a cell
             if len(res) == 1 and len(res[0]) == 1:
                 res = res[0][0]
             # it's a single list
             elif len(res) == 1:
                 res = res[0]
@@ -1517,15 +1509,15 @@
             reset_row_positions,
             redraw,
             return_id=False,
             keep_formatting=keep_formatting,
         )
 
     @data.setter
-    def data(self, value):
+    def data(self, value: list[list[object]]) -> None:
         self.data_reference(value)
 
     def set_data(
         self,
         *key: CreateSpanTypes,
         data: object = None,
         undo: bool | None = None,
@@ -2846,20 +2838,15 @@
         elif convert_align(align):
             self.RI.align = convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
         self.set_refresh_timer(redraw)
         return self
 
-    def index_align(
-        self,
-        align: str = None,
-        redraw: bool = True,
-    ) -> str | Sheet:
-        return self.row_index_align(align, redraw)
+    index_align = row_index_align
 
     def align(
         self,
         *key: CreateSpanTypes,
         align: str | None = None,
         redraw: bool = True,
     ) -> Span:
@@ -2909,41 +2896,54 @@
         #     return self.MT.selected._replace(type_=self.MT.selected.type_[:-1])
         return self.MT.selected
 
     @property
     def selected(self) -> tuple[()] | Selected:
         return self.MT.selected
 
+    @selected.setter
+    def selected(self, selected: tuple[()] | Selected) -> Sheet:
+        if selected:
+            self.MT.set_currently_selected(
+                r=selected[0],
+                c=selected[1],
+                item=selected[4],
+                box=selected[3],
+            )
+        else:
+            self.MT.deselect()
+        return self
+
     def get_selected_rows(
         self,
         get_cells: bool = False,
         get_cells_as_rows: bool = False,
         return_tuple: bool = False,
-    ) -> tuple | set:
+    ) -> tuple[int] | tuple[tuple[int, int]] | set[int] | set[tuple[int, int]]:
         if return_tuple:
             return tuple(self.MT.get_selected_rows(get_cells=get_cells, get_cells_as_rows=get_cells_as_rows))
         return self.MT.get_selected_rows(get_cells=get_cells, get_cells_as_rows=get_cells_as_rows)
 
     def get_selected_columns(
         self,
         get_cells: bool = False,
         get_cells_as_columns: bool = False,
         return_tuple: bool = False,
-    ) -> tuple | set:
+    ) -> tuple[int] | tuple[tuple[int, int]] | set[int] | set[tuple[int, int]]:
         if return_tuple:
             return tuple(self.MT.get_selected_cols(get_cells=get_cells, get_cells_as_cols=get_cells_as_columns))
         return self.MT.get_selected_cols(get_cells=get_cells, get_cells_as_cols=get_cells_as_columns)
 
     def get_selected_cells(
         self,
         get_rows: bool = False,
         get_columns: bool = False,
         sort_by_row: bool = False,
         sort_by_column: bool = False,
-    ) -> list | set:
+    ) -> list[tuple[int, int]] | set[tuple[int, int]]:
         if sort_by_row and sort_by_column:
             sels = sorted(
                 self.MT.get_selected_cells(get_rows=get_rows, get_cols=get_columns),
                 key=lambda t: t[1],
             )
             return sorted(sels, key=lambda t: t[0])
         elif sort_by_row:
@@ -2964,14 +2964,22 @@
     def get_all_selection_boxes_with_types(self) -> list[tuple[tuple[int, int, int, int], str]]:
         return self.MT.get_all_selection_boxes_with_types()
 
     @property
     def boxes(self) -> list[tuple[tuple[int, int, int, int], str]]:
         return self.MT.get_all_selection_boxes_with_types()
 
+    @boxes.setter
+    def boxes(self, boxes: Sequence[tuple[tuple[int, int, int, int], str]]) -> Sheet:
+        self.MT.deselect()
+        self.MT.reselect_from_get_boxes(
+            boxes={box[0] if isinstance(box[0], tuple) else tuple(box[0]): box[1] for box in boxes}
+        )
+        return self
+
     def cell_selected(
         self,
         r: int,
         c: int,
         rows: bool = False,
         columns: bool = False,
     ) -> bool:
@@ -3019,34 +3027,34 @@
             c=column,
             **kwargs,
         )
         return self
 
     def select_row(self, row: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.RI.select_row(
-            int(row) if not isinstance(row, int) else row,
+            row if isinstance(row, int) else int(row),
             redraw=False,
             run_binding_func=run_binding_func,
         )
         self.set_refresh_timer(redraw)
         return self
 
     def select_column(self, column: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.CH.select_col(
-            int(column) if not isinstance(column, int) else column,
+            column if isinstance(column, int) else int(column),
             redraw=False,
             run_binding_func=run_binding_func,
         )
         self.set_refresh_timer(redraw)
         return self
 
     def select_cell(self, row: int, column: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.MT.select_cell(
-            int(row) if not isinstance(row, int) else row,
-            int(column) if not isinstance(column, int) else column,
+            row if isinstance(row, int) else int(row),
+            column if isinstance(column, int) else int(column),
             redraw=False,
             run_binding_func=run_binding_func,
         )
         self.set_refresh_timer(redraw)
         return self
 
     def select_all(self, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
@@ -3719,17 +3727,31 @@
     def all_columns_displayed(self, a: bool | None = None) -> bool:
         v = bool(self.MT.all_columns_displayed)
         if isinstance(a, bool):
             self.MT.all_columns_displayed = a
         return v
 
     @property
+    def all_columns(self) -> bool:
+        return self.MT.all_columns_displayed
+
+    @all_columns.setter
+    def all_columns(self, a: bool) -> Sheet:
+        self.MT.all_columns_displayed = a
+        return self
+
+    @property
     def displayed_columns(self) -> list[int]:
         return self.MT.displayed_columns
 
+    @displayed_columns.setter
+    def displayed_columns(self, columns: list[int]) -> Sheet:
+        self.display_columns(columns=columns, reset_col_positions=False, redraw=True)
+        return self
+
     # Hiding Rows
 
     def displayed_row_to_data(self, r: int) -> int:
         return r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
 
     data_r = displayed_row_to_data
     drow = displayed_row_to_data
@@ -3825,17 +3847,31 @@
     def all_rows_displayed(self, a: bool | None = None) -> bool:
         v = bool(self.MT.all_rows_displayed)
         if isinstance(a, bool):
             self.MT.all_rows_displayed = a
         return v
 
     @property
+    def all_rows(self) -> bool:
+        return self.MT.all_rows_displayed
+
+    @all_rows.setter
+    def all_rows(self, a: bool) -> Sheet:
+        self.MT.all_rows_displayed = a
+        return self
+
+    @property
     def displayed_rows(self) -> list[int]:
         return self.MT.displayed_rows
 
+    @displayed_rows.setter
+    def displayed_rows(self, rows: list[int]) -> Sheet:
+        self.display_rows(rows=rows, reset_row_positions=False, redraw=True)
+        return self
+
     # Hiding Sheet Elements
 
     def hide(
         self,
         canvas: Literal[
             "all",
             "row_index",
@@ -4238,17 +4274,15 @@
         self.MT.redo_stack = stack
         return self
 
     def redraw(self, redraw_header: bool = True, redraw_row_index: bool = True) -> Sheet:
         self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
         return self
 
-    def refresh(self, redraw_header: bool = True, redraw_row_index: bool = True) -> Sheet:
-        self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
-        return self
+    refresh = redraw
 
     # Tags
 
     def tag(
         self,
         *key: CreateSpanTypes,
         tags: Iterator[str] | str = "",
@@ -4377,15 +4411,18 @@
     # Treeview Mode
 
     def tree_build(
         self,
         data: list[list[object]],
         iid_column: int,
         parent_column: int,
+        text_column: None | int = None,
     ) -> Sheet:
+        if text_column is None:
+            text_column = iid_column
         tally_of_ids = defaultdict(lambda: -1)
         ncols = max(map(len, data), default=0)
         for rn, row in enumerate(data):
             if ncols > (lnr := len(row)):
                 row += self.MT.get_empty_row_seq(rn, end=ncols, start=lnr)
             iid, pid = row[iid_column].lower(), row[parent_column].lower()
             if not iid:
@@ -4396,31 +4433,31 @@
                 while iid in tally_of_ids:
                     new = f"{row[iid_column]}_DUPLICATED_{x}"
                     iid = new.lower()
                     x += 1
                 tally_of_ids[iid] += 1
                 row[iid_column] = new
             if iid not in self.RI.tree:
-                self.RI.tree[iid] = Node(row[iid_column], iid, "")
+                self.RI.tree[iid] = Node(row[text_column], iid, "")
             if iid == pid or self.RI.pid_causes_recursive_loop(iid, pid):
                 row[parent_column] = ""
                 pid = ""
             if pid:
                 if pid not in self.RI.tree:
-                    self.RI.tree[pid] = Node(row[parent_column], pid)
+                    self.RI.tree[pid] = Node(row[text_column], pid)
                 self.RI.tree[iid].parent = self.RI.tree[pid]
                 self.RI.tree[pid].children.append(self.RI.tree[iid])
             else:
                 self.RI.tree[iid].parent = ""
             self.RI.tree_rns[iid] = rn
         for n in self.RI.tree.values():
             if n.parent is None:
                 n.parent = ""
                 newrow = self.MT.get_empty_row_seq(len(data), ncols)
-                newrow[iid_column] = n.text
+                newrow[iid_column] = n.iid
                 self.RI.tree_rns[n.iid] = len(data)
                 data.append(newrow)
         self.insert_rows(
             idx=0,
             rows=[[self.RI.tree[iid]] + data[self.RI.tree_rns[iid]] for iid in self.get_children()],
             row_index=True,
             create_selections=False,
@@ -4446,15 +4483,15 @@
         return self.RI.tree_open_ids
 
     def tree_set_open(self, open_ids: set[str]) -> Sheet:
         """
         Accepts set[str] of iids that are open in the treeview
         Closes everything else
         """
-        self.RI.tree_open_ids = open_ids
+        self.RI.tree_open_ids = open_ids if isinstance(open_ids, set) else set(open_ids)
         self.hide_rows(
             set(self.MT.displayed_rows),
             redraw=False,
             deselect_all=False,
             data_indexes=True,
         )
         self.show_rows(
@@ -4807,16 +4844,17 @@
         """
         return [
             self.MT._row_index[self.displayed_row_to_data(rn)].iid
             for rn in self.get_selected_rows(get_cells_as_rows=cells)
         ]
 
     def selection_set(self, *items) -> Sheet:
-        self.deselect()
-        self.selection_add(*items)
+        if any(item.lower() in self.RI.tree for item in unpack(items)):
+            self.deselect()
+            self.selection_add(*items)
         return self
 
     def selection_add(self, *items) -> Sheet:
         for item in unpack(items):
             if (item := item.lower()) not in self.RI.tree:
                 continue
             if not self.item_displayed(item):
@@ -4864,20 +4902,16 @@
         for func in self.bound_events[event]:
             func(data)
 
     def set_refresh_timer(self, redraw: bool = True) -> None:
         if redraw and self.after_redraw_id is None:
             self.after_redraw_id = self.after(self.after_redraw_time_ms, self.after_redraw)
 
-    def after_redraw(
-        self,
-        redraw_header: bool = True,
-        redraw_row_index: bool = True,
-    ) -> None:
-        self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
+    def after_redraw(self) -> None:
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         self.after_redraw_id = None
 
     def del_options_using_span(
         self,
         span: Span,
         key: str,
         redraw: bool = True,
```

### Comparing `tksheet-7.1.7/tksheet/sheet_options.py` & `tksheet-7.1.8/tksheet/sheet_options.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/text_editor.py` & `tksheet-7.1.8/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/themes.py` & `tksheet-7.1.8/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/top_left_rectangle.py` & `tksheet-7.1.8/tksheet/top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.7/tksheet/vars.py` & `tksheet-7.1.8/tksheet/vars.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,24 @@
     "<<SheetModified>>",
     "<<SheetRedrawn>>",
     "<<SheetSelect>>",
 }
 backwards_compatibility_keys: dict[str, str] = {
     "font": "table_font",
 }
+text_editor_to_unbind: tuple[str] = (
+    "<Alt-Return>",
+    "<Alt-KP_Enter>",
+    "<Option-Return>",
+    "<Tab>",
+    "<Return>",
+    "<KP_Enter>",
+    "<FocusOut>",
+    "<Escape>",
+)
 scrollbar_options_keys: set[str] = {
     "vertical_scroll_background",
     "horizontal_scroll_background",
     "vertical_scroll_troughcolor",
     "horizontal_scroll_troughcolor",
     "vertical_scroll_lightcolor",
     "horizontal_scroll_lightcolor",
```

### Comparing `tksheet-7.1.7/tksheet.egg-info/PKG-INFO` & `tksheet-7.1.8/tksheet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.7
+Version: 7.1.8
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

