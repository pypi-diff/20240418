# Comparing `tmp/github_custom_actions-1.0.1.tar.gz` & `tmp/github_custom_actions-1.1.0.tar.gz`

## Comparing `github_custom_actions-1.0.1.tar` & `github_custom_actions-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.dev.in
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.in
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/requirements.txt
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.github/workflows/static.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/mkdocs.yml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/index.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/quick_start.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/reference.md
--rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_github_vars.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 github_custom_actions-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/requirements.dev.in
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/en/index.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/en/quick_start.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/en/reference.md
+-rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/docs/src/ru/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tests/test_action_base.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tests/test_github_vars.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 github_custom_actions-1.1.0/PKG-INFO
```

### Comparing `github_custom_actions-1.0.1/.pre-commit-config.yaml` & `github_custom_actions-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/activate.sh` & `github_custom_actions-1.1.0/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/requirements.dev.txt` & `github_custom_actions-1.1.0/requirements.dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,29 +54,29 @@
     #   pytest
     #   virtualenv
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
 isort==5.11.5
     # via pylint
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 lazy-object-proxy==1.9.0
     # via astroid
 markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocstrings
 mccabe==0.7.0
     # via pylint
 mergedeep==1.3.4
```

### Comparing `github_custom_actions-1.0.1/tasks.py` & `github_custom_actions-1.1.0/tasks.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/.github/workflows/ci.yml` & `github_custom_actions-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/.github/workflows/docs.yml` & `github_custom_actions-1.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/.github/workflows/pip_publish.yml` & `github_custom_actions-1.1.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/.github/workflows/static.yml` & `github_custom_actions-1.1.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/docs/mkdocs.yml` & `github_custom_actions-1.1.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/docs/src/en/index.md` & `github_custom_actions-1.1.0/docs/src/en/index.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/docs/src/en/quick_start.md` & `github_custom_actions-1.1.0/docs/src/en/quick_start.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,17 @@
         super().__init__(inputs=MyInputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
         self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.summary.text += (
+            self.render(
+                "### {{ inputs.my_input }}.\n"
+                "Have a nice day!"
+            )
+        )
+
+if __name__ == "__main__":
+    MyAction().run()
 ```
```

### Comparing `github_custom_actions-1.0.1/docs/src/en/images/var_ide_hover_docstring.jpg` & `github_custom_actions-1.1.0/docs/src/en/images/var_ide_hover_docstring.jpg`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/docs/src/ru/index.md` & `github_custom_actions-1.1.0/docs/src/ru/index.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/scripts/include_pyproject_requirements.py` & `github_custom_actions-1.1.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/scripts/verup.sh` & `github_custom_actions-1.1.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/src/github_custom_actions/github_vars.py` & `github_custom_actions-1.1.0/src/github_custom_actions/github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/src/github_custom_actions/inputs_outputs.py` & `github_custom_actions-1.1.0/src/github_custom_actions/inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/tests/test_github_vars.py` & `github_custom_actions-1.1.0/tests/test_github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/LICENSE.txt` & `github_custom_actions-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/README.md` & `github_custom_actions-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,23 @@
         super().__init__(inputs=MyInputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
         self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.summary.text += (
+            self.render(
+                "### {{ inputs.my_input }}.\n"
+                "Have a nice day!"
+            )
+        )
+
+if __name__ == "__main__":
+    MyAction().run()
 ```
 # Documentation
 
 [Github Custom Actions](https://andgineer.github.io/github-custom-actions/)
 
 # Developers
```

### Comparing `github_custom_actions-1.0.1/pyproject.toml` & `github_custom_actions-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.0.1/PKG-INFO` & `github_custom_actions-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -56,14 +56,23 @@
         super().__init__(inputs=MyInputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
         self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.summary.text += (
+            self.render(
+                "### {{ inputs.my_input }}.\n"
+                "Have a nice day!"
+            )
+        )
+
+if __name__ == "__main__":
+    MyAction().run()
 ```
 # Documentation
 
 [Github Custom Actions](https://andgineer.github.io/github-custom-actions/)
 
 # Developers
```

