# Comparing `tmp/repelsec-0.5.tar.gz` & `tmp/repelsec-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repelsec-0.5.tar", last modified: Mon Apr 15 18:00:37 2024, max compression
+gzip compressed data, was "repelsec-0.6.tar", last modified: Thu Apr 18 17:41:51 2024, max compression
```

## Comparing `repelsec-0.5.tar` & `repelsec-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:37.649452 repelsec-0.5/
--rw-rw-rw-   0        0        0     1090 2024-04-05 16:11:12.000000 repelsec-0.5/LICENSE
--rw-rw-rw-   0        0        0     3884 2024-04-15 18:00:37.648444 repelsec-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3481 2024-04-15 18:00:06.000000 repelsec-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:37.613547 repelsec-0.5/repelsec/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:11:12.000000 repelsec-0.5/repelsec/__init__.py
--rw-rw-rw-   0        0        0    24455 2024-04-11 17:12:38.000000 repelsec-0.5/repelsec/cwe_vulnerabilities.py
--rw-rw-rw-   0        0        0     4300 2024-04-06 15:25:47.000000 repelsec-0.5/repelsec/functions.py
--rw-rw-rw-   0        0        0     6167 2024-04-12 15:04:11.000000 repelsec-0.5/repelsec/generate_pdf.py
--rw-rw-rw-   0        0        0    19229 2024-04-15 17:10:54.000000 repelsec-0.5/repelsec/main.py
--rw-rw-rw-   0        0        0    13581 2024-04-06 16:49:37.000000 repelsec-0.5/repelsec/unit_tests.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:37.646911 repelsec-0.5/repelsec.egg-info/
--rw-rw-rw-   0        0        0     3884 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      138 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 18:00:37.000000 repelsec-0.5/repelsec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 18:00:37.649452 repelsec-0.5/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-04-15 18:00:35.000000 repelsec-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:41:51.963818 repelsec-0.6/
+-rw-rw-rw-   0        0        0     1090 2024-04-05 16:11:12.000000 repelsec-0.6/LICENSE
+-rw-rw-rw-   0        0        0     3884 2024-04-18 17:41:51.963818 repelsec-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3481 2024-04-15 18:00:06.000000 repelsec-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 17:41:51.932555 repelsec-0.6/repelsec/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:11:12.000000 repelsec-0.6/repelsec/__init__.py
+-rw-rw-rw-   0        0        0    24158 2024-04-18 14:50:12.000000 repelsec-0.6/repelsec/cwe_vulnerabilities.py
+-rw-rw-rw-   0        0        0     4300 2024-04-06 15:25:47.000000 repelsec-0.6/repelsec/functions.py
+-rw-rw-rw-   0        0        0     6167 2024-04-12 15:04:11.000000 repelsec-0.6/repelsec/generate_pdf.py
+-rw-rw-rw-   0        0        0    19231 2024-04-18 12:15:15.000000 repelsec-0.6/repelsec/main.py
+-rw-rw-rw-   0        0        0    13590 2024-04-16 16:26:04.000000 repelsec-0.6/repelsec/unit_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:41:51.963818 repelsec-0.6/repelsec.egg-info/
+-rw-rw-rw-   0        0        0     3884 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      138 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 17:41:51.000000 repelsec-0.6/repelsec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 17:41:51.963818 repelsec-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-04-18 17:41:34.000000 repelsec-0.6/setup.py
```

### Comparing `repelsec-0.5/LICENSE` & `repelsec-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `repelsec-0.5/PKG-INFO` & `repelsec-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repelsec
-Version: 0.5
+Version: 0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nvdlib~=0.7.5
 Requires-Dist: xmltodict~=0.13.0
 Requires-Dist: pandas~=2.1.1
 Requires-Dist: argparse~=1.4.0
 Requires-Dist: setuptools~=69.0.2
```

### Comparing `repelsec-0.5/README.md` & `repelsec-0.6/README.md`

 * *Files identical despite different names*

### Comparing `repelsec-0.5/repelsec/cwe_vulnerabilities.py` & `repelsec-0.6/repelsec/cwe_vulnerabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         self.remediation_advice = ("Prepared statements, client and server side input validation, safe stored "
                                    "procedures, or escaping user input can be used to mitigate against SQL injection "
                                    "attacks.")
         self.remediation_days = 15
 
     @staticmethod
     def scan(line_str):
-        if "Statement" in line_str and "PreparedStatement" not in line_str and "prepareStatement" not in line_str:
+        pattern_found = re.findall(pattern=r"\b(Statement) (.*) =", string=line_str)
+
+        if pattern_found:
             return True
         else:
             return False
 
 
 class CWE111:
     def __init__(self):
@@ -92,15 +94,15 @@
         self.remediation_advice = ("Implement exception handling; use another data type such as Long or "
                                    "BigInteger if performing operations close to the maximum of an Integer")
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
 
-        pattern_found = re.findall(pattern=r"int (. *) = Integer.MAX_VALUE \+", string=line_str)
+        pattern_found = re.findall(pattern=r"int (.*) = Integer.MAX_VALUE \+", string=line_str)
 
         if pattern_found:
             return True
         else:
             return False
 
 
@@ -116,15 +118,15 @@
         self.remediation_advice = ("Implement exception handling; use another data type such as Long or "
                                    "BigInteger if performing operations close to the minimum of an Integer")
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
 
-        pattern_found = re.findall(pattern=r"int(. *) = Integer.MIN_VALUE \-", string=line_str)
+        pattern_found = re.findall(pattern=r"int(.*) = Integer.MIN_VALUE \-", string=line_str)
 
         if pattern_found:
             return True
         else:
             return False
 
 
@@ -137,19 +139,18 @@
         self.severity = "Low"
         self.url = "https://cwe.mitre.org/data/definitions/209.html"
         self.remediation_advice = "When an exception is caught, only print insensitive and desired data to a user."
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
-        if "catch" in line_str and "Exception e" in line_str:
-            if "System.out.println(e)" in line_str or "e.printStackTrace()" in line_str:
-                return True
-
-        return False
+        if "System.out.println(e)" in line_str or "e.printStackTrace()" in line_str:
+            return True
+        else:
+            return False
 
 
 class CWE246:
     def __init__(self):
         self.id = "CWE-246"
         self.name = "J2EE Bad Practices: Direct Use of Sockets"
         self.description = "The J2EE application directly uses sockets instead of using framework method calls."
@@ -179,18 +180,17 @@
         self.severity = "Low"
         self.url = "https://cwe.mitre.org/data/definitions/259.html"
         self.remediation_advice = "Passwords should be hashed and stored safely in a password-protected external file"
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
-        formatted_str = line_str.replace(" ", "")
         pattern_found = re.findall(
-            pattern=r"password=[\"']|pwd=[\"']|passwd=[\"']|pw=[\"']|pword=[\"']|pass=[\"']|passcode=[\"']",
-            string=formatted_str, flags=re.IGNORECASE)
+            pattern=r"(password|pwd|passwd|pw|pword|pass|passcode) = [\"']([^\"']+)[\"']",
+            string=line_str, flags=re.IGNORECASE)
 
         if pattern_found:
             return True
         else:
             return False
 
 
@@ -203,18 +203,17 @@
         self.severity = "Low"
         self.url = "https://cwe.mitre.org/data/definitions/321.html"
         self.remediation_advice = "Cryptographic keys should be stored safely in a password-protected external file"
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
-        formatted_str = line_str.replace(" ", "")
         pattern_found = re.findall(
-            pattern=r"key=[\"']|token=[\"']|encryption_key=[\"']|auth=[\"']|secret=[\"']|encryption=[\"']",
-            string=formatted_str, flags=re.IGNORECASE)
+            pattern=r"(key|token|encryption_key|auth|secret|encryption) = [\"']([^\"']+)[\"']",
+            string=line_str, flags=re.IGNORECASE)
 
         if pattern_found:
             return True
         else:
             return False
 
 
@@ -550,15 +549,15 @@
         self.url = "https://cwe.mitre.org/data/definitions/766.html"
         self.remediation_advice = "Data should be private, static, and final whenever possible. This will assure that your code is protected by instantiating early, preventing access, and preventing tampering."
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
         pattern_found = re.findall(
-            pattern=r"public(static |final | )(byte|short|long|double|String|float|int|char|boolean|BigDecimal) (username|password)",
+            pattern=r"public (.*) (username|password|email|isAuthenticated|jwtSecret)",
             string=line_str, flags=re.IGNORECASE)
 
         if pattern_found:
             return True
         else:
             return False
 
@@ -573,15 +572,16 @@
         self.severity = "Low"
         self.url = "https://cwe.mitre.org/data/definitions/798.html"
         self.remediation_advice = "Credentials should be hashed and stored safely in a password-protected external file"
         self.remediation_days = 120
 
     @staticmethod
     def scan(line_str):
-        formatted_str = line_str.replace(" ", "")
-        pattern_found = re.findall(pattern=r"username=[\"']|uname=[\"']|id=[\"']|user=[\"']", string=formatted_str,
-                                   flags=re.IGNORECASE)
+        pattern_found = re.findall(
+            pattern=r"(username|uname|user|id) = [\"']([^\"']+)[\"']",
+            string=line_str,
+            flags=re.IGNORECASE)
 
         if pattern_found:
             return True
         else:
             return False
```

### Comparing `repelsec-0.5/repelsec/functions.py` & `repelsec-0.6/repelsec/functions.py`

 * *Files identical despite different names*

### Comparing `repelsec-0.5/repelsec/generate_pdf.py` & `repelsec-0.6/repelsec/generate_pdf.py`

 * *Files identical despite different names*

### Comparing `repelsec-0.5/repelsec/main.py` & `repelsec-0.6/repelsec/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,8 +387,9 @@
             pdf.output(pdf_path, 'F')
 
             if args.password:
                 encrypted_path = os.path.join(output_path, "e_sast.pdf")
                 sec.add_pdf_password(pdf_path, encrypted_path, args.password)
 
         end_time = time()
-        print(f"SAST Scan time {round((end_time - start_time), 4)} Seconds")
+
+        print(f"SAST Scan time {round((end_time - start_time), 8)} Seconds")
```

### Comparing `repelsec-0.5/repelsec/unit_tests.py` & `repelsec-0.6/repelsec/unit_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
-from functions import *
 from repelsec import cwe_vulnerabilities
+from repelsec.functions import *
 
 
 class TestFunctions(unittest.TestCase):
     if __name__ == '__main__':
         unittest.main()
 
     def test_valid_path_function(self):
```

### Comparing `repelsec-0.5/repelsec.egg-info/PKG-INFO` & `repelsec-0.6/repelsec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repelsec
-Version: 0.5
+Version: 0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nvdlib~=0.7.5
 Requires-Dist: xmltodict~=0.13.0
 Requires-Dist: pandas~=2.1.1
 Requires-Dist: argparse~=1.4.0
 Requires-Dist: setuptools~=69.0.2
```

### Comparing `repelsec-0.5/setup.py` & `repelsec-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="repelsec",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     include_package_data=True,
     install_requires=read_requirements(),
     entry_points='''
     [console_scripts]
     repelsec=repelsec.main:main
     ''',
```

