# Comparing `tmp/reward_pkg_23246642-0.0.4.tar.gz` & `tmp/reward_pkg_23246642-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reward_pkg_23246642-0.0.4.tar", last modified: Wed Apr 17 20:08:15 2024, max compression
+gzip compressed data, was "reward_pkg_23246642-0.0.5.tar", last modified: Wed Apr 17 21:22:48 2024, max compression
```

## Comparing `reward_pkg_23246642-0.0.4.tar` & `reward_pkg_23246642-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 20:08:15.611231 reward_pkg_23246642-0.0.4/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 11:07:59.000000 reward_pkg_23246642-0.0.4/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      441 2024-04-17 20:08:15.607231 reward_pkg_23246642-0.0.4/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 11:08:21.000000 reward_pkg_23246642-0.0.4/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 20:08:15.603231 reward_pkg_23246642-0.0.4/calculate_rewards_pkg/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 14:46:11.000000 reward_pkg_23246642-0.0.4/calculate_rewards_pkg/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      850 2024-04-17 20:06:32.000000 reward_pkg_23246642-0.0.4/calculate_rewards_pkg/calculate_rewards.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 20:08:15.607231 reward_pkg_23246642-0.0.4/reward_pkg_23246642.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      441 2024-04-17 20:08:15.000000 reward_pkg_23246642-0.0.4/reward_pkg_23246642.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      275 2024-04-17 20:08:15.000000 reward_pkg_23246642-0.0.4/reward_pkg_23246642.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-17 20:08:15.000000 reward_pkg_23246642-0.0.4/reward_pkg_23246642.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       22 2024-04-17 20:08:15.000000 reward_pkg_23246642-0.0.4/reward_pkg_23246642.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-17 20:08:15.611231 reward_pkg_23246642-0.0.4/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      867 2024-04-17 20:07:35.000000 reward_pkg_23246642-0.0.4/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 21:22:48.102778 reward_pkg_23246642-0.0.5/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 11:07:59.000000 reward_pkg_23246642-0.0.5/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      441 2024-04-17 21:22:48.098778 reward_pkg_23246642-0.0.5/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 11:08:21.000000 reward_pkg_23246642-0.0.5/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 21:22:48.098778 reward_pkg_23246642-0.0.5/calculate_rewards_pkg/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 14:46:11.000000 reward_pkg_23246642-0.0.5/calculate_rewards_pkg/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      936 2024-04-17 21:19:50.000000 reward_pkg_23246642-0.0.5/calculate_rewards_pkg/calculate_rewards.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-17 21:22:48.098778 reward_pkg_23246642-0.0.5/reward_pkg_23246642.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      441 2024-04-17 21:22:48.000000 reward_pkg_23246642-0.0.5/reward_pkg_23246642.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      275 2024-04-17 21:22:48.000000 reward_pkg_23246642-0.0.5/reward_pkg_23246642.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-17 21:22:48.000000 reward_pkg_23246642-0.0.5/reward_pkg_23246642.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       22 2024-04-17 21:22:48.000000 reward_pkg_23246642-0.0.5/reward_pkg_23246642.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-17 21:22:48.102778 reward_pkg_23246642-0.0.5/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      867 2024-04-17 21:22:34.000000 reward_pkg_23246642-0.0.5/setup.py
```

### Comparing `reward_pkg_23246642-0.0.4/calculate_rewards_pkg/calculate_rewards.py` & `reward_pkg_23246642-0.0.5/calculate_rewards_pkg/calculate_rewards.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,12 @@
     
     def get_reward_for_items(self, items):
         return self.calculate_total_reward(items) 
 
 class Reward:
     def __init__(self, name, category):
         self.name = name
-        self.category = category
+        self.category = category
+        
+    def __iter__(self):
+        yield self.name
+        yield self.category
```

### Comparing `reward_pkg_23246642-0.0.4/setup.py` & `reward_pkg_23246642-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reward-pkg-23246642",
     # Replace with your own username above
-    version="0.0.4",
+    version="0.0.5",
     author="Serena Santosh",
     author_email="serenachrismathew@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

