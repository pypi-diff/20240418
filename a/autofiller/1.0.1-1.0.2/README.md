# Comparing `tmp/autofiller-1.0.1.tar.gz` & `tmp/autofiller-1.0.2.tar.gz`

## Comparing `autofiller-1.0.1.tar` & `autofiller-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 autofiller-1.0.1/src/autofiller/__init__.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 autofiller-1.0.1/src/autofiller/__main__.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 autofiller-1.0.1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autofiller-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 autofiller-1.0.1/README.md
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 autofiller-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 autofiller-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 autofiller-1.0.2/src/autofiller/__init__.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 autofiller-1.0.2/src/autofiller/__main__.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 autofiller-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 autofiller-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 autofiller-1.0.2/README.md
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 autofiller-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 autofiller-1.0.2/PKG-INFO
```

### Comparing `autofiller-1.0.1/src/autofiller/__main__.py` & `autofiller-1.0.2/src/autofiller/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,22 +94,23 @@
         self.goaway()
         sleep(.05)
         keyboard.type(text)
 
     def add_random(self, type):
         match type:
             case 'text':
-                regex = (er.match_range(3, 5, er.word_char) + ' ') * randint(1, 5)
-                self.give(regex.invert())
+                regex = (er.match_range(3, 5, er.word_char) + ' ') * randint(2, 5)
+                self.give(regex.invert()[:-1])
             case 'name':
                 self.give(random_name.generate_name())
             case 'json':
                 self.give('{ "TODO": "Random JSON" }')
             case 'email':
-                self.give(er.email.invert())
+                regex = er.word + er.opt('-' + er.word) + '@' + er.word + '.' + er.anyof('com', 'net', 'org')
+                self.give(regex.invert())
 
 app = QApplication(sys.argv)
 window = Window()
 
 def on_press(key:KeyCode):
     global modifiers
     if key in (Key.cmd, Key.cmd_l, Key.cmd_r):
```

### Comparing `autofiller-1.0.1/.gitignore` & `autofiller-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autofiller-1.0.1/LICENSE.txt` & `autofiller-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autofiller-1.0.1/README.md` & `autofiller-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autofiller-1.0.1/pyproject.toml` & `autofiller-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autofiller-1.0.1/PKG-INFO` & `autofiller-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autofiller
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small popup to input various random data for you
 Project-URL: Documentation, https://github.com/smartycope/autofiller#readme
 Project-URL: Issues, https://github.com/smartycope/autofiller/issues
 Project-URL: Source, https://github.com/smartycope/autofiller
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

