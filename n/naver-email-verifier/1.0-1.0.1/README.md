# Comparing `tmp/naver_email_verifier-1.0.tar.gz` & `tmp/naver_email_verifier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver_email_verifier-1.0.tar", last modified: Thu Apr 18 05:21:39 2024, max compression
+gzip compressed data, was "naver_email_verifier-1.0.1.tar", last modified: Thu Apr 18 05:44:54 2024, max compression
```

## Comparing `naver_email_verifier-1.0.tar` & `naver_email_verifier-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:39.944692 naver_email_verifier-1.0/
--rw-rw-rw-   0        0        0     1089 2024-04-18 05:16:40.000000 naver_email_verifier-1.0/LICENSE
--rw-rw-rw-   0        0        0      204 2024-04-18 05:21:39.944692 naver_email_verifier-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1453 2024-04-18 05:20:02.000000 naver_email_verifier-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:39.912956 naver_email_verifier-1.0/naver_email_verifier/
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:39.943687 naver_email_verifier-1.0/naver_email_verifier/__pycache__/
--rw-rw-rw-   0        0        0      176 2024-04-18 04:43:03.000000 naver_email_verifier-1.0/naver_email_verifier/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2955 2024-04-18 05:11:50.000000 naver_email_verifier-1.0/naver_email_verifier/__pycache__/verifier.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 05:21:39.940030 naver_email_verifier-1.0/naver_email_verifier.egg-info/
--rw-rw-rw-   0        0        0      204 2024-04-18 05:21:39.000000 naver_email_verifier-1.0/naver_email_verifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-18 05:21:39.000000 naver_email_verifier-1.0/naver_email_verifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:21:39.000000 naver_email_verifier-1.0/naver_email_verifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 05:21:39.000000 naver_email_verifier-1.0/naver_email_verifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-18 05:21:39.000000 naver_email_verifier-1.0/naver_email_verifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:21:39.944692 naver_email_verifier-1.0/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-04-18 04:40:32.000000 naver_email_verifier-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.652297 naver_email_verifier-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-18 05:16:40.000000 naver_email_verifier-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      206 2024-04-18 05:44:54.651449 naver_email_verifier-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1427 2024-04-18 05:43:14.000000 naver_email_verifier-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.630366 naver_email_verifier-1.0.1/naver_email_verifier/
+drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.649399 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/
+-rw-rw-rw-   0        0        0      176 2024-04-18 04:43:03.000000 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3906 2024-04-18 05:40:59.000000 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/verifier.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.647400 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:44:54.652297 naver_email_verifier-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-04-18 05:43:30.000000 naver_email_verifier-1.0.1/setup.py
```

### Comparing `naver_email_verifier-1.0/LICENSE` & `naver_email_verifier-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naver_email_verifier-1.0/README.md` & `naver_email_verifier-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # NaverChecker
 
 `NaverChecker`는 네이버 이메일 사용자 ID의 사용 여부를 확인하는 파이썬 라이브러리입니다.
 
 이 라이브러리는 내부적으로 `httpx.Client`를 사용하여 네이버 API에 HTTP 요청을 보내어,
 
-해당 이메일 ID가 이미 존재하는지 안하는지 를 확인합니다.
+해당 네이버 이메일 ID가 존재하는지를 확인합니다.
 
 ## 설치 방법
 
 패키지를 설치하려면 다음 pip 명령어를 사용합니다:
 
 ```bash
 pip install naver_email_verifier
@@ -20,24 +20,23 @@
 
 **동기 및 비동기 지원**: 사용자의 요구에 맞게 동기 또는 비동기 방식을 선택할 수 있습니다.
 
 ```python
 from naver_email_verifier import NaverChecker
 
 # 동기 방식
-checker = NaverChecker()
-is_used = checker.is_id_in_use_sync("example_user_id")
+naver_checker = NaverChecker()
+is_used = naver_checker.is_id_in_use_sync("example_user_id")
 print("존재하는 계정입니다." if is_used else "존재하지 않는 계정입니다.")
 
 # 비동기 방식
 import asyncio
 
 async def check_async():
-    checker = NaverChecker()
-    is_used = await checker.is_id_in_use_async("example_user_id")
+    is_used = await naver_checker.is_id_in_use_async("seokwon84354")
     print("존재하는 계정입니다." if is_used else "존재하지 않는 계정입니다.")
 
 asyncio.run(check_async())
 ```
 
 ## 리소스 해제
```

### Comparing `naver_email_verifier-1.0/setup.py` & `naver_email_verifier-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             package = dirpath.replace(os.path.sep, ".")
             packages.append(package)
     return packages
 
 
 setup(
     name="naver_email_verifier",
-    version="1.0",
+    version="1.0.1",
     packages=find_pyc_packages(),
     package_data={"": ["*.pyc"]},
     exclude_package_data={"": ["*.py"]},
     install_requires=[
         "httpx",
     ],
     author="Seok Won Choi",
```

