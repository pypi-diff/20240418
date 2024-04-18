# Comparing `tmp/starrailcard-2.1.3.tar.gz` & `tmp/starrailcard-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.3.tar", max compression
+gzip compressed data, was "starrailcard-2.1.5.tar", max compression
```

## Comparing `starrailcard-2.1.3.tar` & `starrailcard-2.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.3/LICENSE
--rw-r--r--   0        0        0     1165 2024-04-17 16:14:22.125126 starrailcard-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.3/README.md
--rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.3/starrailcard/__init__.py
--rw-r--r--   0        0        0    11836 2024-04-17 16:12:22.105894 starrailcard-2.1.3/starrailcard/client.py
--rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.3/starrailcard/requirements.txt
--rw-r--r--   0        0        0     2461 2024-04-14 21:56:24.992763 starrailcard-2.1.3/starrailcard/src/api/api.py
--rw-r--r--   0        0        0     3487 2024-04-14 22:43:00.884583 starrailcard-2.1.3/starrailcard/src/api/enka.py
--rw-r--r--   0        0        0    25187 2024-04-14 22:52:21.950058 starrailcard-2.1.3/starrailcard/src/api/enka_parsed.py
--rw-r--r--   0        0        0      487 2024-04-09 16:19:13.263140 starrailcard-2.1.3/starrailcard/src/api/error.py
--rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.3/starrailcard/src/assets/font/font_hsr.ttf
--rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.3/starrailcard/src/data/avatar.json
--rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.3/starrailcard/src/data/element.json
--rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.3/starrailcard/src/data/keys.json
--rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.3/starrailcard/src/data/paths.json
--rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.3/starrailcard/src/data/relict_sets.json
--rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.3/starrailcard/src/data/stats.json
--rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.3/starrailcard/src/data/weapons.json
--rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.3/starrailcard/src/generator/style_profile_phone.py
--rw-r--r--   0        0        0    24567 2024-04-17 16:11:52.691388 starrailcard-2.1.3/starrailcard/src/generator/style_relict_score.py
--rw-r--r--   0        0        0    30356 2024-04-17 16:11:41.400283 starrailcard-2.1.3/starrailcard/src/generator/style_ticket.py
--rw-r--r--   0        0        0    11769 2024-04-14 20:59:53.695835 starrailcard-2.1.3/starrailcard/src/model/api_mihomo.py
--rw-r--r--   0        0        0     4759 2024-04-13 14:26:08.588002 starrailcard-2.1.3/starrailcard/src/model/StarRailCard.py
--rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.3/starrailcard/src/model/style.py
--rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.3/starrailcard/src/model/ukrainization_model.py
--rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.3/starrailcard/src/model/utils_model.py
--rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/max.json
--rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/score.json
--rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.3/starrailcard/src/tools/calculator/src/utils.py
--rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.3/starrailcard/src/tools/calculator/stats.py
--rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.3/starrailcard/src/tools/cashe.py
--rw-r--r--   0        0        0      709 2024-04-09 17:29:46.754642 starrailcard-2.1.3/starrailcard/src/tools/enums.py
--rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.3/starrailcard/src/tools/git.py
--rw-r--r--   0        0        0    10025 2024-04-14 05:20:03.169865 starrailcard-2.1.3/starrailcard/src/tools/http.py
--rw-r--r--   0        0        0      938 2024-04-09 16:56:51.818599 starrailcard-2.1.3/starrailcard/src/tools/json_data.py
--rw-r--r--   0        0        0     6341 2024-04-14 04:42:09.584031 starrailcard-2.1.3/starrailcard/src/tools/options.py
--rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.3/starrailcard/src/tools/pill/__init__.py
--rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.3/starrailcard/src/tools/pill/color.py
--rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.3/starrailcard/src/tools/pill/color_controle.py
--rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.3/starrailcard/src/tools/pill/grandiend_v2.py
--rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.3/starrailcard/src/tools/pill/grandient_v1.py
--rw-r--r--   0        0        0     3952 2024-04-14 22:23:43.804859 starrailcard-2.1.3/starrailcard/src/tools/pill/image_controle.py
--rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.3/starrailcard/src/tools/pill/style_editor.py
--rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.3/starrailcard/src/tools/pill/text_controle.py
--rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.3/starrailcard/src/tools/translator.py
--rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.3/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.3/starrailcard/src/tools/ukrainization.py
--rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.3/starrailcard/utils.py
--rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 starrailcard-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.5/LICENSE
+-rw-r--r--   0        0        0     1106 2024-04-18 21:49:53.836647 starrailcard-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.5/README.md
+-rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.5/starrailcard/__init__.py
+-rw-r--r--   0        0        0    11836 2024-04-17 16:12:22.105894 starrailcard-2.1.5/starrailcard/client.py
+-rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.5/starrailcard/requirements.txt
+-rw-r--r--   0        0        0     2461 2024-04-14 21:56:24.992763 starrailcard-2.1.5/starrailcard/src/api/api.py
+-rw-r--r--   0        0        0     3487 2024-04-14 22:43:00.884583 starrailcard-2.1.5/starrailcard/src/api/enka.py
+-rw-r--r--   0        0        0    25187 2024-04-14 22:52:21.950058 starrailcard-2.1.5/starrailcard/src/api/enka_parsed.py
+-rw-r--r--   0        0        0      487 2024-04-09 16:19:13.263140 starrailcard-2.1.5/starrailcard/src/api/error.py
+-rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.5/starrailcard/src/assets/font/font_hsr.ttf
+-rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.5/starrailcard/src/data/avatar.json
+-rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.5/starrailcard/src/data/element.json
+-rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.5/starrailcard/src/data/keys.json
+-rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.5/starrailcard/src/data/paths.json
+-rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.5/starrailcard/src/data/relict_sets.json
+-rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.5/starrailcard/src/data/stats.json
+-rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.5/starrailcard/src/data/weapons.json
+-rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.5/starrailcard/src/generator/style_profile_phone.py
+-rw-r--r--   0        0        0    24567 2024-04-17 16:11:52.691388 starrailcard-2.1.5/starrailcard/src/generator/style_relict_score.py
+-rw-r--r--   0        0        0    30356 2024-04-17 16:11:41.400283 starrailcard-2.1.5/starrailcard/src/generator/style_ticket.py
+-rw-r--r--   0        0        0    11769 2024-04-14 20:59:53.695835 starrailcard-2.1.5/starrailcard/src/model/api_mihomo.py
+-rw-r--r--   0        0        0     4759 2024-04-13 14:26:08.588002 starrailcard-2.1.5/starrailcard/src/model/StarRailCard.py
+-rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.5/starrailcard/src/model/style.py
+-rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.5/starrailcard/src/model/ukrainization_model.py
+-rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.5/starrailcard/src/model/utils_model.py
+-rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.5/starrailcard/src/tools/calculator/src/utils.py
+-rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.5/starrailcard/src/tools/calculator/stats.py
+-rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.5/starrailcard/src/tools/cashe.py
+-rw-r--r--   0        0        0      709 2024-04-09 17:29:46.754642 starrailcard-2.1.5/starrailcard/src/tools/enums.py
+-rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.5/starrailcard/src/tools/git.py
+-rw-r--r--   0        0        0    10025 2024-04-14 05:20:03.169865 starrailcard-2.1.5/starrailcard/src/tools/http.py
+-rw-r--r--   0        0        0      938 2024-04-09 16:56:51.818599 starrailcard-2.1.5/starrailcard/src/tools/json_data.py
+-rw-r--r--   0        0        0     6341 2024-04-14 04:42:09.584031 starrailcard-2.1.5/starrailcard/src/tools/options.py
+-rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.5/starrailcard/src/tools/pill/__init__.py
+-rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.5/starrailcard/src/tools/pill/color.py
+-rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.5/starrailcard/src/tools/pill/color_controle.py
+-rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.5/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.5/starrailcard/src/tools/pill/grandient_v1.py
+-rw-r--r--   0        0        0     3952 2024-04-14 22:23:43.804859 starrailcard-2.1.5/starrailcard/src/tools/pill/image_controle.py
+-rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.5/starrailcard/src/tools/pill/style_editor.py
+-rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.5/starrailcard/src/tools/pill/text_controle.py
+-rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.5/starrailcard/src/tools/translator.py
+-rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.5/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.5/starrailcard/src/tools/ukrainization.py
+-rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.5/starrailcard/utils.py
+-rw-r--r--   0        0        0     4845 1970-01-01 00:00:00.000000 starrailcard-2.1.5/PKG-INFO
```

### Comparing `starrailcard-2.1.3/LICENSE` & `starrailcard-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/pyproject.toml` & `starrailcard-2.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "starrailcard"
-version = "2.1.3"
+version = "2.1.5"
 description = "This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players."
 authors = ["DEViantUA <deviantapi@gmail.com>"]
 license = "MIT License with Additional Restrictions"
 
 readme = 'README.md'  # Markdown files are supported
 
 repository = "https://github.com/DEViantUA/StarRailCard"
 homepage = "https://github.com/DEViantUA/StarRailCard"
 
 keywords = ["honkai", "cards", "generation", "honkaistarraill","raill", "starraill", "builds", "honkairail", "honkai"] 
 
 [tool.poetry.dependencies]
-Pillow = "^10.0.1"
+Pillow = "*"
 python = "^3.9"
-aiofiles = "^0.7.0"
-aiohttp = "^3.8.1"
-cachetools = "^5.3.1"
-imageio = "^2.14.0"
-moviepy = "^1.0.3"
-more-itertools = "^8.9.0"
-numpy = "^1.21.2"
-pydantic = "^1.9.0"
-beautifulsoup4 = "^4.12.3"
-anyio = "^4.3.0"
+aiofiles = "*"
+aiohttp = "*"
+cachetools = "*"
+imageio = "*"
+moviepy = "*"
+more-itertools = "*"
+numpy = "*"
+pydantic = "*"
+beautifulsoup4 = "*"
+anyio = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `starrailcard-2.1.3/README.md` & `starrailcard-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/client.py` & `starrailcard-2.1.5/starrailcard/client.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/api/api.py` & `starrailcard-2.1.5/starrailcard/src/api/api.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/api/enka.py` & `starrailcard-2.1.5/starrailcard/src/api/enka.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.1.5/starrailcard/src/api/enka_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.5/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/data/avatar.json` & `starrailcard-2.1.5/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.5/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/data/stats.json` & `starrailcard-2.1.5/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/data/weapons.json` & `starrailcard-2.1.5/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.5/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.5/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.5/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.1.5/starrailcard/src/model/api_mihomo.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.5/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/model/style.py` & `starrailcard-2.1.5/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.5/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.5/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.5/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.5/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/enums.py` & `starrailcard-2.1.5/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/git.py` & `starrailcard-2.1.5/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/http.py` & `starrailcard-2.1.5/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.5/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/options.py` & `starrailcard-2.1.5/starrailcard/src/tools/options.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/image_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.5/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/translator.py` & `starrailcard-2.1.5/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/treePaths.py` & `starrailcard-2.1.5/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.5/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/starrailcard/utils.py` & `starrailcard-2.1.5/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.3/PKG-INFO` & `starrailcard-2.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.3
+Version: 2.1.5
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 License: MIT License with Additional Restrictions
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Author: DEViantUA
 Author-email: deviantapi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=10.0.1,<11.0.0)
-Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: anyio (>=4.3.0,<5.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: cachetools (>=5.3.1,<6.0.0)
-Requires-Dist: imageio (>=2.14.0,<3.0.0)
-Requires-Dist: more-itertools (>=8.9.0,<9.0.0)
-Requires-Dist: moviepy (>=1.0.3,<2.0.0)
-Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: Pillow
+Requires-Dist: aiofiles
+Requires-Dist: aiohttp
+Requires-Dist: anyio
+Requires-Dist: beautifulsoup4
+Requires-Dist: cachetools
+Requires-Dist: imageio
+Requires-Dist: more-itertools
+Requires-Dist: moviepy
+Requires-Dist: numpy
+Requires-Dist: pydantic
 Project-URL: Repository, https://github.com/DEViantUA/StarRailCard
 Description-Content-Type: text/markdown
 
 <p align="center">
  <img src="https://raw.githubusercontent.com/DEViantUA/StarRailCard/main/Examples/image/starRailCardBanner.png" alt="Баннер"/>
 </p>
```

