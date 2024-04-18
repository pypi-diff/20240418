# Comparing `tmp/env_wrangler-0.1.0.tar.gz` & `tmp/env_wrangler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_wrangler-0.1.0.tar", last modified: Wed Apr 17 22:07:43 2024, max compression
+gzip compressed data, was "env_wrangler-0.1.1.tar", last modified: Thu Apr 18 16:30:21 2024, max compression
```

## Comparing `env_wrangler-0.1.0.tar` & `env_wrangler-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.895646 env_wrangler-0.1.0/
--rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.0/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      187 2024-04-15 19:14:54.000000 env_wrangler-0.1.0/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.0/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.0/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     3095 2024-04-17 22:07:43.895399 env_wrangler-0.1.0/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1686 2024-04-17 21:53:33.000000 env_wrangler-0.1.0/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.0/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.891784 env_wrangler-0.1.0/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.0/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.0/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.0/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-17 22:07:43.895696 env_wrangler-0.1.0/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.0/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.889353 env_wrangler-0.1.0/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.893124 env_wrangler-0.1.0/src/env_wrangler/
--rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-17 18:51:55.000000 env_wrangler-0.1.0/src/env_wrangler/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     4972 2024-04-17 22:00:33.000000 env_wrangler-0.1.0/src/env_wrangler/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)       85 2024-04-17 21:59:30.000000 env_wrangler-0.1.0/src/env_wrangler/constants.py
--rw-r--r--   0 tsantor    (501) staff       (20)     3401 2024-04-17 22:00:34.000000 env_wrangler-0.1.0/src/env_wrangler/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.894260 env_wrangler-0.1.0/src/env_wrangler/data/
--rw-r--r--   0 tsantor    (501) staff       (20)      405 2024-04-17 19:45:34.000000 env_wrangler-0.1.0/src/env_wrangler/data/env-wrangler.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-17 21:29:40.000000 env_wrangler-0.1.0/src/env_wrangler/settings.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.895163 env_wrangler-0.1.0/src/env_wrangler.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     3095 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      634 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-17 22:07:43.000000 env_wrangler-0.1.0/src/env_wrangler.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-17 22:07:43.894854 env_wrangler-0.1.0/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     5026 2024-04-17 22:01:47.000000 env_wrangler-0.1.0/tests/test_core.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.0/tests/test_settings.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.388373 env_wrangler-0.1.1/
+-rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      187 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.1/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     3292 2024-04-18 16:30:21.388098 env_wrangler-0.1.1/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.1/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.1/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.383588 env_wrangler-0.1.1/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.1/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.1/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.1/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-18 16:30:21.388438 env_wrangler-0.1.1/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.381051 env_wrangler-0.1.1/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.385187 env_wrangler-0.1.1/src/env_wrangler/
+-rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-18 16:01:14.000000 env_wrangler-0.1.1/src/env_wrangler/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     6182 2024-04-18 16:19:08.000000 env_wrangler-0.1.1/src/env_wrangler/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)       85 2024-04-18 13:55:19.000000 env_wrangler-0.1.1/src/env_wrangler/constants.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     4031 2024-04-18 16:26:57.000000 env_wrangler-0.1.1/src/env_wrangler/core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.386390 env_wrangler-0.1.1/src/env_wrangler/data/
+-rw-r--r--   0 tsantor    (501) staff       (20)      564 2024-04-18 16:12:33.000000 env_wrangler-0.1.1/src/env_wrangler/data/env-wrangler.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.1/src/env_wrangler/settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.1/src/env_wrangler/utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.387836 env_wrangler-0.1.1/src/env_wrangler.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     3292 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.387431 env_wrangler-0.1.1/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     5595 2024-04-18 15:41:07.000000 env_wrangler-0.1.1/tests/test_core.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.1/tests/test_settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.1/tests/test_utils.py
```

### Comparing `env_wrangler-0.1.0/LICENSE` & `env_wrangler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.0/PKG-INFO` & `env_wrangler-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,20 +21,22 @@
 License-File: AUTHORS.md
 Requires-Dist: python-dotenv
 Requires-Dist: click
 Provides-Extra: dev
 
 # Env Wrangler
 
-![Coverage](https://img.shields.io/badge/coverage-97%25-brightgreen)
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Overview
 
 Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 
+Plays nice with [cookiecutter-django](https://github.com/cookiecutter/cookiecutter-django).
+
 ## Installation
 
 ```bash
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
@@ -73,14 +75,15 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 # TODO
 - Add tests for cli commands
+- Write secrets to file non-destructively (eg - add key if not there, remove key if no longer present)
 
 ## Issues
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
```

### Comparing `env_wrangler-0.1.0/README.md` & `env_wrangler-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Env Wrangler
 
-![Coverage](https://img.shields.io/badge/coverage-97%25-brightgreen)
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Overview
 
 Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 
+Plays nice with [cookiecutter-django](https://github.com/cookiecutter/cookiecutter-django).
+
 ## Installation
 
 ```bash
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
@@ -48,11 +50,12 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 # TODO
 - Add tests for cli commands
+- Write secrets to file non-destructively (eg - add key if not there, remove key if no longer present)
 
 ## Issues
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
```

### Comparing `env_wrangler-0.1.0/pyproject.toml` & `env_wrangler-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.0/src/env_wrangler/core.py` & `env_wrangler-0.1.1/src/env_wrangler/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,46 +11,65 @@
     config = {}
     for env_file in env_files:
         config |= dotenv_values(env_file)
     return config
 
 
 def save_dict_to_json_file(data: dict, file_path: Path) -> Path:
-    """Save a dictionary to a JSON file."""
+    """Save a dictionary to a JSON file (non-destructive)."""
     if not data:
         return None
     file_path = Path(file_path).expanduser()
-    file_path.write_text(json.dumps(data, indent=2))
+    if file_path.exists():
+        existing_data = json.loads(file_path.read_text())
+        existing_data.update(data)
+        data = existing_data
+    # We ensure it is sorted before writing
+    file_path.write_text(json.dumps(data, indent=2, sort_keys=True))
     return file_path
 
 
 def save_dict_to_env_file(data: dict, file_path: str) -> Path:
-    """Save a dictionary to an env file."""
+    """Save a dictionary to an env file (non-destructive)."""
     if not data:
         return None
-    env_content = "\n".join([f"{key}={value}" for key, value in data.items()])
     file_path = Path(file_path).expanduser()
+    if file_path.exists():
+        existing_data = dict(
+            line.split("=") for line in file_path.read_text().splitlines() if line
+        )
+        existing_data.update(data)
+        data = existing_data
+    # We ensure it is sorted before writing
+    env_content = "\n".join([f"{key}={value}" for key, value in sorted(data.items())])
     file_path.write_text(env_content)
     return file_path
 
 
 def filter_keys_by_substring(input_dict: dict, words_to_keep: list[str]) -> dict:
     """
     Filters a dictionary to keep only keys that include any of the specified words.
 
     :param input_dict: Dictionary to be filtered.
     :param words_to_keep: List of words to check against the keys in the dictionary.
     """
-    secrets = {
+    return {
         key: input_dict[key]
         for key in input_dict
         if any(word in key for word in words_to_keep)
     }
-    # Safeguard to prevent extracting masked values
-    return {key: value for key, value in secrets.items() if value != MASK_VALUE}
+
+
+def remove_masked_values(input_dict: dict) -> dict:
+    """
+    Filters a dictionary to remove masked values.
+
+    :param input_dict: Dictionary to be filtered.
+    """
+    return {key: value for key, value in input_dict.items() if value != MASK_VALUE}
 
 
 def mask_sensitive_data_in_file(file_path: str, filter_keys: list) -> Path:
     """Mask sensitive data in a .env file.
 
     Args:
         file_path (str): The path to the .env file.
```

### Comparing `env_wrangler-0.1.0/src/env_wrangler/settings.py` & `env_wrangler-0.1.1/src/env_wrangler/settings.py`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.0/src/env_wrangler.egg-info/PKG-INFO` & `env_wrangler-0.1.1/src/env_wrangler.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,20 +21,22 @@
 License-File: AUTHORS.md
 Requires-Dist: python-dotenv
 Requires-Dist: click
 Provides-Extra: dev
 
 # Env Wrangler
 
-![Coverage](https://img.shields.io/badge/coverage-97%25-brightgreen)
+![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Overview
 
 Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 
+Plays nice with [cookiecutter-django](https://github.com/cookiecutter/cookiecutter-django).
+
 ## Installation
 
 ```bash
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
@@ -73,14 +75,15 @@
 make pytest
 make coverage
 make open_coverage
 ```
 
 # TODO
 - Add tests for cli commands
+- Write secrets to file non-destructively (eg - add key if not there, remove key if no longer present)
 
 ## Issues
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
```

### Comparing `env_wrangler-0.1.0/src/env_wrangler.egg-info/SOURCES.txt` & `env_wrangler-0.1.1/src/env_wrangler.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 requirements/requirements_dev.txt
 requirements/requirements_test.txt
 src/env_wrangler/__init__.py
 src/env_wrangler/cli.py
 src/env_wrangler/constants.py
 src/env_wrangler/core.py
 src/env_wrangler/settings.py
+src/env_wrangler/utils.py
 src/env_wrangler.egg-info/PKG-INFO
 src/env_wrangler.egg-info/SOURCES.txt
 src/env_wrangler.egg-info/dependency_links.txt
 src/env_wrangler.egg-info/entry_points.txt
 src/env_wrangler.egg-info/requires.txt
 src/env_wrangler.egg-info/top_level.txt
 src/env_wrangler/data/env-wrangler.cfg
 tests/test_core.py
-tests/test_settings.py
+tests/test_settings.py
+tests/test_utils.py
```

### Comparing `env_wrangler-0.1.0/tests/test_core.py` & `env_wrangler-0.1.1/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from dotenv import dotenv_values
 from env_wrangler.constants import MASK_VALUE
 from env_wrangler.core import envs_to_dict
 from env_wrangler.core import filter_keys_by_substring
 from env_wrangler.core import json_to_env
 from env_wrangler.core import mask_sensitive_data_in_file
+from env_wrangler.core import remove_masked_values
 from env_wrangler.core import save_dict_to_env_file
 from env_wrangler.core import save_dict_to_json_file
 from env_wrangler.core import unmask_sensitive_data_in_file
 
 
 def test_envs_to_dict(tmp_path):
     # Create two .env files in the temporary directory
@@ -28,14 +29,15 @@
         "KEY4": "VALUE4",
     }
 
 
 def test_save_dict_to_json_file(tmp_path):
     data = {"key1": "value1", "key2": "value2"}
     file_path = tmp_path / "test.json"
+    file_path.write_text(json.dumps(data, sort_keys=True))
     output_file = save_dict_to_json_file(data, str(file_path))
 
     file_path = Path(file_path)
     loaded_data = json.loads(file_path.read_text())
 
     assert isinstance(output_file, Path)
     assert loaded_data == data
@@ -46,16 +48,18 @@
     file_path = tmp_path / "test.json"
     output_file = save_dict_to_json_file(data, str(file_path))
 
     assert output_file is None
 
 
 def test_save_dict_to_env_file(tmp_path):
-    data = {"key1": "value1", "key2": "value2"}
+    data = {"key1": "value1", "key2": "value2", "key3": "value3", "key4": "value4"}
     file_path = tmp_path / "test.env"
+    # Write only a few keys to the file to test that the function appends new keys
+    file_path.write_text("key1=value1\nkey2=value2")
     output_file = save_dict_to_env_file(data, str(file_path))
 
     file_path = Path(file_path)
     lines = file_path.read_text().splitlines()
 
     loaded_data = {}
     for line in lines:
@@ -87,14 +91,26 @@
 
     assert result == {
         "ACCESS_KEY": "my-access-key",
         "ACCESS_TOKEN": "my-access-token",
     }
 
 
+def test_remove_masked_values():
+    input_dict = {
+        "key1": "value1",
+        "key2": MASK_VALUE,
+        "key3": "value3",
+        "key4": MASK_VALUE,
+    }
+    expected_dict = {"key1": "value1", "key3": "value3"}
+
+    assert remove_masked_values(input_dict) == expected_dict
+
+
 def test_mask_sensitive_data_in_file(tmp_path):
     # Create a .env file in the temporary directory
     env_file = tmp_path / ".env"
     env_file.write_text("SECRET_KEY=secret\nPASSWORD=password\nFOO=bar\nBAR=baz")
 
     # Call mask_sensitive_data with the path to the .env file and a list of sensitive keys
     output_file = mask_sensitive_data_in_file(str(env_file), ["SECRET_KEY", "PASSWORD"])
```

### Comparing `env_wrangler-0.1.0/tests/test_settings.py` & `env_wrangler-0.1.1/tests/test_settings.py`

 * *Files identical despite different names*

