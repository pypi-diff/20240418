# Comparing `tmp/tebbytools-0.2.3.tar.gz` & `tmp/tebbytools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tebbytools-0.2.3.tar", last modified: Wed Apr 17 03:29:43 2024, max compression
+gzip compressed data, was "tebbytools-0.2.4.tar", last modified: Thu Apr 18 15:27:36 2024, max compression
```

## Comparing `tebbytools-0.2.3.tar` & `tebbytools-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 03:29:43.597245 tebbytools-0.2.3/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-17 03:29:43.596988 tebbytools-0.2.3/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1921 2024-04-17 03:26:55.000000 tebbytools-0.2.3/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-17 03:29:43.597282 tebbytools-0.2.3/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-17 03:29:31.000000 tebbytools-0.2.3/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 03:29:43.595011 tebbytools-0.2.3/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 03:29:43.595923 tebbytools-0.2.3/src/tebbytools/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-04-17 03:25:44.000000 tebbytools-0.2.3/src/tebbytools/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.2.3/src/tebbytools/reviewlist.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     4935 2024-04-17 02:58:03.000000 tebbytools-0.2.3/src/tebbytools/wordbank.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 03:29:43.596813 tebbytools-0.2.3/src/tebbytools.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-17 03:29:43.000000 tebbytools-0.2.3/src/tebbytools.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      267 2024-04-17 03:29:43.000000 tebbytools-0.2.3/src/tebbytools.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-17 03:29:43.000000 tebbytools-0.2.3/src/tebbytools.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-17 03:29:43.000000 tebbytools-0.2.3/src/tebbytools.egg-info/top_level.txt
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-17 03:29:43.596579 tebbytools-0.2.3/tests/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      906 2024-04-17 03:25:59.000000 tebbytools-0.2.3/tests/test.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.768087 tebbytools-0.2.4/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-18 15:27:36.767719 tebbytools-0.2.4/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     1921 2024-04-17 03:26:55.000000 tebbytools-0.2.4/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-18 15:27:36.768144 tebbytools-0.2.4/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      472 2024-04-18 15:27:30.000000 tebbytools-0.2.4/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.765371 tebbytools-0.2.4/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.766540 tebbytools-0.2.4/src/tebbytools/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       66 2024-04-17 03:25:44.000000 tebbytools-0.2.4/src/tebbytools/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     2754 2024-04-17 02:55:21.000000 tebbytools-0.2.4/src/tebbytools/reviewlist.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     5194 2024-04-18 15:25:49.000000 tebbytools-0.2.4/src/tebbytools/wordbank.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.767487 tebbytools-0.2.4/src/tebbytools.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      286 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      267 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       11 2024-04-18 15:27:36.000000 tebbytools-0.2.4/src/tebbytools.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-18 15:27:36.767205 tebbytools-0.2.4/tests/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      906 2024-04-17 03:25:59.000000 tebbytools-0.2.4/tests/test.py
```

### Comparing `tebbytools-0.2.3/README.md` & `tebbytools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tebbytools-0.2.3/src/tebbytools/reviewlist.py` & `tebbytools-0.2.4/src/tebbytools/reviewlist.py`

 * *Files identical despite different names*

### Comparing `tebbytools-0.2.3/src/tebbytools/wordbank.py` & `tebbytools-0.2.4/src/tebbytools/wordbank.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,21 @@
 
     def get_todays_words(self):
         """
         Get the list of words added today
         """
         return self.get_words_from_past_n_days(0)
 
+    def get_todays_new_words(self):
+        """
+        Get the list of words added today that have not been added before
+        """
+        todays_words = self.get_todays_words()
+        return [word for word in todays_words if self.occurences(word) == 1]
+
     def get_words_by_tag(self, tag):
         """
         Get a list of all the words with a specific tag
         """
         bank = self.get_bank()
         words = []
         for entry in bank:
```

### Comparing `tebbytools-0.2.3/tests/test.py` & `tebbytools-0.2.4/tests/test.py`

 * *Files identical despite different names*

