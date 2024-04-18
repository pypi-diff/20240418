# Comparing `tmp/dara_core-1.8.1-py3-none-any.whl.zip` & `tmp/dara_core-1.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3896096 bytes, number of entries: 112
+Zip file size: 3896099 bytes, number of entries: 112
 -rw-r--r--  2.0 unx     2186 b- defN 80-Jan-01 00:00 dara/core/__init__.py
 -rw-r--r--  2.0 unx      965 b- defN 80-Jan-01 00:00 dara/core/actions.py
 -rw-r--r--  2.0 unx      851 b- defN 80-Jan-01 00:00 dara/core/auth/__init__.py
 -rw-r--r--  2.0 unx     2638 b- defN 80-Jan-01 00:00 dara/core/auth/base.py
 -rw-r--r--  2.0 unx     4692 b- defN 80-Jan-01 00:00 dara/core/auth/basic.py
 -rw-r--r--  2.0 unx     3511 b- defN 80-Jan-01 00:00 dara/core/auth/definitions.py
 -rw-r--r--  2.0 unx     4380 b- defN 80-Jan-01 00:00 dara/core/auth/routes.py
@@ -102,13 +102,13 @@
 -rw-r--r--  2.0 unx    13608 b- defN 80-Jan-01 00:00 dara/core/visual/dynamic_component.py
 -rw-r--r--  2.0 unx     5840 b- defN 80-Jan-01 00:00 dara/core/visual/progress_updater.py
 -rw-r--r--  2.0 unx     5707 b- defN 80-Jan-01 00:00 dara/core/visual/template.py
 -rw-r--r--  2.0 unx      794 b- defN 80-Jan-01 00:00 dara/core/visual/themes/__init__.py
 -rw-r--r--  2.0 unx     1942 b- defN 80-Jan-01 00:00 dara/core/visual/themes/dark.py
 -rw-r--r--  2.0 unx     2744 b- defN 80-Jan-01 00:00 dara/core/visual/themes/definitions.py
 -rw-r--r--  2.0 unx     1944 b- defN 80-Jan-01 00:00 dara/core/visual/themes/light.py
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_core-1.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6773 b- defN 80-Jan-01 00:00 dara_core-1.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_core-1.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 dara_core-1.8.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    10153 b- defN 16-Jan-01 00:00 dara_core-1.8.1.dist-info/RECORD
-112 files, 9966267 bytes uncompressed, 3879914 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_core-1.8.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6773 b- defN 80-Jan-01 00:00 dara_core-1.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_core-1.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 dara_core-1.8.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    10153 b- defN 16-Jan-01 00:00 dara_core-1.8.2.dist-info/RECORD
+112 files, 9966267 bytes uncompressed, 3879917 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -315,23 +315,23 @@
 
 Filename: dara/core/visual/themes/definitions.py
 Comment: 
 
 Filename: dara/core/visual/themes/light.py
 Comment: 
 
-Filename: dara_core-1.8.1.dist-info/LICENSE
+Filename: dara_core-1.8.2.dist-info/LICENSE
 Comment: 
 
-Filename: dara_core-1.8.1.dist-info/METADATA
+Filename: dara_core-1.8.2.dist-info/METADATA
 Comment: 
 
-Filename: dara_core-1.8.1.dist-info/WHEEL
+Filename: dara_core-1.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: dara_core-1.8.1.dist-info/entry_points.txt
+Filename: dara_core-1.8.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dara_core-1.8.1.dist-info/RECORD
+Filename: dara_core-1.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dara_core-1.8.1.dist-info/LICENSE` & `dara_core-1.8.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dara_core-1.8.1.dist-info/METADATA` & `dara_core-1.8.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dara-core
-Version: 1.8.1
+Version: 1.8.2
 Summary: Dara Framework Core
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Sam Smith
 Author-email: sam@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: aiorwlock (>=1.4.0,<2.0.0)
 Requires-Dist: anyio (>=4.0.0)
 Requires-Dist: async-asgi-testclient (>=1.4.11,<2.0.0)
 Requires-Dist: click (==8.1.3)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: create-dara-app (==1.8.1)
+Requires-Dist: create-dara-app (==1.8.2)
 Requires-Dist: croniter (>=1.0.15,<2.0.0)
 Requires-Dist: cryptography (>=42.0.4)
-Requires-Dist: dara-components (==1.8.1) ; extra == "all"
+Requires-Dist: dara-components (==1.8.2) ; extra == "all"
 Requires-Dist: exceptiongroup (>=1.1.3,<2.0.0)
 Requires-Dist: fastapi (==0.109.0)
 Requires-Dist: fastapi-vite (==0.3.1)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: jinja2 (>=2.1.1,<3.1.0)
 Requires-Dist: odfpy
 Requires-Dist: openpyxl
@@ -46,15 +46,15 @@
 Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
 Requires-Dist: xlrd
 Project-URL: Repository, https://github.com/causalens/dara
 Description-Content-Type: text/markdown
 
 # Dara Application Framework
 
-<img src="https://github.com/causalens/dara/blob/VERSION-1.8.1/img/dara_light.svg?raw=true">
+<img src="https://github.com/causalens/dara/blob/VERSION-1.8.2/img/dara_light.svg?raw=true">
 
 ![Master tests](https://github.com/causalens/dara/actions/workflows/tests.yml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/dara-core.svg?color=dark-green)](https://pypi.org/project/dara-core/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dara-core.svg?color=dark-green)](https://pypi.org/project/dara-core/)
 [![NPM](https://img.shields.io/npm/v/@darajs/components.svg?color=dark-green)](https://www.npmjs.com/package/@darajs/components)
 
@@ -91,15 +91,15 @@
 poetry run dara start
 
 # with pip installation make sure to activate the new virtual environment
 source .venv/bin/activate
 dara start
 ```
 
-![Dara App](https://github.com/causalens/dara/blob/VERSION-1.8.1/img/components_gallery.png?raw=true)
+![Dara App](https://github.com/causalens/dara/blob/VERSION-1.8.2/img/components_gallery.png?raw=true)
 
 Note: `pip` installation uses [PEP 660](https://peps.python.org/pep-0660/) `pyproject.toml`-based editable installs which require `pip >= 21.3` and `setuptools >= 64.0.0`. You can upgrade both with:
 
 ```bash
 python -m pip install --upgrade pip
 pip install --user --upgrade setuptools
 ```
@@ -108,27 +108,27 @@
 
 ## Dara App examples
 
 Explore some of our favorite apps - a great way of getting started and getting to know the framework!
 
 | Dara App                                                                                                 | Description                                                                                                                                                                                                       |
 | -------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| ![Large Language Model](https://github.com/causalens/dara/blob/VERSION-1.8.1/img/llm.png?raw=true)              | Demonstrates how to use incorporate a LLM chat box into your decision app to understand model insights                                                                                                            |
-| ![Plot Interactivity](https://github.com/causalens/dara/blob/VERSION-1.8.1/img/plot_interactivity.png?raw=true) | Demonstrates how to enable the user to interact with plots, trigger actions based on clicks, mouse movements and other interactions with `Bokeh` or `Plotly` plots                                                |
-| ![Graph Editor](https://github.com/causalens/dara/blob/VERSION-1.8.1/img/graph_viewer.png?raw=true)             | Demonstrates how to use the `CausalGraphViewer` component to display your graphs or networks, customising the displayed information through colors and tooltips, and updating the page based on user interaction. |
+| ![Large Language Model](https://github.com/causalens/dara/blob/VERSION-1.8.2/img/llm.png?raw=true)              | Demonstrates how to use incorporate a LLM chat box into your decision app to understand model insights                                                                                                            |
+| ![Plot Interactivity](https://github.com/causalens/dara/blob/VERSION-1.8.2/img/plot_interactivity.png?raw=true) | Demonstrates how to enable the user to interact with plots, trigger actions based on clicks, mouse movements and other interactions with `Bokeh` or `Plotly` plots                                                |
+| ![Graph Editor](https://github.com/causalens/dara/blob/VERSION-1.8.2/img/graph_viewer.png?raw=true)             | Demonstrates how to use the `CausalGraphViewer` component to display your graphs or networks, customising the displayed information through colors and tooltips, and updating the page based on user interaction. |
 
 Check out our [App Gallery](https://dara.causalens.com/gallery) for more inspiration!
 
 ## Repository introduction
 
 This repository covers the Dara Application Framework first-party packages.
 
 - `dara-core`: The core of the Dara framework, this includes the core framework code for creating applications.
 - `dara-components`: Components for the Dara Framework.
 - `create-dara-app`: A CLI tool for creating new Dara applications.
 
-More information on the repository structure can be found in the [CONTRIBUTING.md](https://github.com/causalens/dara/blob/VERSION-1.8.1/CONTRIBUTING.md) file.
+More information on the repository structure can be found in the [CONTRIBUTING.md](https://github.com/causalens/dara/blob/VERSION-1.8.2/CONTRIBUTING.md) file.
 
 ## License
 
-Dara is open-source and licensed under the [Apache 2.0 License](https://github.com/causalens/dara/blob/VERSION-1.8.1/LICENSE).
+Dara is open-source and licensed under the [Apache 2.0 License](https://github.com/causalens/dara/blob/VERSION-1.8.2/LICENSE).
```

## Comparing `dara_core-1.8.1.dist-info/RECORD` & `dara_core-1.8.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -101,12 +101,12 @@
 dara/core/visual/dynamic_component.py,sha256=bTDTYu12B3wSZmqFPisQvvnA_Q-fyYp0Ds0Y08lE-jM,13608
 dara/core/visual/progress_updater.py,sha256=35_fb_F68YjtYf8MMRA76FoajjfPAlutmqz5fUNgTPs,5840
 dara/core/visual/template.py,sha256=y0KJU2913Q10y1TVMpTVnIxIoUsabzYfpUHEGuX2QyM,5707
 dara/core/visual/themes/__init__.py,sha256=aM4mgoIYo2neBSw5FRzswsht7PUKjLthiHLmFIkyRKw,794
 dara/core/visual/themes/dark.py,sha256=UQGDooOc8ric73eHs9E0ltYP4UCrwqQ3QxqN_fb4PwY,1942
 dara/core/visual/themes/definitions.py,sha256=m3oN0txs65MZepqjj7AKMMxybf2aq5fTjcTwJmHqEbk,2744
 dara/core/visual/themes/light.py,sha256=-Tviq8oEwGbdFULoDOqPuHO0UpAZGsBy8qFi0kAGolQ,1944
-dara_core-1.8.1.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-dara_core-1.8.1.dist-info/METADATA,sha256=g6nFtODTk76trY-faIyd4mKom5JcFs-zSk3kQgfWuq4,6773
-dara_core-1.8.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-dara_core-1.8.1.dist-info/entry_points.txt,sha256=H__D5sNIGuPIhVam0DChNL-To5k8Y7nY7TAFz9Mz6cc,139
-dara_core-1.8.1.dist-info/RECORD,,
+dara_core-1.8.2.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+dara_core-1.8.2.dist-info/METADATA,sha256=h2SeJJg0Yiexzi-uHzFpHmJv-95ch9J-u76-_QHcB80,6773
+dara_core-1.8.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+dara_core-1.8.2.dist-info/entry_points.txt,sha256=H__D5sNIGuPIhVam0DChNL-To5k8Y7nY7TAFz9Mz6cc,139
+dara_core-1.8.2.dist-info/RECORD,,
```

