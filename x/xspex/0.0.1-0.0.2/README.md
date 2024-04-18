# Comparing `tmp/xspex-0.0.1.tar.gz` & `tmp/xspex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspex-0.0.1.tar", last modified: Tue Apr 16 20:07:12 2024, max compression
+gzip compressed data, was "xspex-0.0.2.tar", last modified: Thu Apr 18 18:22:19 2024, max compression
```

## Comparing `xspex-0.0.1.tar` & `xspex-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.513534 xspex-0.0.1/
--rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.1/LICENSE
--rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.1/MANIFEST.in
--rw-r--r--   0 xuewc      (501) staff       (20)      865 2024-04-16 20:07:12.513461 xspex-0.0.1/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      192 2024-04-16 17:14:47.000000 xspex-0.0.1/README.md
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.509898 xspex-0.0.1/helpers/
--rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.1/helpers/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.1/helpers/identify_xspec.py
--rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.1/helpers/report_xspec_version.cxx
--rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.1/helpers/template.py
--rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.1/pyproject.toml
--rw-r--r--   0 xuewc      (501) staff       (20)      787 2024-04-16 20:07:12.513827 xspex-0.0.1/setup.cfg
--rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-04-16 18:26:25.000000 xspex-0.0.1/setup.py
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.510206 xspex-0.0.1/src/
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.510404 xspex-0.0.1/src/include/
--rw-r--r--   0 xuewc      (501) staff       (20)    20735 2024-04-15 18:47:50.000000 xspex-0.0.1/src/include/xspex.hpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.511306 xspex-0.0.1/src/xspex/
--rw-r--r--   0 xuewc      (501) staff       (20)   338082 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     8031 2024-04-16 19:19:56.000000 xspex-0.0.1/src/xspex/primitive.py
--rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.513241 xspex-0.0.1/src/xspex.egg-info/
--rw-r--r--   0 xuewc      (501) staff       (20)      865 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.egg-info/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      503 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.egg-info/SOURCES.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.egg-info/dependency_links.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-16 19:53:25.000000 xspex-0.0.1/src/xspex.egg-info/not-zip-safe
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.egg-info/requires.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-16 20:07:12.000000 xspex-0.0.1/src/xspex.egg-info/top_level.txt
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.512763 xspex-0.0.1/template/
--rw-r--r--   0 xuewc      (501) staff       (20)     4704 2024-04-16 19:22:20.000000 xspex-0.0.1/template/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.1/template/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-16 20:07:12.512920 xspex-0.0.1/tests/
--rw-r--r--   0 xuewc      (501) staff       (20)     1248 2024-04-16 19:24:39.000000 xspex-0.0.1/tests/test_primitive.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794935 xspex-0.0.2/
+-rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.2/LICENSE
+-rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.2/MANIFEST.in
+-rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-18 18:22:19.794843 xspex-0.0.2/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)      887 2024-04-18 18:21:14.000000 xspex-0.0.2/README.md
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.791562 xspex-0.0.2/helpers/
+-rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/identify_xspec.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/report_xspec_version.cxx
+-rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.2/helpers/template.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.2/pyproject.toml
+-rw-r--r--   0 xuewc      (501) staff       (20)      787 2024-04-18 18:22:19.795273 xspex-0.0.2/setup.cfg
+-rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-04-18 18:14:35.000000 xspex-0.0.2/setup.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.791753 xspex-0.0.2/src/
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.792003 xspex-0.0.2/src/include/
+-rw-r--r--   0 xuewc      (501) staff       (20)    23356 2024-04-18 18:17:18.000000 xspex-0.0.2/src/include/xspex.hpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.792617 xspex-0.0.2/src/xspex/
+-rw-r--r--   0 xuewc      (501) staff       (20)   338104 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     9303 2024-04-18 18:10:33.000000 xspex-0.0.2/src/xspex/primitive.py
+-rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794549 xspex-0.0.2/src/xspex.egg-info/
+-rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)      523 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/SOURCES.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/dependency_links.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-17 17:48:09.000000 xspex-0.0.2/src/xspex.egg-info/not-zip-safe
+-rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/requires.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-18 18:22:19.000000 xspex-0.0.2/src/xspex.egg-info/top_level.txt
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.793949 xspex-0.0.2/template/
+-rw-r--r--   0 xuewc      (501) staff       (20)     4726 2024-04-17 10:50:41.000000 xspex-0.0.2/template/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.2/template/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-18 18:22:19.794313 xspex-0.0.2/tests/
+-rw-r--r--   0 xuewc      (501) staff       (20)     6286 2024-04-18 18:10:32.000000 xspex-0.0.2/tests/test_basic.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7261 2024-04-18 18:10:32.000000 xspex-0.0.2/tests/test_primitive.py
```

### Comparing `xspex-0.0.1/LICENSE` & `xspex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xspex-0.0.1/helpers/identify_xspec.py` & `xspex-0.0.2/helpers/identify_xspec.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.1/helpers/template.py` & `xspex-0.0.2/helpers/template.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.1/setup.cfg` & `xspex-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `xspex-0.0.1/setup.py` & `xspex-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
 sys.path.append(os.path.dirname(__file__))
 from helpers import template
 from helpers.identify_xspec import get_xspec_macros
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 # Check HEASARC is set up. The following does not provide a useful
 # message from 'pip install' so how do we make it more meaningful?
 #
 HEADAS = os.getenv('HEADAS')
 if HEADAS is None:
     sys.stderr.write('ERROR: unable to find HEADAS environment variable.\n')
```

### Comparing `xspex-0.0.1/src/include/xspex.hpp` & `xspex-0.0.2/src/include/xspex.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -390,213 +390,291 @@
 	        eptr, nelem, pptr, pbuf.size,
 	        filename.c_str(), spectrumNumber,
 		    tableType.c_str(), optr, errors.data()
 		);
 	    return result;
 	  }
 
+
     template <xsccCall model, int NumPars>
     void wrapper_C_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         const string initStr = "";  //*reinterpret_cast<string *>(in[5]);
         float *optr = reinterpret_cast<float *>(out);
 
         auto pars_ = std::vector<double>(NumPars);
         auto energyArray_ = std::vector<double>(nelem + 1);
         auto result_ = std::vector<double>(nelem);
         auto errors_ = std::vector<double>(nelem);
 
         double *pptr_ = pars_.data();
         double *eptr_ = energyArray_.data();
         double *optr_ = result_.data();
-
-        float_to_double(pptr, pptr_, NumPars);
         float_to_double(eptr, eptr_, nelem + 1);
-        model(eptr_, nelem, pptr_, spectrumNumber, optr_, errors_.data(), initStr.c_str());
-        double_to_float(optr_, optr, nelem);
+
+        for (int i = 0; i < batch; ++i) {
+            float *pptr_i = pptr + i * NumPars;
+            float *optr_i = optr + i * nelem;
+            float_to_double(pptr_i, pptr_, NumPars);
+            model(
+                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                errors_.data(), initStr.c_str()
+            );
+            double_to_float(optr_, optr_i, nelem);
+        }
     }
+
     template <xsccCall model, int NumPars>
     void wrapper_C_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         const string initStr = "";  //*reinterpret_cast<string *>(in[5]);
         double *optr = reinterpret_cast<double *>(out);
 
         auto errors = std::vector<double>(nelem);
 
-        model(eptr, nelem, pptr, spectrumNumber, optr, errors.data(), initStr.c_str());
+        for (int i = 0; i < batch; ++i) {
+            double *pptr_i = pptr + i * NumPars;
+            double *optr_i = optr + i * nelem;
+            model(
+                eptr, nelem, pptr_i, spectrumNumber, optr_i,
+                errors.data(), initStr.c_str()
+            );
+        }
     }
 
 
     template <xsf77Call model, int NumPars>
     void wrapper_f_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         float *optr = reinterpret_cast<float *>(out);
 
         auto errors = std::vector<float>(nelem);
 
-        model(eptr, nelem, pptr, spectrumNumber, optr, errors.data());
+        for (int i = 0; i < batch; ++i) {
+            float *pptr_i = pptr + i * NumPars;
+            float *optr_i = optr + i * nelem;
+            model(
+                eptr, nelem, pptr_i, spectrumNumber, optr_i, errors.data()
+            );
+        }
     }
+
     template <xsf77Call model, int NumPars>
     void wrapper_f_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         double *optr = reinterpret_cast<double *>(out);
 
         auto pars_ = std::vector<float>(NumPars);
         auto energyArray_ = std::vector<float>(nelem + 1);
         auto result_ = std::vector<float>(nelem);
         auto errors_ = std::vector<float>(nelem);
 
         float *pptr_ = pars_.data();
         float *eptr_ = energyArray_.data();
         float *optr_ = result_.data();
+        double_to_float(eptr, eptr_, nelem + 1);
 
+        for (int i = 0; i < batch; ++i) {
+            double *pptr_i = pptr + i * NumPars;
+            double *optr_i = optr + i * nelem;
+            double_to_float(pptr_i, pptr_, NumPars);
+            model(
+                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                errors_.data()
+            );
+            float_to_double(optr_, optr_i, nelem);
+        }
         double_to_float(pptr, pptr_, NumPars);
-        double_to_float(eptr, eptr_, nelem + 1);
-        model(eptr_, nelem, pptr_, spectrumNumber, optr_, errors_.data());
-        float_to_double(optr_, optr, nelem);
     }
 
 
     template <xsF77Call model, int NumPars>
     void wrapper_F_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         float *optr = reinterpret_cast<float *>(out);
 
         auto pars_ = std::vector<double>(NumPars);
         auto energyArray_ = std::vector<double>(nelem + 1);
         auto result_ = std::vector<double>(nelem);
         auto errors_ = std::vector<double>(nelem);
 
         double *pptr_ = pars_.data();
         double *eptr_ = energyArray_.data();
         double *optr_ = result_.data();
-
-        float_to_double(pptr, pptr_, NumPars);
         float_to_double(eptr, eptr_, nelem + 1);
-        model(eptr_, nelem, pptr_, spectrumNumber, optr_, errors_.data());
-        double_to_float(optr_, optr, nelem);
+
+        for (int i = 0; i < batch; ++i) {
+            float *pptr_i = pptr + i * NumPars;
+            float *optr_i = optr + i * nelem;
+            float_to_double(pptr_i, pptr_, NumPars);
+            model(
+                eptr_, nelem, pptr_, spectrumNumber, optr_, errors_.data()
+            );
+            double_to_float(optr_, optr_i, nelem);
+        }
     }
+
     template <xsF77Call model, int NumPars>
     void wrapper_F_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[2]);
         const int nelem = *reinterpret_cast<int *>(in[3]);
+        const int batch = *reinterpret_cast<int *>(in[4]);
         double *optr = reinterpret_cast<double *>(out);
 
         auto errors = std::vector<double>(nelem);
 
-        model(eptr, nelem, pptr, spectrumNumber, optr, errors.data());
+        for (int i = 0; i < batch; ++i) {
+            double *pptr_i = pptr + i * NumPars;
+            double *optr_i = optr + i * nelem;
+            model(
+                eptr, nelem, pptr_i, spectrumNumber, optr_i,
+                errors.data()
+            );
+        }
     }
 
 
     template <xsccCall model, int NumPars>
     void wrapper_con_C_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         float *mptr = reinterpret_cast<float *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const string initStr = "";  //*reinterpret_cast<string *>(in[5]);
+        const int batch = *reinterpret_cast<int *>(in[5]);
+        const string initStr = "";  //*reinterpret_cast<string *>(in[6]);
         float *optr = reinterpret_cast<float *>(out);
 
         auto pars_ = std::vector<double>(NumPars);
         auto energyArray_ = std::vector<double>(nelem + 1);
         auto model_ = std::vector<double>(nelem);
         auto errors_ = std::vector<double>(nelem);
+        auto out_ = std::vector<double>(nelem);
 
         double *pptr_ = pars_.data();
         double *eptr_ = energyArray_.data();
         double *mptr_ = model_.data();
-
-        float_to_double(pptr, pptr_, NumPars);
+        double *optr_ = out_.data();
         float_to_double(eptr, eptr_, nelem + 1);
         float_to_double(mptr, mptr_, nelem + 1);
-        model(eptr_, nelem, pptr_, spectrumNumber, mptr_, errors_.data(), initStr.c_str());
-        double_to_float(mptr_, optr, nelem);
+
+        for (int i = 0; i < batch; ++i) {
+            float *pptr_i = pptr + i * NumPars;
+            float *optr_i = optr + i * nelem;
+            std::copy(mptr_, mptr_ + nelem, optr_);
+            float_to_double(pptr_i, pptr_, NumPars);
+            model(
+                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                errors_.data(), initStr.c_str()
+            );
+            double_to_float(optr_, optr_i, nelem);
+        }
     }
+
     template <xsccCall model, int NumPars>
     void wrapper_con_C_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         double *mptr = reinterpret_cast<double *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
-        const string initStr = "";  //*reinterpret_cast<string *>(in[5]);
+        const int batch = *reinterpret_cast<int *>(in[5]);
+        const string initStr = "";  //*reinterpret_cast<string *>(in[6]);
         double *optr = reinterpret_cast<double *>(out);
 
-        auto model_ = std::vector<double>(nelem);
         auto errors_ = std::vector<double>(nelem);
 
-        double *mptr_ = model_.data();
-        std::copy(mptr, mptr + nelem, mptr_);
-
-        model(eptr, nelem, pptr, spectrumNumber, mptr_, errors_.data(), initStr.c_str());
-
-        std::copy(mptr_, mptr_ + nelem, optr);
+        for (int i = 0; i < batch; ++i) {
+            double *pptr_i = pptr + i * NumPars;
+            double *optr_i = optr + i * nelem;
+            std::copy(mptr, mptr + nelem, optr_i);
+            model(
+                eptr, nelem, pptr_i, spectrumNumber, optr_i,
+                errors_.data(), initStr.c_str()
+            );
+        }
     }
 
 
     template <xsf77Call model, int NumPars>
     void wrapper_con_f_XLA_f32(void *out, void **in) {
         float *pptr = reinterpret_cast<float *>(in[0]);
         float *eptr = reinterpret_cast<float *>(in[1]);
         float *mptr = reinterpret_cast<float *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
+        const int batch = *reinterpret_cast<int *>(in[5]);
         float *optr = reinterpret_cast<float *>(out);
 
-        auto model_ = std::vector<float>(nelem);
         auto errors_ = std::vector<float>(nelem);
 
-        float *mptr_ = model_.data();
-        std::copy(mptr, mptr + nelem, mptr_);
-
-        model(eptr, nelem, pptr, spectrumNumber, mptr_, errors_.data());
-
-        std::copy(mptr_, mptr_ + nelem, optr);
+        for (int i = 0; i < batch; ++i) {
+            float *pptr_i = pptr + i * NumPars;
+            float *optr_i = optr + i * nelem;
+            std::copy(mptr, mptr + nelem, optr_i);
+            model(eptr, nelem, pptr_i, spectrumNumber, optr_i, errors_.data());
+        }
     }
+
     template <xsf77Call model, int NumPars>
     void wrapper_con_f_XLA_f64(void *out, void **in) {
         double *pptr = reinterpret_cast<double *>(in[0]);
         double *eptr = reinterpret_cast<double *>(in[1]);
         double *mptr = reinterpret_cast<double *>(in[2]);
         const int spectrumNumber = *reinterpret_cast<int *>(in[3]);
         const int nelem = *reinterpret_cast<int *>(in[4]);
+        const int batch = *reinterpret_cast<int *>(in[5]);
         double *optr = reinterpret_cast<double *>(out);
 
         auto pars_ = std::vector<float>(NumPars);
         auto energyArray_ = std::vector<float>(nelem + 1);
         auto model_ = std::vector<float>(nelem);
         auto errors_ = std::vector<float>(nelem);
+        auto out_ = std::vector<float>(nelem);
 
         float *pptr_ = pars_.data();
         float *eptr_ = energyArray_.data();
         float *mptr_ = model_.data();
-
-        double_to_float(pptr, pptr_, NumPars);
+        float *optr_ = out_.data();
         double_to_float(eptr, eptr_, nelem + 1);
         double_to_float(mptr, mptr_, nelem + 1);
-        model(eptr_, nelem, pptr_, spectrumNumber, mptr_, errors_.data());
-        float_to_double(mptr_, optr, nelem);
+
+        for (int i = 0; i < batch; ++i) {
+            double *pptr_i = pptr + i * NumPars;
+            double *optr_i = optr + i * nelem;
+            std::copy(mptr_, mptr_ + nelem, optr_);
+            double_to_float(pptr_i, pptr_, NumPars);
+            model(
+                eptr_, nelem, pptr_, spectrumNumber, optr_,
+                errors_.data()
+            );
+            float_to_double(optr_, optr_i, nelem);
+        }
     }
 
 
     template <typename T>
     py::capsule EncapsulateFunction(T *fn) {
         return py::capsule((void *)fn, "xla._CUSTOM_CALL_TARGET");
     }
```

### Comparing `xspex-0.0.1/src/xspex/__init__.py` & `xspex-0.0.2/src/xspex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,18 +354,18 @@
     'apec'
     >>> m.modeltype
     <ModelType.Add: 1>
     >>> [(p.name, p.default, p.units) for p in m.parameters]
     [('kT', 1.0, 'keV'), ('Abundanc', 1.0, None), ('Redshift', 0.0, None)]
 
     """
-
     # We want case-insensitive comparison but for the keys to retain
     # their case. Using casefold() rather than lower() is a bit OTT
     # here as I would bet model.dat is meant to be US-ASCII.
+    model = str(model)
     check = model.casefold()
     out = next((v for k, v in _info.items() if k.casefold() == check), None)
     if out is None:
         raise ValueError(f"Unrecognized Xspec model '{model}'")
 
     return out
```

### Comparing `xspex-0.0.1/src/xspex/primitive.py` & `xspex-0.0.2/src/xspex/primitive.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Xspec model primitives for JAX."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from functools import partial
+from math import prod
 
 import jax
 import jax.numpy as jnp
 from jax.core import Primitive, ShapedArray
 from jax.interpreters import ad, batching, mlir, xla
 from jax.lib import xla_client
 from jaxlib.hlo_helpers import custom_call
@@ -16,43 +17,40 @@
 
 
 def avals_to_layouts(avals):
     return [list(reversed(range(aval.ndim))) for aval in avals]
 
 
 class XspecPrimitiveBase(Primitive, ABC):
-    _has_jvp: bool
-
     def __init__(self, name: str):
         name = str(name)
         if name not in xspex.list_models():
             raise ValueError(f"Xspec v{xspex.version()} has no '{name}' model")
 
         super().__init__(f'XS{name}')
         self._model_name = name
-        self._model_type = xspex.info(name).modeltype.name.lower()
+        self._nparam = len(xspex.info(name).parameters)
 
         self.def_impl(partial(xla.apply_primitive, self))
         # self.def_impl(getattr(xspex, name))
 
-        self.def_abstract_eval(self.abstract_eval)
+        self.def_abstract_eval(self.get_abstract_eval())
 
         mlir.register_lowering(self, self.lowering, platform='cpu')
 
         batching.primitive_batchers[self] = self.batching
 
-        ad.primitive_jvps[self] = partial(self.jvp)
+        ad.primitive_jvps[self] = self.jvp
 
     @abstractmethod
     def __call__(self, *args, **kwargs):
         pass
 
-    @staticmethod
     @abstractmethod
-    def abstract_eval(*args, **kwargs):
+    def get_abstract_eval(self):
         pass
 
     @abstractmethod
     def lowering(self, *args, **kwargs):
         pass
 
     @abstractmethod
@@ -60,139 +58,163 @@
         pass
 
     def jvp(self, primals, tangents):
         raise NotImplementedError(f'JVP is not implemented for {self}')
 
 
 class XspecPrimitive(XspecPrimitiveBase):
-    _has_jvp: bool = True
-
     def __call__(self, params, egrid, spec_num):
         return self.bind(params, egrid, spec_num)
 
-    @staticmethod
-    def abstract_eval(params, egrid, spec_num):
-        return ShapedArray([egrid.shape[-1] - 1], egrid.dtype)
+    def get_abstract_eval(self):
+        name = self.name
+        npar = self._nparam
+
+        def abstract_eval(params, egrid, spec_num):
+            params_shape = jnp.shape(params)
+            if params_shape[-1] != npar:
+                raise ValueError(f'{name} params shape must be (..., {npar})')
+            egrid_shape = jnp.shape(egrid)
+            if len(egrid_shape) > 1:
+                raise ValueError('egrid must be 1D array')
+            spec_num_shape = jnp.shape(spec_num)
+            if len(spec_num_shape):
+                raise ValueError('spec_num must be a integer')
+
+            shape = params_shape[:-1] + (egrid_shape[-1] - 1,)
+            dtype = jax.dtypes.canonicalize_dtype(egrid.dtype)
+            return ShapedArray(shape=shape, dtype=dtype)
+
+        return abstract_eval
 
     def lowering(self, ctx, params, egrid, spec_num):
         egrid_type = mlir.ir.RankedTensorType(egrid.type)
         etype = egrid_type.element_type
         if isinstance(etype, mlir.ir.F32Type):
             call_target_name = f'{self._model_name}_f32'
         elif isinstance(etype, mlir.ir.F64Type):
             call_target_name = f'{self._model_name}_f64'
         else:
             raise NotImplementedError(f'unsupported dtype {etype}')
         out_shape = ctx.avals_out[0].shape
         out_type = mlir.ir.RankedTensorType.get(out_shape, etype)
         out_n = mlir.ir_constant(out_shape[-1])
+        batch_n = mlir.ir_constant(prod(out_shape[:-1]))
         return custom_call(
             call_target_name,
             result_types=[out_type],
-            operands=[params, egrid, spec_num, out_n],
-            operand_layouts=avals_to_layouts(ctx.avals_in) + [()],
+            operands=[params, egrid, spec_num, out_n, batch_n],
+            operand_layouts=avals_to_layouts(ctx.avals_in) + [(), ()],
             result_layouts=avals_to_layouts(ctx.avals_out)
         ).results
 
     def batching(self, vector_arg_values, batch_axes):
         if batch_axes[1] is not None:
             raise NotImplementedError('egrid batching is not implemented')
         if batch_axes[2] is not None:
             raise NotImplementedError('spec_num batching is not implemented')
 
         params, egrid, spec_num = vector_arg_values
-        if params.ndim == 1:
-            return self(params, egrid, spec_num), batch_axes[0]
-        else:
-            res = [
-                self.batching((p, egrid, spec_num), batch_axes)[0]
-                for p in params
-            ]
-            return jnp.array(res), batch_axes[0]
+        params = jnp.moveaxis(params, batch_axes[0], 0)
+        return self(params, egrid, spec_num), 0
 
     def jvp(self, primals, tangents):
         params, egrid, spec_num = primals
         d_params = tangents[0]
 
-        out = self(params, egrid, spec_num)
+        primals_out = self(params, egrid, spec_num)
         f_vmap = jax.vmap(jax.jit(self), in_axes=(0, None, None), out_axes=0)
         eps = jnp.finfo(params.dtype).eps
-        identy = jnp.eye(len(params))
+        identity = jnp.eye(len(params))
         params_abs = jnp.where(
             jnp.equal(params, 0.0),
             jnp.ones_like(params),
             jnp.abs(params)
         )
+        params_abs = jnp.expand_dims(params_abs, axis=-1)
 
         # See Numerical Recipes Chapter 5.7
         USE_CENTRAL_DIFF = True
         if USE_CENTRAL_DIFF:
             delta = params_abs * eps ** (1.0 / 3.0)
-            params_pos_perturb = params + identy * delta
+            params_pos_perturb = params + identity * delta
             out_pos_perturb = f_vmap(params_pos_perturb, egrid, spec_num)
-            params_neg_perturb = params - identy * delta
+            params_neg_perturb = params - identity * delta
             out_neg_perturb = f_vmap(params_neg_perturb, egrid, spec_num)
             d_out = (out_pos_perturb - out_neg_perturb) / (2.0 * delta)
         else:
             delta = params_abs * jnp.sqrt(eps)
-            params_perturb = params + identy * delta
+            params_perturb = params + identity * delta
             out_perturb = f_vmap(params_perturb, egrid, spec_num)
-            d_out = (out_perturb - out) / delta
+            d_out = (out_perturb - primals_out) / delta
 
         tangents_out = d_params @ d_out
-        return out, tangents_out
+        return primals_out, tangents_out
 
 
 class XspecConvPrimitive(XspecPrimitiveBase):
-    _has_jvp: bool = False
-
     def __call__(self, params, egrid, flux, spec_num):
         return self.bind(params, egrid, flux, spec_num)
 
-    @staticmethod
-    def abstract_eval(params, egrid, flux, spec_num):
-        return ShapedArray([egrid.shape[-1] - 1], egrid.dtype)
+    def get_abstract_eval(self):
+        name = self.name
+        npar = self._nparam
+
+        def abstract_eval(params, egrid, flux, spec_num):
+            params_shape = jnp.shape(params)
+            if params_shape[-1] != npar:
+                raise ValueError(f'{name} params shape must be (..., {npar})')
+            egrid_shape = jnp.shape(egrid)
+            if len(egrid_shape) > 1:
+                raise ValueError('egrid must be 1D array')
+            flux_shape = jnp.shape(flux)
+            if len(flux_shape) > 1:
+                raise ValueError('flux must be 1D array')
+            spec_num_shape = jnp.shape(spec_num)
+            if len(spec_num_shape):
+                raise ValueError('spec_num must be a integer')
+
+            shape = params_shape[:-1] + (egrid_shape[-1] - 1,)
+            dtype = jax.dtypes.canonicalize_dtype(egrid.dtype)
+            return ShapedArray(shape=shape, dtype=dtype)
+
+        return abstract_eval
 
     def lowering(self, ctx, params, egrid, flux, spec_num):
         egrid_type = mlir.ir.RankedTensorType(egrid.type)
         etype = egrid_type.element_type
         if isinstance(etype, mlir.ir.F32Type):
             call_target_name = f'{self._model_name}_f32'
         elif isinstance(etype, mlir.ir.F64Type):
             call_target_name = f'{self._model_name}_f64'
         else:
             raise NotImplementedError(f'unsupported dtype {etype}')
         out_shape = ctx.avals_out[0].shape
         out_type = mlir.ir.RankedTensorType.get(out_shape, etype)
         out_n = mlir.ir_constant(out_shape[-1])
+        batch_n = mlir.ir_constant(prod(out_shape[:-1]))
         return custom_call(
             call_target_name,
             result_types=[out_type],
-            operands=[params, egrid, flux, spec_num, out_n],
-            operand_layouts=avals_to_layouts(ctx.avals_in) + [()],
+            operands=[params, egrid, flux, spec_num, out_n, batch_n],
+            operand_layouts=avals_to_layouts(ctx.avals_in) + [(), ()],
             result_layouts=avals_to_layouts(ctx.avals_out)
         ).results
 
     def batching(self, vector_arg_values, batch_axes):
         if batch_axes[1] is not None:
             raise NotImplementedError('egrid batching is not implemented')
         if batch_axes[2] is not None:
             raise NotImplementedError('flux batching is not implemented')
         if batch_axes[3] is not None:
             raise NotImplementedError('spec_num batching is not implemented')
 
         params, egrid, flux, spec_num = vector_arg_values
-        if params.ndim == 1:
-            return self(params, egrid, flux, spec_num), batch_axes[0]
-        else:
-            res = [
-                self.batching((p, egrid, flux, spec_num), batch_axes)[0]
-                for p in params
-            ]
-            return jnp.array(res), batch_axes[0]
+        params = jnp.moveaxis(params, batch_axes[0], 0)
+        return self(params, egrid, flux, spec_num), 0
 
 
 def get_primitive(
     model: str
 ) -> tuple[XspecPrimitive | XspecConvPrimitive, xspex.XspecModel]:
     """Return the primitive for the given Xspec model.
 
@@ -212,14 +234,15 @@
     --------
 
     >>> apec, info = get_primitive('apec')
     >>> apec
     'apec'
 
     """
+    model = str(model)
     check = model.casefold()
     p = next(
         (v for k, v in XSModel['primitive'].items() if k.casefold() == check),
         None
     )
     if p is None:
         raise ValueError(f"Unrecognized Xspec model '{model}'")
```

### Comparing `xspex-0.0.1/src/xspex.cpp` & `xspex-0.0.2/src/xspex.cpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.1/template/__init__.py` & `xspex-0.0.2/template/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,18 @@
     'apec'
     >>> m.modeltype
     <ModelType.Add: 1>
     >>> [(p.name, p.default, p.units) for p in m.parameters]
     [('kT', 1.0, 'keV'), ('Abundanc', 1.0, None), ('Redshift', 0.0, None)]
 
     """
-
     # We want case-insensitive comparison but for the keys to retain
     # their case. Using casefold() rather than lower() is a bit OTT
     # here as I would bet model.dat is meant to be US-ASCII.
+    model = str(model)
     check = model.casefold()
     out = next((v for k, v in _info.items() if k.casefold() == check), None)
     if out is None:
         raise ValueError(f"Unrecognized Xspec model '{model}'")
 
     return out
```

### Comparing `xspex-0.0.1/template/xspex.cpp` & `xspex-0.0.2/template/xspex.cpp`

 * *Files identical despite different names*

