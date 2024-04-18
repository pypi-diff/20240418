# Comparing `tmp/sts_lib-0.25.0.tar.gz` & `tmp/sts_lib-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.25.0.tar", last modified: Tue Apr 16 13:29:13 2024, max compression
+gzip compressed data, was "sts_lib-0.26.0.tar", last modified: Thu Apr 18 15:53:22 2024, max compression
```

## Comparing `sts_lib-0.25.0.tar` & `sts_lib-0.26.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.151542 sts_lib-0.25.0/
--rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts_lib-0.25.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-15 22:41:48.000000 sts_lib-0.25.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7705 2024-04-16 13:29:13.150543 sts_lib-0.25.0/PKG-INFO
--rw-rw-rw-   0        0        0     6252 2024-04-16 13:28:10.000000 sts_lib-0.25.0/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-16 13:29:13.152541 sts_lib-0.25.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-15 22:41:48.000000 sts_lib-0.25.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.095598 sts_lib-0.25.0/sts/
--rw-rw-rw-   0        0        0    43731 2024-04-16 13:28:21.000000 sts_lib-0.25.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7754 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.096597 sts_lib-0.25.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.115578 sts_lib-0.25.0/sts/data/config/
--rw-rw-rw-   0        0        0      723 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      383 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      289 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      337 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      303 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      215 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      301 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      383 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      211 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      225 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      215 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      209 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      381 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      426 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      287 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.135558 sts_lib-0.25.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    21142 2024-04-16 13:23:40.000000 sts_lib-0.25.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.138554 sts_lib-0.25.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-15 22:41:48.000000 sts_lib-0.25.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 13:29:13.148544 sts_lib-0.25.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     7705 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-16 13:29:13.000000 sts_lib-0.25.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.094695 sts_lib-0.26.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-18 15:53:10.000000 sts_lib-0.26.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-18 15:53:10.000000 sts_lib-0.26.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7669 2024-04-18 15:53:22.093691 sts_lib-0.26.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6216 2024-04-18 15:53:10.000000 sts_lib-0.26.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-18 15:53:22.095690 sts_lib-0.26.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-18 15:53:10.000000 sts_lib-0.26.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.048737 sts_lib-0.26.0/sts/
+-rw-rw-rw-   0        0        0    43558 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.049736 sts_lib-0.26.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.064741 sts_lib-0.26.0/sts/data/config/
+-rw-rw-rw-   0        0        0      723 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      383 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      289 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      337 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      303 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      215 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      301 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      383 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      211 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      225 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      215 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      209 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      381 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      427 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      287 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.080705 sts_lib-0.26.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    21185 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.083701 sts_lib-0.26.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-18 15:53:10.000000 sts_lib-0.26.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 15:53:22.091693 sts_lib-0.26.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     7669 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-18 15:53:21.000000 sts_lib-0.26.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.25.0/LICENSE` & `sts_lib-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/PKG-INFO` & `sts_lib-0.26.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.25.0
+Version: 0.26.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -112,17 +112,17 @@
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
  * @property {string} file - path of the dictionary file to generate, as an
- *     absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). It should be a .tlist (compiled
- *     trie), .jlist (compiled table), or .list (plain text table).
+ *     absolute path, or a path relative to the directory of this config file.
+ *     It should be a .tlist (compiled trie), .jlist (compiled table), or .list
+ *     (plain text table).
  * @property {string} [mode=load] - the mode to handle the loaded source files:
  *     "load" to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} [src] - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
```

### Comparing `sts_lib-0.25.0/README.md` & `sts_lib-0.26.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -77,17 +77,17 @@
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
  * @property {string} file - path of the dictionary file to generate, as an
- *     absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). It should be a .tlist (compiled
- *     trie), .jlist (compiled table), or .list (plain text table).
+ *     absolute path, or a path relative to the directory of this config file.
+ *     It should be a .tlist (compiled trie), .jlist (compiled table), or .list
+ *     (plain text table).
  * @property {string} [mode=load] - the mode to handle the loaded source files:
  *     "load" to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} [src] - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
```

### Comparing `sts_lib-0.25.0/setup.cfg` & `sts_lib-0.26.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/__init__.py` & `sts_lib-0.26.0/sts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.25.0'
+__version__ = '0.26.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -171,23 +171,23 @@
                     length += 1
 
             i += 1
             length -= 1
 
         return i - pos
 
-    @staticmethod
-    def split(text):
+    @classmethod
+    def split(cls, text):
         """Split a text into a list of Unicode composites.
         """
         i = 0
         total = len(text)
         result = []
         while i < total:
-            length = Unicode.composite_length(text, i)
+            length = cls.composite_length(text, i)
             result.append(text[i:i + length])
             i += length
         return result
 
 
 class StsDict():
     """Base class of an STS dictionary.
@@ -904,28 +904,28 @@
 
 class StsMaker():
     """A class for making dictionary file(s).
     """
     config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
     dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
 
-    def make(self, config_name, base_dir=None, output_dir=None,
+    def make(self, config_name, base_dir=None,
              skip_check=False, skip_requires=False, quiet=False):
         """Make dictionary file(s) according to a config.
 
         scheme of config (.json):
             {
                 "name": "...",
                 "requires": [
                     "..."  // a required config (relative to this config file)
                 ],
                 "dicts": [  // dictionaries to generate
                     {
                         "file": "...",  // path of the generated dictionary
-                                        // file, relative to output_dir
+                                        // file, relative to config dir
                         "mode": "...",  // mode to handle the loaded sources:
                                         // load, swap, join
                         "src": ["...", ...]  // list of the source file paths,
                                              // should be .txt or .list files
                         "sort": true,   // truthy to sort the keys of the
                                         // generated dictionary
                         "include": "...",  // regex filter for output values
@@ -936,16 +936,14 @@
                 ]
             }
 
         Args:
             config_name: a str for the config file or name
             base_dir: a str for the base directory to parse the config path
                 from config_name, or None for CWD
-            output_dir: a str for the output directory, or None for
-                the directory of the config file
             skip_check: truthy to generate every dictionary no matter that it's
                 already up-to-date
             skip_requires: truthy to skip making from required configs
             quiet: truthy to skip reporting details
 
         Returns:
             a str for the path of the last generated dictionary file
@@ -956,19 +954,19 @@
 
         with open(config_file, 'r', encoding='UTF-8') as fh:
             config = json.load(fh)
 
         # handle required configs
         if not skip_requires:
             for cf in config.get('requires', []):
-                self.make(cf, base_dir=config_dir, output_dir=output_dir, skip_requires=skip_requires, quiet=quiet)
+                self.make(cf, base_dir=config_dir, skip_requires=skip_requires, quiet=quiet)
 
         # make the requested dicts
         for dict_ in config['dicts']:
-            dest = os.path.normpath(os.path.join(output_dir or config_dir, dict_['file']))
+            dest = os.path.normpath(os.path.join(config_dir, dict_['file']))
             format = os.path.splitext(dest)[1][1:].lower()
             mode = dict_.get('mode', 'load')
             src = dict_.get('src', [])
             sort = dict_.get('sort', False)
             include = dict_.get('include', None)
             exclude = dict_.get('exclude', None)
             check = dict_.get('check', False)
```

### Comparing `sts_lib-0.25.0/sts/cli.py` & `sts_lib-0.26.0/sts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,19 @@
         print(f'{key} => {" ".join(values)}')
 
 
 def make(args):
     """Generate conversion dictionary(ies).
     """
     configs = args['config']
-    dir = args['dir']
     skip_check = args['force']
     quiet = args['quiet']
 
     for config in configs:
-        StsMaker().make(config, output_dir=dir, skip_check=skip_check, quiet=quiet)
+        StsMaker().make(config, skip_check=skip_check, quiet=quiet)
 
 
 def convert(args):
     """Convert a file using the given config.
     """
     inputs = args['file']
     outputs = args['output']
@@ -169,16 +168,14 @@
     # subcommand: make
     parser_make = subparsers.add_parser('make',
                                         help=make.__doc__, description=make.__doc__)
     parser_make.add_argument('config', nargs='+',
                              help="""the config(s) to generate""")
     parser_make.add_argument('--force', default=False, action='store_true',
                              help="""bypass update check and generate dicitonary(ies) anyway""")
-    parser_make.add_argument('-d', '--dir', default=None,
-                             help="""the directory to save the output (default: relative to config)""")
     parser_make.add_argument('-q', '--quiet', default=False, action='store_true',
                              help="""do not show process information""")
 
     return parser.parse_args(argv)
 
 
 def main():
```

### Comparing `sts_lib-0.25.0/sts/data/config/_default.json` & `sts_lib-0.26.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.26.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.26.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.26.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.26.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.26.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.26.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.26.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.26.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.26.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.26.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.26.0/sts/data/htmlpage.tpl.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 <!DOCTYPE html>
 <html>
 <head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width">
-<title>簡繁秘書 v%VERSION%</title>
+<title>簡繁祕書 v%VERSION%</title>
 <style>
 kbd { border: 1px solid #999; border-radius: 2px; padding: 2px 4px; background-color: #f5f5f5; font-weight: bold; }
-dialog header { margin-bottom: .5em; font-style: bold; }
+dialog header { margin-bottom: .5em; font-weight: bold; }
+dialog section { margin: .5em 0; }
 dialog section label { display: block; }
 dialog footer { margin-top: 1em; display: flex; gap: .5em 1em; flex-direction: row; flex-wrap: wrap; }
 dialog footer input { flex-grow: 1; }
 body > footer { margin-top: 1em; text-align: center; font-size: small; }
 #viewer { border: thin ridge #0066CC; padding: 0.5em; background-color: #f8f8ee; white-space: pre-wrap; }
 #viewer a { border: thin dotted #AAA; color: unset; text-decoration: none; }
 #viewer a:focus { outline: medium solid blue; }
@@ -688,13 +689,13 @@
   <li><kbd>Shift</kbd>+<kbd>Tab</kbd>／<kbd>Tab</kbd>：移至上／下一個字或欄位。</li>
   <li><kbd>Q</kbd>／<kbd>E</kbd>：移至上／下一個未審字。</li>
   <li><kbd>A</kbd>／<kbd>D</kbd>：移至上／下一個待校字（非單選字）。</li>
   <li><kbd>Z</kbd>／<kbd>C</kbd>：移至上／下一個相同字。</li>
   <li><kbd>W</kbd>／<kbd>S</kbd>：套用前／後一個候選字。</li>
   <li><kbd>0</kbd>-<kbd>9</kbd>：套用對應的候選字（<kbd>0</kbd>對應轉換前的字）。</li>
   <li><kbd>`</kbd> (<kbd>1</kbd>左邊的反引號)：將此字切換為編輯模式，編輯模式下本鍵以外的操作鍵將無效。</li>
-  <li><kbd>Enter</kbd>：執行進階指令。</li>
+  <li><kbd>Enter</kbd>：開啟選單執行指令。</li>
 </ul>
 </details>
 <footer>Generated with <a href="https://pypi.org/project/sts-lib/">STS (Simplified-Traditional Secretary)</a> v%VERSION%. Released under <a href="http://www.apache.org/licenses/LICENSE-2.0">Apache License 2.0</a>.</footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -12,10 +12,10 @@
     * Shift+Tab／Tab：移至上／下一個字或欄位。
     * Q／E：移至上／下一個未審字。
     * A／D：移至上／下一個待校字（非單選字）。
     * Z／C：移至上／下一個相同字。
     * W／S：套用前／後一個候選字。
     * 0-9：套用對應的候選字（0對應轉換前的字）。
     * ` (1左邊的反引號)：將此字切換為編輯模式，編輯模式下本鍵以外的操作鍵將無效。
-    * Enter：執行進階指令。
+    * Enter：開啟選單執行指令。
 Generated with _S_T_S_ _(_S_i_m_p_l_i_f_i_e_d_-_T_r_a_d_i_t_i_o_n_a_l_ _S_e_c_r_e_t_a_r_y_) v%VERSION%. Released
 under _A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0.
```

### Comparing `sts_lib-0.25.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.26.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts/data/scheme/variant.txt` & `sts_lib-0.26.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.25.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.26.0/sts_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.25.0
+Version: 0.26.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -112,17 +112,17 @@
  *     (with or without ".json")
  * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
  */
 
 /**
  * @typedef {Object} dictScheme
  * @property {string} file - path of the dictionary file to generate, as an
- *     absolute path, or a path relative to the specified output directory
- *     (or the directory of this config file). It should be a .tlist (compiled
- *     trie), .jlist (compiled table), or .list (plain text table).
+ *     absolute path, or a path relative to the directory of this config file.
+ *     It should be a .tlist (compiled trie), .jlist (compiled table), or .list
+ *     (plain text table).
  * @property {string} [mode=load] - the mode to handle the loaded source files:
  *     "load" to simply merge the loaded keys and values; "swap" to reverse the
  *     dictionary (i.e. use the values as keys and the keys as values); "join"
  *     to build from a chain of dictionaries (in which case src must be an
  *     array of subarrays of strings)
  * @property {Array.<(string|string[])>} [src] - the source files. Each as an
  *     absolute path, or a path relative to the directory of this config file,
```

### Comparing `sts_lib-0.25.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.26.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

