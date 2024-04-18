# Comparing `tmp/jsp_vis-1.0.1.tar.gz` & `tmp/jsp_vis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsp_vis-1.0.1.tar", last modified: Thu Apr 18 08:46:00 2024, max compression
+gzip compressed data, was "jsp_vis-1.0.2.tar", last modified: Thu Apr 18 15:10:52 2024, max compression
```

## Comparing `jsp_vis-1.0.1.tar` & `jsp_vis-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 08:46:00.239188 jsp_vis-1.0.1/
--rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_vis-1.0.1/LICENSE
--rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-12-26 19:19:03.000000 jsp_vis-1.0.1/MANIFEST.in
--rw-r--r--   0 qwerty     (501) staff       (20)     6609 2024-04-18 08:46:00.239114 jsp_vis-1.0.1/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)     4395 2024-04-18 08:44:25.000000 jsp_vis-1.0.1/README.md
--rw-r--r--   0 qwerty     (501) staff       (20)      995 2024-04-18 08:45:56.000000 jsp_vis-1.0.1/pyproject.toml
--rw-r--r--   0 qwerty     (501) staff       (20)      402 2024-04-18 08:46:00.239401 jsp_vis-1.0.1/setup.cfg
--rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_vis-1.0.1/setup.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 08:46:00.236451 jsp_vis-1.0.1/src/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 08:46:00.237580 jsp_vis-1.0.1/src/jsp_vis/
--rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-11 16:14:58.000000 jsp_vis-1.0.1/src/jsp_vis/__init__.py
--rw-r--r--   0 qwerty     (501) staff       (20)     7864 2024-04-16 19:04:18.000000 jsp_vis-1.0.1/src/jsp_vis/console.py
--rw-r--r--   0 qwerty     (501) staff       (20)     2686 2024-04-16 19:04:18.000000 jsp_vis-1.0.1/src/jsp_vis/cv2_window.py
--rw-r--r--   0 qwerty     (501) staff       (20)     1725 2024-04-16 17:22:15.000000 jsp_vis-1.0.1/src/jsp_vis/rgb_array.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 08:46:00.238694 jsp_vis-1.0.1/src/jsp_vis.egg-info/
--rw-r--r--   0 qwerty     (501) staff       (20)     6609 2024-04-18 08:46:00.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)      461 2024-04-18 08:46:00.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/SOURCES.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 08:46:00.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/dependency_links.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-11 16:22:28.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/not-zip-safe
--rw-r--r--   0 qwerty     (501) staff       (20)       98 2024-04-18 08:46:00.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/requires.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        8 2024-04-18 08:46:00.000000 jsp_vis-1.0.1/src/jsp_vis.egg-info/top_level.txt
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 08:46:00.238552 jsp_vis-1.0.1/tests/
--rw-r--r--   0 qwerty     (501) staff       (20)      682 2024-04-16 18:50:13.000000 jsp_vis-1.0.1/tests/test_render_console.py
--rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-16 19:07:53.000000 jsp_vis-1.0.1/tests/test_render_cv2_window.py
--rw-r--r--   0 qwerty     (501) staff       (20)      574 2024-04-16 18:52:00.000000 jsp_vis-1.0.1/tests/test_render_rgb_array.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843762 jsp_vis-1.0.2/
+-rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_vis-1.0.2/LICENSE
+-rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-12-26 19:19:03.000000 jsp_vis-1.0.2/MANIFEST.in
+-rw-r--r--   0 qwerty     (501) staff       (20)     6534 2024-04-18 15:10:52.843697 jsp_vis-1.0.2/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)     4321 2024-04-18 15:10:27.000000 jsp_vis-1.0.2/README.md
+-rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 15:10:50.000000 jsp_vis-1.0.2/pyproject.toml
+-rw-r--r--   0 qwerty     (501) staff       (20)      402 2024-04-18 15:10:52.844000 jsp_vis-1.0.2/setup.cfg
+-rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_vis-1.0.2/setup.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.840985 jsp_vis-1.0.2/src/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.842111 jsp_vis-1.0.2/src/jsp_vis/
+-rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-11 16:14:58.000000 jsp_vis-1.0.2/src/jsp_vis/__init__.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     7864 2024-04-16 19:04:18.000000 jsp_vis-1.0.2/src/jsp_vis/console.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     2686 2024-04-16 19:04:18.000000 jsp_vis-1.0.2/src/jsp_vis/cv2_window.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1725 2024-04-16 17:22:15.000000 jsp_vis-1.0.2/src/jsp_vis/rgb_array.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843222 jsp_vis-1.0.2/src/jsp_vis.egg-info/
+-rw-r--r--   0 qwerty     (501) staff       (20)     6534 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)      461 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-11 16:22:28.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/not-zip-safe
+-rw-r--r--   0 qwerty     (501) staff       (20)       98 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/requires.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        8 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843065 jsp_vis-1.0.2/tests/
+-rw-r--r--   0 qwerty     (501) staff       (20)      682 2024-04-16 18:50:13.000000 jsp_vis-1.0.2/tests/test_render_console.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-16 19:07:53.000000 jsp_vis-1.0.2/tests/test_render_cv2_window.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      574 2024-04-16 18:52:00.000000 jsp_vis-1.0.2/tests/test_render_rgb_array.py
```

### Comparing `jsp_vis-1.0.1/LICENSE` & `jsp_vis-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/PKG-INFO` & `jsp_vis-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jsp-vis
-Version: 1.0.1
+Version: 1.0.2
 Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
-Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
+Author-email: Alexander Nasuta <alexander.nasuta@wzl-iqs.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2024 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,15 +21,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/Alexander-Nasuta/pypitemplate
+Project-URL: Homepage, https://github.com/Alexander-Nasuta/jsp-vis
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -55,30 +55,26 @@
 <div id="top"></div>
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
    <!--
   <a href="https://cybernetics-lab.de/">
-    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png" alt="Logo" height="80">
+    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png">
   </a>
    -->
 
   <h1 align="center">
      Job Shop Scheduling Problem Visualisations
   </h1>
 
-   
-   <a>
-    <img src="https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif" alt="Logo" height="180">
-  </a>
-
 
 </div>
 
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif)
 
 - **Github**: https://github.com/Alexander-Nasuta/jsp-vis
 
 - **PyPi**: https://pypi.org/project/jsp-vis/
 
 
 # About The Project
@@ -91,15 +87,15 @@
 The window visualisation is essentially only rendering the rgb_array visualisation in a window using OpenCV.
 The console visualisation might be used for the `asni` mode of a render function, the rgb_array visualisation for the `rgb_array` mode and the window visualisation for the `human` mode.
 
 # Installation
 
 Install the package with pip:
 ```
-   pip install todo
+   pip install jsp-vis
 ```
 
 # Minimal Working Example: console visualisation
 
 ```python
 from jsp_vis.console import gantt_chart_console
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,73 +1,74 @@
-Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.1 Summary: A flexible
+Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.2 Summary: A flexible
 enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta Author-email: Alexander Nasuta
-ima.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander Nasuta
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/Alexander-
-Nasuta/pypitemplate Platform: unix Platform: linux Platform: osx Platform:
-cygwin Platform: win32 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: opencv-python Requires-Dist: plotly
-Requires-Dist: matplotlib Requires-Dist: numpy Requires-Dist: pandas Requires-
-Dist: kaleido Provides-Extra: dev Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: tox; extra == "dev" Requires-Dist: twine; extra == "dev"
+wzl-iqs.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander
+Nasuta Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions: The above copyright
+notice and this permission notice shall be included in all copies or
+substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT
+WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
+FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
+THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://
+github.com/Alexander-Nasuta/jsp-vis Platform: unix Platform: linux Platform:
+osx Platform: cygwin Platform: win32 Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: opencv-python Requires-Dist:
+plotly Requires-Dist: matplotlib Requires-Dist: numpy Requires-Dist: pandas
+Requires-Dist: kaleido Provides-Extra: dev Requires-Dist: pip-tools; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Requires-Dist: tox; extra == "dev" Requires-Dist: twine; extra == "dev"
 
            ************ JJoobb SShhoopp SScchheedduulliinngg PPrroobblleemm VViissuuaalliissaattiioonnss ************
-                                    [Logo]
-- **Github**: https://github.com/Alexander-Nasuta/jsp-vis - **PyPi**: https://
-pypi.org/project/jsp-vis/ # About The Project Ths project provides
-visualisation for the Job Shop Scheduling Problem (JSP). This is focused on
-Gantt charts. The input date for the visualisation is inspired by [plotly's
-Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a standalone
-package and in designed to be used in combination with a JSP-reinforcement
-learning environments that follow the [Gymnasium Environment](https://
-gymnasium.farama.org/) standard. The render function of the environment can be
-used to render the Gantt chart. Typically the render function can implement
-different modes like `human`, `rgb_array` or `ansi` rendering. The `jsp-vis`
-package offers three different visualisations: console visualisation, rgb_array
-visualisation and window visualisation. The window visualisation is essentially
-only rendering the rgb_array visualisation in a window using OpenCV. The
-console visualisation might be used for the `asni` mode of a render function,
-the rgb_array visualisation for the `rgb_array` mode and the window
-visualisation for the `human` mode. # Installation Install the package with
-pip: ``` pip install todo ``` # Minimal Working Example: console visualisation
-```python from jsp_vis.console import gantt_chart_console import pandas as pd
-df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish': 16, 'Resource':
-'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31, 'Resource': 'Machine
-1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34, 'Resource': 'Machine 2'},
-{'Task': 'Job 0', 'Start': 34, 'Finish': 46, 'Resource': 'Machine 3'}, {'Task':
-'Job 1', 'Start': 0, 'Finish': 5, 'Resource': 'Machine 0'}, {'Task': 'Job 1',
-'Start': 5, 'Finish': 21, 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start':
-21, 'Finish': 28, 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28,
-'Finish': 32, 'Resource': 'Machine 3'} ]) num_of_machines = 4
-gantt_chart_console(df, num_of_machines) ``` The code above will render the
-following Gantt chart in the console: ![](https://raw.githubusercontent.com/
-Alexander-Nasuta/jsp-vis/main/resources/example_console.png) # Minimal Working
-Example: console visualisation ```python from jsp_vis.cv2_window import
-render_gantt_in_window import pandas as pd df = pd.DataFrame([ {'Task': 'Job
-0', 'Start': 5, 'Finish': 16, 'Resource': 'Machine 0'}, {'Task': 'Job 0',
-'Start': 28, 'Finish': 31, 'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start':
-31, 'Finish': 34, 'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34,
-'Finish': 46, 'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish':
-5, 'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
+ft06_console.gif) - **Github**: https://github.com/Alexander-Nasuta/jsp-vis -
+**PyPi**: https://pypi.org/project/jsp-vis/ # About The Project Ths project
+provides visualisation for the Job Shop Scheduling Problem (JSP). This is
+focused on Gantt charts. The input date for the visualisation is inspired by
+[plotly's Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a
+standalone package and in designed to be used in combination with a JSP-
+reinforcement learning environments that follow the [Gymnasium Environment]
+(https://gymnasium.farama.org/) standard. The render function of the
+environment can be used to render the Gantt chart. Typically the render
+function can implement different modes like `human`, `rgb_array` or `ansi`
+rendering. The `jsp-vis` package offers three different visualisations: console
+visualisation, rgb_array visualisation and window visualisation. The window
+visualisation is essentially only rendering the rgb_array visualisation in a
+window using OpenCV. The console visualisation might be used for the `asni`
+mode of a render function, the rgb_array visualisation for the `rgb_array` mode
+and the window visualisation for the `human` mode. # Installation Install the
+package with pip: ``` pip install jsp-vis ``` # Minimal Working Example:
+console visualisation ```python from jsp_vis.console import gantt_chart_console
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
+'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
+'Resource': 'Machine 3'} ]) num_of_machines = 4 gantt_chart_console(df,
+num_of_machines) ``` The code above will render the following Gantt chart in
+the console: ![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/
+main/resources/example_console.png) # Minimal Working Example: console
+visualisation ```python from jsp_vis.cv2_window import render_gantt_in_window
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
 'Resource': 'Machine 3'} ]) num_of_machines = 4 render_gantt_in_window( df=df,
 n_machines=num_of_machines, wait=2000 # time in ms that the `cv2`-window is
 open. # wait=None # ''None'' will keep the window open till a keyboard occurs.
 ) ``` The code above will render the following Gantt chart in the console: ![]
 (https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
```

### Comparing `jsp_vis-1.0.1/README.md` & `jsp_vis-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 <div id="top"></div>
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
    <!--
   <a href="https://cybernetics-lab.de/">
-    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png" alt="Logo" height="80">
+    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png">
   </a>
    -->
 
   <h1 align="center">
      Job Shop Scheduling Problem Visualisations
   </h1>
 
-   
-   <a>
-    <img src="https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif" alt="Logo" height="180">
-  </a>
-
 
 </div>
 
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif)
 
 - **Github**: https://github.com/Alexander-Nasuta/jsp-vis
 
 - **PyPi**: https://pypi.org/project/jsp-vis/
 
 
 # About The Project
@@ -39,15 +35,15 @@
 The window visualisation is essentially only rendering the rgb_array visualisation in a window using OpenCV.
 The console visualisation might be used for the `asni` mode of a render function, the rgb_array visualisation for the `rgb_array` mode and the window visualisation for the `human` mode.
 
 # Installation
 
 Install the package with pip:
 ```
-   pip install todo
+   pip install jsp-vis
 ```
 
 # Minimal Working Example: console visualisation
 
 ```python
 from jsp_vis.console import gantt_chart_console
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,46 +1,47 @@
 
            ************ JJoobb SShhoopp SScchheedduulliinngg PPrroobblleemm VViissuuaalliissaattiioonnss ************
-                                    [Logo]
-- **Github**: https://github.com/Alexander-Nasuta/jsp-vis - **PyPi**: https://
-pypi.org/project/jsp-vis/ # About The Project Ths project provides
-visualisation for the Job Shop Scheduling Problem (JSP). This is focused on
-Gantt charts. The input date for the visualisation is inspired by [plotly's
-Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a standalone
-package and in designed to be used in combination with a JSP-reinforcement
-learning environments that follow the [Gymnasium Environment](https://
-gymnasium.farama.org/) standard. The render function of the environment can be
-used to render the Gantt chart. Typically the render function can implement
-different modes like `human`, `rgb_array` or `ansi` rendering. The `jsp-vis`
-package offers three different visualisations: console visualisation, rgb_array
-visualisation and window visualisation. The window visualisation is essentially
-only rendering the rgb_array visualisation in a window using OpenCV. The
-console visualisation might be used for the `asni` mode of a render function,
-the rgb_array visualisation for the `rgb_array` mode and the window
-visualisation for the `human` mode. # Installation Install the package with
-pip: ``` pip install todo ``` # Minimal Working Example: console visualisation
-```python from jsp_vis.console import gantt_chart_console import pandas as pd
-df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish': 16, 'Resource':
-'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31, 'Resource': 'Machine
-1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34, 'Resource': 'Machine 2'},
-{'Task': 'Job 0', 'Start': 34, 'Finish': 46, 'Resource': 'Machine 3'}, {'Task':
-'Job 1', 'Start': 0, 'Finish': 5, 'Resource': 'Machine 0'}, {'Task': 'Job 1',
-'Start': 5, 'Finish': 21, 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start':
-21, 'Finish': 28, 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28,
-'Finish': 32, 'Resource': 'Machine 3'} ]) num_of_machines = 4
-gantt_chart_console(df, num_of_machines) ``` The code above will render the
-following Gantt chart in the console: ![](https://raw.githubusercontent.com/
-Alexander-Nasuta/jsp-vis/main/resources/example_console.png) # Minimal Working
-Example: console visualisation ```python from jsp_vis.cv2_window import
-render_gantt_in_window import pandas as pd df = pd.DataFrame([ {'Task': 'Job
-0', 'Start': 5, 'Finish': 16, 'Resource': 'Machine 0'}, {'Task': 'Job 0',
-'Start': 28, 'Finish': 31, 'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start':
-31, 'Finish': 34, 'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34,
-'Finish': 46, 'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish':
-5, 'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
+ft06_console.gif) - **Github**: https://github.com/Alexander-Nasuta/jsp-vis -
+**PyPi**: https://pypi.org/project/jsp-vis/ # About The Project Ths project
+provides visualisation for the Job Shop Scheduling Problem (JSP). This is
+focused on Gantt charts. The input date for the visualisation is inspired by
+[plotly's Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a
+standalone package and in designed to be used in combination with a JSP-
+reinforcement learning environments that follow the [Gymnasium Environment]
+(https://gymnasium.farama.org/) standard. The render function of the
+environment can be used to render the Gantt chart. Typically the render
+function can implement different modes like `human`, `rgb_array` or `ansi`
+rendering. The `jsp-vis` package offers three different visualisations: console
+visualisation, rgb_array visualisation and window visualisation. The window
+visualisation is essentially only rendering the rgb_array visualisation in a
+window using OpenCV. The console visualisation might be used for the `asni`
+mode of a render function, the rgb_array visualisation for the `rgb_array` mode
+and the window visualisation for the `human` mode. # Installation Install the
+package with pip: ``` pip install jsp-vis ``` # Minimal Working Example:
+console visualisation ```python from jsp_vis.console import gantt_chart_console
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
+'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
+'Resource': 'Machine 3'} ]) num_of_machines = 4 gantt_chart_console(df,
+num_of_machines) ``` The code above will render the following Gantt chart in
+the console: ![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/
+main/resources/example_console.png) # Minimal Working Example: console
+visualisation ```python from jsp_vis.cv2_window import render_gantt_in_window
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
 'Resource': 'Machine 3'} ]) num_of_machines = 4 render_gantt_in_window( df=df,
 n_machines=num_of_machines, wait=2000 # time in ms that the `cv2`-window is
 open. # wait=None # ''None'' will keep the window open till a keyboard occurs.
 ) ``` The code above will render the following Gantt chart in the console: ![]
 (https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
```

### Comparing `jsp_vis-1.0.1/pyproject.toml` & `jsp_vis-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsp-vis"
-version = "1.0.1"
+version = "1.0.2"
 description = "A flexible enviorment for job shop scheduling using the disjunctive graph apporach."
 readme = "README.md"
-authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@ima.rwth-aachen.de" }]
+authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@wzl-iqs.rwth-aachen.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
@@ -32,14 +32,14 @@
     "pytest",
     "pytest-cov",
     "tox",
     "twine"
 ]
 
 [project.urls]
-Homepage = "https://github.com/Alexander-Nasuta/pypitemplate"
+Homepage = "https://github.com/Alexander-Nasuta/jsp-vis"
 
 [tool.pytest.ini_options]
 addopts = "--cov=jsp_vis -p no:warnings"
 testpaths = [
     "tests",
 ]
```

### Comparing `jsp_vis-1.0.1/src/jsp_vis/console.py` & `jsp_vis-1.0.2/src/jsp_vis/console.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/src/jsp_vis/cv2_window.py` & `jsp_vis-1.0.2/src/jsp_vis/cv2_window.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/src/jsp_vis/rgb_array.py` & `jsp_vis-1.0.2/src/jsp_vis/rgb_array.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/src/jsp_vis.egg-info/PKG-INFO` & `jsp_vis-1.0.2/src/jsp_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jsp-vis
-Version: 1.0.1
+Version: 1.0.2
 Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
-Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
+Author-email: Alexander Nasuta <alexander.nasuta@wzl-iqs.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2024 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,15 +21,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/Alexander-Nasuta/pypitemplate
+Project-URL: Homepage, https://github.com/Alexander-Nasuta/jsp-vis
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -55,30 +55,26 @@
 <div id="top"></div>
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
    <!--
   <a href="https://cybernetics-lab.de/">
-    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png" alt="Logo" height="80">
+    <img src="https://github.com/Alexander-Nasuta/graph-jsp-env/raw/master/resources/readme_images/logo.png">
   </a>
    -->
 
   <h1 align="center">
      Job Shop Scheduling Problem Visualisations
   </h1>
 
-   
-   <a>
-    <img src="https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif" alt="Logo" height="180">
-  </a>
-
 
 </div>
 
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/ft06_console.gif)
 
 - **Github**: https://github.com/Alexander-Nasuta/jsp-vis
 
 - **PyPi**: https://pypi.org/project/jsp-vis/
 
 
 # About The Project
@@ -91,15 +87,15 @@
 The window visualisation is essentially only rendering the rgb_array visualisation in a window using OpenCV.
 The console visualisation might be used for the `asni` mode of a render function, the rgb_array visualisation for the `rgb_array` mode and the window visualisation for the `human` mode.
 
 # Installation
 
 Install the package with pip:
 ```
-   pip install todo
+   pip install jsp-vis
 ```
 
 # Minimal Working Example: console visualisation
 
 ```python
 from jsp_vis.console import gantt_chart_console
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,73 +1,74 @@
-Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.1 Summary: A flexible
+Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.2 Summary: A flexible
 enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta Author-email: Alexander Nasuta
-ima.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander Nasuta
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/Alexander-
-Nasuta/pypitemplate Platform: unix Platform: linux Platform: osx Platform:
-cygwin Platform: win32 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: opencv-python Requires-Dist: plotly
-Requires-Dist: matplotlib Requires-Dist: numpy Requires-Dist: pandas Requires-
-Dist: kaleido Provides-Extra: dev Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: tox; extra == "dev" Requires-Dist: twine; extra == "dev"
+wzl-iqs.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander
+Nasuta Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions: The above copyright
+notice and this permission notice shall be included in all copies or
+substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT
+WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
+FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
+THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://
+github.com/Alexander-Nasuta/jsp-vis Platform: unix Platform: linux Platform:
+osx Platform: cygwin Platform: win32 Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: opencv-python Requires-Dist:
+plotly Requires-Dist: matplotlib Requires-Dist: numpy Requires-Dist: pandas
+Requires-Dist: kaleido Provides-Extra: dev Requires-Dist: pip-tools; extra ==
+"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
+"dev" Requires-Dist: tox; extra == "dev" Requires-Dist: twine; extra == "dev"
 
            ************ JJoobb SShhoopp SScchheedduulliinngg PPrroobblleemm VViissuuaalliissaattiioonnss ************
-                                    [Logo]
-- **Github**: https://github.com/Alexander-Nasuta/jsp-vis - **PyPi**: https://
-pypi.org/project/jsp-vis/ # About The Project Ths project provides
-visualisation for the Job Shop Scheduling Problem (JSP). This is focused on
-Gantt charts. The input date for the visualisation is inspired by [plotly's
-Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a standalone
-package and in designed to be used in combination with a JSP-reinforcement
-learning environments that follow the [Gymnasium Environment](https://
-gymnasium.farama.org/) standard. The render function of the environment can be
-used to render the Gantt chart. Typically the render function can implement
-different modes like `human`, `rgb_array` or `ansi` rendering. The `jsp-vis`
-package offers three different visualisations: console visualisation, rgb_array
-visualisation and window visualisation. The window visualisation is essentially
-only rendering the rgb_array visualisation in a window using OpenCV. The
-console visualisation might be used for the `asni` mode of a render function,
-the rgb_array visualisation for the `rgb_array` mode and the window
-visualisation for the `human` mode. # Installation Install the package with
-pip: ``` pip install todo ``` # Minimal Working Example: console visualisation
-```python from jsp_vis.console import gantt_chart_console import pandas as pd
-df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish': 16, 'Resource':
-'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31, 'Resource': 'Machine
-1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34, 'Resource': 'Machine 2'},
-{'Task': 'Job 0', 'Start': 34, 'Finish': 46, 'Resource': 'Machine 3'}, {'Task':
-'Job 1', 'Start': 0, 'Finish': 5, 'Resource': 'Machine 0'}, {'Task': 'Job 1',
-'Start': 5, 'Finish': 21, 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start':
-21, 'Finish': 28, 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28,
-'Finish': 32, 'Resource': 'Machine 3'} ]) num_of_machines = 4
-gantt_chart_console(df, num_of_machines) ``` The code above will render the
-following Gantt chart in the console: ![](https://raw.githubusercontent.com/
-Alexander-Nasuta/jsp-vis/main/resources/example_console.png) # Minimal Working
-Example: console visualisation ```python from jsp_vis.cv2_window import
-render_gantt_in_window import pandas as pd df = pd.DataFrame([ {'Task': 'Job
-0', 'Start': 5, 'Finish': 16, 'Resource': 'Machine 0'}, {'Task': 'Job 0',
-'Start': 28, 'Finish': 31, 'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start':
-31, 'Finish': 34, 'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34,
-'Finish': 46, 'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish':
-5, 'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
+ft06_console.gif) - **Github**: https://github.com/Alexander-Nasuta/jsp-vis -
+**PyPi**: https://pypi.org/project/jsp-vis/ # About The Project Ths project
+provides visualisation for the Job Shop Scheduling Problem (JSP). This is
+focused on Gantt charts. The input date for the visualisation is inspired by
+[plotly's Gantt chart api](https://plotly.com/python/gantt/). `jsp-vis` is a
+standalone package and in designed to be used in combination with a JSP-
+reinforcement learning environments that follow the [Gymnasium Environment]
+(https://gymnasium.farama.org/) standard. The render function of the
+environment can be used to render the Gantt chart. Typically the render
+function can implement different modes like `human`, `rgb_array` or `ansi`
+rendering. The `jsp-vis` package offers three different visualisations: console
+visualisation, rgb_array visualisation and window visualisation. The window
+visualisation is essentially only rendering the rgb_array visualisation in a
+window using OpenCV. The console visualisation might be used for the `asni`
+mode of a render function, the rgb_array visualisation for the `rgb_array` mode
+and the window visualisation for the `human` mode. # Installation Install the
+package with pip: ``` pip install jsp-vis ``` # Minimal Working Example:
+console visualisation ```python from jsp_vis.console import gantt_chart_console
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
+'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
+'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
+'Resource': 'Machine 3'} ]) num_of_machines = 4 gantt_chart_console(df,
+num_of_machines) ``` The code above will render the following Gantt chart in
+the console: ![](https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/
+main/resources/example_console.png) # Minimal Working Example: console
+visualisation ```python from jsp_vis.cv2_window import render_gantt_in_window
+import pandas as pd df = pd.DataFrame([ {'Task': 'Job 0', 'Start': 5, 'Finish':
+16, 'Resource': 'Machine 0'}, {'Task': 'Job 0', 'Start': 28, 'Finish': 31,
+'Resource': 'Machine 1'}, {'Task': 'Job 0', 'Start': 31, 'Finish': 34,
+'Resource': 'Machine 2'}, {'Task': 'Job 0', 'Start': 34, 'Finish': 46,
+'Resource': 'Machine 3'}, {'Task': 'Job 1', 'Start': 0, 'Finish': 5,
+'Resource': 'Machine 0'}, {'Task': 'Job 1', 'Start': 5, 'Finish': 21,
 'Resource': 'Machine 2'}, {'Task': 'Job 1', 'Start': 21, 'Finish': 28,
 'Resource': 'Machine 1'}, {'Task': 'Job 1', 'Start': 28, 'Finish': 32,
 'Resource': 'Machine 3'} ]) num_of_machines = 4 render_gantt_in_window( df=df,
 n_machines=num_of_machines, wait=2000 # time in ms that the `cv2`-window is
 open. # wait=None # ''None'' will keep the window open till a keyboard occurs.
 ) ``` The code above will render the following Gantt chart in the console: ![]
 (https://raw.githubusercontent.com/Alexander-Nasuta/jsp-vis/main/resources/
```

### Comparing `jsp_vis-1.0.1/tests/test_render_console.py` & `jsp_vis-1.0.2/tests/test_render_console.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/tests/test_render_cv2_window.py` & `jsp_vis-1.0.2/tests/test_render_cv2_window.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.1/tests/test_render_rgb_array.py` & `jsp_vis-1.0.2/tests/test_render_rgb_array.py`

 * *Files identical despite different names*

