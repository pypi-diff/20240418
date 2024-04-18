# Comparing `tmp/open2fa-1.3.6-py3-none-any.whl.zip` & `tmp/open2fa-1.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20612 bytes, number of entries: 17
+Zip file size: 20608 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
 -rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
 -rw-r--r--  2.0 unx     4747 b- defN 24-Mar-19 13:19 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
--rw-r--r--  2.0 unx      659 b- defN 24-Feb-11 08:07 open2fa/config.py
+-rw-r--r--  2.0 unx      660 b- defN 24-Apr-11 22:49 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
--rw-r--r--  2.0 unx    17929 b- defN 24-Mar-25 23:38 open2fa/main.py
+-rw-r--r--  2.0 unx    17949 b- defN 24-Apr-14 18:43 open2fa/main.py
 -rw-r--r--  2.0 unx     1742 b- defN 24-Mar-23 03:26 open2fa/msgs.py
--rw-r--r--  2.0 unx     2289 b- defN 24-Mar-16 18:22 open2fa/totp.py
+-rw-r--r--  2.0 unx     2248 b- defN 24-Apr-16 18:10 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-02 21:53 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    11046 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/RECORD
-17 files, 58516 bytes uncompressed, 18542 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-18 05:06 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11094 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-18 05:06 open2fa-1.3.7.dist-info/RECORD
+17 files, 58544 bytes uncompressed, 18538 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/LICENSE
+Filename: open2fa-1.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/METADATA
+Filename: open2fa-1.3.7.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/WHEEL
+Filename: open2fa-1.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/entry_points.txt
+Filename: open2fa-1.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/top_level.txt
+Filename: open2fa-1.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.3.6.dist-info/RECORD
+Filename: open2fa-1.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/config.py

```diff
@@ -1,13 +1,14 @@
 import os
 from pathlib import Path
 
 OPEN2FA_DIR = str(os.environ.get('OPEN2FA_DIR', Path.home() / '.open2fa'))
 OPEN2FA_UUID_PATH = os.path.join(OPEN2FA_DIR, 'open2fa.uuid')
 
+
 OPEN2FA_UUID = os.environ.get('OPEN2FA_UUID', None)
 if OPEN2FA_UUID is None and os.path.exists(
     os.path.join(OPEN2FA_DIR, 'open2fa.uuid')
 ):
     # read from file if filepath set
     with open(os.path.join(OPEN2FA_DIR, 'open2fa.uuid'), 'r') as f:
         OPEN2FA_UUID = f.read().strip()
```

## open2fa/main.py

```diff
@@ -408,19 +408,20 @@
     def api_url(self) -> TYPE.Union[str, None]:
         """shorthand for self.o2fa_api_url"""
         return self.o2fa_api_url
 
     def refresh(self) -> 'Open2FA':
         """Return most-recent new Open2FA object of the current instance."""
         # create new o2fa object with the same attributes
-        return Open2FA(
+        self = Open2FA(
             o2fa_dir=self.o2fa_dir,
             o2fa_uuid=self.uuid,
             o2fa_api_url=self.api_url,
         )
+        return self
 
     @logf()
     def remote_delete(
         self,
         secret: TYPE.Optional[str] = None,
         name: TYPE.Optional[str] = None,
     ) -> int:
```

## open2fa/totp.py

```diff
@@ -23,21 +23,18 @@
     def __repr__(self) -> str:
         return default_repr(self)
 
 
 def generate_totp_2fa_code(
     secret: str, interval_length: int = 30
 ) -> TOTP2FACode:
-    """
-    Generate a TOTP token using the provided secret key.
-    Args:
-        secret (str): The base32 encoded secret key.
-        interval_length (int): The time step in seconds. Default is 30 seconds.
-    Returns:
-        A TOTP2FACode object with the generated code as well as other info
+    """Generate a TOTP token using the provided secret key.
+    ~secret (str): The base32 encoded secret key.
+    ~interval_length (int): The time step in seconds. Default is 30 seconds.
+    -> TOTP2FACode: the generated code object as well as other info
     """
 
     # Decode the base32 encoded secret key. Casefold=True allows for
     # lowercase alphabet in the key.
     key = b64.b32decode(secret, casefold=True)
 
     # Calculate the number of intervals that have passed since Unix epoch.
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.3.6"
+__version__ = "1.3.7"
```

## Comparing `open2fa-1.3.6.dist-info/LICENSE` & `open2fa-1.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.3.6.dist-info/METADATA` & `open2fa-1.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.3.6
+Version: 1.3.7
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
@@ -19,25 +19,26 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: logfunc <=2.4.3
 Requires-Dist: cryptography <=41.0.7
-Requires-Dist: pyshared <1.6
+Requires-Dist: pyshared >=1.5
 Requires-Dist: base58 ==2.1.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-mock ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
+Requires-Dist: pyshared >=1.5 ; extra == 'dev'
 
 # open2fa
 
 [open2fa.liberfy.ai](https://open2fa.liberfy.ai) NOW LIVE
 
 Open2FA is a 100% LIBRE tool for generating Two-Factor Authentication (2FA) (TOTP) codes, with optional, secure, remote sync/restore/etc capabilities, as well as optional webui 2FA code generation.
 
@@ -266,15 +267,15 @@
 
 - The Open2FA UUID is `0e4742ef-780b-406d-8651-7766cf67be3f`
 - The Open2FA ID is `XF1628BGJeibVv8C9UacG4`
 - The Open2FA Secret is `QGcst74V9JXnyBnQmWSoCx`
 
 ## Remote Commands
 
-Push TOTP Secrets to the remote server\*\*:
+### Push TOTP Secrets to the remote server:
 
 ```bash
 open2fa remote push
 ```
 
 ### Pull TOTP Secrets from the remote server:
```

## Comparing `open2fa-1.3.6.dist-info/RECORD` & `open2fa-1.3.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 open2fa/__init__.py,sha256=-I3NORVmVqf-xgcfaF3KRHZEidP6u0HyV3sMkhAO5RA,113
 open2fa/cli.py,sha256=srswxrGSgQIa0rVYd1xfT7cl9sVJahkrv3t_okYp_a4,10069
 open2fa/cli_utils.py,sha256=OU_M-MNDYNx6dIVw1vSmXBk2mYxYmC098DQ9YxcivR4,4747
 open2fa/common.py,sha256=44pDlWVJhfGbCW_TczO7Urc_0JFpynfEkP6FJYd6r-Y,4334
-open2fa/config.py,sha256=EYO7Xn0rU8gBeH57zXb8W2uPspEVb5Xv18TrUnaGBhI,659
+open2fa/config.py,sha256=VixFalMSdS2vOtVhs6D2Jh1-wIeo98fMvD1BZIJbJog,660
 open2fa/ex.py,sha256=nc_q0UdNdbk-KFR0XmcQbpdhtqbs1SnWcus4XzqAq70,923
-open2fa/main.py,sha256=1lZm1g3ZTNpt4YCOPsFvNINlY0dXf9IWuvnOqkRBA14,17929
+open2fa/main.py,sha256=FA878v5GxJj3Co8Vvoms1zNWXIRgtM1HveoZY28SJwU,17949
 open2fa/msgs.py,sha256=iMBtZbL-a1zro4FgeYneo1Q6MsfNrGafCL-isbv38Qw,1742
-open2fa/totp.py,sha256=2t0qw9zGC3kdIhVFBvObNEWpw1-o8A6NYn1rFLe0RNo,2289
+open2fa/totp.py,sha256=WKZXQlGlaa7eZK5SR3yBIfUq6PhDAUJpWAiwWJewmMY,2248
 open2fa/utils.py,sha256=j6Nom2zc51aDsY79d1sW6qmSyXrGirIa0cP7AE_wNDg,2139
-open2fa/version.py,sha256=5ZbAQtod5QalTI1C2N07edlxplzG_Q2XvGOSyOok4uA,22
-open2fa-1.3.6.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-open2fa-1.3.6.dist-info/METADATA,sha256=T4JJRQWE_YEhXAPZMqisUK1spkyoi3RyxKSBzKYBI7c,11046
-open2fa-1.3.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-open2fa-1.3.6.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
-open2fa-1.3.6.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
-open2fa-1.3.6.dist-info/RECORD,,
+open2fa/version.py,sha256=9peaXOar2qezOPJEKG6cD_A0aaXrzdVN8h-v6fBoBEk,22
+open2fa-1.3.7.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+open2fa-1.3.7.dist-info/METADATA,sha256=6Hf8yN9s47pcT3h0759NlHvqXUVkb0wMEE4Pqx-Na5k,11094
+open2fa-1.3.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+open2fa-1.3.7.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
+open2fa-1.3.7.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
+open2fa-1.3.7.dist-info/RECORD,,
```

