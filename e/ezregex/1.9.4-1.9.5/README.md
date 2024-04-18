# Comparing `tmp/ezregex-1.9.4.tar.gz` & `tmp/ezregex-1.9.5.tar.gz`

## Comparing `ezregex-1.9.4.tar` & `ezregex-1.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.4/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.4/MANIFEST.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.4/requirements.txt
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.4/setup.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.4/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.4/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/EZRegex.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/_dialects.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/_docs.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/generate.py
--rw-r--r--   0        0        0    24543 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/invert.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/invert_old.py
--rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/assets/sorted_words.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/elements.py
--rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/interface.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/psuedonymns.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/elements.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/groups.py
--rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/regexs.jsonc
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/replacements.jsonc
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_EZRegex.py
--rw-r--r--   0        0        0    17019 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_elements.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_generate.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_invert.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_javascript.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_operators.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_python.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_replacement.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    15201 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/tests.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.4/LICENSE
--rw-r--r--   0        0        0    52510 2020-02-02 00:00:00.000000 ezregex-1.9.4/README.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.4/pyproject.toml
--rw-r--r--   0        0        0    53450 2020-02-02 00:00:00.000000 ezregex-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.5/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.5/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.5/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.5/setup.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.5/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.5/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/EZRegex.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/_dialects.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/_docs.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/generate.py
+-rw-r--r--   0        0        0    24619 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/invert.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/invert_old.py
+-rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/assets/sorted_words.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/elements.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/interface.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/psuedonymns.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/psuedonymns.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/elements.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/psuedonymns.py
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/groups.py
+-rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/regexs.jsonc
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/replacements.jsonc
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_EZRegex.py
+-rw-r--r--   0        0        0    17019 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_elements.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_generate.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_invert.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_javascript.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_operators.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_python.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_replacement.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    15201 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/tests.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.5/LICENSE
+-rw-r--r--   0        0        0    52510 2020-02-02 00:00:00.000000 ezregex-1.9.5/README.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0    53450 2020-02-02 00:00:00.000000 ezregex-1.9.5/PKG-INFO
```

### Comparing `ezregex-1.9.4/setup.py` & `ezregex-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/.github/FUNDING.yml` & `ezregex-1.9.5/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/.github/workflows/unit-tests.yml` & `ezregex-1.9.5/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/EZRegex.py` & `ezregex-1.9.5/ezregex/EZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/_dialects.py` & `ezregex-1.9.5/ezregex/_dialects.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/_docs.py` & `ezregex-1.9.5/ezregex/_docs.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/api.py` & `ezregex-1.9.5/ezregex/api.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/api.pyi` & `ezregex-1.9.5/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/generate.py` & `ezregex-1.9.5/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/invert.py` & `ezregex-1.9.5/ezregex/invert.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
 
 with open(Path(__file__).parent / 'assets' / 'sorted_words.json') as f:
-    words = json.load(f).keys()
+    words = json.load(f)
 
 # Don't use string.whitespace, because we don't want to use weird difficult to print characters.
 # We want the replacement to be readable.
 _whitespace   = ' '
 _everything   = string.digits + string.ascii_letters + string.punctuation + _whitespace + '_'
 
 def _randWord(length=None, word='lookup'):
@@ -30,15 +30,16 @@
         length = randint(3, 9)
 
     if word == 'random':
         return ''.join(choices(string.ascii_letters, k=length))
 
     elif word == 'lookup':
         try:
-            return choice(words[length])
+            # The keys are strings, not ints, and I don't feel like fixing it
+            return choice(words[str(length)])
         except KeyError:
             return _randWord(length, word='random')
 
     elif word is None:
         return 'word'
 
     else:
```

### Comparing `ezregex-1.9.4/ezregex/invert_old.py` & `ezregex-1.9.5/ezregex/invert_old.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/assets/sorted_words.json` & `ezregex-1.9.5/ezregex/assets/sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/base/elements.py` & `ezregex-1.9.5/ezregex/base/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/base/interface.py` & `ezregex-1.9.5/ezregex/base/interface.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/javascript/elements.py` & `ezregex-1.9.5/ezregex/javascript/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/javascript/psuedonymns.py` & `ezregex-1.9.5/ezregex/javascript/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/perl/elements.py` & `ezregex-1.9.5/ezregex/perl/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/perl/psuedonymns.py` & `ezregex-1.9.5/ezregex/perl/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/python/elements.py` & `ezregex-1.9.5/ezregex/python/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/ezregex/python/psuedonymns.py` & `ezregex-1.9.5/ezregex/python/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/groups.py` & `ezregex-1.9.5/tests/groups.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/regexs.jsonc` & `ezregex-1.9.5/tests/regexs.jsonc`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/replacements.jsonc` & `ezregex-1.9.5/tests/replacements.jsonc`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_EZRegex.py` & `ezregex-1.9.5/tests/test_EZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_elements.py` & `ezregex-1.9.5/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_generate.py` & `ezregex-1.9.5/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_invert.py` & `ezregex-1.9.5/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_javascript.py` & `ezregex-1.9.5/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_operators.py` & `ezregex-1.9.5/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_python.py` & `ezregex-1.9.5/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/test_replacement.py` & `ezregex-1.9.5/tests/test_replacement.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/testing_color_algorithm.ipynb` & `ezregex-1.9.5/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/tests/tests.py` & `ezregex-1.9.5/tests/tests.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/.gitignore` & `ezregex-1.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/LICENSE` & `ezregex-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/README.md` & `ezregex-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/pyproject.toml` & `ezregex-1.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.4/PKG-INFO` & `ezregex-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ezregex
-Version: 1.9.4
+Version: 1.9.5
 Summary: A readable and intuitive way to generate Regular Expressions
 Project-URL: Documentation, https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation
 Project-URL: Issues, https://github.com/smartycope/ezregex/issues
 Project-URL: Source, https://github.com/smartycope/ezregex
 Project-URL: Official Website, https://ezregex.org
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ezregex Version: 1.9.4 Summary: A readable and
+Metadata-Version: 2.3 Name: ezregex Version: 1.9.5 Summary: A readable and
 intuitive way to generate Regular Expressions Project-URL: Documentation,
 https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation Project-
 URL: Issues, https://github.com/smartycope/ezregex/issues Project-URL: Source,
 https://github.com/smartycope/ezregex Project-URL: Official Website, https://
 ezregex.org Author-email: Copeland Carter
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
```

