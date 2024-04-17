# Comparing `tmp/bpp-anubis-2024.3.22.tar.gz` & `tmp/bpp_anubis-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpp-anubis-2024.3.22.tar", last modified: Wed Mar 20 19:52:12 2024, max compression
+gzip compressed data, was "bpp_anubis-2024.4.20.tar", last modified: Wed Apr 17 22:55:55 2024, max compression
```

## Comparing `bpp-anubis-2024.3.22.tar` & `bpp_anubis-2024.4.20.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 19:52:12.881856 bpp-anubis-2024.3.22/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1598 2024-03-20 19:52:12.881856 bpp-anubis-2024.3.22/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 19:52:12.879856 bpp-anubis-2024.3.22/anubis/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3801 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/account_splitter.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/arg_parser_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/copy.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/feature_file_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/parallelizer.py
--rw-rw-rw-   0 root         (0) root         (0)     8925 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/anubis/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 19:52:12.881856 bpp-anubis-2024.3.22/bpp_anubis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1598 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-20 19:52:12.000000 bpp-anubis-2024.3.22/bpp_anubis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 19:52:12.881856 bpp-anubis-2024.3.22/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1192 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 19:52:12.880856 bpp-anubis-2024.3.22/tests/
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-20 19:51:55.000000 bpp-anubis-2024.3.22/tests/test_sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:55:55.011059 bpp_anubis-2024.4.20/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-17 22:55:55.011059 bpp_anubis-2024.4.20/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:55:55.009059 bpp_anubis-2024.4.20/anubis/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/arg_parser_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3197 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/feature_file_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/parallelizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     6767 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/anubis/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:55:55.011059 bpp_anubis-2024.4.20/bpp_anubis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-17 22:55:54.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-17 22:55:55.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 22:55:54.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-17 22:55:54.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 22:55:54.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 22:55:54.000000 bpp_anubis-2024.4.20/bpp_anubis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 22:55:55.011059 bpp_anubis-2024.4.20/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:55:55.010059 bpp_anubis-2024.4.20/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-17 22:55:36.000000 bpp_anubis-2024.4.20/tests/test_sample.py
```

### Comparing `bpp-anubis-2024.3.22/LICENSE` & `bpp_anubis-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `bpp-anubis-2024.3.22/PKG-INFO` & `bpp_anubis-2024.4.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpp-anubis
-Version: 2024.3.22
+Version: 2024.4.20
 Summary: Tools for running behave tests in parallel
 Home-page: https://gitlab.com/blueprintprep/bpp-qa/utilities/anubis
 Author: matthew bahloul
 Author-email: matthew.bahloul@blueprintprep.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bpp-anubis-2024.3.22/README.rst` & `bpp_anubis-2024.4.20/README.rst`

 * *Files identical despite different names*

### Comparing `bpp-anubis-2024.3.22/anubis/__main__.py` & `bpp_anubis-2024.4.20/anubis/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,79 @@
 # __main__.py
+import logging
 import os
-import sys
 import shutil
+import sys
+from anubis import arg_parser_main, results
+from anubis.feature_file_parser import get_tests
+from anubis.parallelizer import test_runner
+from anubis.text import print_console_output
+from behave.model import Feature, Scenario, ScenarioOutline
 from datetime import datetime
 from multiprocessing import Pool
-from random import choice
-from anubis import feature_file_parser, arg_parser_main, results
-from anubis.parallelizer import command_builder, command_runner
-from anubis.copy import art, power
-import logging
 
 
-def main():
+def main() -> int:
     # Misc Setup -------------------------------------------------------------------------------------------------------
-    start = datetime.now()
+    start: datetime = datetime.now()
     args, args_unknown = arg_parser_main.parse_arguments()
-    None if args.quiet else print(choice(art) + '\nRunning Anubis  |  powered by ' + choice(power), end='\n\n')
+    print_console_output('startup_statement', **vars(args))
 
     # Set up output dirs and files -------------------------------------------------------------------------------------
     # create a directory that will contain results and be exported
-    None if args.quiet else print(f'--- Setting Up Output\n\tSending output to <{args.output}>')
-
-    if os.path.isdir(args.output):
-        shutil.rmtree(args.output)
+    print_console_output('output_statement', **vars(args))
     os.makedirs(args.output, exist_ok=True)
 
     # set up logging
     logging.basicConfig(
         filename=args.log_file,
         filemode='w',
         level=logging.DEBUG,
         format='[%(asctime)s] [%(levelname)s] %(message)s',
         datefmt='%H:%M:%S'
     )
-    root_logger = logging.getLogger()
-    root_logger.info('Args: \n\t' + "\n\t".join(a.__repr__() for a in args._get_kwargs()))
+    logger: logging.Logger = logging.getLogger()
+    logger.info('Args: \n\t' + "\n\t".join(str(a) for a in vars(args).items()))
 
     # Run the tests ----------------------------------------------------------------------------------------------------
-    if not args.quiet:
-        print('\n--- Getting Tests')
-        print('\ttests: ' + ", ".join(d for d in args.features))
-        print(f'\ttags: {", ".join(["@" + tag for group in args.tags for tag in group]) if args.tags else "n/a"}')
-
+    print_console_output('parameter_statement', **vars(args))
     # get all testable tests and run them
-    tests_to_run = feature_file_parser.get_tests(args.features, args.tags, args.unit)
+    tests_to_run: list[Feature | Scenario | ScenarioOutline] = get_tests(args.features, args.tags, args.unit)
     passed, failed, total = 0, 0, 0
-    None if args.quiet else print(f'\n--- {"PRETENDING TO RUN" if args.dry_run else "RUNNING"} TESTS')
-
-    best_split = -(-len(tests_to_run) // args.processes)
-    max_processes = min(best_split, args.processes)
-    test_split = {i: [] for i in range(max_processes)}
+    best_split: int = -(-len(tests_to_run) // args.processes)
+    max_proc: int = min(best_split, args.processes)
+    test_split: dict = {i: [] for i in range(max_proc)}
 
     # split the tests into groups
-    i = 0
+    i: int = 0
     while len(tests_to_run) > 0:
         test_split[i].append(tests_to_run.pop())
-        i = (i + 1) % max_processes
+        i = (i + 1) % max_proc
 
-    command_data = [command_builder(i, args, args_unknown, tests) for i, tests in test_split.items()]
-
-    None if args.quiet else [print(f'\t{c[0]}') for c in command_data]
-    args_for_map = [(command, args.quiet) for command, _ in command_data]
-    output_files = [output_file for _, output_file in command_data]
-
-    # run the tests
-    if not args.dry_run:
-        with Pool(processes=max_processes) as pool:
-            pool.starmap(command_runner, args_for_map)
+    # run the tests and handle the output
+    if not args.dry_run and best_split > 0:
+        print_console_output('running_statement', test_split=test_split, **vars(args))
+
+        with Pool(processes=max_proc) as pool:
+            run_args: list = [(i, args, args_unknown, [t.location.filename for t in tests]) for i, tests in test_split.items()]
+            output_files: list = pool.starmap(test_runner, run_args)
 
         results.write_result_aggregate(files=output_files, aggregate_out_file=args.aggregate)
         logging.info(f'output files: {output_files}')
 
-        # do the math to print out the results summary
-        results.write_junit(args.aggregate, args.junit)
+        # logic to print out the results
         passed, failed, total = results.get_result_values(args.aggregate)
-        results.print_result_summary(args, args.D, start, datetime.now(), passed, failed)
-        root_logger.info(f'passed: {passed}')
-        root_logger.info(f'failed: {failed}')
-
-    print()  # this just makes the output neater
-    shutil.rmtree(args.output) if args.output.endswith('.tempoutput') else None
+        results.print_result_summary(args, start, datetime.now(), passed, failed)
+        logger.info(f'passed: {passed}, failed: {failed}')
+    else:
+        print_console_output('dry_run_statement', test_split=test_split, **vars(args))
+    if args.output.endswith('.tempoutput'): shutil.rmtree(args.output)
 
     # exit correctly
     if args.pass_with_no_tests or total == 0:
-        print(f'𓃥 {"dry run" if args.dry_run else "no tests found"} --> this run passes by default 𓃥')
+        print_console_output('end_statement', **vars(args))
         return 0
-    return 0 if passed / total >= args.pass_threshold else 1
+    return 1 - int(passed/total >= args.pass_threshold)  # python boolean int to exit code
 
 
 if __name__ == '__main__':
-    sys.exit(main())  # run everything
+    sys.exit(main())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bpp-anubis-2024.3.22/anubis/feature_file_parser.py` & `bpp_anubis-2024.4.20/anubis/feature_file_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,71 @@
 import os
 from behave.model import Feature as BehaveFeature, Scenario, ScenarioOutline
 from behave.model_core import FileLocation
+from behave.parser import parse_file
 from behave.tag_expression import TagExpression
 from glob import glob
 from pathlib import Path
 
 
-def get_tests(paths, tags, unit) -> list[BehaveFeature]:
-    parsed_gherkin = parse_with_behave_parser(paths)
-    return get_testable_tests_with_behave(parsed_gherkin, tags, unit)
+def matches_tags(tags: list, tag_expression: TagExpression) -> bool:
+    """Given a list of tags and a tag expression, figure out if the tags match the tag expression"""
+    # if there are no tags or no tag expression, the test is testable
+    if not tag_expression:
+        return True
+    if not tags:
+        return False
 
+    booleans: list = []
+    for and_group in tag_expression.ands:
+        group_booleans: list = []
+        for tag in and_group:
+            if tag.startswith('-') or tag.startswith('not '):
+                group_booleans.append(tag not in tags)
+            else:
+                group_booleans.append(tag in tags)
+        booleans.append(all(group_booleans))
+    return all(booleans)
 
-def parse_with_behave_parser(paths: list) -> list[BehaveFeature]:
-    from behave.parser import parse_feature, parse_tags, parse_file
-    parsed_gherkin = []
+
+def get_tests(paths: list, tags: list, unit: str) -> list[BehaveFeature]:
+    """Given a list of feature files and tags, return a list of tests matching those criteria"""
+    parsed_gherkin = parse_tests(paths)
+    return get_testable_tests(parsed_gherkin, tags, unit)
+
+
+def parse_tests(paths: list) -> list[BehaveFeature]:
+    """Given a list of feature files parse each feature and return list of tests"""
+    parsed_gherkin: list[BehaveFeature] = []
 
     # get all paths to the feature files and take care of duplicates
-    all_paths = []
+    all_paths: list = []
     for path in paths:
-        if os.path.isfile(path):
-            all_paths.append(path)
-        else:
-            all_paths.extend(glob(f'{path}/**/*.feature', recursive=True))
-
-    all_paths = list(set([Path(str(Path(path).absolute())) for path in all_paths]))
+        all_paths.extend([path] if os.path.isfile(path) else glob(f'{path}/**/*.feature', recursive=True))
 
     # parse the feature files, remove None cases
-    for path in all_paths:
+    for path in set([Path(str(Path(path).absolute())) for path in all_paths]):
         parsed_gherkin.append(parse_file(path))
 
     return [gherkin for gherkin in parsed_gherkin if gherkin]
 
 
-def get_testable_tests_with_behave(gherkin: list[BehaveFeature], tags: list[list[str]], unit) -> list[BehaveFeature]:
-    # flatten the list of tags
-    tags = [tag for group in tags for tag in group]
+def get_testable_tests(gherkin: list[BehaveFeature], tags: list[list[str]], unit) -> list[BehaveFeature]:
+    """given a list of tests and tags, return tests that match those tags"""
+    tags: list = [tag for group in tags for tag in group]
+    testable_tests: list = []
+    expression: TagExpression = TagExpression(tags)
 
-    all_testable_items = []
-    expression = TagExpression(tags)
     if unit.lower() == 'feature':
-        all_testable_items.extend([feature for feature in gherkin if is_testable_based_on_tags(feature.tags, expression)])
+        testable_tests.extend([f for f in gherkin if matches_tags(f.tags, expression)])
     elif unit.lower() == 'scenario':
-        all_testable_items.extend([scenario for feature in gherkin for scenario in feature if is_testable_based_on_tags(scenario.effective_tags, expression)])
+        testable_tests.extend([s for feature in gherkin for s in feature if matches_tags(s.effective_tags, expression)])
     else:  # unit == 'example'
-        for feature in gherkin:
-            for scenario in feature:
-                is_testable = is_testable_based_on_tags(scenario.effective_tags, expression)
-                if isinstance(scenario, ScenarioOutline) and is_testable:
-                    for example in scenario.examples:
-                        for row in example.table.rows:
-                            setattr(row, 'location', FileLocation(f'{example.filename}', row.line))
-                    all_testable_items.extend(row for ex in scenario.examples for row in ex.table.rows)
-                elif isinstance(scenario, Scenario) and is_testable:
-                    all_testable_items.append(scenario)
-
-    [setattr(item, 'location', FileLocation(os.path.join(os.getcwd(), f'{item.location}'), item.line)) for item in all_testable_items]
-    return all_testable_items
-
-
-def is_testable_based_on_tags(tags: list, tag_expression: TagExpression) -> bool:
-    # if there are no tags or no tag expression, the test is testable
-    if not tag_expression:
-        return True
-    if not tags:
-        return False
-
-    booleans = []
-    for and_group in tag_expression.ands:
-        group_booleans = []
-        for tag in and_group:
-            if tag.startswith('-') or tag.startswith('not '):
-                group_booleans.append(tag not in tags)
-            else:
-                group_booleans.append(tag in tags)
-        booleans.append(all(group_booleans))
-    return all(booleans)
+        for s in [s for feature in gherkin for s in feature if matches_tags(s.effective_tags, expression)]:
+            if isinstance(s, ScenarioOutline):
+                for example, row in [(e, r) for e in s.examples for r in e.table.rows]:
+                    setattr(row, 'location', FileLocation(f'{example.filename}', row.line))
+                testable_tests.extend(row for ex in s.examples for row in ex.table.rows)
+            elif isinstance(s, Scenario):
+                testable_tests.append(s)
+    [setattr(item, 'location', FileLocation(os.path.join(os.getcwd(), f'{item.location}'), item.line)) for item in testable_tests]
+    return testable_tests
```

### Comparing `bpp-anubis-2024.3.22/bpp_anubis.egg-info/PKG-INFO` & `bpp_anubis-2024.4.20/bpp_anubis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpp-anubis
-Version: 2024.3.22
+Version: 2024.4.20
 Summary: Tools for running behave tests in parallel
 Home-page: https://gitlab.com/blueprintprep/bpp-qa/utilities/anubis
 Author: matthew bahloul
 Author-email: matthew.bahloul@blueprintprep.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bpp-anubis-2024.3.22/setup.py` & `bpp_anubis-2024.4.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="bpp-anubis",
-    version="2024.3.22",
+    version="2024.4.20",
     url="https://gitlab.com/blueprintprep/bpp-qa/utilities/anubis",
     license='MIT',
 
     author="matthew bahloul",
     author_email="matthew.bahloul@blueprintprep.com",
 
     description="Tools for running behave tests in parallel",
```

