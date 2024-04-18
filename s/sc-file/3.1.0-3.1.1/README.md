# Comparing `tmp/sc_file-3.1.0.tar.gz` & `tmp/sc_file-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.1.0.tar", max compression
+gzip compressed data, was "sc_file-3.1.1.tar", max compression
```

## Comparing `sc_file-3.1.0.tar` & `sc_file-3.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.1.0/LICENSE
--rw-r--r--   0        0        0      795 2024-04-14 13:32:38.416625 sc_file-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     5065 2024-04-14 13:42:36.111901 sc_file-3.1.0/README.md
--rw-r--r--   0        0        0      186 2024-04-14 13:44:35.652910 sc_file-3.1.0/scfile/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.1.0/scfile/__main__.py
--rw-r--r--   0        0        0     1209 2024-04-14 13:33:45.025072 sc_file-3.1.0/scfile/consts.py
--rw-r--r--   0        0        0     1143 2024-04-14 13:45:32.018913 sc_file-3.1.0/scfile/enums.py
--rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.1.0/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.1.0/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.1.0/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.1.0/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.1.0/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.1.0/scfile/exceptions/ol.py
--rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.1.0/scfile/file/__init__.py
--rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.1.0/scfile/file/base.py
--rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.1.0/scfile/file/data.py
--rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.1.0/scfile/file/dds/encoder.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.1.0/scfile/file/dds/structure.py
--rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.1.0/scfile/file/decoder.py
--rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.1.0/scfile/file/encoder.py
--rw-r--r--   0        0        0     7342 2024-04-14 13:11:08.724324 sc_file-3.1.0/scfile/file/mcsa/decoder.py
--rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.1.0/scfile/file/mcsa/flags.py
--rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.1.0/scfile/file/mcsa/versions.py
--rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.1.0/scfile/file/mic/decoder.py
--rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.1.0/scfile/file/obj/encoder.py
--rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.1.0/scfile/file/ol/converter/base.py
--rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.1.0/scfile/file/ol/converter/bgra8.py
--rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.1.0/scfile/file/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.1.0/scfile/file/ol/decoder.py
--rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.1.0/scfile/file/ol/formats.py
--rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.1.0/scfile/file/png/encoder.py
--rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.1.0/scfile/io/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.1.0/scfile/io/base.py
--rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.1.0/scfile/io/binary.py
--rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.1.0/scfile/io/mcsa.py
--rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.1.0/scfile/io/ol.py
--rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.1.0/scfile/types.py
--rw-r--r--   0        0        0     3862 2024-04-14 13:46:22.120912 sc_file-3.1.0/scfile/utils/convert.py
--rw-r--r--   0        0        0     3027 2024-04-02 04:43:06.633771 sc_file-3.1.0/scfile/utils/model.py
--rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 sc_file-3.1.0/setup.py
--rw-r--r--   0        0        0     5579 1970-01-01 00:00:00.000000 sc_file-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.1.1/LICENSE
+-rw-r--r--   0        0        0      795 2024-04-17 23:28:14.269001 sc_file-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5065 2024-04-14 14:09:27.400282 sc_file-3.1.1/README.md
+-rw-r--r--   0        0        0      186 2024-04-14 13:44:35.652910 sc_file-3.1.1/scfile/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-14 13:10:00.131909 sc_file-3.1.1/scfile/__main__.py
+-rw-r--r--   0        0        0     1361 2024-04-14 14:13:20.447282 sc_file-3.1.1/scfile/consts.py
+-rw-r--r--   0        0        0     1143 2024-04-14 13:45:32.018913 sc_file-3.1.1/scfile/enums.py
+-rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.1.1/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.1.1/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.1.1/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/file/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.1.1/scfile/file/base.py
+-rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.1.1/scfile/file/data.py
+-rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.1.1/scfile/file/dds/encoder.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.1.1/scfile/file/dds/structure.py
+-rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.1.1/scfile/file/decoder.py
+-rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.1.1/scfile/file/encoder.py
+-rw-r--r--   0        0        0     7342 2024-04-14 13:11:08.724324 sc_file-3.1.1/scfile/file/mcsa/decoder.py
+-rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/mcsa/flags.py
+-rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.1.1/scfile/file/mcsa/versions.py
+-rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.1.1/scfile/file/mic/decoder.py
+-rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/obj/encoder.py
+-rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/base.py
+-rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.1.1/scfile/file/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.1.1/scfile/file/ol/decoder.py
+-rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/file/ol/formats.py
+-rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/file/png/encoder.py
+-rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.1.1/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/base.py
+-rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/binary.py
+-rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.1.1/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.1.1/scfile/io/ol.py
+-rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.1.1/scfile/types.py
+-rw-r--r--   0        0        0     3862 2024-04-14 13:46:22.120912 sc_file-3.1.1/scfile/utils/convert.py
+-rw-r--r--   0        0        0     3027 2024-04-02 04:43:06.633771 sc_file-3.1.1/scfile/utils/model.py
+-rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 sc_file-3.1.1/setup.py
+-rw-r--r--   0        0        0     5579 1970-01-01 00:00:00.000000 sc_file-3.1.1/PKG-INFO
```

### Comparing `sc_file-3.1.0/LICENSE` & `sc_file-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/pyproject.toml` & `sc_file-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.1.0"
+version = "3.1.1"
 description = "Utility & Library for decoding stalcraft assets"
 authors = ["onejeuu <bloodtrail@beber1k.ru>"]
 
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/onejeuu/sc-file"
```

### Comparing `sc_file-3.1.0/README.md` & `sc_file-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/__main__.py` & `sc_file-3.1.1/scfile/__main__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/consts.py` & `sc_file-3.1.1/scfile/consts.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,60 +3,74 @@
 
 class Signature:
     """
     Big-Endian Source File Signature.
     Integer.
     """
 
+    MCSA = 0x4D435341
     MIC = 0x894D4943
     OL = 0x0A9523FD
-    MCSA = 0x4D435341
 
 
 class Magic:
     """
     Big-Endian Output File Signature.
     List[Integer].
     """
 
-    PNG = [0x89, 0x50, 0x4E, 0x47]
     DDS = [0x44, 0x44, 0x53, 0x20]
+    PNG = [0x89, 0x50, 0x4E, 0x47]
 
 
 class Factor:
-    # int range + 1
+    """
+    Integer range + 1.
+    """
+
     I8 = 0x80
     U8 = 0x100
     I16 = 0x8000
     U16 = 0x10000
 
 
 class OlString:
+    """
+    Xor encoded zero-end string.
+    """
+
     SIZE = 17  # 16 bytes + last 0x00 byte
     XOR = ord("g")
     NULL = ord("G")
 
 
 class McsaModel:
+    """
+    Mcsa model constants.
+    """
+
     ROOT_BONE_ID = -1
     # I dont know specific limit
     # This is done for case when file was read incorrectly
     # So as not to overflow memory
     # ? Trees and new year toys have hundreds of thousands of vertices...
     COUNT_LIMIT = 0x100000
 
 
 class McsaSize:
-    # Number of elements in each structure
+    """
+    Count of elements in each mcsa data structure.
+    """
+
     POSITION = 4
     TEXTURE = 2
     NORMALS = 4
     POLYGONS = 3
     COLOR = 4
 
 
 # Files suffixes that can be converted
-SUPPORTED_SUFFIXES = {FileSuffix.MIC, FileSuffix.OL, FileSuffix.MCSA, FileSuffix.MCVD}
+SUPPORTED_SUFFIXES = {FileSuffix.MCSA, FileSuffix.MCVD, FileSuffix.MIC, FileSuffix.OL}
 
 # Dds cubemap faces count
 # +x, -x, +y, -y, +z, -z
 CUBEMAP_FACES = 6
```

### Comparing `sc_file-3.1.0/scfile/enums.py` & `sc_file-3.1.1/scfile/enums.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/exceptions/basic.py` & `sc_file-3.1.1/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/exceptions/decode.py` & `sc_file-3.1.1/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/exceptions/mcsa.py` & `sc_file-3.1.1/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/exceptions/ol.py` & `sc_file-3.1.1/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/base.py` & `sc_file-3.1.1/scfile/file/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/dds/encoder.py` & `sc_file-3.1.1/scfile/file/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/dds/structure.py` & `sc_file-3.1.1/scfile/file/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/decoder.py` & `sc_file-3.1.1/scfile/file/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/encoder.py` & `sc_file-3.1.1/scfile/file/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/mcsa/decoder.py` & `sc_file-3.1.1/scfile/file/mcsa/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/mcsa/flags.py` & `sc_file-3.1.1/scfile/file/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/mic/decoder.py` & `sc_file-3.1.1/scfile/file/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/obj/encoder.py` & `sc_file-3.1.1/scfile/file/obj/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/ol/converter/base.py` & `sc_file-3.1.1/scfile/file/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/file/ol/decoder.py` & `sc_file-3.1.1/scfile/file/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/io/base.py` & `sc_file-3.1.1/scfile/io/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/io/mcsa.py` & `sc_file-3.1.1/scfile/io/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/utils/convert.py` & `sc_file-3.1.1/scfile/utils/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/scfile/utils/model.py` & `sc_file-3.1.1/scfile/utils/model.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.1.0/setup.py` & `sc_file-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['build = build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'Utility & Library for decoding stalcraft assets',
     'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nDesigned for artworks creation and the like.\n\n> [!NOTE]\n> There is not and will not be encoding back into game formats.\n\n> [!WARNING]\n> Do not use game assets directly. \\\n> Any changes in game client can be detected.\n\nYou can use executable program from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Model   | .mcvd         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`.\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in same directory with a new suffix._\n\n2. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n3. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n4. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n5. Convert all `.mcsa` files in current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n6. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoded content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Recommended to create virtual environment.\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
     'author_email': 'bloodtrail@beber1k.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/onejeuu/sc-file',
```

### Comparing `sc_file-3.1.0/PKG-INFO` & `sc_file-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.1.0
+Version: 3.1.1
 Summary: Utility & Library for decoding stalcraft assets
 Home-page: https://github.com/onejeuu/sc-file
 License: MIT
 Author: onejeuu
 Author-email: bloodtrail@beber1k.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

