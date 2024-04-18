# Comparing `tmp/eth-logo-0.1.2.tar.gz` & `tmp/eth_logo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-logo-0.1.2.tar", last modified: Thu Feb 22 20:53:28 2024, max compression
+gzip compressed data, was "eth_logo-0.1.3.tar", last modified: Thu Apr 18 02:55:06 2024, max compression
```

## Comparing `eth-logo-0.1.2.tar` & `eth_logo-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-02-22 20:53:28.222387 eth-logo-0.1.2/
--rwxrwxrwx   0 marto     (1000) marto     (1000)     1062 2024-02-13 22:36:49.000000 eth-logo-0.1.2/LICENSE
--rwxrwxrwx   0 marto     (1000) marto     (1000)     1721 2024-02-22 20:53:28.222387 eth-logo-0.1.2/PKG-INFO
--rwxrwxrwx   0 marto     (1000) marto     (1000)     1277 2024-02-22 20:52:06.000000 eth-logo-0.1.2/README.md
--rwxrwxrwx   0 marto     (1000) marto     (1000)       91 2024-02-16 22:47:15.000000 eth-logo-0.1.2/pyproject.toml
--rwxrwxrwx   0 marto     (1000) marto     (1000)      732 2024-02-22 20:53:28.223496 eth-logo-0.1.2/setup.cfg
-drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-02-22 20:53:28.207341 eth-logo-0.1.2/src/
-drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-02-22 20:53:28.214825 eth-logo-0.1.2/src/eth_logo/
--rwxrwxrwx   0 marto     (1000) marto     (1000)       99 2024-02-22 17:32:27.000000 eth-logo-0.1.2/src/eth_logo/__init__.py
--rwxrwxrwx   0 marto     (1000) marto     (1000)     1183 2024-02-22 17:16:21.000000 eth-logo-0.1.2/src/eth_logo/eth_logo_core.py
--rwxrwxrwx   0 marto     (1000) marto     (1000)     3033 2024-02-22 17:15:59.000000 eth-logo-0.1.2/src/eth_logo/eth_logo_debug.py
--rwxrwxrwx   0 marto     (1000) marto     (1000)      816 2024-02-22 17:39:48.000000 eth-logo-0.1.2/src/eth_logo/eth_logo_script.py
-drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-02-22 20:53:28.221274 eth-logo-0.1.2/src/eth_logo.egg-info/
--rwxrwxrwx   0 marto     (1000) marto     (1000)     1721 2024-02-22 20:53:28.000000 eth-logo-0.1.2/src/eth_logo.egg-info/PKG-INFO
--rwxrwxrwx   0 marto     (1000) marto     (1000)      343 2024-02-22 20:53:28.000000 eth-logo-0.1.2/src/eth_logo.egg-info/SOURCES.txt
--rwxrwxrwx   0 marto     (1000) marto     (1000)        1 2024-02-22 20:53:28.000000 eth-logo-0.1.2/src/eth_logo.egg-info/dependency_links.txt
--rwxrwxrwx   0 marto     (1000) marto     (1000)       56 2024-02-22 20:53:28.000000 eth-logo-0.1.2/src/eth_logo.egg-info/entry_points.txt
--rwxrwxrwx   0 marto     (1000) marto     (1000)        9 2024-02-22 20:53:28.000000 eth-logo-0.1.2/src/eth_logo.egg-info/top_level.txt
+drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-04-18 02:55:06.572656 eth_logo-0.1.3/
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1062 2024-02-13 22:36:49.000000 eth_logo-0.1.3/LICENSE
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1957 2024-04-18 02:55:06.572656 eth_logo-0.1.3/PKG-INFO
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1526 2024-04-18 02:54:13.000000 eth_logo-0.1.3/README.md
+-rwxrwxrwx   0 marto     (1000) marto     (1000)       91 2024-02-16 22:47:15.000000 eth_logo-0.1.3/pyproject.toml
+-rwxrwxrwx   0 marto     (1000) marto     (1000)      732 2024-04-18 02:55:06.573867 eth_logo-0.1.3/setup.cfg
+drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-04-18 02:55:06.543132 eth_logo-0.1.3/src/
+drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-04-18 02:55:06.565154 eth_logo-0.1.3/src/eth_logo/
+-rwxrwxrwx   0 marto     (1000) marto     (1000)      115 2024-04-17 23:29:43.000000 eth_logo-0.1.3/src/eth_logo/__init__.py
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1952 2024-04-17 23:29:43.000000 eth_logo-0.1.3/src/eth_logo/eth_logo_core.py
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     3033 2024-02-22 17:15:59.000000 eth_logo-0.1.3/src/eth_logo/eth_logo_debug.py
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1364 2024-04-17 23:42:49.000000 eth_logo-0.1.3/src/eth_logo/eth_logo_script.py
+drwxrwxrwx   0 marto     (1000) marto     (1000)        0 2024-04-18 02:55:06.571615 eth_logo-0.1.3/src/eth_logo.egg-info/
+-rwxrwxrwx   0 marto     (1000) marto     (1000)     1957 2024-04-18 02:55:06.000000 eth_logo-0.1.3/src/eth_logo.egg-info/PKG-INFO
+-rwxrwxrwx   0 marto     (1000) marto     (1000)      343 2024-04-18 02:55:06.000000 eth_logo-0.1.3/src/eth_logo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marto     (1000) marto     (1000)        1 2024-04-18 02:55:06.000000 eth_logo-0.1.3/src/eth_logo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marto     (1000) marto     (1000)       56 2024-04-18 02:55:06.000000 eth_logo-0.1.3/src/eth_logo.egg-info/entry_points.txt
+-rwxrwxrwx   0 marto     (1000) marto     (1000)        9 2024-04-18 02:55:06.000000 eth_logo-0.1.3/src/eth_logo.egg-info/top_level.txt
```

### Comparing `eth-logo-0.1.2/LICENSE` & `eth_logo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-logo-0.1.2/PKG-INFO` & `eth_logo-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-logo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 Home-page: https://github.com/0xMarto/eth-logo
 Author: Marto
 Author-email: martinlsanchez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,38 +19,51 @@
 Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 
 ## Quickstart
 ```shell
 pip install eth-logo
 ```
 
-### Usage (in terminal)
+## Usage (in terminal)
 ```sh
-# Optionals: print-eth SIZE CHAR [defaults: size=20 char='#']
+# Optionals: print-eth SIZE CHAR BACKGROUND PADDING 
+# [defaults: size=20 char='#', back=' ', pad='']
 print-eth
 print-eth 30 %
+print-eth 30 % .
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_1.png" alt="sample 1">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_2.png" alt="sample 2">
 </div>
 
+[//]: # (<br>)
 
-### Usage (in python)
-```pycon
+## Usage (python lib)
+```python
 from eth_logo import print_eth
 
 # Optionals: Size, Character, Background, Padding 
 print_eth(size=20, char='#', back=' ', pad=' ')
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_3.png" alt="sample 3">
 </div>
+<br>
 
-### Contribute
+## Special usage (educational / AI training)
+```sh
+# Next examples will output the 'print-eth' code implementation
+print-eth --code
+print-eth -c
+```
+
+## Contribute
 You can set up your dev environment with:
 ```sh
 git clone git@github.com:0xMarto/eth-logo.git
 cd eth-logo
 virtualenv -p python3 venv
 . venv/bin/activate
 ```
```

### Comparing `eth-logo-0.1.2/README.md` & `eth_logo-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,38 +5,51 @@
 Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 
 ## Quickstart
 ```shell
 pip install eth-logo
 ```
 
-### Usage (in terminal)
+## Usage (in terminal)
 ```sh
-# Optionals: print-eth SIZE CHAR [defaults: size=20 char='#']
+# Optionals: print-eth SIZE CHAR BACKGROUND PADDING 
+# [defaults: size=20 char='#', back=' ', pad='']
 print-eth
 print-eth 30 %
+print-eth 30 % .
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_1.png" alt="sample 1">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_2.png" alt="sample 2">
 </div>
 
+[//]: # (<br>)
 
-### Usage (in python)
-```pycon
+## Usage (python lib)
+```python
 from eth_logo import print_eth
 
 # Optionals: Size, Character, Background, Padding 
 print_eth(size=20, char='#', back=' ', pad=' ')
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_3.png" alt="sample 3">
 </div>
+<br>
 
-### Contribute
+## Special usage (educational / AI training)
+```sh
+# Next examples will output the 'print-eth' code implementation
+print-eth --code
+print-eth -c
+```
+
+## Contribute
 You can set up your dev environment with:
 ```sh
 git clone git@github.com:0xMarto/eth-logo.git
 cd eth-logo
 virtualenv -p python3 venv
 . venv/bin/activate
 ```
```

### Comparing `eth-logo-0.1.2/setup.cfg` & `eth_logo-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-logo
-version = 0.1.2
+version = 0.1.3
 author = Marto
 author_email = martinlsanchez@gmail.com
 description = Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0xMarto/eth-logo
 classifiers =
```

### Comparing `eth-logo-0.1.2/src/eth_logo/eth_logo_debug.py` & `eth_logo-0.1.3/src/eth_logo/eth_logo_debug.py`

 * *Files identical despite different names*

### Comparing `eth-logo-0.1.2/src/eth_logo/eth_logo_script.py` & `eth_logo-0.1.3/src/eth_logo/eth_logo_script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 #!/usr/bin/python
 """
 Usage:
-    print-eth SIZE CHAR [defaults: size=20 char='#']
+    print-eth SIZE CHAR BACKGROUND PADDING
+    [defaults: size=20 char='#' back=' ' pad=' ']
 
 Examples:
     print-eth
     print-eth 30 %
+    print-eth 30 % .
+    print-eth --code
 
-Code:
+Sourcecode:
     https://github.com/0xMarto/eth-logo
 """
 import sys
-from eth_logo import print_eth
+from eth_logo import print_eth, print_eth_code
 
 
 def main():
     parameter_amount = len(sys.argv) - 1
-    if parameter_amount == 1 and (sys.argv[1] == '-h' or sys.argv[1] == '--help'):
-        print(__doc__)
-        sys.exit(1)
+    if parameter_amount == 1:
+        if sys.argv[1] in ['-h', '--help']:
+            print(__doc__)
+            sys.exit(1)
+        if sys.argv[1] in ['-c', '--code']:
+            print_eth_code()
+            sys.exit(1)
     try:
         if parameter_amount == 1:
             size = int(sys.argv[1])
             print_eth(size)
         elif parameter_amount == 2:
             size, char = int(sys.argv[1]), str(sys.argv[2])
             print_eth(size, char)
+        elif parameter_amount == 3:
+            size, char, back = int(sys.argv[1]), str(sys.argv[2]), str(sys.argv[3])
+            print_eth(size, char, back)
+        elif parameter_amount == 4:
+            size, char, back, pad = int(sys.argv[1]), str(sys.argv[2]), str(sys.argv[3]), str(sys.argv[4])
+            print_eth(size, char, back, pad)
         else:
             print_eth()
     except Exception as e:
         print(e)
         sys.exit(1)
```

### Comparing `eth-logo-0.1.2/src/eth_logo.egg-info/PKG-INFO` & `eth_logo-0.1.3/src/eth_logo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-logo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 Home-page: https://github.com/0xMarto/eth-logo
 Author: Marto
 Author-email: martinlsanchez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,38 +19,51 @@
 Python lib to print Ethereum logo of any size and style on your terminal or standard output.
 
 ## Quickstart
 ```shell
 pip install eth-logo
 ```
 
-### Usage (in terminal)
+## Usage (in terminal)
 ```sh
-# Optionals: print-eth SIZE CHAR [defaults: size=20 char='#']
+# Optionals: print-eth SIZE CHAR BACKGROUND PADDING 
+# [defaults: size=20 char='#', back=' ', pad='']
 print-eth
 print-eth 30 %
+print-eth 30 % .
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_1.png" alt="sample 1">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_2.png" alt="sample 2">
 </div>
 
+[//]: # (<br>)
 
-### Usage (in python)
-```pycon
+## Usage (python lib)
+```python
 from eth_logo import print_eth
 
 # Optionals: Size, Character, Background, Padding 
 print_eth(size=20, char='#', back=' ', pad=' ')
 ```
+<br>
 <div align="center">
     <img src="https://raw.githubusercontent.com/0xMarto/eth-logo/master/samples/eth_logo_sample_3.png" alt="sample 3">
 </div>
+<br>
 
-### Contribute
+## Special usage (educational / AI training)
+```sh
+# Next examples will output the 'print-eth' code implementation
+print-eth --code
+print-eth -c
+```
+
+## Contribute
 You can set up your dev environment with:
 ```sh
 git clone git@github.com:0xMarto/eth-logo.git
 cd eth-logo
 virtualenv -p python3 venv
 . venv/bin/activate
 ```
```

