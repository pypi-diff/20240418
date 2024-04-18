# Comparing `tmp/qualesim-quiets-1.0.2.tar.gz` & `tmp/qualesim-quiets-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.2.tar", last modified: Wed Apr 17 07:31:55 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.0.3.tar", last modified: Wed Apr 17 09:29:36 2024, max compression
```

## Comparing `qualesim-quiets-1.0.2.tar` & `qualesim-quiets-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.2/LICENSE
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      789 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.2/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.207607 qualesim-quiets-1.0.2/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.211607 qualesim-quiets-1.0.2/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.2/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.211607 qualesim-quiets-1.0.2/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.2/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.2/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    43747 2024-04-17 02:46:48.000000 qualesim-quiets-1.0.2/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.2/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      789 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      405 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-17 07:31:55.000000 qualesim-quiets-1.0.2/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.2/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:31:55.215607 qualesim-quiets-1.0.2/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.2/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.880848 qualesim-quiets-1.0.3/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.3/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 09:29:36.880848 qualesim-quiets-1.0.3/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.3/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.872848 qualesim-quiets-1.0.3/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.876848 qualesim-quiets-1.0.3/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.3/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.876848 qualesim-quiets-1.0.3/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.3/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.3/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    44663 2024-04-17 09:19:15.000000 qualesim-quiets-1.0.3/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.3/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.876848 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-17 09:29:36.000000 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-17 09:29:36.000000 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 09:29:36.000000 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-17 09:29:36.000000 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-17 09:29:36.000000 qualesim-quiets-1.0.3/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 09:29:36.880848 qualesim-quiets-1.0.3/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-17 09:19:55.000000 qualesim-quiets-1.0.3/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 09:29:36.880848 qualesim-quiets-1.0.3/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.3/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 08:24:10.000000 qualesim-quiets-1.0.3/tests/test_example_quiets_whitepaper.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.3/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.3/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.2/LICENSE` & `qualesim-quiets-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.2/PKG-INFO` & `qualesim-quiets-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.2
+Version: 1.0.3
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: ply
+Requires-Dist: pyquiet
 
 # DQCSim-Quiets
 
 #### 介绍
 1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
```

### Comparing `qualesim-quiets-1.0.2/qualesim_quiets/frontend.py` & `qualesim-quiets-1.0.3/qualesim_quiets/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,26 @@
                 out_double[i] = output_double[i][0]
             ret = dict(**out_int, **out_double)
 
             res_state_vector = dict()
             res_cls = dict()
             res_sv = dict()
             # quantum output.
+            for ml in func_data.func_qubit.keys():
+                if len(func_data.func_qubit[ml]) == 1:
+                    try:
+                        func_data.qubit_measure[func_data.func_qubit[ml][0]] = (self.get_measurement(func_data.func_qubit[ml][0]).value,self.get_measurement(func_data.func_qubit[ml][0])["probability"],self.get_measurement(func_data.func_qubit[ml][0])["state_vector"])
+                    except:
+                        pass
+                else:
+                    for mi in range(len(func_data.func_qubit[ml])):
+                        try:
+                            func_data.qubit_measure[func_data.func_qubit[ml][mi]] = (self.get_measurement(func_data.func_qubit[ml][mi]).value,self.get_measurement(func_data.func_qubit[ml][mi])["probability"],self.get_measurement(func_data.func_qubit[ml][mi])["state_vector"])
+                        except:
+                            pass
             for jj in func_data.qubit_measure.keys():
                 func_data.res_dict.append(func_data.qubit_measure[jj][0])
                 for ii in func_data.func_qubit.keys():
                     if (
                         len(func_data.func_qubit[ii]) == 1
                         and func_data.func_qubit[ii][0] == jj
                     ):
```

### Comparing `qualesim-quiets-1.0.2/qualesim_quiets/utils.py` & `qualesim-quiets-1.0.3/qualesim_quiets/utils.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.2/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.0.3/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.2
+Version: 1.0.3
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: ply
+Requires-Dist: pyquiet
 
 # DQCSim-Quiets
 
 #### 介绍
 1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
```

### Comparing `qualesim-quiets-1.0.2/setup.py` & `qualesim-quiets-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.2",
+    version="1.0.3",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.2/tests/test_cls.py` & `qualesim-quiets-1.0.3/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.2/tests/test_gate.py` & `qualesim-quiets-1.0.3/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.2/tests/test_qifile.py` & `qualesim-quiets-1.0.3/tests/test_qifile.py`

 * *Files identical despite different names*

