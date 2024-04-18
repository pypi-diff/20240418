# Comparing `tmp/ansys_pre_commit_hooks-0.2.9.tar.gz` & `tmp/ansys_pre_commit_hooks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_pre_commit_hooks-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_pre_commit_hooks-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_pre_commit_hooks-0.2.9.tar` & `ansys_pre_commit_hooks-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/LICENSE
--rw-r--r--   0        0        0    11642 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/README.rst
--rw-r--r--   0        0        0     2118 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1458 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0    19674 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/add_license_headers.py
--rw-r--r--   0        0        0     1245 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2
--rw-r--r--   0        0        0     1091 2024-02-16 19:13:56.910412 ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt
--rw-r--r--   0        0        0    13233 1970-01-01 00:00:00.000000 ansys_pre_commit_hooks-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11642 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/README.rst
+-rw-r--r--   0        0        0     2928 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1458 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0    23610 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/add_license_headers.py
+-rw-r--r--   0        0        0     1245 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2
+-rw-r--r--   0        0        0     1091 2024-04-18 13:36:48.559685 ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    13089 1970-01-01 00:00:00.000000 ansys_pre_commit_hooks-0.3.0/PKG-INFO
```

### Comparing `ansys_pre_commit_hooks-0.2.9/LICENSE` & `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.2.9/README.rst` & `ansys_pre_commit_hooks-0.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 Set custom arguments
 ^^^^^^^^^^^^^^^^^^^^
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-   rev: v0.2.9
+   rev: v0.3.0
    hooks:
    - id: add-license-headers
      args: ["--custom_copyright", "custom copyright phrase", "--custom_template", "template_name", "--custom_license", "license_name", "--ignore_license_check", "--start_year", "2023"]
 
 ``args`` can also be formatted as follows:
 
 .. code:: yaml
@@ -125,28 +125,28 @@
 directories named ``src``, ``examples``, and ``tests``. To specify additional files and/or directories
 the hook should run on, add the necessary regex to the ``files`` line in your
 .pre-commit-config.yaml file:
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-     rev: v0.2.9
+     rev: v0.3.0
      hooks:
      - id: add-license-headers
        files: '(src|examples|tests|newFolder)/.*\.(py|newExtension)|\.(proto|newExtension)'
 
 Ignore specific files or file types
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 In .pre-commit-config.yaml:
 
 .. code:: yaml
 
   - repo: https://github.com/ansys/pre-commit-hooks
-    rev: v0.2.9
+    rev: v0.3.0
     hooks:
     - id: add-license-headers
       exclude: |
           (?x)^(
               path/to/file1.py |
               path/to/.*\.(ts|cpp) |
               (.folder1|folder2)/.* |
```

### Comparing `ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/__init__.py` & `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/add_license_headers.py` & `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/add_license_headers.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import pathlib
 from platform import python_version
 import shutil
 import sys
 from tempfile import NamedTemporaryFile
 
 import git
-from reuse import _util, header, lint, project
+from reuse import _annotate, _util, lint, project
 
 DEFAULT_TEMPLATE = "ansys"
 """Default template to use for license headers."""
 DEFAULT_COPYRIGHT = "ANSYS, Inc. and/or its affiliates."
 """Default copyright line for license headers."""
 DEFAULT_LICENSE = "MIT"
 """Default license for headers."""
@@ -82,15 +82,15 @@
     # Get custom license
     parser.add_argument(
         "--custom_license",
         type=str,
         help="Default license for headers.",
         default=DEFAULT_LICENSE,
     )
-    # Get custom license
+    # Get the start year
     parser.add_argument(
         "--start_year",
         type=str,
         help="Start year for copyright line in headers.",
         default=DEFAULT_START_YEAR,
     )
     # Ignore license check by default is False when action='store_true'
@@ -196,20 +196,14 @@
     missing_headers = set(lint_json["non_compliant"]["missing_copyright_info"])
 
     # If ignore_license_check is False, check files for missing licensing information
     if not args.ignore_license_check:
         missing_licensing_info = set(lint_json["non_compliant"]["missing_licensing_info"])
         missing_headers = missing_headers.union(missing_licensing_info)
 
-        if lint_json["non_compliant"]["missing_licenses"]:
-            missing_licenses = set(
-                lint_json["non_compliant"]["missing_licenses"][args.custom_license]
-            )
-            missing_headers = missing_headers.union(missing_licenses)
-
     # Remove temporary file
     os.remove(filename)
 
     return missing_headers
 
 
 def set_header_args(
@@ -240,17 +234,17 @@
     -------
     argparse.Namespace
         Namespace of arguments with their values.
     """
     # Provide values for license header arguments
     args = parser.parse_args([file_path])
     if start_year == current_year:
-        args.year = [str(current_year)]
+        args.year = [current_year]
     else:
-        args.year = [start_year, str(current_year)]
+        args.year = [int(start_year), current_year]
     args.copyright_style = "string-c"
     args.copyright = [copyright]
     args.merge_copyrights = True
     args.template = template
     args.skip_unrecognised = True
     args.parser = parser
 
@@ -292,56 +286,49 @@
     """
     files = values["files"]
     start_year = values["start_year"]
     current_year = values["current_year"]
     copyright = values["copyright"]
     template = values["template"]
 
-    if i < len(files):
+    for file in files:
+        args = set_header_args(parser, start_year, current_year, file, copyright, template)
         # If the committed file is in missing_headers
-        if (files[i] in missing_headers) or (os.path.getsize(files[i]) == 0):
+        if (file in missing_headers) or (os.path.getsize(file) == 0):
             changed_headers = 1
             # Run REUSE on the file
-            args = set_header_args(parser, start_year, current_year, files[i], copyright, template)
             if not args.ignore_license_check:
                 args.license = [values["license"]]
-            header.run(args, proj)
 
-            # Check if the next file is in missing_headers
-            return check_exists(changed_headers, parser, values, proj, missing_headers, i + 1)
+            _annotate.run(args, proj)
         else:
-            # Save current copy of files[i]
+            # Save current copy of file
             before_hook = NamedTemporaryFile(mode="w", delete=False).name
-            shutil.copyfile(files[i], before_hook)
+            shutil.copyfile(file, before_hook)
 
             # Update the header
             # tmp captures the stdout of the header.run() function
             with NamedTemporaryFile(mode="w", delete=True) as tmp:
-                args = set_header_args(
-                    parser, start_year, current_year, files[i], copyright, template
-                )
-                header.run(args, proj, tmp)
+                _annotate.run(args, proj, tmp)
 
             # Check if the file before add-license-headers was run is the same as the one
             # after add-license-headers was run. If not, apply the syntax changes
             # from other hooks before add-license-headers was run to the file
-            if check_same_content(before_hook, files[i]) == False:
-                add_hook_changes(before_hook, files[i])
+            if check_same_content(before_hook, file) == False:
+                add_hook_changes(before_hook, file)
 
             # Check if the file content before add-license-headers was run has been changed
             # Assuming the syntax was fixed in the above if statement, this check is
             # solely for the file's content
-            if check_same_content(before_hook, files[i]) == False:
+            if check_same_content(before_hook, file) == False:
                 changed_headers = 1
-                print(f"Successfully changed header of {files[i]}")
+                print(f"Successfully changed header of {file}")
 
             os.remove(before_hook)
 
-            return check_exists(changed_headers, parser, values, proj, missing_headers, i + 1)
-
     return changed_headers
 
 
 def check_same_content(before_hook, after_hook):
     """
     Check if file before the hook ran is the same as after the hook ran.
 
@@ -443,14 +430,107 @@
             full_path_files.append(os.path.abspath(os.path.join(*split_str)))
         else:
             full_path_files.append(os.path.abspath(file))
 
     return full_path_files
 
 
+def update_license_file(arg_dict):
+    """
+    Update the LICENSE file to match MIT.txt, adjusting the year span to each repository.
+
+    Parameters
+    ----------
+    arg_dict: dict
+        Dictionary containing the committed files, custom copyright, template, license,
+        changed_headers, start & end year, and git_repo
+    """
+    # Get location of LICENSE file in the repository the hook runs on
+    git_root = arg_dict["git_repo"].git.rev_parse("--show-toplevel")
+    repo_license_loc = os.path.join(git_root, "LICENSE").replace(os.sep, "/")
+    save_repo_license = shutil.copyfile(repo_license_loc, f"{repo_license_loc}_save")
+
+    # Get the location of MIT.txt in the hook's assets folder
+    hook_loc = pathlib.Path(__file__).parent.resolve()
+    hook_license_file = os.path.join(hook_loc, "assets", "LICENSES", f"{DEFAULT_LICENSE}.txt")
+
+    # Copy MIT.txt from the assets folder to the LICENSE file in the repository
+    if os.path.isfile(repo_license_loc) and (arg_dict["license"] == DEFAULT_LICENSE):
+        shutil.copyfile(hook_license_file, repo_license_loc)
+
+    # Whether or not the year in LICENSE was updated
+    # 0 is unchanged, 1 is changed
+    changed = 0
+
+    # Check if custom_license is MIT
+    if os.path.isfile(repo_license_loc) and (arg_dict["license"] == DEFAULT_LICENSE):
+        if "3.9" in python_version():
+            file = fileinput.input(repo_license_loc, inplace=True)
+        else:
+            file = fileinput.input(repo_license_loc, inplace=True, encoding="utf8")
+
+        copyright = arg_dict["copyright"]
+        start_year = str(arg_dict["start_year"])
+        current_year = str(arg_dict["current_year"])
+
+        for line in file:
+            if copyright in line:
+                # Copyright line: "Copyright (c) 2023 - 2024 ANSYS, Inc. and/or its affiliates."
+                # Get the index of the closing parenthesis of the copyright line
+                paren_index = line.index(")") + 2
+                # Get the index of the start of the copyright statement
+                cpright_index = line.index(copyright) - 1
+                # Create the year string to be replaced in the copyright line
+                # For example, "2024", or "2023 - 2024"
+                year_range = (
+                    f"{start_year} - {current_year}"
+                    if (start_year != current_year)
+                    else current_year
+                )
+
+                # If the start and end year are different
+                if start_year != current_year:
+                    if "-" in line:
+                        # Get the index of the dash in the year range of the LICENSE file
+                        dash_index = line.index("-") - 1
+                        # Get the start year of the existing copyright line in the LICENSE file
+                        existing_start_year = line[paren_index:dash_index]
+                        # If the start year argument and the existing start year are different,
+                        # replace the existing start year with the new one.
+                        # For example, the existing start year is 2023, but the start_year
+                        # argument is 2022.
+                        if start_year != existing_start_year:
+                            line = line.replace(existing_start_year, start_year)
+                    else:
+                        # Replace the existing copyright years with the new year_range
+                        line = line.replace(line[paren_index:cpright_index], year_range)
+                    print(line.rstrip())
+                else:
+                    if "-" in line:
+                        # If there is a year range in the existing LICENSE file, but the
+                        # start_year and current_year are the same, remove the year range
+                        # and replace it with the current year
+                        line = line.replace(line[paren_index:cpright_index], current_year)
+                    print(line.rstrip())
+            else:
+                print(line.rstrip())
+
+    fileinput.close()
+
+    # If the year changed, print a message that the LICENSE file was changed
+    if not check_same_content(save_repo_license, repo_license_loc):
+        changed = 1
+        print(f"Successfully updated year in {repo_license_loc}")
+
+    # Remove the temporary file
+    os.remove(save_repo_license)
+
+    return changed
+
+
 def cleanup(assets: dict, os_git_root: str) -> None:
     """
     Unlink the default asset files, and remove directories if empty.
 
     Parameters
     ----------
     assets: dict
@@ -512,14 +592,17 @@
         "template": args.custom_template,
         "license": args.custom_license,
         "start_year": args.start_year,
         "current_year": dt.today().year,
         "git_repo": git_repo,
     }
 
+    # Update the year in the copyright line of the LICENSE file
+    license_return_code = update_license_file(values)
+
     # Run REUSE on root of the repository
     git_root = values["git_repo"].git.rev_parse("--show-toplevel")
 
     # git_root with correct line separators for operating system
     os_git_root = git_root.replace("/", os.sep)
 
     # Dictionary containing the asset folder information
@@ -534,35 +617,36 @@
         },
     }
 
     # Add header arguments to parser. Arguments are: copyright, license, contributor,
     # year, style, copyright-style, template, exclude-year, merge-copyrights, single-line,
     # multi-line, explicit-license, force-dot-license, recursive, no-replace,
     # skip-unrecognized, and skip-existing
-    header.add_arguments(parser)
+    # header.add_arguments(parser)
+    _annotate.add_arguments(parser)
 
     # Link the default template and/or license from the assets folder to your git repo.
     link_assets(assets, os_git_root, args)
 
     # Project to run `REUSE <https://reuse.software/>`_ on
     proj = project.Project(git_root)
 
     # Get files missing headers (copyright and/or license information)
     missing_headers = list(list_noncompliant_files(args, proj))
 
     # Add or update headers of required files.
     # Return 1 if files were added or updated, and return 0 if no files were altered.
-    return_code = check_exists(changed_headers, parser, values, proj, missing_headers, 0)
+    file_return_code = check_exists(changed_headers, parser, values, proj, missing_headers, 0)
 
     # Unlink default files & remove .reuse and LICENSES folders if empty
     cleanup(assets, os_git_root)
 
-    # Returns 1 if REUSE changes noncompliant files
+    # Returns 1 if REUSE changes noncompliant files or the year was updated in LICENSE
     # Returns 0 if all files are compliant
-    return return_code
+    return 1 if (license_return_code or file_return_code) == 1 else 0
 
 
 def main():
     """Find files missing license headers and run `REUSE <https://reuse.software/>`_ on them."""
     return find_files_missing_header()
```

### Comparing `ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2` & `ansys_pre_commit_hooks-0.3.0/src/ansys/pre_commit_hooks/assets/.reuse/templates/ansys.jinja2`

 * *Files identical despite different names*

### Comparing `ansys_pre_commit_hooks-0.2.9/src/ansys/pre_commit_hooks/assets/LICENSES/MIT.txt` & `ansys_pre_commit_hooks-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 ANSYS, Inc. and/or its affiliates.
+Copyright (c) 2023 - 2024 ANSYS, Inc. and/or its affiliates.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `ansys_pre_commit_hooks-0.2.9/PKG-INFO` & `ansys_pre_commit_hooks-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: ansys-pre-commit-hooks
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python wrapper to create Ansys-tailored pre-commit hooks
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: importlib-metadata==7.0.1
-Requires-Dist: reuse==2.1.0
-Requires-Dist: GitPython==3.1.41
-Requires-Dist: ansys-sphinx-theme==0.13.3 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
+Requires-Dist: importlib-metadata==7.1.0
+Requires-Dist: reuse==3.0.2
+Requires-Dist: GitPython==3.1.43
+Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: sphinx-autoapi==3.0.0 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==2.0.0 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==2.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: pytest==8.0.0 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: reuse==2.1.0 ; extra == "tests"
-Requires-Dist: GitPython==3.1.41 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Documentation, https://pre-commit-hooks.docs.ansys.com
 Project-URL: Homepage, https://github.com/ansys/pre-commit-hooks
 Project-URL: Source, https://github.com/ansys/pre-commit-hooks
 Project-URL: Tracker, https://github.com/ansys/pre-commit-hooks/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
@@ -115,15 +112,15 @@
 
 Set custom arguments
 ^^^^^^^^^^^^^^^^^^^^
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-   rev: v0.2.9
+   rev: v0.3.0
    hooks:
    - id: add-license-headers
      args: ["--custom_copyright", "custom copyright phrase", "--custom_template", "template_name", "--custom_license", "license_name", "--ignore_license_check", "--start_year", "2023"]
 
 ``args`` can also be formatted as follows:
 
 .. code:: yaml
@@ -160,28 +157,28 @@
 directories named ``src``, ``examples``, and ``tests``. To specify additional files and/or directories
 the hook should run on, add the necessary regex to the ``files`` line in your
 .pre-commit-config.yaml file:
 
 .. code:: yaml
 
    - repo: https://github.com/ansys/pre-commit-hooks
-     rev: v0.2.9
+     rev: v0.3.0
      hooks:
      - id: add-license-headers
        files: '(src|examples|tests|newFolder)/.*\.(py|newExtension)|\.(proto|newExtension)'
 
 Ignore specific files or file types
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 In .pre-commit-config.yaml:
 
 .. code:: yaml
 
   - repo: https://github.com/ansys/pre-commit-hooks
-    rev: v0.2.9
+    rev: v0.3.0
     hooks:
     - id: add-license-headers
       exclude: |
           (?x)^(
               path/to/file1.py |
               path/to/.*\.(ts|cpp) |
               (.folder1|folder2)/.* |
```

