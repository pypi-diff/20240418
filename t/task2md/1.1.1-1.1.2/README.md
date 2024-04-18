# Comparing `tmp/task2md-1.1.1.tar.gz` & `tmp/task2md-1.1.2.tar.gz`

## Comparing `task2md-1.1.1.tar` & `task2md-1.1.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 task2md-1.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.1.1/.markdownlint.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.1.1/.python-version
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.1.1/.releaserc
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.1.1/.vale.ini
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.1.1/.yamllint
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.1.1/Taskfile.project.yml
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.1.1/Taskfile.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.1.1/lychee.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.1.1/mkdocs.yml
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.1.1/requirements.lock
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/cli.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task2md.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/file.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/header.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/task.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/task/variable.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.1.1/docs/util/dir.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/__init__.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/__init__.py
--rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/file.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/header.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/index.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/task.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/template/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/util/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.1.1/src/task2md/util/dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_dir.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_file.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/test_task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/files/empty.yml
--rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/files/lint.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/__init__.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_file.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_header.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_index.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_task.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/task/test_variable.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.1.1/tests/util/test_dir.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.1.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.1.1/LICENSE
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.1.1/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 task2md-1.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.1.2/.markdownlint.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.1.2/.python-version
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.1.2/.releaserc
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.1.2/.vale.ini
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.1.2/.yamllint
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.1.2/Taskfile.project.yml
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.1.2/Taskfile.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.1.2/lychee.toml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 task2md-1.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.1.2/requirements.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/cli.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task2md.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task/file.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task/header.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task/index.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task/task.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/task/variable.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.1.2/docs/util/dir.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/__init__.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/__init__.py
+-rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/file.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/header.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/index.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/task.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/template/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/util/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.1.2/src/task2md/util/dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/test_dir.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/test_file.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/test_task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/files/empty.yml
+-rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/files/lint.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/__init__.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/test_file.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/test_header.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/test_index.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/test_task.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/task/test_variable.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.1.2/tests/util/test_dir.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.1.2/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.1.2/PKG-INFO
```

### Comparing `task2md-1.1.1/.gitlab-ci.yml` & `task2md-1.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/.pre-commit-config.yaml` & `task2md-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/Taskfile.project.yml` & `task2md-1.1.2/Taskfile.project.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/Taskfile.yml` & `task2md-1.1.2/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/requirements-dev.lock` & `task2md-1.1.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/src/task2md/task2md.py` & `task2md-1.1.2/src/task2md/task2md.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from task2md.template.file import File
 from task2md.template.index import Index
 from task2md.util.dir import Dir
 
 
 @click.group()
-@click.version_option("1.1.1", prog_name="task2md")
+@click.version_option("1.1.2", prog_name="task2md")
 def cli() -> None:
     """A CLI tool to generate markdown documentation files from Task files."""
     pass
 
 
 @cli.command()
 @click.option(
```

### Comparing `task2md-1.1.1/src/task2md/template/file.py` & `task2md-1.1.2/src/task2md/template/file.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/src/task2md/template/header.py` & `task2md-1.1.2/src/task2md/template/header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/src/task2md/template/index.py` & `task2md-1.1.2/src/task2md/template/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 | --------- | ----------- | ------ |
 """
         for file in self.task_files:
             name = file.get_filename()
             description = file.header.description
             tags = ", ".join(file.header.tags)
 
-            output += f"| [{name}]({name}) | {description} | {tags} |\n"
+            output += f"| [{name}]({name}.md) | {description} | {tags} |\n"
 
         return output + "\n"
```

### Comparing `task2md-1.1.1/src/task2md/template/task.py` & `task2md-1.1.2/src/task2md/template/task.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/src/task2md/template/variable.py` & `task2md-1.1.2/src/task2md/template/variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/src/task2md/util/dir.py` & `task2md-1.1.2/src/task2md/util/dir.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/test_dir.py` & `task2md-1.1.2/tests/test_dir.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,18 @@
         assert "| `MEX " in output
         assert "Notes:" in output
         assert "starting by dot" in output
         assert '!!! info "Requirements:' in output
         assert "    - yamllint or docker" in output
         output_index = self.get_output_content("index.md")
         assert (
-            "| [lint](lint) | A set of tasks to lint different types of files. "
+            "| [lint](lint.md) | A set of tasks to lint different types of files. "
             "| lint, docker, CI |" in output_index
         )
-        assert "| [empty](empty) | - |  |" in output_index
+        assert "| [empty](empty.md) | - |  |" in output_index
         os.remove("empty.md")
         os.remove("lint.md")
         os.remove("index.md")
 
     def test_dir_long_options_default_dir(self) -> None:
         runner = CliRunner()
         result = runner.invoke(
```

### Comparing `task2md-1.1.1/tests/test_file.py` & `task2md-1.1.2/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/test_task2md.py` & `task2md-1.1.2/tests/test_task2md.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/files/lint.yml` & `task2md-1.1.2/tests/files/lint.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/task/test_file.py` & `task2md-1.1.2/tests/task/test_file.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/task/test_header.py` & `task2md-1.1.2/tests/task/test_header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/task/test_index.py` & `task2md-1.1.2/tests/task/test_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         i.task_files.append(f1)
         i.task_files.append(f2)
         assert len(i.task_files) == 2
 
         output = i.to_md()
         assert "# Available task templates" in output
         assert "| Templates | Description | Tags   |" in output
-        assert "| [lint1](lint1) | desc1 | tag11, tag12, tag13 |" in output
-        assert "| [lint2](lint2) | desc2 | tag21, tag22 |" in output
+        assert "| [lint1](lint1.md) | desc1 | tag11, tag12, tag13 |" in output
+        assert "| [lint2](lint2.md) | desc2 | tag21, tag22 |" in output
```

### Comparing `task2md-1.1.1/tests/task/test_task.py` & `task2md-1.1.2/tests/task/test_task.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/tests/task/test_variable.py` & `task2md-1.1.2/tests/task/test_variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/LICENSE` & `task2md-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/README.md` & `task2md-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `task2md-1.1.1/pyproject.toml` & `task2md-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "task2md"
-version = "1.1.1"
+version = "1.1.2"
 description = "A program to generate markdown documentation files from Task files"
 authors = [
     { name = "FX Soubirou", email = "soubirou@yahoo.fr" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
```

### Comparing `task2md-1.1.1/PKG-INFO` & `task2md-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: task2md
-Version: 1.1.1
+Version: 1.1.2
 Summary: A program to generate markdown documentation files from Task files
 Project-URL: Homepage, https://gitlab.com/op_so/task/task2md
 Project-URL: Documentation, https://op_so.gitlab.io/task/task2md/
 Author-email: FX Soubirou <soubirou@yahoo.fr>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

