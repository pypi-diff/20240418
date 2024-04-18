# Comparing `tmp/anycrc-0.2.3.tar.gz` & `tmp/anycrc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.2.3.tar", last modified: Sat Apr 13 21:10:29 2024, max compression
+gzip compressed data, was "anycrc-0.3.0.tar", last modified: Wed Apr 17 23:49:14 2024, max compression
```

## Comparing `anycrc-0.2.3.tar` & `anycrc-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.493120 anycrc-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 21:10:20.000000 anycrc-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-13 21:10:29.493120 anycrc-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-13 21:10:20.000000 anycrc-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.489120 anycrc-0.2.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.489120 anycrc-0.2.3/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    15739 2024-04-13 21:10:20.000000 anycrc-0.2.3/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)    18595 2024-04-13 21:10:20.000000 anycrc-0.2.3/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-13 21:10:20.000000 anycrc-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:10:29.493120 anycrc-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-13 21:10:20.000000 anycrc-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.489120 anycrc-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.489120 anycrc-0.2.3/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 21:10:20.000000 anycrc-0.2.3/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-13 21:10:20.000000 anycrc-0.2.3/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    15050 2024-04-13 21:10:20.000000 anycrc-0.2.3/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:10:29.493120 anycrc-0.2.3/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-13 21:10:29.000000 anycrc-0.2.3/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-13 21:10:29.000000 anycrc-0.2.3/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:10:29.000000 anycrc-0.2.3/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 21:10:29.000000 anycrc-0.2.3/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.093035 anycrc-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 23:49:10.000000 anycrc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 23:49:14.093035 anycrc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-17 23:49:10.000000 anycrc-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.089035 anycrc-0.3.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.089035 anycrc-0.3.0/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    26952 2024-04-17 23:49:10.000000 anycrc-0.3.0/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-04-17 23:49:10.000000 anycrc-0.3.0/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-17 23:49:10.000000 anycrc-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:49:14.093035 anycrc-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 23:49:10.000000 anycrc-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.089035 anycrc-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.089035 anycrc-0.3.0/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 23:49:10.000000 anycrc-0.3.0/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-17 23:49:10.000000 anycrc-0.3.0/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    15050 2024-04-17 23:49:10.000000 anycrc-0.3.0/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:49:14.093035 anycrc-0.3.0/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 23:49:14.000000 anycrc-0.3.0/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 23:49:14.000000 anycrc-0.3.0/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:49:14.000000 anycrc-0.3.0/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 23:49:14.000000 anycrc-0.3.0/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.2.3/LICENSE` & `anycrc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.2.3/PKG-INFO` & `anycrc-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-The fastest Python CRC library available.
-
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
 
 ## Installation
 
 `pip install anycrc`
 
 ## Usage
 
 Use an existing model:
 
 ```python
 >>> import anycrc
->>> data = b'Hello World!'
 >>> crc32 = anycrc.Model('CRC32-ISO-HDLC')
->>> crc32.calc(data)
+>>> crc32.calc(b'Hello World!')
 472456355
 ```
 
 Read the data in chunks:
 
 ```python
 >>> crc32.reset() #set to the initial value
```

### Comparing `anycrc-0.2.3/README.md` & `anycrc-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-The fastest Python CRC library available.
-
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
 
 ## Installation
 
 `pip install anycrc`
 
 ## Usage
 
 Use an existing model:
 
 ```python
 >>> import anycrc
->>> data = b'Hello World!'
 >>> crc32 = anycrc.Model('CRC32-ISO-HDLC')
->>> crc32.calc(data)
+>>> crc32.calc(b'Hello World!')
 472456355
 ```
 
 Read the data in chunks:
 
 ```python
 >>> crc32.reset() #set to the initial value
```

### Comparing `anycrc-0.2.3/lib/crcany/crc.c` & `anycrc-0.3.0/lib/crcany/crc.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 /* crc.c -- Generic CRC calculations
  * Copyright (C) 2014, 2016, 2017, 2020, 2021 Mark Adler
  * For conditions of distribution and use, see copyright notice in crcany.c.
  */
 
+/*
+* Edited by Hussain Al Marzooq to add support for the slice-by-16 algorithm
+*/
+  
 #include <stddef.h>
 #include <assert.h>
 #include "crc.h"
 
 word_t crc_bitwise(model_t *model, word_t crc, void const *dat, size_t len) {
     unsigned char const *buf = dat;
     word_t poly = model->poly;
@@ -283,14 +287,305 @@
     if (model->ref)
         while (len--)
             crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
     else if (model->width <= 8) {
         while (len--)
             crc = model->table_byte[(crc ^ *buf++) & 0xff];
         crc >>= shift;
+    }
+    else {
+        while (len--)
+            crc = (crc << 8) ^
+                  model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
+        crc &= ONES(model->width);
+    }
+
+    // Post-process and return the CRC.
+    if (model->rev)
+        crc = reverse(crc, model->width);
+    return crc;
+}
+
+void crc_table_slice16(model_t *model, unsigned little, unsigned word_bits) {
+    unsigned opp = little ^ model->ref;
+    unsigned top =
+        model->ref ? 0 :
+                     word_bits - (model->width > 8 ? model->width : 8);
+    word_t xor = model->xorout;
+    if (model->width < 8 && !model->ref)
+        xor <<= 8 - model->width;
+    unsigned word_bytes = word_bits >> 3;
+    for (unsigned k = 0; k < 256; k++) {
+        word_t crc = model->table_byte[k];
+        model->table_word[0][k] = opp ? swaplow(crc << top, word_bytes) :
+                                        crc << top;
+        for (unsigned n = 1; n < 16; n++) {
+            crc ^= xor;
+            if (model->ref)
+                crc = (crc >> 8) ^ model->table_byte[crc & 0xff];
+            else if (model->width <= 8)
+                crc = model->table_byte[crc];
+            else {
+                crc = (crc << 8) ^
+                      model->table_byte[(crc >> (model->width - 8)) & 0xff];
+                crc &= ONES(model->width);
+            }
+            crc ^= xor;
+            model->table_word[n][k] = opp ? swaplow(crc << top, word_bytes) :
+                                            crc << top;
+        }
+    }
+}
+
+word_t crc_slice16_32(model_t *model, word_t crc, void const *dat, size_t len) {
+    unsigned char const *buf = dat;
+
+    // If requested, return the initial CRC.
+    if (buf == NULL)
+        return model->init;
+
+    // Prepare common constants.
+    unsigned little = 1;
+    little = *((unsigned char *)(&little));
+    unsigned top = model->ref ? 0 :
+                   WORDBITS - (model->width > 8 ? model->width : 8);
+    unsigned shift = model->width <= 8 ? 8 - model->width : model->width - 8;
+
+    // Pre-process the CRC.
+    if (model->rev)
+        crc = reverse(crc, model->width);
+
+    // Process the first few bytes up to a word_t boundary, if any.
+    if (model->ref) {
+        crc &= ONES(model->width);
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
+            len--;
+        }
+    }
+    else if (model->width <= 8) {
+        crc <<= shift;
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = model->table_byte[(crc ^ *buf++) & 0xff];
+            len--;
+        }
+    }
+    else
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = (crc << 8) ^
+                  model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
+            len--;
+        }
+
+    // Process as many 16 byte chunks as are available.
+    if (len >= 16) {
+        crc <<= top;
+        if (little) {
+            if (!model->ref)
+                crc = swap(crc);
+            do {
+                crc ^= *(uint32_t const *)buf;
+				uint32_t crc2 = *(uint32_t const *)(buf + 4);
+				uint32_t crc3 = *(uint32_t const *)(buf + 8);
+				uint32_t crc4 = *(uint32_t const *)(buf + 12);
+				
+                crc = model->table_word[15][crc & 0xff]
+                    ^ model->table_word[14][(crc >> 8) & 0xff]
+                    ^ model->table_word[13][(crc >> 16) & 0xff]
+                    ^ model->table_word[12][(crc >> 24) & 0xff]
+                    ^ model->table_word[11][crc2 & 0xff]
+                    ^ model->table_word[10][(crc2 >> 8) & 0xff]
+                    ^ model->table_word[9][(crc2 >> 16) & 0xff]
+                    ^ model->table_word[8][crc2 >> 24]
+					^ model->table_word[7][crc3 & 0xff]
+                    ^ model->table_word[6][(crc3 >> 8) & 0xff]
+                    ^ model->table_word[5][(crc3 >> 16) & 0xff]
+                    ^ model->table_word[4][crc3 >> 24]
+                    ^ model->table_word[3][crc4 & 0xff]
+                    ^ model->table_word[2][(crc4 >> 8) & 0xff]
+                    ^ model->table_word[1][(crc4 >> 16) & 0xff]
+                    ^ model->table_word[0][crc4 >> 24];
+					
+                buf += 16;
+                len -= 16;
+            } while (len >= 16);
+            if (!model->ref)
+                crc = swap(crc);
+        }
+        else {
+            if (model->ref)
+                crc = swap(crc);
+            do {
+                crc ^= *(uint32_t const *)buf;
+				uint32_t crc2 = *(uint32_t const *)(buf + 4);
+				uint32_t crc3 = *(uint32_t const *)(buf + 8);
+				uint32_t crc4 = *(uint32_t const *)(buf + 12);
+				
+                crc = model->table_word[0][crc4 & 0xff]
+                    ^ model->table_word[1][(crc4 >> 8) & 0xff]
+                    ^ model->table_word[2][(crc4 >> 16) & 0xff]
+                    ^ model->table_word[3][(crc4 >> 24) & 0xff]
+                    ^ model->table_word[4][crc3 & 0xff]
+                    ^ model->table_word[5][(crc3 >> 8) & 0xff]
+                    ^ model->table_word[6][(crc3 >> 16) & 0xff]
+                    ^ model->table_word[7][crc3 >> 24]
+                    ^ model->table_word[8][crc2 & 0xff]
+                    ^ model->table_word[9][(crc2 >> 8) & 0xff]
+                    ^ model->table_word[10][(crc2 >> 16) & 0xff]
+                    ^ model->table_word[11][crc2 >> 24]
+                    ^ model->table_word[12][crc & 0xff]
+                    ^ model->table_word[13][(crc >> 8) & 0xff]
+                    ^ model->table_word[14][(crc >> 16) & 0xff]
+                    ^ model->table_word[15][(crc >> 24) & 0xff];
+					
+                buf += 16;
+                len -= 16;
+            } while (len >= 16);
+            if (model->ref)
+                crc = swap(crc);
+        }
+        crc >>= top;
+    }
+
+    // Process any remaining bytes after the last 16 byte chunk.
+    if (model->ref)
+        while (len--)
+            crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
+    else if (model->width <= 8) {
+        while (len--)
+            crc = model->table_byte[(crc ^ *buf++) & 0xff];
+        crc >>= shift;
+    }
+    else {
+        while (len--)
+            crc = (crc << 8) ^
+                  model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
+        crc &= ONES(model->width);
+    }
+
+    // Post-process and return the CRC.
+    if (model->rev)
+        crc = reverse(crc, model->width);
+    return crc;
+}
+
+word_t crc_slice16_64(model_t *model, word_t crc, void const *dat, size_t len) {
+    unsigned char const *buf = dat;
+
+    // If requested, return the initial CRC.
+    if (buf == NULL)
+        return model->init;
+
+    // Prepare common constants.
+    unsigned little = 1;
+    little = *((unsigned char *)(&little));
+    unsigned top = model->ref ? 0 :
+                   WORDBITS - (model->width > 8 ? model->width : 8);
+    unsigned shift = model->width <= 8 ? 8 - model->width : model->width - 8;
+
+    // Pre-process the CRC.
+    if (model->rev)
+        crc = reverse(crc, model->width);
+
+    // Process the first few bytes up to a word_t boundary, if any.
+    if (model->ref) {
+        crc &= ONES(model->width);
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
+            len--;
+        }
+    }
+    else if (model->width <= 8) {
+        crc <<= shift;
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = model->table_byte[(crc ^ *buf++) & 0xff];
+            len--;
+        }
+    }
+    else
+        while (len && ((ptrdiff_t)buf & (WORDCHARS - 1))) {
+            crc = (crc << 8) ^
+                  model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
+            len--;
+        }
+
+    // Process as many 16 byte chunks as are available.
+    if (len >= 16) {
+        crc <<= top;
+        if (little) {
+            if (!model->ref)
+                crc = swap(crc);
+            do {
+                crc ^= *(uint64_t const *)buf;
+				uint64_t crc2 = *(uint64_t const *)(buf + 8);
+				
+                crc = model->table_word[15][crc & 0xff]
+                    ^ model->table_word[14][(crc >> 8) & 0xff]
+                    ^ model->table_word[13][(crc >> 16) & 0xff]
+                    ^ model->table_word[12][(crc >> 24) & 0xff]
+                    ^ model->table_word[11][(crc >> 32) & 0xff]
+                    ^ model->table_word[10][(crc >> 40) & 0xff]
+                    ^ model->table_word[9][(crc >> 48) & 0xff]
+                    ^ model->table_word[8][crc >> 56]
+					^ model->table_word[7][crc2 & 0xff]
+                    ^ model->table_word[6][(crc2 >> 8) & 0xff]
+                    ^ model->table_word[5][(crc2 >> 16) & 0xff]
+                    ^ model->table_word[4][(crc2 >> 24) & 0xff]
+                    ^ model->table_word[3][(crc2 >> 32) & 0xff]
+                    ^ model->table_word[2][(crc2 >> 40) & 0xff]
+                    ^ model->table_word[1][(crc2 >> 48) & 0xff]
+                    ^ model->table_word[0][crc2 >> 56];
+					
+                buf += 16;
+                len -= 16;
+            } while (len >= 16);
+            if (!model->ref)
+                crc = swap(crc);
+        }
+        else {
+            if (model->ref)
+                crc = swap(crc);
+            do {
+                crc ^= *(uint64_t const *)buf;
+				uint64_t crc2 = *(uint64_t const *)(buf + 8);
+				
+                crc = model->table_word[0][crc2 & 0xff]
+                    ^ model->table_word[1][(crc2 >> 8) & 0xff]
+                    ^ model->table_word[2][(crc2 >> 16) & 0xff]
+                    ^ model->table_word[3][(crc2 >> 24) & 0xff]
+                    ^ model->table_word[4][(crc2 >> 32) & 0xff]
+                    ^ model->table_word[5][(crc2 >> 40) & 0xff]
+                    ^ model->table_word[6][(crc2 >> 48) & 0xff]
+                    ^ model->table_word[7][crc2 >> 56]
+                    ^ model->table_word[8][crc & 0xff]
+                    ^ model->table_word[9][(crc >> 8) & 0xff]
+                    ^ model->table_word[10][(crc >> 16) & 0xff]
+                    ^ model->table_word[11][(crc >> 24) & 0xff]
+                    ^ model->table_word[12][(crc >> 32) & 0xff]
+                    ^ model->table_word[13][(crc >> 40) & 0xff]
+                    ^ model->table_word[14][(crc >> 48) & 0xff]
+                    ^ model->table_word[15][crc >> 56];
+					
+                buf += 16;
+                len -= 16;
+            } while (len >= 16);
+            if (model->ref)
+                crc = swap(crc);
+        }
+        crc >>= top;
+    }
+
+    // Process any remaining bytes after the last 16 byte chunk.
+    if (model->ref)
+        while (len--)
+            crc = (crc >> 8) ^ model->table_byte[(crc ^ *buf++) & 0xff];
+    else if (model->width <= 8) {
+        while (len--)
+            crc = model->table_byte[(crc ^ *buf++) & 0xff];
+        crc >>= shift;
     }
     else {
         while (len--)
             crc = (crc << 8) ^
                   model->table_byte[((crc >> shift) ^ *buf++) & 0xff];
         crc &= ONES(model->width);
     }
```

### Comparing `anycrc-0.2.3/lib/crcany/model.c` & `anycrc-0.3.0/lib/crcany/model.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 /* model.c -- Generic CRC parameter model routines
  * Copyright (C) 2014, 2016, 2017, 2020 Mark Adler
  * For conditions of distribution and use, see copyright notice in crcany.c.
  */
+ 
+/*
+* Edited by Hussain Al Marzooq to add support for the slice-by-16 algorithm
+*/
 
 #include "model.h"
 
 /* --- Parameter processing routines --- */
 
 #include <stdio.h>
 #include <string.h>
```

### Comparing `anycrc-0.2.3/src/anycrc/anycrc.pyx` & `anycrc-0.3.0/src/anycrc/anycrc.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -19,54 +19,69 @@
         word_t poly, poly_hi
         word_t init, init_hi
         word_t xorout, xorout_hi
         word_t check, check_hi
         word_t res, res_hi
         word_t table_comb[67]
         word_t table_byte[256]
-        word_t table_word[WORDCHARS][256]
+        word_t table_word[16][256]
         
     cdef int read_model(model_t *model, char *str, int lenient)
     cdef void process_model(model_t *model)
     
 cdef extern from '../../lib/crcany/crc.h':
     cdef void crc_table_bytewise(model_t *model)
-    cdef void crc_table_wordwise(model_t *model, unsigned little, unsigned bits)
-    cdef word_t crc_wordwise(model_t *model, word_t crc, const void* dat, size_t len)
-
+    cdef word_t crc_bytewise(model_t *model, word_t crc, const void* dat, size_t len); #for testing
+    cdef void crc_table_slice16(model_t *model, unsigned little, unsigned bits)
+    cdef word_t crc_slice16_32(model_t *model, word_t crc, const void* dat, size_t len)
+    cdef word_t crc_slice16_64(model_t *model, word_t crc, const void* dat, size_t len)
+    
 cdef class CRC:
     cdef model_t model
     cdef word_t register
+    cdef word_size
     
-    def __init__(self, unsigned short width, word_t poly, word_t init, char ref_in, char ref_out, word_t xor_out, word_t check=0, word_t residue=0):
+    def __init__(self, unsigned char width, word_t poly, word_t init, char ref_in, char ref_out, word_t xor_out, word_t check=0, word_t residue=0):
         refin = 'true' if ref_in else 'false'
         refout = 'true' if ref_out else 'false'
         
         string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name=""'.encode('utf-8')
         cdef int error_code = read_model(&self.model, string, 0)
         
         if error_code != 0:
             raise ValueError('An error occurred while retrieving the model, check the arguments passed to the CRC class')
             
         process_model(&self.model)
         crc_table_bytewise(&self.model)
         
         cdef unsigned endian = 1 if sys.byteorder == 'little' else 0
-        cdef unsigned word_size = 64 if sys.maxsize > 2 ** 32 else 32
+        self.word_size = 64 if sys.maxsize > 2 ** 32 else 32
         
-        crc_table_wordwise(&self.model, endian , word_size)
+        crc_table_slice16(&self.model, endian, self.word_size)
         self.register = self.model.init
         
     def calc(self, data):
         if isinstance(data, str):
             data = (<unicode> data).encode('utf-8')
             
-        cdef unsigned char* dat = data
-        cdef crc = crc_wordwise(&self.model, self.register, dat, len(data))
-        self.register = crc
-        return crc
+        cdef const unsigned char* data_p = data
+        
+        if self.word_size == 64:
+            self.register = crc_slice16_64(&self.model, self.register, data_p, len(data))
+        else:
+            self.register = crc_slice16_32(&self.model, self.register, data_p, len(data))
+            
+        return self.register
+        
+    def _calc(self, data):
+        if isinstance(data, str):
+            data = (<unicode> data).encode('utf-8')
+            
+        cdef const unsigned char* data_p = data
+        self.register = crc_bytewise(&self.model, self.register, data_p, len(data))
+        return self.register
         
     def reset(self):
         self.register = self.model.init
         
 def Model(name):
-    return CRC(*models[name])
+    return CRC(*models[name])
```

### Comparing `anycrc-0.2.3/src/anycrc/models.py` & `anycrc-0.3.0/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.2.3/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.3.0/src/anycrc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-The fastest Python CRC library available.
-
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time.
 
 ## Installation
 
 `pip install anycrc`
 
 ## Usage
 
 Use an existing model:
 
 ```python
 >>> import anycrc
->>> data = b'Hello World!'
 >>> crc32 = anycrc.Model('CRC32-ISO-HDLC')
->>> crc32.calc(data)
+>>> crc32.calc(b'Hello World!')
 472456355
 ```
 
 Read the data in chunks:
 
 ```python
 >>> crc32.reset() #set to the initial value
```

