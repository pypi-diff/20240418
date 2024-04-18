# Comparing `tmp/YYJ-1.0.1.tar.gz` & `tmp/YYJ-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\YYJ-1.0.1.tar", last modified: Tue Apr 16 11:45:56 2024, max compression
+gzip compressed data, was "dist\YYJ-1.0.2.tar", last modified: Thu Apr 18 12:21:42 2024, max compression
```

## Comparing `YYJ-1.0.1.tar` & `YYJ-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.274067 YYJ-1.0.1/
--rw-rw-rw-   0        0        0     1010 2024-04-16 11:45:56.274067 YYJ-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-16 10:40:13.000000 YYJ-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.266932 YYJ-1.0.1/YYJ/
--rw-rw-rw-   0        0        0     1006 2024-04-16 10:21:45.000000 YYJ-1.0.1/YYJ/__core.py
--rw-rw-rw-   0        0        0       25 2024-04-16 11:33:26.000000 YYJ-1.0.1/YYJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.272070 YYJ-1.0.1/YYJ.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 11:45:56.274067 YYJ-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-16 11:45:47.000000 YYJ-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:21:42.569285 YYJ-1.0.2/
+-rw-rw-rw-   0        0        0     1010 2024-04-18 12:21:42.568275 YYJ-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-16 10:40:13.000000 YYJ-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 12:21:42.562709 YYJ-1.0.2/YYJ/
+-rw-rw-rw-   0        0        0      639 2024-04-18 12:20:58.000000 YYJ-1.0.2/YYJ/ChatYYJ.py
+-rw-rw-rw-   0        0        0     1245 2024-04-18 12:21:02.000000 YYJ-1.0.2/YYJ/__core.py
+-rw-rw-rw-   0        0        0       25 2024-04-16 11:33:26.000000 YYJ-1.0.2/YYJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:21:42.567105 YYJ-1.0.2/YYJ.egg-info/
+-rw-rw-rw-   0        0        0     1010 2024-04-18 12:21:42.000000 YYJ-1.0.2/YYJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-18 12:21:42.000000 YYJ-1.0.2/YYJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:21:42.000000 YYJ-1.0.2/YYJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-18 12:21:42.000000 YYJ-1.0.2/YYJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:21:42.569285 YYJ-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-18 12:21:12.000000 YYJ-1.0.2/setup.py
```

### Comparing `YYJ-1.0.1/PKG-INFO` & `YYJ-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YYJ
-Version: 1.0.1
+Version: 1.0.2
 Summary: 瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制
 Home-page: https://pornhub.com
 Author: marf
 Author-email: chenmarf460@gmail.com
 License: Apache 2.0
 Description: 到这就说明宿舍仔你成功一部分了，还是那句话：欢迎狙击
 Keywords: yyj,pornhub
```

### Comparing `YYJ-1.0.1/YYJ/__core.py` & `YYJ-1.0.2/YYJ/__core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-class YYJ(object):
+class YYJinterface(object):
+    def __init__(self) -> None:
+        pass
+
+    def __call__(self):
+        pass
+
+    def __str__(self) -> str:
+        pass
+
+    def joker(self) -> None:
+        pass
+
+class YYJ(YYJinterface):
     def __init__(self) -> None:
         self.__emoji = '\U0001F613'
         self.__describe = '瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制'
 
         return
     
     def __call__(self) -> None:
@@ -28,15 +41,15 @@
 def main() -> None:
     yyj = YYJ()
     yyj.joker()
 
     try:
         print(yyj)
     except:
-        print('没你事儿了')
+        print('没你事儿了，一边凉快去。')
 
     return
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `YYJ-1.0.1/YYJ.egg-info/PKG-INFO` & `YYJ-1.0.2/YYJ.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YYJ
-Version: 1.0.1
+Version: 1.0.2
 Summary: 瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制
 Home-page: https://pornhub.com
 Author: marf
 Author-email: chenmarf460@gmail.com
 License: Apache 2.0
 Description: 到这就说明宿舍仔你成功一部分了，还是那句话：欢迎狙击
 Keywords: yyj,pornhub
```

### Comparing `YYJ-1.0.1/setup.py` & `YYJ-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="YYJ",
-    version="1.0.1",
+    version="1.0.2",
     author="marf",
     author_email="chenmarf460@gmail.com",
     description="瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pornhub.com",
     packages=setuptools.find_packages(),
```

