# Comparing `tmp/glide-client-0.0.1a3.tar.gz` & `tmp/glide_client-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glide-client-0.0.1a3.tar", last modified: Sun Feb 18 18:54:29 2024, max compression
+gzip compressed data, was "glide_client-0.0.1a4.tar", last modified: Thu Apr 18 21:58:49 2024, max compression
```

## Comparing `glide-client-0.0.1a3.tar` & `glide_client-0.0.1a4.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-02-18 18:54:29.880726 glide-client-0.0.1a3/
--rw-r--r--   0 roman      (501) staff       (20)    11356 2024-02-18 17:14:00.000000 glide-client-0.0.1a3/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)     2113 2024-02-18 18:54:29.880190 glide-client-0.0.1a3/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     1459 2024-02-18 18:50:40.000000 glide-client-0.0.1a3/README.md
--rw-r--r--   0 roman      (501) staff       (20)      742 2024-02-18 18:54:23.000000 glide-client-0.0.1a3/pyproject.toml
--rw-r--r--   0 roman      (501) staff       (20)       38 2024-02-18 18:54:29.880833 glide-client-0.0.1a3/setup.cfg
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-02-18 18:54:29.873578 glide-client-0.0.1a3/src/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-02-18 18:54:29.875681 glide-client-0.0.1a3/src/glide/
--rw-r--r--   0 roman      (501) staff       (20)       59 2024-02-18 18:37:05.000000 glide-client-0.0.1a3/src/glide/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)        0 2024-02-18 18:34:29.000000 glide-client-0.0.1a3/src/glide/py.typed
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-02-18 18:54:29.876756 glide-client-0.0.1a3/src/glide/schemas/
--rw-r--r--   0 roman      (501) staff       (20)       59 2024-02-18 18:37:02.000000 glide-client-0.0.1a3/src/glide/schemas/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)       59 2024-02-18 18:37:02.000000 glide-client-0.0.1a3/src/glide/schemas/lang.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-02-18 18:54:29.879586 glide-client-0.0.1a3/src/glide_client.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)     2113 2024-02-18 18:54:29.000000 glide-client-0.0.1a3/src/glide_client.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)      328 2024-02-18 18:54:29.000000 glide-client-0.0.1a3/src/glide_client.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2024-02-18 18:54:29.000000 glide-client-0.0.1a3/src/glide_client.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)       47 2024-02-18 18:54:29.000000 glide-client-0.0.1a3/src/glide_client.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)        6 2024-02-18 18:54:29.000000 glide-client-0.0.1a3/src/glide_client.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11356 2024-04-18 21:58:33.530156 glide_client-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     1498 2024-04-18 21:58:33.530156 glide_client-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1284 2024-04-18 21:58:49.506261 glide_client-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/async_client.py
+-rw-r--r--   0        0        0      759 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/exceptions.py
+-rw-r--r--   0        0        0      351 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/lang/__init__.py
+-rw-r--r--   0        0        0     8657 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/lang/router_async.py
+-rw-r--r--   0        0        0     3544 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/lang/schemas.py
+-rw-r--r--   0        0        0      111 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/logging.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/py.typed
+-rw-r--r--   0        0        0      457 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/schames.py
+-rw-r--r--   0        0        0       59 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/testing/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/src/glide/typing.py
+-rw-r--r--   0        0        0      297 2024-04-18 21:58:49.506261 glide_client-0.0.1a4/src/glide/version.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:58:33.534156 glide_client-0.0.1a4/tests/__init__.py
+-rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 glide_client-0.0.1a4/PKG-INFO
```

### Comparing `glide-client-0.0.1a3/LICENSE` & `glide_client-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `glide-client-0.0.1a3/PKG-INFO` & `glide_client-0.0.1a4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: glide-client
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: An official Python client for Glide, an open resilient fast model gateway
-Author-email: Roman Hlushko <roman@einstack.ai>
+Keywords: llm,llmops,gateway,infrastructure
+Author-Email: Roman Hlushko <roman@einstack.ai>
 License: Apache-2.0
 Project-URL: Homepage, https://glide.einstack.ai/
 Project-URL: Documentation, https://glide.einstack.ai/
 Project-URL: Repository, https://github.com/me/spam.git
 Project-URL: Issues, https://github.com/EinStack/glide-python
-Keywords: llm,llmops,gateway,infrastructure
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: websockets>=12.0
 Requires-Dist: pydantic>=2.6.1
+Description-Content-Type: text/markdown
 
 <div align="center">
-    <img loading="lazy" src="https://raw.githubusercontent.com/EinStack/glide-python/blob/main/docs/glide_logo.png" alt="Glide Logo" width="200px" height="200px" />
+    <img loading="lazy" src="https://github.com/EinStack/glide-python/blob/main/docs/glide_logo.png?raw=1" alt="Glide Logo" width="200px" height="200px" />
     <h1>Glide Python Client</h1>
     <p>🐍 An official Python client for <a href="https://github.com/EinStack/glide">Glide, an open reliable fast model gateway</a>.</p>
     <a href="https://discord.gg/pt53Ej7rrc"><img src="https://img.shields.io/discord/1181281407813828710" alt="Discord" /></a>
     <a href="https://glide.einstack.ai/"><img src="https://img.shields.io/badge/build-view-violet%20?style=flat&logo=books&label=docs&link=https%3A%2F%2Fglide.einstack.ai%2F" alt="Glide Docs" /></a>
     <a href="https://github.com/EinStack/glide-python/blob/main/LICENSE"><img src="https://img.shields.io/github/license/EinStack/glide-python.svg?style=flat-square&color=%233f90c8" alt="License" /></a>
     <a href="https://artifacthub.io/packages/helm/einstack/glide"><img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/einstack" alt="ArtifactHub" /></a>
 </div>
@@ -32,16 +31,17 @@
 > Glide is under active development right now 🛠️
 
 > [!Important]
 > Give us a star⭐ to support the project and watch👀 our repositories not to miss any update
 
 ## Features
 
-- 🐍Modern typed Python with [Pydantic-based](https://github.com/pydantic/pydantic) data classes
-- Sync and asyncio support
+- 🐍 Modern typed Python with [Pydantic-based](https://github.com/pydantic/pydantic) data classes
+- 🛠️ Sync (soon) and asyncio support
+- 🎭 Easily mockable in tests
 
 ## Installation
 
 Coming soon
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: glide-client Version: 0.0.1a3 Summary: An official
-Python client for Glide, an open resilient fast model gateway Author-email:
-Roman Hlushko
+Metadata-Version: 2.1 Name: glide-client Version: 0.0.1a4 Summary: An official
+Python client for Glide, an open resilient fast model gateway Keywords:
+llm,llmops,gateway,infrastructure Author-Email: Roman Hlushko
 einstack.ai> License: Apache-2.0 Project-URL: Homepage, https://
 glide.einstack.ai/ Project-URL: Documentation, https://glide.einstack.ai/
 Project-URL: Repository, https://github.com/me/spam.git Project-URL: Issues,
-https://github.com/EinStack/glide-python Keywords:
-llm,llmops,gateway,infrastructure Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: httpx>=0.26.0
-Requires-Dist: websockets>=12.0 Requires-Dist: pydantic>=2.6.1
+https://github.com/EinStack/glide-python Requires-Python: >=3.8 Requires-Dist:
+httpx>=0.26.0 Requires-Dist: websockets>=12.0 Requires-Dist: pydantic>=2.6.1
+Description-Content-Type: text/markdown
                                  [Glide Logo]
                        ************ GGlliiddee PPyytthhoonn CClliieenntt ************
 ð An official Python client for _G_l_i_d_e_,_ _a_n_ _o_p_e_n_ _r_e_l_i_a_b_l_e_ _f_a_s_t_ _m_o_d_e_l_ _g_a_t_e_w_a_y.
                   _[_D_i_s_c_o_r_d_]_[_G_l_i_d_e_ _D_o_c_s_]_[_L_i_c_e_n_s_e_]_[_A_r_t_i_f_a_c_t_H_u_b_]
 --- > [!Warning] > Glide is under active development right now ð ï¸ >
 [!Important] > Give us a starâ­ to support the project and watchð our
-repositories not to miss any update ## Features - ðModern typed Python with
-[Pydantic-based](https://github.com/pydantic/pydantic) data classes - Sync and
-asyncio support ## Installation Coming soon ## Usage Coming soon
+repositories not to miss any update ## Features - ð Modern typed Python with
+[Pydantic-based](https://github.com/pydantic/pydantic) data classes - ð ï¸
+Sync (soon) and asyncio support - ð­ Easily mockable in tests ## Installation
+Coming soon ## Usage Coming soon
```

### Comparing `glide-client-0.0.1a3/README.md` & `glide_client-0.0.1a4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-    <img loading="lazy" src="https://raw.githubusercontent.com/EinStack/glide-python/blob/main/docs/glide_logo.png" alt="Glide Logo" width="200px" height="200px" />
+    <img loading="lazy" src="https://github.com/EinStack/glide-python/blob/main/docs/glide_logo.png?raw=1" alt="Glide Logo" width="200px" height="200px" />
     <h1>Glide Python Client</h1>
     <p>🐍 An official Python client for <a href="https://github.com/EinStack/glide">Glide, an open reliable fast model gateway</a>.</p>
     <a href="https://discord.gg/pt53Ej7rrc"><img src="https://img.shields.io/discord/1181281407813828710" alt="Discord" /></a>
     <a href="https://glide.einstack.ai/"><img src="https://img.shields.io/badge/build-view-violet%20?style=flat&logo=books&label=docs&link=https%3A%2F%2Fglide.einstack.ai%2F" alt="Glide Docs" /></a>
     <a href="https://github.com/EinStack/glide-python/blob/main/LICENSE"><img src="https://img.shields.io/github/license/EinStack/glide-python.svg?style=flat-square&color=%233f90c8" alt="License" /></a>
     <a href="https://artifacthub.io/packages/helm/einstack/glide"><img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/einstack" alt="ArtifactHub" /></a>
 </div>
@@ -14,16 +14,17 @@
 > Glide is under active development right now 🛠️
 
 > [!Important]
 > Give us a star⭐ to support the project and watch👀 our repositories not to miss any update
 
 ## Features
 
-- 🐍Modern typed Python with [Pydantic-based](https://github.com/pydantic/pydantic) data classes
-- Sync and asyncio support
+- 🐍 Modern typed Python with [Pydantic-based](https://github.com/pydantic/pydantic) data classes
+- 🛠️ Sync (soon) and asyncio support
+- 🎭 Easily mockable in tests
 
 ## Installation
 
 Coming soon
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
                                  [Glide Logo]
                        ************ GGlliiddee PPyytthhoonn CClliieenntt ************
 ð An official Python client for _G_l_i_d_e_,_ _a_n_ _o_p_e_n_ _r_e_l_i_a_b_l_e_ _f_a_s_t_ _m_o_d_e_l_ _g_a_t_e_w_a_y.
                   _[_D_i_s_c_o_r_d_]_[_G_l_i_d_e_ _D_o_c_s_]_[_L_i_c_e_n_s_e_]_[_A_r_t_i_f_a_c_t_H_u_b_]
 --- > [!Warning] > Glide is under active development right now ð ï¸ >
 [!Important] > Give us a starâ­ to support the project and watchð our
-repositories not to miss any update ## Features - ðModern typed Python with
-[Pydantic-based](https://github.com/pydantic/pydantic) data classes - Sync and
-asyncio support ## Installation Coming soon ## Usage Coming soon
+repositories not to miss any update ## Features - ð Modern typed Python with
+[Pydantic-based](https://github.com/pydantic/pydantic) data classes - ð ï¸
+Sync (soon) and asyncio support - ð­ Easily mockable in tests ## Installation
+Coming soon ## Usage Coming soon
```

### Comparing `glide-client-0.0.1a3/pyproject.toml` & `glide_client-0.0.1a4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 [project]
 name = "glide-client"
-version = "0.0.1-alpha.3"
 description = "An official Python client for Glide, an open resilient fast model gateway"
-license = {text = "Apache-2.0"}
 authors = [
-    {name = "Roman Hlushko", email = "roman@einstack.ai"},
+    { name = "Roman Hlushko", email = "roman@einstack.ai" },
 ]
-
+dynamic = []
 readme = "README.md"
 keywords = [
     "llm",
     "llmops",
     "gateway",
     "infrastructure",
 ]
-
 dependencies = [
     "httpx>=0.26.0",
     "websockets>=12.0",
     "pydantic>=2.6.1",
 ]
 requires-python = ">=3.8"
+version = "0.0.1a4"
+
+[project.license]
+text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://glide.einstack.ai/"
 Documentation = "https://glide.einstack.ai/"
 Repository = "https://github.com/me/spam.git"
 Issues = "https://github.com/EinStack/glide-python"
 
+[tool.pdm]
+distribution = true
+
+[tool.pdm.version]
+source = "scm"
+write_to = "glide/version.py"
+write_template = "# Copyright EinStack\n# SPDX-License-Identifier: APACHE-2.0\nimport sys\nfrom typing import Final\n\n\nPYTHON_VERSION: Final[str] = \".\".join(\n    (\n        str(sys.version_info.major),\n        str(sys.version_info.minor),\n        str(sys.version_info.micro),\n    )\n)\n__version__: Final[str] = \"{}\"\n"
+
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff>=0.2.2",
     "mypy>=1.8.0",
+    "black>=24.2.0",
+]
+
+[build-system]
+requires = [
+    "pdm-backend",
 ]
+build-backend = "pdm.backend"
```

