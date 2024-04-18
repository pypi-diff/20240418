# Comparing `tmp/vplanet-2.5.4.tar.gz` & `tmp/vplanet-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vplanet-2.5.4.tar", last modified: Tue Apr 16 22:32:15 2024, max compression
+gzip compressed data, was "vplanet-2.5.5.tar", last modified: Thu Apr 18 02:35:32 2024, max compression
```

## Comparing `vplanet-2.5.4.tar` & `vplanet-2.5.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 22:32:14.000000 vplanet-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-16 22:32:15.931968 vplanet-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-16 22:32:14.000000 vplanet-2.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:32:15.931968 vplanet-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-16 22:32:15.000000 vplanet-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.927968 vplanet-2.5.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)   172506 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/atmesc.c
--rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/binary.c
--rw-r--r--   0 runner    (1001) docker     (127)    45227 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/body.c
--rw-r--r--   0 runner    (1001) docker     (127)    35908 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/control.c
--rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/distorb.c
--rw-r--r--   0 runner    (1001) docker     (127)    84904 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/distrot.c
--rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/eqtide.c
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/evolve.c
--rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/flare.c
--rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/galhabit.c
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/halt.c
--rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/magmoc.c
--rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/options.c
--rw-r--r--   0 runner    (1001) docker     (127)    83338 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/output.c
--rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/poise.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/python_interface.c
--rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/radheat.c
--rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/spinbody.c
--rw-r--r--   0 runner    (1001) docker     (127)    77773 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/stellar.c
--rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/system.c
--rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/thermint.c
--rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/update.c
--rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/verify.c
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 22:32:15.000000 vplanet-2.5.4/src/vplanet.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/vplanet/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/quantity_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/vplanet_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:15.931968 vplanet-2.5.4/vplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 22:32:15.000000 vplanet-2.5.4/vplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:35:32.549599 vplanet-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 02:35:30.000000 vplanet-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-18 02:35:32.549599 vplanet-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-18 02:35:30.000000 vplanet-2.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:35:32.549599 vplanet-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-18 02:35:30.000000 vplanet-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:35:32.545599 vplanet-2.5.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   171012 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/atmesc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/binary.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45778 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/body.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35908 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/control.c
+-rw-r--r--   0 runner    (1001) docker     (127)   260032 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/distorb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    84903 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/distrot.c
+-rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/eqtide.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/evolve.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/flare.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/galhabit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/halt.c
+-rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/magmoc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)   160386 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/options.c
+-rw-r--r--   0 runner    (1001) docker     (127)    83338 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/output.c
+-rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/poise.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/python_interface.c
+-rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/radheat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/spinbody.c
+-rw-r--r--   0 runner    (1001) docker     (127)    77790 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/stellar.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35212 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/system.c
+-rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/thermint.c
+-rw-r--r--   0 runner    (1001) docker     (127)   159233 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/update.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/verify.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-18 02:35:30.000000 vplanet-2.5.5/src/vplanet.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:35:32.549599 vplanet-2.5.5/vplanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/quantity_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/vplanet_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-18 02:35:30.000000 vplanet-2.5.5/vplanet/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:35:32.549599 vplanet-2.5.5/vplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 02:35:32.000000 vplanet-2.5.5/vplanet.egg-info/top_level.txt
```

### Comparing `vplanet-2.5.4/LICENSE` & `vplanet-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/PKG-INFO` & `vplanet-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.4
+Version: 2.5.5
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.4 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.5 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
```

### Comparing `vplanet-2.5.4/README.md` & `vplanet-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/setup.py` & `vplanet-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/atmesc.c` & `vplanet-2.5.5/src/atmesc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1442,47 +1442,45 @@
 
 double fdAtmEscXi(BODY *body, int iBody) {
   double dXi =
         body[iBody].dRocheRadius / (body[iBody].dRadius * body[iBody].dXFrac);
   return dXi;
 }
 
-double fdKTide(BODY *body, IO *io, int iBody) {
+double fdKTide(BODY *body, IO *io, int iNumBodies, int iBody) {
   double dKTide;
 
   // For stars and circumbinary planets, assume no Ktide enhancement
   if (body[iBody].bBinary && body[iBody].iBodyType == 0) {
     dKTide = 1.0;
   } else {
-    if (body[iBody].dAtmEscXi > 1) {
-      dKTide = (1 - 3 / (2 * body[iBody].dAtmEscXi) +
-                1 / (2 * pow(body[iBody].dAtmEscXi, 3)));
-      /*
-      fprintf(stderr,"%.5e: ",evolve->dTime/YEARSEC);
-      fprintf(stderr,"%.5e ",xi);
-      fprintf(stderr,"%.5e\n",body[iBody].dKTide);
-      */
-      if (dKTide < body[iBody].dMinKTide) {
-        dKTide = body[iBody].dMinKTide;
+    if (iNumBodies > 1) {
+      if (body[iBody].dAtmEscXi > 1) {
+        dKTide = (1 - 3 / (2 * body[iBody].dAtmEscXi) +
+                  1 / (2 * pow(body[iBody].dAtmEscXi, 3)));
+        if (dKTide < body[iBody].dMinKTide) {
+          dKTide = body[iBody].dMinKTide;
+        }
+      } else {
+        if (!io->baRocheMessage[iBody] && io->iVerbose >= VERBINPUT &&
+            (!body[iBody].bUseBondiLimited && !body[iBody].bAtmEscAuto)) {
+          fprintf(stderr,
+                  "WARNING: Roche lobe radius is larger than %s's XUV radius. "
+                  "Evolution may not be accurate.\n",
+                  body[iBody].cName);
+          fprintf(stderr, "Consider setting bUseBondiLimited = 1 or bAtmEscAuto "
+                          "= 1 to limit envelope mass loss.\n");
+          io->baRocheMessage[iBody] = 1;
+        }
+        // Fix dKTide to prevent infs when in Roche Lobe overflow
+        dKTide = 1.0;
       }
     } else {
-      if (!io->baRocheMessage[iBody] && io->iVerbose >= VERBINPUT &&
-          (!body[iBody].bUseBondiLimited && !body[iBody].bAtmEscAuto)) {
-        fprintf(stderr,
-                "WARNING: Roche lobe radius is larger than %s's XUV radius. "
-                "Evolution may not be accurate.\n",
-                body[iBody].cName);
-        fprintf(stderr, "Consider setting bUseBondiLimited = 1 or bAtmEscAuto "
-                        "= 1 to limit envelope mass loss.\n");
-        io->baRocheMessage[iBody] = 1;
-      }
-      // Fix dKTide to prevent infs when in Roche Lobe overflow
       dKTide = 1.0;
     }
-    // body[iBody].dKTide = 1.0;
   }
 
   return dKTide;
 }
 
 /**
 If necessary, change how the code handle hydrogen envelope escape
@@ -1690,27 +1688,27 @@
                                 fnUpdate, iBody, iModule);
   } else if (body[iBody].dSurfaceWaterMass > 0) {
     ForceBehaviorWaterEscape(body, module, evolve, io, system, update, fnUpdate,
                              iBody, iModule);
   }
 }
 
-void AuxPropsLehmer17(BODY *body, int iBody) {
+void AuxPropsLehmer17(BODY *body, EVOLVE *evolve, int iBody) {
   if (body[iBody].bAutoThermTemp) {
     body[iBody].dThermTemp = fdThermalTemp(body, iBody);
   }
   body[iBody].dGravAccel = BIGG *
                            (body[iBody].dMass - body[iBody].dEnvelopeMass) /
                            (body[iBody].dRadSolid * body[iBody].dRadSolid);
   body[iBody].dScaleHeight = body[iBody].dAtmGasConst * body[iBody].dThermTemp /
                              body[iBody].dGravAccel;
   body[iBody].dPresSurf =
         fdLehmerPres(body[iBody].dEnvelopeMass, body[iBody].dGravAccel,
                      body[iBody].dRadSolid);
-  body[iBody].dRadXUV = fdLehmerRadius(body, iBody);
+  body[iBody].dRadXUV = fdLehmerRadius(body, evolve->iNumBodies, iBody);
   body[iBody].dRadius = body[iBody].dRadXUV / body[iBody].dXFrac;
 }
 
 
 /**
 Initializes several helper variables and properties used in the integration.
 
@@ -1722,22 +1720,22 @@
 
 // XXX A lot of this function should be moved to ForceBehavior! PropsAux is only
 // for computing parameters that make the derivatives easier to interpret
 void fnPropsAuxAtmEsc(BODY *body, EVOLVE *evolve, IO *io, UPDATE *update,
                       int iBody) {
 
   if (body[iBody].iPlanetRadiusModel == ATMESC_LEHMER17) {
-    AuxPropsLehmer17(body, iBody);
+    AuxPropsLehmer17(body, evolve, iBody);
   }
 
   // Compute various radii of interest
   body[iBody].dBondiRadius = fdBondiRadius(body, iBody);
-  body[iBody].dRocheRadius = fdRocheRadius(body, iBody);
+  body[iBody].dRocheRadius = fdRocheRadius(body, evolve->iNumBodies, iBody);
   body[iBody].dAtmEscXi    = fdAtmEscXi(body, iBody);
-  body[iBody].dKTide       = fdKTide(body, io, iBody);
+  body[iBody].dKTide       = fdKTide(body, io, evolve->iNumBodies, iBody);
 
   // The XUV flux
   if (body[iBody].bCalcFXUV) {
     body[iBody].dFXUV = fdXUVFlux(body, iBody);
   }
 
   // The H2O XUV escape efficiency
@@ -2129,15 +2127,15 @@
               "envelope ",
               body[iBody].cName);
         fprintf(stderr, "mass exceeds this threshold.\n");
       }
 
       // Calculate auxiliary properties
       body[iBody].dRadSolid = fdMassToRad_LehmerCatling17(body[iBody].dMass - body[iBody].dEnvelopeMass);
-      AuxPropsLehmer17(body,iBody);      
+      AuxPropsLehmer17(body,&(control->Evolve), iBody);      
     } else {
       fprintf(stderr,
               "ERROR: The Lehmer & Catling (2017) model requires a star.\n");
       exit(EXIT_INPUT);
     }
   } else {
     int iCol, bError = 0;
@@ -2308,15 +2306,15 @@
   if (body[iBody].dEnvelopeMass > 0) {
     body[iBody].dSolidMass = body[iBody].dMass - body[iBody].dEnvelopeMass;
   }
 
   // Setup radius and other radii of interest
   VerifyRadiusAtmEsc(body, control, options, update, body[iBody].dAge, iBody);
   body[iBody].dBondiRadius = fdBondiRadius(body, iBody);
-  body[iBody].dRocheRadius = fdRocheRadius(body, iBody);
+  body[iBody].dRocheRadius = fdRocheRadius(body, control->Evolve.iNumBodies, iBody);
 
   control->fnForceBehavior[iBody][iModule]   = &fnForceBehaviorAtmEsc;
   control->fnPropsAux[iBody][iModule]        = &fnPropsAuxAtmEsc;
   control->Evolve.fnBodyCopy[iBody][iModule] = &BodyCopyAtmEsc;
 }
 
 /**************** ATMESC update ****************/
@@ -3425,19 +3423,23 @@
 @param iBody The current body Number
 @param dTmp Temporary variable used for unit conversions
 @param cUnit The unit for this variable
 */
 void WriteHRefODragMod(BODY *body, CONTROL *control, OUTPUT *output,
                        SYSTEM *system, UNITS *units, UPDATE *update, int iBody,
                        double *dTmp, char cUnit[]) {
-  double rat = (body[iBody].dCrossoverMass / ATOMMASS - QOH) /
-               (body[iBody].dCrossoverMass / ATOMMASS - 1.);
-  double XO = fdAtomicOxygenMixingRatio(body[iBody].dSurfaceWaterMass,
-                                        body[iBody].dOxygenMass);
-  *dTmp     = pow(1. + (XO / (1. - XO)) * QOH * rat, -1);
+  if (body[iBody].dCrossoverMass / ATOMMASS - 1. != 0) {
+    double rat = (body[iBody].dCrossoverMass / ATOMMASS - QOH) /
+                (body[iBody].dCrossoverMass / ATOMMASS - 1.);
+    double XO = fdAtomicOxygenMixingRatio(body[iBody].dSurfaceWaterMass,
+                                          body[iBody].dOxygenMass);
+    *dTmp     = pow(1. + (XO / (1. - XO)) * QOH * rat, -1);
+  } else {
+    *dTmp = -1;
+  }
   strcpy(cUnit, "");
 }
 
 
 /**
 Logs the molecular oxygen mixing ratio.
 
@@ -4078,15 +4080,15 @@
 */
 double fdPlanetRadius(BODY *body, SYSTEM *system, int *iaBody) {
 
   if (body[iaBody[0]].iPlanetRadiusModel == ATMESC_LEHMER17) {
     body[iaBody[0]].dPresSurf =
           fdLehmerPres(body[iaBody[0]].dEnvelopeMass,
                        body[iaBody[0]].dGravAccel, body[iaBody[0]].dRadSolid);
-    body[iaBody[0]].dRadXUV = fdLehmerRadius(body, iaBody[0]);
+    body[iaBody[0]].dRadXUV = fdLehmerRadius(body, system->iNumBodies, iaBody[0]);
   }
 
   double foo;
   if (body[iaBody[0]].iPlanetRadiusModel == ATMESC_LOP12) {
     // If no envelope, return solid body radius according to Sotin+2007 model
     if (body[iaBody[0]].dEnvelopeMass <= body[iaBody[0]].dMinEnvelopeMass) {
       foo = fdMassToRad_Sotin07(body[iaBody[0]].dMass);
@@ -4130,14 +4132,19 @@
     if ((body[iBody].dRGDuration == 0.) &&
         (fdInstellation(body, iBody) < fdHZRG14(body, iBody))) {
       body[iBody].dRGDuration = body[iBody].dAge;
     }
     return 0;
   }
 
+  /* If the central body is not a star, then allow water to escape */
+  if (!body[0].bStellar) {
+    return 1;
+  }
+
   // 2. Check if planet is beyond RG limit; if user requested water loss to stop
   // (the cold trap prevents water loss) then water does not escape.
   // NOTE: The RG flux limit below is calculated based on body zero's
   // spectrum! The Kopparapu+14 limit is for a single star only. This
   // approximation for a binary is only valid if the two stars have
   // similar spectral types, or if body zero dominates the flux.
   double dInstellation = fdInstellation(body, iBody);
@@ -4359,70 +4366,15 @@
     num += (x[i] - xavg) * (y[i] - yavg);
     den += (x[i] - xavg) * (x[i] - xavg);
   }
   daCoeffs[0] = num / den;                 // Slope
   daCoeffs[1] = yavg - daCoeffs[0] * xavg; // Intercept
 }
 
-/**
- Calculate sound speed of a diatomic H (H2) isothermal gaseous atmosphere in
- which the temperature is set by the local equilibrium temperature.
-
- @param dTemp double stellar effective temperature
- @param dRad double stellar radius
- @param dSemi double planetary semi-major axis
-
- @return sound speed
-*/
-double fdEqH2AtmosphereSoundSpeed(double dTemp, double dRad, double dSemi) {
 
-  double dCS = 2300.0 * sqrt(dTemp / 5800.0) * pow(dRad / RSUN, 0.25) *
-               pow(dSemi / (0.1 * AUM), 0.25);
-  return dCS;
-}
-
-/**
- Calculate the Roche radius assuming body 0 is the host star using Eqn. 8 from
- Luger et al. (2015)
-
- @param body BODY struct
- @param iBody int body indentifier
-
- @return Body's Roche radius
-*/
-double fdRocheRadius(BODY *body, int iBody) {
-  double dRoche = pow(body[iBody].dMass / (3.0 * body[0].dMass), 1. / 3.) *
-                  body[iBody].dSemi;
-  return dRoche;
-}
-
-/**
- Calculate the Bondi radius assuming body 0 is the host star and that the
- planetary atmosphere at the Bondi radius is diatomic H2 at the blackbody
- equilibrium temperature set by thermal emission from the host star adapting
- equation. Adapted from equations 2 and 4 from Owen & Wu (2016)
-
- @param body BODY struct
- @param iBody int body indentifier
-
- @return Body's Bondi radius
-*/
-double fdBondiRadius(BODY *body, int iBody) {
-  double dBondiRadius;
-  // Compute sound speed in planet's atmosphere assuming a diatomic H atmosphere
-  // assuming body 0 is the star
-  if (body[0].bStellar) {
-    double dSoundSpeed = fdEqH2AtmosphereSoundSpeed(body[0].dTemperature, body[0].dRadius,
-                                         body[iBody].dSemi);
-    dBondiRadius = BIGG * body[iBody].dMass / (2.0 * dSoundSpeed * dSoundSpeed);
-  } else {
-    dBondiRadius = -1;
-  }
-  return dBondiRadius;
-}
 
 /**
  Calculate the whether or not incident XUV flux exceeds critical flux between
  the radiation/recombination-limited and energy-limited H envelope escape
  regimes following Luger+2015 Eqn. 13
 
  @param body BODY struct
```

### Comparing `vplanet-2.5.4/src/binary.c` & `vplanet-2.5.5/src/binary.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/body.c` & `vplanet-2.5.5/src/body.c`

 * *Files 1% similar despite different names*

```diff
@@ -573,27 +573,27 @@
    @param dGravAccel Body's gravitational acceleration
    @param dRadSurf Surface Radius of rocky core
    @param dScaleHeight Atmospheric scale height
    @param dPresSurf pressure at surface due to envelope
    @param dRadXUV radius from center of planet where optical depth of XUV is
   unity
    */
-double fdLehmerRadius(BODY *body, int iBody) {
+double fdLehmerRadius(BODY *body, int iNumBodies, int iBody) {
   double dRadXUV, dRoche;
 
   // Set floor for surface pressure to prevent overflow error
   if (body[iBody].dPresSurf > 1e-100) {
     dRadXUV = body[iBody].dRadSolid * body[iBody].dRadSolid /
             (body[iBody].dScaleHeight *
                    log(body[iBody].dPresXUV / body[iBody].dPresSurf) +
              body[iBody].dRadSolid);
   } else {
     dRadXUV = body[iBody].dRadSolid;
   }
-  dRoche = fdRocheRadius(body, iBody);
+  dRoche = fdRocheRadius(body, iNumBodies, iBody);
   // printf("%lf %lf %lf %lf
   // %lf\n",body[iBody].dPresXUV,body[iBody].dPresSurf,body[iBody].dGravAccel,body[iBody].dEnvelopeMass,dRadXUV);
   if (dRadXUV <= 0) {
     dRadXUV = dRoche;
   }
   if (dRadXUV > dRoche) {
     dRadXUV = dRoche;
@@ -604,14 +604,32 @@
   if (body[iBody].dEnvelopeMass == 0) {
     dRadXUV = body[iBody].dRadSolid;
   }
   return dRadXUV;
 }
 
 /**
+ Calculate sound speed of a diatomic H (H2) isothermal gaseous atmosphere in
+ which the temperature is set by the local equilibrium temperature.
+
+ @param dTemp double stellar effective temperature
+ @param dRad double stellar radius
+ @param dSemi double planetary semi-major axis
+
+ @return sound speed
+*/
+double fdEqH2AtmosphereSoundSpeed(double dTemp, double dRad, double dSemi) {
+
+  double dCS = 2300.0 * sqrt(dTemp / 5800.0) * pow(dRad / RSUN, 0.25) *
+               pow(dSemi / (0.1 * AUM), 0.25);
+  return dCS;
+}
+
+
+/**
   Lehmer+ (2017)'s model for the pressure of a planet where it's losing its
   atmopshere due to XUV radiation.
 
    @param dMassEnv Envelope's mass
    @param dGravAccel Body's gravitational acceleration
    @param dRadSurf Surface Radius of rocky core
    @param dPresXUV Pressure at base of thermosphere
```

### Comparing `vplanet-2.5.4/src/control.c` & `vplanet-2.5.5/src/control.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/distorb.c` & `vplanet-2.5.5/src/distorb.c`

 * *Files 1% similar despite different names*

```diff
@@ -1267,182 +1267,149 @@
   } else if (control->Evolve.iDistOrbModel == LL2) {
     VerifyPericenter(body, control, options, files->Infile[iBody + 1].cIn,
                      iBody, control->Io.iVerbose);
     control->fnPropsAux[iBody][iModule] = &PropsAuxDistOrb;
 
     CalcHK(body, iBody);
     CalcPQ(body, iBody);
+  
+    if (iBody == 1) {
+      system->daLOrb = malloc(3 * sizeof(double));
+
+      system->daLaplaceD = malloc(1 * sizeof(double *));
+      system->daAlpha0   = malloc(1 * sizeof(double *));
+
+      system->iaLaplaceN =
+            malloc((control->Evolve.iNumBodies) * sizeof(int *));
+      system->daAlpha0[0] =
+            malloc(fniNchoosek(control->Evolve.iNumBodies - 1, 2) *
+                    sizeof(double *));
+      system->daLaplaceD[0] =
+            malloc(fniNchoosek(control->Evolve.iNumBodies - 1, 2) *
+                    sizeof(double *));
+      for (j = 0; j < fniNchoosek(control->Evolve.iNumBodies - 1, 2); j++) {
+        system->daLaplaceD[0][j] = malloc(2 * sizeof(double));
+        system->daAlpha0[0][j]   = malloc(1 * sizeof(double));
+      }
+      for (j = 1; j < (control->Evolve.iNumBodies); j++) {
+        system->iaLaplaceN[j] =
+              malloc((control->Evolve.iNumBodies) * sizeof(int));
+      }
+    }
 
-    if (body[iBody].bEigenSet == 1) {
-      /* This should be improved. It's not really clear what this code does. */
+    for (jBody = 1; jBody < (control->Evolve.iNumBodies); jBody++) {
+      body[jBody].daLOrb    = malloc(3 * sizeof(double));
+      body[jBody].daLOrbTmp = malloc(3 * sizeof(double));
+
+      if (body[iBody].dSemi < body[jBody].dSemi) {
+        system->iaLaplaceN[iBody][jBody] =
+              fniCombCount(iBody, jBody, control->Evolve.iNumBodies - 1);
+        system->daAlpha0[0][system->iaLaplaceN[iBody][jBody]][0] =
+              body[iBody].dSemi / body[jBody].dSemi;
+        system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][0] =
+              fndDerivLaplaceCoeff(1, body[iBody].dSemi / body[jBody].dSemi,
+                                    1, 1.5);
+        system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][1] =
+              fndDerivLaplaceCoeff(1, body[iBody].dSemi / body[jBody].dSemi,
+                                    2, 1.5);
+      } else if (body[iBody].dSemi > body[jBody].dSemi) {
+        system->iaLaplaceN[iBody][jBody] =
+              fniCombCount(jBody, iBody, control->Evolve.iNumBodies - 1);
+        system->daAlpha0[0][system->iaLaplaceN[iBody][jBody]][0] =
+              body[jBody].dSemi / body[iBody].dSemi;
+        system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][0] =
+              fndDerivLaplaceCoeff(1, body[jBody].dSemi / body[iBody].dSemi,
+                                    1, 1.5);
+        system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][1] =
+              fndDerivLaplaceCoeff(1, body[jBody].dSemi / body[iBody].dSemi,
+                                    2, 1.5);
+      }
+    }
+
+    if (iBody == (control->Evolve.iNumBodies - 1)) {
+      VerifyGRCorrLL2(body, control->Evolve.iNumBodies);
+      if (control->bInvPlane) {
+        inv_plane(body, system, control->Evolve.iNumBodies);
+      }
       system->daEigenValEcc = malloc(2 * sizeof(double *));
-      system->daEigenValInc = malloc(2 * sizeof(double *));
       system->daEigenVecEcc =
             malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
+      system->daEigenValInc = malloc(2 * sizeof(double *));
       system->daEigenVecInc =
             malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
       system->daEigenPhase = malloc(2 * sizeof(double *));
 
-      system->daEigenValEcc[0] = malloc(1 * sizeof(double));
-      system->daEigenValInc[0] = malloc(1 * sizeof(double));
-      system->daEigenVecEcc[0] = malloc(1 * sizeof(double));
-      system->daEigenVecInc[0] = malloc(1 * sizeof(double));
-      system->daEigenPhase[0]  = malloc(1 * sizeof(double));
-      system->daEigenPhase[1]  = malloc(1 * sizeof(double));
-
-      system->daEigenValEcc[0][0] = 0.0;
-      // system->daEigenValInc[0][0] = -0.000123627489;
-      system->daEigenValInc[0][0] = -0.000119874715;
-      system->daEigenVecEcc[0][0] = 0.0;
-      // system->daEigenVecInc[0][0] = 0.00506143322;
-      system->daEigenVecInc[0][0] = 0.0036367199;
-
-      system->daEigenPhase[0][0] = 0.0;
-      //       system->daEigenPhase[1][0] =
-      //       atan2(body[iBody].dHecc,body[iBody].dKecc);
-      system->daEigenPhase[1][0] = 2.6348951757;
-
-    } else {
-      /* Conditions for recalc'ing eigenvalues */
-      if (iBody == 1) {
-        system->daLOrb = malloc(3 * sizeof(double));
-
-        system->daLaplaceD = malloc(1 * sizeof(double *));
-        system->daAlpha0   = malloc(1 * sizeof(double *));
-
-        system->iaLaplaceN =
-              malloc((control->Evolve.iNumBodies) * sizeof(int *));
-        system->daAlpha0[0] =
-              malloc(fniNchoosek(control->Evolve.iNumBodies - 1, 2) *
-                     sizeof(double *));
-        system->daLaplaceD[0] =
-              malloc(fniNchoosek(control->Evolve.iNumBodies - 1, 2) *
-                     sizeof(double *));
-        for (j = 0; j < fniNchoosek(control->Evolve.iNumBodies - 1, 2); j++) {
-          system->daLaplaceD[0][j] = malloc(2 * sizeof(double));
-          system->daAlpha0[0][j]   = malloc(1 * sizeof(double));
-        }
-        for (j = 1; j < (control->Evolve.iNumBodies); j++) {
-          system->iaLaplaceN[j] =
-                malloc((control->Evolve.iNumBodies) * sizeof(int));
-        }
-      }
+      system->daA =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
+      system->daB =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
+      system->daAsoln =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->daBsoln =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->daAcopy =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
 
-      for (jBody = 1; jBody < (control->Evolve.iNumBodies); jBody++) {
-        body[jBody].daLOrb    = malloc(3 * sizeof(double));
-        body[jBody].daLOrbTmp = malloc(3 * sizeof(double));
-
-        if (body[iBody].dSemi < body[jBody].dSemi) {
-          system->iaLaplaceN[iBody][jBody] =
-                fniCombCount(iBody, jBody, control->Evolve.iNumBodies - 1);
-          system->daAlpha0[0][system->iaLaplaceN[iBody][jBody]][0] =
-                body[iBody].dSemi / body[jBody].dSemi;
-          system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][0] =
-                fndDerivLaplaceCoeff(1, body[iBody].dSemi / body[jBody].dSemi,
-                                     1, 1.5);
-          system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][1] =
-                fndDerivLaplaceCoeff(1, body[iBody].dSemi / body[jBody].dSemi,
-                                     2, 1.5);
-        } else if (body[iBody].dSemi > body[jBody].dSemi) {
-          system->iaLaplaceN[iBody][jBody] =
-                fniCombCount(jBody, iBody, control->Evolve.iNumBodies - 1);
-          system->daAlpha0[0][system->iaLaplaceN[iBody][jBody]][0] =
-                body[jBody].dSemi / body[iBody].dSemi;
-          system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][0] =
-                fndDerivLaplaceCoeff(1, body[jBody].dSemi / body[iBody].dSemi,
-                                     1, 1.5);
-          system->daLaplaceD[0][system->iaLaplaceN[iBody][jBody]][1] =
-                fndDerivLaplaceCoeff(1, body[jBody].dSemi / body[iBody].dSemi,
-                                     2, 1.5);
-        }
+      for (jBody = 0; jBody < (control->Evolve.iNumBodies - 1); jBody++) {
+        system->daA[jBody] =
+              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+        system->daB[jBody] =
+              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+        system->daEigenVecEcc[jBody] =
+              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+        system->daEigenVecInc[jBody] =
+              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+        system->daAcopy[jBody] =
+              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
       }
 
-      //     body[iBody].dSemiPrev = body[iBody].dSemiPrev;
-
-      if (iBody == (control->Evolve.iNumBodies - 1)) {
-        VerifyGRCorrLL2(body, control->Evolve.iNumBodies);
-        if (control->bInvPlane) {
-          inv_plane(body, system, control->Evolve.iNumBodies);
-        }
-        system->daEigenValEcc = malloc(2 * sizeof(double *));
-        system->daEigenVecEcc =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->daEigenValInc = malloc(2 * sizeof(double *));
-        system->daEigenVecInc =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->daEigenPhase = malloc(2 * sizeof(double *));
-
-        system->daA =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->daB =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->daAsoln =
+      for (i = 0; i < 2; i++) {
+        system->daEigenValEcc[i] =
               malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->daBsoln =
+        system->daEigenValInc[i] =
               malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->daAcopy =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-
-        for (jBody = 0; jBody < (control->Evolve.iNumBodies - 1); jBody++) {
-          system->daA[jBody] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daB[jBody] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daEigenVecEcc[jBody] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daEigenVecInc[jBody] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daAcopy[jBody] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        }
-
-        for (i = 0; i < 2; i++) {
-          system->daEigenValEcc[i] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daEigenValInc[i] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daEigenPhase[i] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        }
-        system->daScale =
+        system->daEigenPhase[i] =
               malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->iaRowswap =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(int));
+      }
+      system->daScale =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->iaRowswap =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(int));
 
 
-        SolveEigenVal(body, &control->Evolve, system);
+      SolveEigenVal(body, &control->Evolve, system);
 
-        system->daetmp =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->daitmp =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
-        system->iaRowswap =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(int));
-        system->dah0 =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->dak0 =
-              malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->dap0 =
+      system->daetmp =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
+      system->daitmp =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double *));
+      system->iaRowswap =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(int));
+      system->dah0 =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->dak0 =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->dap0 =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->daq0 =
+            malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+
+      for (i = 0; i < (control->Evolve.iNumBodies - 1); i++) {
+        system->daetmp[i] =
               malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->daq0 =
+        system->daitmp[i] =
               malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-
-        for (i = 0; i < (control->Evolve.iNumBodies - 1); i++) {
-          system->daetmp[i] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-          system->daitmp[i] =
-                malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        }
-        system->daS = malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-        system->daT = malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
-
-        ScaleEigenVec(body, &control->Evolve, system);
       }
+      system->daS = malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+      system->daT = malloc((control->Evolve.iNumBodies - 1) * sizeof(double));
+
+      ScaleEigenVec(body, &control->Evolve, system);
     }
 
+
     body[iBody].iGravPerts = control->Evolve.iNumBodies - 1;
     VerifyPerturbersDistOrbLL2(body, control->Evolve.iNumBodies, iBody);
 
     for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
       /* h = Ecc*sin(LongP) */
       InitializeHeccDistOrbLL2(body, update, iBody, iPert);
 
@@ -1450,26 +1417,26 @@
       InitializeKeccDistOrbLL2(body, update, iBody, iPert);
 
       /* p = s*sin(LongA) */
       InitializePincDistOrbLL2(body, update, iBody, iPert);
 
       /* q = s*cos(LongA) */
       InitializeQincDistOrbLL2(body, update, iBody, iPert);
-    }
+    //}
 
-    /* If the mutual inclination of any object gets above MAXMUTUALINCLL2,
-       print a warning message. */
+      /* If the mutual inclination of any object gets above MAXMUTUALINCLL2,
+        print a warning message. */
     control->Io.dMaxMutualInc = MAXMUTUALINCLL2 * PI / 180;
 
-    // if (body[iBody].bGRCorr) {
-    //       fprintf(stderr,"ERROR: %s cannot be used in LL2 orbital
-    //       solution.\n",options[OPT_GRCORR].cName);
-    //       LineExit(files->Infile[iBody+1].cIn,options[OPT_GRCORR].iLine[iBody+1]);
-    //     }
-  }
+      // if (body[iBody].bGRCorr) {
+      //       fprintf(stderr,"ERROR: %s cannot be used in LL2 orbital
+      //       solution.\n",options[OPT_GRCORR].cName);
+      //       LineExit(files->Infile[iBody+1].cIn,options[OPT_GRCORR].iLine[iBody+1]);
+    }
+  } // DistorbModel == LL2
 
   control->fnForceBehavior[iBody][iModule]   = &ForceBehaviorDistOrb;
   control->Evolve.fnBodyCopy[iBody][iModule] = &BodyCopyDistOrb;
 }
 
 
 /***************** DISTORB Update *****************/
@@ -1505,60 +1472,62 @@
 }
 
 void FinalizeUpdateHeccDistOrb(BODY *body, UPDATE *update, int *iEqn, int iVar,
                                int iBody, int iFoo) {
   /* The indexing gets a bit confusing here. iPert = 0 to iGravPerts-1
    * correspond to all perturbing planets, iPert = iGravPerts corresponds to the
    * stellar general relativistic correction, if applied */
+   /* XXX This should be changed to body[iBody].iGravPerts knows before hecc and kecc 
+   are initialized in update.c if the GR correction has been applied! */
 
   int iPert;
 
+  update[iBody].iaModule[iVar][*iEqn] = DISTORB;
   if (body[iBody].bGRCorr) {
     update[iBody].padDHeccDtDistOrb =
           malloc((body[iBody].iGravPerts + 1) * sizeof(double *));
     update[iBody].iaHeccDistOrb =
           malloc((body[iBody].iGravPerts + 1) * sizeof(int));
     for (iPert = 0; iPert < body[iBody].iGravPerts + 1; iPert++) {
-      update[iBody].iaModule[iVar][*iEqn] = DISTORB;
+
       update[iBody].iaHeccDistOrb[iPert]  = (*iEqn)++;
     }
   } else {
     update[iBody].padDHeccDtDistOrb =
           malloc(body[iBody].iGravPerts * sizeof(double *));
     update[iBody].iaHeccDistOrb = malloc(body[iBody].iGravPerts * sizeof(int));
     for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
-      update[iBody].iaModule[iVar][*iEqn] = DISTORB;
       update[iBody].iaHeccDistOrb[iPert]  = (*iEqn)++;
     }
   }
 }
 
 void FinalizeUpdateKeccDistOrb(BODY *body, UPDATE *update, int *iEqn, int iVar,
                                int iBody, int iFoo) {
   /* The indexing gets a bit confusing here. iPert = 0 to iGravPerts-1
    * correspond to all perturbing planets, iPert = iGravPerts corresponds to the
    * stellar general relativistic correction, if applied */
 
   int iPert;
 
+  update[iBody].iaModule[iVar][*iEqn] = DISTORB;
   if (body[iBody].bGRCorr) {
     update[iBody].padDKeccDtDistOrb =
           malloc((body[iBody].iGravPerts + 1) * sizeof(double *));
     update[iBody].iaKeccDistOrb =
           malloc((body[iBody].iGravPerts + 1) * sizeof(int));
     for (iPert = 0; iPert < body[iBody].iGravPerts + 1; iPert++) {
-      update[iBody].iaModule[iVar][*iEqn] = DISTORB;
+ 
       update[iBody].iaKeccDistOrb[iPert]  = (*iEqn)++;
     }
   } else {
     update[iBody].padDKeccDtDistOrb =
           malloc(body[iBody].iGravPerts * sizeof(double *));
     update[iBody].iaKeccDistOrb = malloc(body[iBody].iGravPerts * sizeof(int));
     for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
-      update[iBody].iaModule[iVar][*iEqn] = DISTORB;
       update[iBody].iaKeccDistOrb[iPert]  = (*iEqn)++;
     }
   }
 }
 
 void FinalizeUpdatePincDistOrb(BODY *body, UPDATE *update, int *iEqn, int iVar,
                                int iBody, int iFoo) {
```

### Comparing `vplanet-2.5.4/src/distrot.c` & `vplanet-2.5.5/src/distrot.c`

 * *Files 0% similar despite different names*

```diff
@@ -1066,15 +1066,15 @@
   dDeriv = 0;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += dpAdx * (*(update[iBody].padDXoblDtDistRot[iPert])) +
               dpAdy * (*(update[iBody].padDYoblDtDistRot[iPert]));
   }
 
   if (dDeriv == 0) {
-    dDeriv = -1;
+    *dTmp = -1;
   } else {
     *dTmp = fabs(2 * PI / dDeriv);
   }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
```

### Comparing `vplanet-2.5.4/src/eqtide.c` & `vplanet-2.5.5/src/eqtide.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/evolve.c` & `vplanet-2.5.5/src/evolve.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/flare.c` & `vplanet-2.5.5/src/flare.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/galhabit.c` & `vplanet-2.5.5/src/galhabit.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/halt.c` & `vplanet-2.5.5/src/halt.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/magmoc.c` & `vplanet-2.5.5/src/magmoc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/module.c` & `vplanet-2.5.5/src/module.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/options.c` & `vplanet-2.5.5/src/options.c`

 * *Files 0% similar despite different names*

```diff
@@ -1187,14 +1187,15 @@
 
   strcpy(input.cIn, infile);
   /* Initialize primary input file */
   InitializeInput(&input);
 
   /* First find input files */
   ReadBodyFileNames(control, files, &options[OPT_BODYFILES], &input);
+  system->iNumBodies = control->Evolve.iNumBodies;
 
   // allocate the body struct
   *body = malloc(control->Evolve.iNumBodies * sizeof(BODY));
 
   /* Initialize functions in the module struct */
   InitializeModule(*body, control, module);
```

### Comparing `vplanet-2.5.4/src/output.c` & `vplanet-2.5.5/src/output.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/poise.c` & `vplanet-2.5.5/src/poise.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/python_interface.c` & `vplanet-2.5.5/src/python_interface.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/radheat.c` & `vplanet-2.5.5/src/radheat.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/spinbody.c` & `vplanet-2.5.5/src/spinbody.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/stellar.c` & `vplanet-2.5.5/src/stellar.c`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   dest[iBody].iStellarModel        = src[iBody].iStellarModel;
   dest[iBody].iWindModel           = src[iBody].iWindModel;
   dest[iBody].iXUVModel            = src[iBody].iXUVModel;
   dest[iBody].iMagBrakingModel     = src[iBody].iMagBrakingModel;
   dest[iBody].dLXUV                = src[iBody].dLXUV;
   dest[iBody].bRossbyCut           = src[iBody].bRossbyCut;
   dest[iBody].bEvolveRG            = src[iBody].bEvolveRG;
+  dest[iBody].dLuminosityInitial = src[iBody].dLuminosityInitial;
   dest[iBody].dLuminosityAmplitude = src[iBody].dLuminosityAmplitude;
   dest[iBody].dLuminosityFrequency = src[iBody].dLuminosityFrequency;
   dest[iBody].dLuminosityPhase     = src[iBody].dLuminosityPhase;
 }
 
 /**************** STELLAR options ********************/
 
@@ -1520,15 +1521,14 @@
     if (!isnan(foo)) {
       return foo;
     } else {
       body[iaBody[0]].iStellarModel = STELLAR_MODEL_CONST;
     }
   }
   if (body[iaBody[0]].iStellarModel == STELLAR_MODEL_SINEWAVE) {
-    printf("%lf\n",body[iaBody[0]].dLuminosity);
     foo = fdEffectiveTemperature(body,iaBody[0]);
     return foo;
   }
   if (body[iaBody[0]].iStellarModel == STELLAR_MODEL_NONE ||
       body[iaBody[0]].iStellarModel == STELLAR_MODEL_CONST) {
     return body[iaBody[0]].dTemperature;
   } else {
```

### Comparing `vplanet-2.5.4/src/system.c` & `vplanet-2.5.5/src/system.c`

 * *Files 2% similar despite different names*

```diff
@@ -1061,7 +1061,53 @@
   }
 
   // Add orbiter's mass to central body
   body[0].dMass += body[iBody].dMass;
   body[iBody].dMass = 0;
   body[iBody].dSemi = body[0].dRadius;
 }
+
+/**
+ Calculate the Roche radius assuming body 0 is the host star using Eqn. 8 from
+ Luger et al. (2015)
+
+ @param body BODY struct
+ @param iBody int body indentifier
+
+ @return Body's Roche radius
+*/
+double fdRocheRadius(BODY *body, int iNumBodies, int iBody) {
+  double dRoche; 
+  
+  if (iNumBodies == 1) {
+    dRoche = DBL_MAX;
+  } else {
+    dRoche = pow(body[iBody].dMass / (3.0 * body[0].dMass), 1. / 3.) *
+                  body[iBody].dSemi;
+  }
+  return dRoche;
+}
+
+/**
+ Calculate the Bondi radius assuming body 0 is the host star and that the
+ planetary atmosphere at the Bondi radius is diatomic H2 at the blackbody
+ equilibrium temperature set by thermal emission from the host star adapting
+ equation. Adapted from equations 2 and 4 from Owen & Wu (2016)
+
+ @param body BODY struct
+ @param iBody int body indentifier
+
+ @return Body's Bondi radius
+*/
+double fdBondiRadius(BODY *body, int iBody) {
+  double dBondiRadius;
+  // Compute sound speed in planet's atmosphere assuming a diatomic H atmosphere
+  // assuming body 0 is the star
+  if (body[0].bStellar) {
+    double dSoundSpeed = fdEqH2AtmosphereSoundSpeed(body[0].dTemperature, body[0].dRadius,
+                                         body[iBody].dSemi);
+    dBondiRadius = BIGG * body[iBody].dMass / (2.0 * dSoundSpeed * dSoundSpeed);
+  } else {
+    dBondiRadius = -1;
+  }
+  return dBondiRadius;
+}
```

### Comparing `vplanet-2.5.4/src/thermint.c` & `vplanet-2.5.5/src/thermint.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/update.c` & `vplanet-2.5.5/src/update.c`

 * *Files 0% similar despite different names*

```diff
@@ -1783,14 +1783,15 @@
       update[iBody].iNumEqns[iVar] = update[iBody].iNumHecc;
       update[iBody].pdVar[iVar]    = &body[iBody].dHecc;
       update[iBody].iNumBodies[iVar] =
             malloc(update[iBody].iNumHecc * sizeof(int));
       update[iBody].iaBody[iVar] =
             malloc(update[iBody].iNumHecc * sizeof(int *));
       update[iBody].iaType[iVar] = malloc(update[iBody].iNumHecc * sizeof(int));
+      // XXX +1 allows for GR correction -- better to set iNumKecc based on user input!
       update[iBody].iaModule[iVar] =
             malloc(update[iBody].iNumHecc * sizeof(int));
 
       if (control->Evolve.iOneStep == RUNGEKUTTA) {
         control->Evolve.tmpUpdate[iBody].pdVar[iVar] =
               &control->Evolve.tmpBody[iBody].dHecc;
         control->Evolve.tmpUpdate[iBody].iNumBodies[iVar] =
@@ -1828,14 +1829,15 @@
       update[iBody].iNumEqns[iVar] = update[iBody].iNumKecc;
       update[iBody].pdVar[iVar]    = &body[iBody].dKecc;
       update[iBody].iNumBodies[iVar] =
             malloc(update[iBody].iNumKecc * sizeof(int));
       update[iBody].iaBody[iVar] =
             malloc(update[iBody].iNumKecc * sizeof(int *));
       update[iBody].iaType[iVar] = malloc(update[iBody].iNumKecc * sizeof(int));
+      // XXX +1 allows for GR correction -- better to set iNumKecc based on user input!
       update[iBody].iaModule[iVar] =
             malloc(update[iBody].iNumKecc * sizeof(int));
 
       if (control->Evolve.iOneStep == RUNGEKUTTA) {
         control->Evolve.tmpUpdate[iBody].pdVar[iVar] =
               &control->Evolve.tmpBody[iBody].dKecc;
         control->Evolve.tmpUpdate[iBody].iNumBodies[iVar] =
```

### Comparing `vplanet-2.5.4/src/verify.c` & `vplanet-2.5.5/src/verify.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/src/vplanet.c` & `vplanet-2.5.5/src/vplanet.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/custom_units.py` & `vplanet-2.5.5/vplanet/custom_units.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/log.py` & `vplanet-2.5.5/vplanet/log.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/output.py` & `vplanet-2.5.5/vplanet/output.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/quantity.py` & `vplanet-2.5.5/vplanet/quantity.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/quantity_support.py` & `vplanet-2.5.5/vplanet/quantity_support.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet/wrapper.py` & `vplanet-2.5.5/vplanet/wrapper.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.4/vplanet.egg-info/PKG-INFO` & `vplanet-2.5.5/vplanet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.4
+Version: 2.5.5
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.4 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.5 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
```

### Comparing `vplanet-2.5.4/vplanet.egg-info/SOURCES.txt` & `vplanet-2.5.5/vplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

