# Comparing `tmp/pulumi_archive-0.0.6a1713330587.tar.gz` & `tmp/pulumi_archive-0.0.6a1713444532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_archive-0.0.6a1713330587.tar", last modified: Wed Apr 17 05:12:07 2024, max compression
+gzip compressed data, was "pulumi_archive-0.0.6a1713444532.tar", last modified: Thu Apr 18 12:51:20 2024, max compression
```

## Comparing `pulumi_archive-0.0.6a1713330587.tar` & `pulumi_archive-0.0.6a1713444532.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:12:07.603336 pulumi_archive-0.0.6a1713330587/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 05:12:07.603336 pulumi_archive-0.0.6a1713330587/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:12:07.603336 pulumi_archive-0.0.6a1713330587/pulumi_archive/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:12:07.603336 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 05:12:07.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-17 05:12:07.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:12:07.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:12:07.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 05:12:07.000000 pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 05:12:01.000000 pulumi_archive-0.0.6a1713330587/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:12:07.603336 pulumi_archive-0.0.6a1713330587/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:20.911896 pulumi_archive-0.0.6a1713444532/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 12:51:20.907896 pulumi_archive-0.0.6a1713444532/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:20.907896 pulumi_archive-0.0.6a1713444532/pulumi_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17891 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:20.907896 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 12:51:20.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 12:51:20.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:51:20.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 12:51:20.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:51:20.000000 pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 12:51:13.000000 pulumi_archive-0.0.6a1713444532/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:51:20.911896 pulumi_archive-0.0.6a1713444532/setup.cfg
```

### Comparing `pulumi_archive-0.0.6a1713330587/PKG-INFO` & `pulumi_archive-0.0.6a1713444532/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.0.6a1713330587
+Version: 0.0.6a1713444532
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_archive-0.0.6a1713330587/README.md` & `pulumi_archive-0.0.6a1713444532/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/__init__.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/_inputs.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/_utilities.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/file.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/get_file.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/get_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -260,60 +260,14 @@
              source_file: Optional[str] = None,
              sources: Optional[Sequence[pulumi.InputType['GetFileSourceArgs']]] = None,
              type: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFileResult:
     """
     Generates an archive from content, a file, or directory of files.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    init = archive.get_file(output_path=f"{path['module']}/files/init.zip",
-        source_file=f"{path['module']}/init.tpl",
-        type="zip")
-    ```
-    <!--End PulumiCodeChooser -->
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    dotfiles = archive.get_file(type="zip",
-        output_path=f"{path['module']}/files/dotfiles.zip",
-        excludes=[f"{path['module']}/unwanted.zip"],
-        sources=[
-            archive.GetFileSourceArgs(
-                content=data["template_file"]["vimrc"]["rendered"],
-                filename=".vimrc",
-            ),
-            archive.GetFileSourceArgs(
-                content=data["template_file"]["ssh_config"]["rendered"],
-                filename=".ssh/config",
-            ),
-        ])
-    ```
-    <!--End PulumiCodeChooser -->
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    lambda_my_function = archive.get_file(output_file_mode="0666",
-        output_path=f"{path['module']}/files/lambda-my-function.js.zip",
-        source_file=f"{path['module']}/../lambda/my-function/index.js",
-        type="zip")
-    ```
-    <!--End PulumiCodeChooser -->
-
 
     :param bool exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to `false`.
     :param Sequence[str] excludes: Specify files to ignore when reading the `source_dir`.
     :param str output_file_mode: String that specifies the octal file mode for all archived files. For example: `"0666"`. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
     :param str output_path: The output of the archive file.
     :param str source_content: Add only this content to the archive with `source_content_filename` as the filename. One and only one of `source`, `source_content_filename` (with `source_content`), `source_file`, or `source_dir` must be specified.
     :param str source_content_filename: Set this as the filename when using `source_content`. One and only one of `source`, `source_content_filename` (with `source_content`), `source_file`, or `source_dir` must be specified.
@@ -368,60 +322,14 @@
                     source_file: Optional[pulumi.Input[Optional[str]]] = None,
                     sources: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetFileSourceArgs']]]]] = None,
                     type: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFileResult]:
     """
     Generates an archive from content, a file, or directory of files.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    init = archive.get_file(output_path=f"{path['module']}/files/init.zip",
-        source_file=f"{path['module']}/init.tpl",
-        type="zip")
-    ```
-    <!--End PulumiCodeChooser -->
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    dotfiles = archive.get_file(type="zip",
-        output_path=f"{path['module']}/files/dotfiles.zip",
-        excludes=[f"{path['module']}/unwanted.zip"],
-        sources=[
-            archive.GetFileSourceArgs(
-                content=data["template_file"]["vimrc"]["rendered"],
-                filename=".vimrc",
-            ),
-            archive.GetFileSourceArgs(
-                content=data["template_file"]["ssh_config"]["rendered"],
-                filename=".ssh/config",
-            ),
-        ])
-    ```
-    <!--End PulumiCodeChooser -->
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_archive as archive
-
-    lambda_my_function = archive.get_file(output_file_mode="0666",
-        output_path=f"{path['module']}/files/lambda-my-function.js.zip",
-        source_file=f"{path['module']}/../lambda/my-function/index.js",
-        type="zip")
-    ```
-    <!--End PulumiCodeChooser -->
-
 
     :param bool exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to `false`.
     :param Sequence[str] excludes: Specify files to ignore when reading the `source_dir`.
     :param str output_file_mode: String that specifies the octal file mode for all archived files. For example: `"0666"`. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
     :param str output_path: The output of the archive file.
     :param str source_content: Add only this content to the archive with `source_content_filename` as the filename. One and only one of `source`, `source_content_filename` (with `source_content`), `source_file`, or `source_dir` must be specified.
     :param str source_content_filename: Set this as the filename when using `source_content`. One and only one of `source`, `source_content_filename` (with `source_content`), `source_file`, or `source_dir` must be specified.
```

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/outputs.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive/provider.py` & `pulumi_archive-0.0.6a1713444532/pulumi_archive/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.6a1713330587/pulumi_archive.egg-info/PKG-INFO` & `pulumi_archive-0.0.6a1713444532/pulumi_archive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.0.6a1713330587
+Version: 0.0.6a1713444532
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_archive-0.0.6a1713330587/pyproject.toml` & `pulumi_archive-0.0.6a1713444532/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_archive"
   description = "A Pulumi package for creating and managing Archive cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.6a1713330587"
+  version = "0.0.6a1713444532"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-archive"
 
 [build-system]
```

