# Comparing `tmp/macos_pkg_builder-1.1.1-py3-none-any.whl.zip` & `tmp/macos_pkg_builder-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6094 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1098 b- defN 24-Mar-30 17:12 macos_pkg_builder/__init__.py
--rw-r--r--  2.0 unx    13455 b- defN 24-Mar-30 17:12 macos_pkg_builder/core.py
--rw-r--r--  2.0 unx     4820 b- defN 24-Mar-30 17:12 macos_pkg_builder-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-30 17:12 macos_pkg_builder-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-30 17:12 macos_pkg_builder-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      507 b- defN 24-Mar-30 17:12 macos_pkg_builder-1.1.1.dist-info/RECORD
-6 files, 19990 bytes uncompressed, 5172 bytes compressed:  74.1%
+Zip file size: 7688 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1113 b- defN 24-Apr-17 22:15 macos_pkg_builder/__init__.py
+-rw-r--r--  2.0 unx    22014 b- defN 24-Apr-17 22:15 macos_pkg_builder/core.py
+-rw-r--r--  2.0 unx     6476 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      507 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/RECORD
+6 files, 30220 bytes uncompressed, 6766 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: macos_pkg_builder/__init__.py
 Comment: 
 
 Filename: macos_pkg_builder/core.py
 Comment: 
 
-Filename: macos_pkg_builder-1.1.1.dist-info/METADATA
+Filename: macos_pkg_builder-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: macos_pkg_builder-1.1.1.dist-info/WHEEL
+Filename: macos_pkg_builder-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: macos_pkg_builder-1.1.1.dist-info/top_level.txt
+Filename: macos_pkg_builder-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: macos_pkg_builder-1.1.1.dist-info/RECORD
+Filename: macos_pkg_builder-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## macos_pkg_builder/__init__.py

```diff
@@ -11,19 +11,19 @@
     >>>     pkg_postinstall_script="Samples/MyApp/MyPostinstall.sh",
     >>>     pkg_file_structure={
     >>>         "Samples/MyApp/MyApp.app": "/Applications/MyApp.app",
     >>>         "Samples/MyApp/MyLaunchDaemon.plist": "/Library/LaunchDaemons/com.myapp.plist",
     >>>     },
     >>> )
 
-    >>> pkg_obj.build()
+    >>> assert pkg_obj.build() is True
 """
 
 __title__:        str = "macos_pkg_builder"
-__version__:      str = "1.1.1"
+__version__:      str = "1.2.0"
 __description__:  str = "macOS Package Builder Library, wrapping the `pkgbuild` and `productbuild` tools."
 __url__:          str = "https://github.com/ripeda/macOS-Pkg-Builder"
 __author__:       str = "RIPEDA Consulting"
 __author_email__: str = "info@ripeda.com"
 __status__:       str = "Production/Stable"
 __all__:         list = ["Packages"]
```

## macos_pkg_builder/core.py

```diff
@@ -2,19 +2,23 @@
 
 """
 macOS Package Builder
 
 Designed to simplify package creation through native tooling, ex. pkgbuild, productbuild, etc.
 """
 
+
 import logging
-import tempfile
+import markdown
 import plistlib
+import tempfile
 import subprocess
 
+import xml.etree.ElementTree as ET
+
 from pathlib import Path
 
 
 PKGBUILD:     str = "/usr/bin/pkgbuild"
 PRODUCTBUILD: str = "/usr/bin/productbuild"
 PRODUCTSIGN:  str = "/usr/bin/productsign"
 SECURITY:     str = "/usr/bin/security"
@@ -34,30 +38,40 @@
                  pkg_preinstall_script:   str = None,
                  pkg_preflight_script:    str = None,
                  pkg_postinstall_script:  str = None,
                  pkg_postflight_script:   str = None,
                  pkg_script_resources:   list = None,
                  pkg_signing_identity:    str = None,
                  pkg_as_distribution:    bool = False,
+                 pkg_title:               str = None,
+                 pkg_welcome:             str = None,
+                 pkg_readme:              str = None,
+                 pkg_license:             str = None,
+                 pkg_background:          str = None,
+                 pkg_background_dark:     str = None,
                 ) -> None:
         """
         pkg_output:             Path to where the package will be saved.
+                                Required.
 
         pkg_bundle_id:          Bundle ID of the package.
+                                Required.
 
         pkg_version:            Version of the package.
                                 Default: 1.0.0
+                                Optional.
 
         pkg_install_location:   Location where the package will be installed.
                                 Default: /
                                 Optional.
 
         pkg_allow_relocation:   Allow the embedded application to be installed where the user has an existing copy (outside expected install location)
                                 Requires a valid bundle to be provided in 'pkg_file_structure' (ex. app, plugin, etc.)
                                 Default: True
+                                Optional.
 
         pkg_file_structure:     File structure of the package.
                                 Configured as a dictionary, where the key is the source file and the value is the destination.
                                 Default: None
                                 Optional if preinstall or postinstall scripts are provided.
 
         pkg_preinstall_script:  Path to the preinstall script.
@@ -75,27 +89,56 @@
         pkg_postflight_script:  Path to the postflight script.
                                 Default: None
                                 Optional.
 
         pkg_script_resources:   List of additional scripts to be included in the package.
                                 This is primarily for pre/postinstall scripts that need additional resources present next to them.
                                 ex. Shipping 'desktoppr' with a wallpaper, and have the postinstall script set the wallpaper.
+                                Default: None
+                                Optional.
 
         pkg_signing_identity:   Signing identity to use when signing the package.
                                 If missing, no signing will be performed.
+                                Default: None
+                                Optional.
 
         pkg_as_distribution:    Convert the package to a product archive.
                                 Default: False
+                                Optional.
+
+        pkg_title:              Title of the distribution package.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
+
+        pkg_welcome:            Content of the WELCOME file as markdown.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
+
+        pkg_readme:             Content of the README file as markdown.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
+
+        pkg_license:            Content of the LICENSE file as markdown.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
+
+        pkg_background:         Path to the background image for the distribution package.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
+
+        pkg_background_dark:    Path to the dark background image for the distribution package.
+                                If not provided, the light background will be used.
+                                Default: None
+                                Optional. Requires 'pkg_as_distribution' to be True.
 
         File Structure:
             {
                 # Source: Destination
                 "~/Developer/MyApp.app": "/Applications/MyApp.app",
                 "~/Developer/MyLaunchDaemon.plist": "/Library/LaunchDaemons/com.myapp.plist",
-
             }
         """
 
         self._pkg_project_identifier = pkg_bundle_id
         self._pkg_project_version    = pkg_version
         self._pkg_install_location   = pkg_install_location
         self._pkg_output             = pkg_output
@@ -105,49 +148,101 @@
         self._pkg_postinstall_script = pkg_postinstall_script
         self._pkg_postflight_script  = pkg_postflight_script
         self._pkg_file_name          = Path(self._pkg_output).name
         self._pkg_allow_relocation   = pkg_allow_relocation
         self._pkg_script_resources   = pkg_script_resources
         self._pkg_signing_identity   = pkg_signing_identity
         self._pkg_as_distribution    = pkg_as_distribution
+        self._pkg_title              = pkg_title
+        self._pkg_welcome            = pkg_welcome
+        self._pkg_readme             = pkg_readme
+        self._pkg_license            = pkg_license
+        self._pkg_background         = pkg_background
+        self._pkg_background_dark    = pkg_background_dark
+
+        _requires_distribution = [
+            self._pkg_title,
+            self._pkg_welcome,
+            self._pkg_readme,
+            self._pkg_license,
+            self._pkg_background,
+            self._pkg_background_dark
+        ]
+
+        if self._pkg_as_distribution is False and any(_requires_distribution):
+            raise Exception("Distribution files require 'pkg_as_distribution' to be True.")
 
-        self._pkg_temp_directory     = tempfile.TemporaryDirectory()
-        self._pkg_temp_directory     = Path(self._pkg_temp_directory.name)
-        self._pkg_build_directory    = Path(self._pkg_temp_directory, "build")
-        self._pkg_scripts_directory  = Path(self._pkg_temp_directory, "scripts")
-        self._pkg_output_directory   = Path(self._pkg_temp_directory, "output")
+        # If a dark background is not provided, use the light background.
+        if self._pkg_background is not None and self._pkg_background_dark is None:
+            self._pkg_background_dark = self._pkg_background
+
+        self._pkg_temp_directory      = tempfile.TemporaryDirectory()
+        self._pkg_temp_directory      = Path(self._pkg_temp_directory.name)
+        self._pkg_build_directory     = Path(self._pkg_temp_directory, "build")
+        self._pkg_scripts_directory   = Path(self._pkg_temp_directory, "scripts")
+        self._pkg_output_directory    = Path(self._pkg_temp_directory, "output")
+        self._pkg_resources_directory = Path(self._pkg_temp_directory, "resources")
+
+        self._markdown_file_mapping = {
+            self._pkg_welcome: "WELCOME.html",
+            self._pkg_readme:  "README.html",
+            self._pkg_license: "LICENSE.html"
+        }
+
+        self._background_mapping = {
+            "light": {
+                "property": self._pkg_background,
+                "file": f"BACKGROUND{Path(self._pkg_background).suffix if self._pkg_background is not None else ''}",
+                "label": "background",
+            },
+            "dark": {
+                "property": self._pkg_background_dark,
+                "file": f"BACKGROUND-DARK{Path(self._pkg_background_dark).suffix if self._pkg_background_dark is not None else ''}",
+                "label": "background-darkAqua",
+            }
+        }
 
 
     def _prepare_scripts(self) -> None:
         """
         Adjusts naming and permissions of scripts to match pkgbuild requirements.
         """
 
         if self._pkg_preinstall_script is not None:
             self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
+            if not Path(self._pkg_preinstall_script).exists():
+                raise FileNotFoundError(f"Preinstall script not found: {self._pkg_preinstall_script}")
             subprocess.run([CP, self._pkg_preinstall_script, self._pkg_scripts_directory.joinpath("preinstall")])
             subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("preinstall")])
 
         if self._pkg_preflight_script is not None:
             self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
+            if not Path(self._pkg_preflight_script).exists():
+                raise FileNotFoundError(f"Preflight script not found: {self._pkg_preflight_script}")
             subprocess.run([CP, self._pkg_preflight_script, self._pkg_scripts_directory.joinpath("preflight")])
             subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("preflight")])
 
         if self._pkg_postinstall_script is not None:
             self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
+            if not Path(self._pkg_postinstall_script).exists():
+                raise FileNotFoundError(f"Postinstall script not found: {self._pkg_postinstall_script}")
             subprocess.run([CP, self._pkg_postinstall_script, self._pkg_scripts_directory.joinpath("postinstall")])
             subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("postinstall")])
 
         if self._pkg_postflight_script is not None:
             self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
+            if not Path(self._pkg_postflight_script).exists():
+                raise FileNotFoundError(f"Postflight script not found: {self._pkg_postflight_script}")
             subprocess.run([CP, self._pkg_postflight_script, self._pkg_scripts_directory.joinpath("postflight")])
             subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("postflight")])
 
         if self._pkg_script_resources is not None:
             for resources in self._pkg_script_resources:
+                if not Path(resources).exists():
+                    raise FileNotFoundError(f"Script resource not found: {resources}")
                 subprocess.run([CP, resources, self._pkg_scripts_directory])
                 subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath(Path(resources).name)])
 
 
     def _prepare_file_structure(self) -> None:
         """
         Adjusts file structure to match pkgbuild requirements.
@@ -156,24 +251,70 @@
         self._pkg_build_directory.mkdir(parents=True, exist_ok=True)
 
         if self._pkg_file_structure is None:
             return
 
         for source, destination in self._pkg_file_structure.items():
             if not Path(source).exists():
-                raise Exception(f"Source file does not exist: {source}")
+                raise FileNotFoundError(f"Source file does not exist: {source}")
 
             internal_destination = Path(f"{self._pkg_build_directory}{destination}")
 
             if not internal_destination.parent.exists():
                 internal_destination.parent.mkdir(parents=True, exist_ok=True)
 
             subprocess.run([CP, "-R", source, internal_destination])
 
 
+    def _prepare_distribution_resources(self) -> None:
+        """
+        Prepare resources for the distribution package.
+        """
+        if self._pkg_as_distribution is False:
+            return
+
+        self._prepare_markdown_resources()
+        self._prepare_background_resources()
+
+
+    def _prepare_background_resources(self) -> None:
+        """
+        Prepare background resources for the distribution package.
+        """
+        # Check if light and dark are the same, if so, only copy one.
+        if self._background_mapping["light"]["property"] == self._background_mapping["dark"]["property"]:
+            self._background_mapping["dark"]["property"] = None
+            self._background_mapping["dark"]["file"] = self._background_mapping["light"]["file"]
+
+        for background in self._background_mapping:
+            if self._background_mapping[background]["property"] is None:
+                continue
+            if not Path(self._background_mapping[background]["property"]).exists():
+                raise FileNotFoundError(f"Background image not found: {self._background_mapping[background]['property']}")
+
+            Path(self._pkg_resources_directory).mkdir(parents=True, exist_ok=True)
+            subprocess.run([CP, self._background_mapping[background]["property"], self._pkg_resources_directory.joinpath(self._background_mapping[background]["file"])])
+
+
+    def _prepare_markdown_resources(self) -> None:
+        """
+        Convert content from markdown to HTML, then save it to the resources directory.
+        """
+        for file in self._markdown_file_mapping:
+            if file is None:
+                continue
+
+            Path(self._pkg_resources_directory).mkdir(parents=True, exist_ok=True)
+
+            with open(self._pkg_resources_directory / self._markdown_file_mapping[file], "w") as f:
+                f.write("<!DOCTYPE html>\n<html>\n<head>\n<style>\nbody { font-family: -apple-system; }\n</style>\n</head>\n<body>\n")
+                f.write(markdown.markdown(file))
+                f.write("</body>\n</html>\n")
+
+
     def _generate_component_file(self) -> None:
         """
         Generate a component file to prevent the relocation of the embedded application(s).
         """
 
         bundle=""
         file = self._pkg_build_directory.parent / "component.plist"
@@ -219,14 +360,40 @@
 
 
         args.extend([self._pkg_build_directory.parent / self._pkg_file_name])
 
         return args
 
 
+    def _sync_distribution_file(self, input_file: tempfile.NamedTemporaryFile) -> None:
+        """
+        Sync the distribution file with the provided content.
+        """
+        tree = ET.parse(input_file.name)
+        root = tree.getroot()
+
+        if self._pkg_title is not None:
+            element = ET.Element("title")
+            element.text = self._pkg_title
+            root.append(element)
+
+        # Check if light and dark are the same, if so, only copy one.
+        for background in self._background_mapping:
+            element = ET.Element(self._background_mapping[background]["label"], file=self._background_mapping[background]["file"], alignment="bottomleft", scaling="tofit")
+            root.append(element)
+
+        for file in self._markdown_file_mapping:
+            if file is not None:
+                element_name = self._markdown_file_mapping[file].split(".")[0].lower()
+                element = ET.Element(element_name, file=self._markdown_file_mapping[file], mimetype="text/html")
+                root.append(element)
+
+        tree.write(input_file.name)
+
+
     def _build_pkg(self) -> bool:
         """
         Build the application package.
         """
         result = subprocess.run(self._generate_pkg_arguments(), capture_output=True)
         if result.returncode != 0:
             logging.info(result.stderr.decode("utf-8"))
@@ -291,19 +458,38 @@
     def _convert_to_product_archive(self) -> bool:
         """
         Convert the package to a product archive.
         """
         if self._pkg_as_distribution is False:
             return True
 
+        # First, synthesize the product archive.
+        distribution_file = tempfile.NamedTemporaryFile(delete=False)
         args = [
             PRODUCTBUILD,
+            "--synthesize",
             "--package", self._pkg_build_directory.parent / self._pkg_file_name,
+            distribution_file.name
+        ]
+
+        result = subprocess.run(args, capture_output=True)
+        if result.returncode != 0:
+            logging.info(result.stderr.decode("utf-8"))
+            return False
+
+        self._sync_distribution_file(distribution_file)
+
+        args = [
+            PRODUCTBUILD,
+            "--distribution", distribution_file.name,
+            "--resources", self._pkg_resources_directory,
+            "--package-path", self._pkg_build_directory.parent,
             self._pkg_build_directory.parent / Path(self._pkg_file_name + ".product")
         ]
+
         result = subprocess.run(args, capture_output=True)
         if result.returncode != 0:
             logging.info(result.stderr.decode("utf-8"))
             return False
 
         # Replace the original package with the product archive.
         Path(self._pkg_build_directory.parent / self._pkg_file_name).unlink()
@@ -322,14 +508,15 @@
 
         if Path(self._pkg_output).exists():
             logging.info(f"Removing existing package: {self._pkg_output}")
             Path(self._pkg_output).unlink()
 
         self._prepare_scripts()
         self._prepare_file_structure()
+        self._prepare_distribution_resources()
         if self._build_pkg() is False:
             logging.info("Package build failed.")
             return False
         if self._sign_pkg() is False:
             logging.info("Package signing failed.")
             return False
         if self._convert_to_product_archive() is False:
```

## Comparing `macos_pkg_builder-1.1.1.dist-info/METADATA` & `macos_pkg_builder-1.2.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: macos_pkg_builder
-Version: 1.1.1
+Version: 1.2.0
 Summary: macOS Package Builder Library, wrapping the `pkgbuild` and `productbuild` tools.
 Home-page: https://github.com/ripeda/macOS-Pkg-Builder
 Author: RIPEDA Consulting
 Author-email: info@ripeda.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: markdown
 
 # macOS-Pkg-Builder
 
 Python module for creating macOS packages more easily through native tooling (pkgbuild). Primarily developed as an alternative to [WhiteBox's Packages](http://s.sudre.free.fr/Software/Packages/about.html) for easier CI/CD integration.
 
 * [GitHub](https://github.com/ripeda/macOS-Pkg-Builder)
 * [PyPi](https://pypi.org/project/macos-pkg-builder)
@@ -20,48 +21,52 @@
 Installation:
 ```
 pip3 install macos-pkg-builder
 ```
 
 Sample invocation:
 ```py
-import macos_pkg_builder
+from macos_pkg_builder import Packages
 
-pkg_obj = macos_pkg_builder.Packages(
+pkg_obj = Packages(
     pkg_output="Sample.pkg",
     pkg_bundle_id="com.myapp.installer",
     pkg_preinstall_script="Samples/MyApp/MyPreinstall.sh",
     pkg_postinstall_script="Samples/MyApp/MyPostinstall.sh",
     pkg_file_structure={
         "Samples/MyApp/MyApp.app": "/Applications/MyApp.app",
         "Samples/MyApp/MyLaunchDaemon.plist": "/Library/LaunchDaemons/com.myapp.plist",
     },
 )
 
-pkg_obj.build()
+assert pkg_obj.build() is True
 ```
 
 
 Format of `Packages` constructor:
 ```py
 """
     pkg_output:             Path to where the package will be saved.
+                            Required.
 
     pkg_bundle_id:          Bundle ID of the package.
+                            Required.
 
     pkg_version:            Version of the package.
                             Default: 1.0.0
+                            Optional.
 
     pkg_install_location:   Location where the package will be installed.
                             Default: /
                             Optional.
 
     pkg_allow_relocation:   Allow the embedded application to be installed where the user has an existing copy (outside expected install location)
                             Requires a valid bundle to be provided in 'pkg_file_structure' (ex. app, plugin, etc.)
                             Default: True
+                            Optional.
 
     pkg_file_structure:     File structure of the package.
                             Configured as a dictionary, where the key is the source file and the value is the destination.
                             Default: None
                             Optional if preinstall or postinstall scripts are provided.
 
     pkg_preinstall_script:  Path to the preinstall script.
@@ -79,27 +84,56 @@
     pkg_postflight_script:  Path to the postflight script.
                             Default: None
                             Optional.
 
     pkg_script_resources:   List of additional scripts to be included in the package.
                             This is primarily for pre/postinstall scripts that need additional resources present next to them.
                             ex. Shipping 'desktoppr' with a wallpaper, and have the postinstall script set the wallpaper.
+                            Default: None
+                            Optional.
 
     pkg_signing_identity:   Signing identity to use when signing the package.
                             If missing, no signing will be performed.
+                            Default: None
+                            Optional.
 
     pkg_as_distribution:    Convert the package to a product archive.
                             Default: False
+                            Optional.
+
+    pkg_title:              Title of the distribution package.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
+
+    pkg_welcome:            Content of the WELCOME file as markdown.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
+
+    pkg_readme:             Content of the README file as markdown.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
+
+    pkg_license:            Content of the LICENSE file as markdown.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
+
+    pkg_background:         Path to the background image for the distribution package.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
+
+    pkg_background_dark:    Path to the dark background image for the distribution package.
+                            If not provided, the light background will be used.
+                            Default: None
+                            Optional. Requires 'pkg_as_distribution' to be True.
 
     File Structure:
         {
             # Source: Destination
             "~/Developer/MyApp.app": "/Applications/MyApp.app",
             "~/Developer/MyLaunchDaemon.plist": "/Library/LaunchDaemons/com.myapp.plist",
-
         }
 """
 ```
 
 ## Additional Supported Use Cases
 
 #### Building single-use packages that don't leave tooling behind
```
