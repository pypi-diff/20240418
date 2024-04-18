# Comparing `tmp/PyMonCtl-0.6-py3-none-any.whl.zip` & `tmp/PyMonCtl-0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 86156 bytes, number of entries: 22
+Zip file size: 86200 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     1202 b- defN 23-Sep-14 06:28 ewmhlib/__init__.py
--rw-rw-rw-  2.0 fat   155796 b- defN 23-Sep-15 18:42 ewmhlib/_ewmhlib.py
+-rw-rw-rw-  2.0 fat   155796 b- defN 23-Sep-20 10:11 ewmhlib/_ewmhlib.py
 -rw-rw-rw-  2.0 fat      572 b- defN 23-Sep-14 06:28 ewmhlib/_main.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Aug-28 15:05 ewmhlib/py.typed
 -rw-rw-rw-  2.0 fat      204 b- defN 23-Sep-13 13:38 ewmhlib/Props/__init__.py
 -rw-rw-rw-  2.0 fat     4192 b- defN 23-Sep-13 13:39 ewmhlib/Props/_props.py
 -rw-rw-rw-  2.0 fat      129 b- defN 23-Sep-13 13:49 ewmhlib/Structs/__init__.py
 -rw-rw-rw-  2.0 fat     3844 b- defN 23-Sep-13 13:43 ewmhlib/Structs/_structs.py
--rw-rw-rw-  2.0 fat     1557 b- defN 23-Sep-15 19:56 pymonctl/__init__.py
+-rw-rw-rw-  2.0 fat     1557 b- defN 23-Sep-20 10:49 pymonctl/__init__.py
 -rw-rw-rw-  2.0 fat    24917 b- defN 23-Jun-16 12:19 pymonctl/_display_manager_lib.py
 -rw-rw-rw-  2.0 fat    32376 b- defN 23-Sep-15 22:20 pymonctl/_main.py
--rw-rw-rw-  2.0 fat    33915 b- defN 23-Sep-19 09:48 pymonctl/_pymonctl_linux.py
+-rw-rw-rw-  2.0 fat    34678 b- defN 23-Sep-20 14:57 pymonctl/_pymonctl_linux.py
 -rw-rw-rw-  2.0 fat    27716 b- defN 23-Sep-18 16:13 pymonctl/_pymonctl_macos.py
 -rw-rw-rw-  2.0 fat    41089 b- defN 23-Sep-18 16:13 pymonctl/_pymonctl_win.py
 -rw-rw-rw-  2.0 fat     8900 b- defN 23-Sep-12 16:36 pymonctl/_structs.py
 -rw-rw-rw-  2.0 fat       67 b- defN 23-May-23 09:29 pymonctl/py.typed
--rw-rw-rw-  2.0 fat      200 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/AUTHORS.txt
--rw-rw-rw-  2.0 fat     1543 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    11786 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1745 b- defN 23-Sep-19 09:48 PyMonCtl-0.6.dist-info/RECORD
-22 files, 351925 bytes uncompressed, 83364 bytes compressed:  76.3%
+-rw-rw-rw-  2.0 fat      200 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/AUTHORS.txt
+-rw-rw-rw-  2.0 fat     1543 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    11786 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1745 b- defN 23-Sep-20 14:59 PyMonCtl-0.7.dist-info/RECORD
+22 files, 352688 bytes uncompressed, 83408 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: pymonctl/_structs.py
 Comment: 
 
 Filename: pymonctl/py.typed
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/AUTHORS.txt
+Filename: PyMonCtl-0.7.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/LICENSE.txt
+Filename: PyMonCtl-0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/METADATA
+Filename: PyMonCtl-0.7.dist-info/METADATA
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/WHEEL
+Filename: PyMonCtl-0.7.dist-info/WHEEL
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/top_level.txt
+Filename: PyMonCtl-0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMonCtl-0.6.dist-info/RECORD
+Filename: PyMonCtl-0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymonctl/__init__.py

```diff
@@ -7,15 +7,15 @@
     "arrangeMonitors", "getMousePos", "version", "Monitor",
     "enableUpdateInfo", "disableUpdateInfo", "isUpdateInfoEnabled", "isWatchdogEnabled", "updateWatchdogInterval",
     "plugListenerRegister", "plugListenerUnregister", "isPlugListenerRegistered",
     "changeListenerRegister", "changeListenerUnregister", "isChangeListenerRegistered",
     "DisplayMode", "ScreenValue", "Size", "Point", "Box", "Rect", "Position", "Orientation"
 ]
 
-__version__ = "0.6"
+__version__ = "0.7"
 
 
 def version(numberOnly: bool = True) -> str:
     """Returns the current version of PyMonCtl module, in the form ''x.x.xx'' as string"""
     return ("" if numberOnly else "PyMonCtl-")+__version__
```

## pymonctl/_pymonctl_linux.py

```diff
@@ -383,54 +383,47 @@
                 rgb = str(round(value, 1))
                 gamma = rgb + ":" + rgb + ":" + rgb
                 cmd = "xrandr --output %s --gamma %s" % (self.name, gamma)
                 _ = _runProc(cmd)
 
     @property
     def mode(self) -> Optional[DisplayMode]:
-        value = None
-        cmd = "xrandr -q | grep %s -A 50 | grep '* \\|*+'" % self.name
-        ret = _runProc(cmd)
-        if ret:
-            try:
-                res = ret.split(" ")
-                lines: List[str] = list(filter(None, res))
-                w, h = lines[0].split("x")
-                r = float(lines[1].replace("+", "").replace("*", ""))
-                value = DisplayMode(int(w), int(h), r)
-            except:
-                pass
-        return value
+        for crtcData in _XgetAllCrtcs(self.name):
+            display, screen, root, res, output, outputInfo, crtc, crtcInfo = crtcData
+            if self.handle == output:
+                if outputInfo.crtc == crtc:
+                    mode = crtcInfo.mode
+                    for resMode in res.modes:
+                        if resMode.id == mode:
+                            retMode = DisplayMode(resMode.width, resMode.height,
+                                                round(resMode.dot_clock / ((resMode.h_total * resMode.v_total) or 1), 2))
+                            return retMode
+        return None
 
     def setMode(self, mode: Optional[DisplayMode]):
         # https://stackoverflow.com/questions/12706631/x11-change-resolution-and-make-window-fullscreen
         # Xlib.ext.randr.set_screen_size(defaultEwmhRoot.root, mode.width, mode.height, 0, 0)
         # Xlib.ext.randr.set_screen_config(defaultEwmhRoot.root, size_id, 0, 0, round(mode.frequency), 0)
         # Xlib.ext.randr.change_output_property()
         if mode is not None:
             cmd = "xrandr --output %s --mode %sx%s -r %s" % (self.name, mode.width, mode.height, round(mode.frequency, 2))
             _ = _runProc(cmd)
 
     @property
     def defaultMode(self) -> Optional[DisplayMode]:
-        value = None
-        cmd = "xrandr -q | grep %s -A 5 | grep ' +\\|*+'" % self.name
-        ret = _runProc(cmd)
-        if ret:
-            try:
-                res = ret.split(" ")
-                lines: List[str] = list(filter(None, res))
-                a, b = lines[0].split("x")
-                w = int(a)
-                h = int(b)
-                r = float(lines[1].replace("+", "").replace("*", ""))
-                value = DisplayMode(w, h, r)
-            except:
-                pass
-        return value
+        for outputData in _XgetAllOutputs(self.name):
+            display, screen, root, res, output, outputInfo = outputData
+            if self.handle == output:
+                for outMode in outputInfo.modes:
+                    for resMode in res.modes:
+                        if outMode == resMode.id:
+                            return DisplayMode(resMode.width, resMode.height,
+                                               round(resMode.dot_clock / ((resMode.h_total * resMode.v_total) or 1), 2))
+                break
+        return None
 
     def setDefaultMode(self):
         cmd = "xrandr --output %s --auto" % self.name
         _ = _runProc(cmd)
 
     @property
     def allModes(self) -> list[DisplayMode]:
@@ -439,15 +432,14 @@
             display, screen, root, res, output, outputInfo = outputData
             if self.handle == output:
                 for outMode in outputInfo.modes:
                     for resMode in res.modes:
                         if outMode == resMode.id:
                             modes.append(DisplayMode(resMode.width, resMode.height,
                                                      round(resMode.dot_clock / ((resMode.h_total * resMode.v_total) or 1), 2)))
-
                 break
         return modes
 
     @property
     def isPrimary(self) -> bool:
         for monitorData in _XgetAllMonitors(self.name):
             display, root, monitor, monName = monitorData
@@ -459,23 +451,24 @@
 
     def turnOn(self):
         cmd = ""
         if self.isSuspended:
             cmd = "xset dpms force on"
         elif not self.isOn:
             cmdPart = ""
+            relativeTo = self.name
             for monName in _XgetAllMonitorsNames():
                 if monName != self.name:
-                    cmdPart = " --right-of %s" % monName
-                    break
-            # cmd = ("xrandr --output %s" % self.name) + cmdPart + " --auto"
-            cmd = ("xrandr --output %s --auto" % self.name)
+                    cmdPart += " --output %s --left-of %s" % (monName, relativeTo)
+                    relativeTo = monName
+            cmd = str("xrandr --output %s --auto" % self.name) + cmdPart
         if cmd:
             _ = _runProc(cmd)
 
+
     def turnOff(self):
         if self.isOn:
             cmd = "xrandr --output %s --off" % self.name
             _ = _runProc(cmd)
 
     @property
     def isOn(self) -> Optional[bool]:
@@ -491,27 +484,36 @@
     def suspend(self):
         # xrandr has no standby option. xset doesn't allow to target just one output (it works at display level)
         cmd = "xset dpms force standby"
         _ = _runProc(cmd)
 
     @property
     def isSuspended(self) -> Optional[bool]:
-        cmd = "xset -q | grep ' Monitor is ' | awk '{ print$4 }'"
+        cmd = "xset -q | grep ' Monitor is '"
         ret = _runProc(cmd)
         if ret:
-            return bool(ret == "Standby")
+            return bool("Standby" in ret)
         return None
 
     def attach(self):
         # This produces the same effect, but requires to keep track of last mode used
         if self._crtc:
             crtc: int = self._crtc["crtc"]
             crtcInfo: Xlib.ext.randr.GetCrtcInfo = self._crtc["crtc_info"]
             randr.set_crtc_config(self.display, crtc, Xlib.X.CurrentTime, crtcInfo.x, crtcInfo.y, crtcInfo.mode, crtcInfo.rotation, crtcInfo.outputs)
             self._crtc = {}
+            cmdPart = ""
+            relativeTo = self.name
+            for monName in _XgetAllMonitorsNames():
+                if monName != self.name:
+                    cmdPart += " --output %s --left-of %s" % (monName, relativeTo)
+                    relativeTo = monName
+            cmd = str("xrandr --output %s --auto" % self.name) + cmdPart
+            _ = _runProc(cmd)
+
 
     def detach(self, permanent: bool = False):
         # This produces the same effect, but requires to keep track of last mode used
         outputs = _XgetAllOutputs(self.name)
         for outputData in outputs:
             display, screen, root, res, output, outputInfo = outputData
             if outputInfo.crtc:
@@ -741,14 +743,18 @@
         for monitorData in monitors:
             display, root, monitor, monName = monitorData
             if monitor.primary == 1 or len(monitors) == 1:
                 for outputData in outputs:
                     display, screen, root, res, output, outputInfo = outputData
                     if monName == outputInfo.name and outputInfo.crtc:
                         return display, screen, root, res, output, outputInfo.name
+    for outputData in outputs:
+        display, screen, root, res, output, outputInfo = outputData
+        if root.id == defaultEwmhRoot.root.id:
+            return display, screen, root, res, output, outputInfo.name
     return None
 
 
 def _runProc(cmd: str, timeout: int = 1):
     if timeout <= 0:
         timeout = 1
     proc = subprocess.run(cmd, text=True, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, timeout=timeout)
```

## Comparing `PyMonCtl-0.6.dist-info/LICENSE.txt` & `PyMonCtl-0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PyMonCtl-0.6.dist-info/METADATA` & `PyMonCtl-0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMonCtl
-Version: 0.6
+Version: 0.7
 Summary: Cross-Platform toolkit to get info on and control monitors connected
 Home-page: https://github.com/Kalmat/PyMonCtl
 Author: Kalmat
 Author-email: palookjones@gmail.com
 License: BSD 3
 Keywords: screen display monitor control geometry size position frequency scale orientation screen-size mouse-position
 Classifier: Development Status :: 4 - Beta
```

## Comparing `PyMonCtl-0.6.dist-info/RECORD` & `PyMonCtl-0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 ewmhlib/_ewmhlib.py,sha256=HEUSomVetXyBmw7C7d93k7ZZY2TdaCHNPujw-hm7S9c,155796
 ewmhlib/_main.py,sha256=TSAP6NdHC_aYmB3P_sWo75VMdUSY4c83jY-eXO5XsnI,572
 ewmhlib/py.typed,sha256=um_23REwXohjYnMT5p33TK57sDRgFPeuuilGTjHG47A,66
 ewmhlib/Props/__init__.py,sha256=K_x-M4CvzfzL05hSS7_MRUoGjGIVojG7f7M9-Vxi5HI,204
 ewmhlib/Props/_props.py,sha256=Fgd4zoPSaIKLMkS2BMGZM08XSGhRmuziX0f-DdPCNY4,4192
 ewmhlib/Structs/__init__.py,sha256=MJd7143A1L27u1F8Wz7roQfFDELny2zPqtfWgmx8-GI,129
 ewmhlib/Structs/_structs.py,sha256=y-FFRnIHWLdQUzS9RM4ZrvnZhYsdV3Smk5kuNpCFhhY,3844
-pymonctl/__init__.py,sha256=xaLbN3u7fA1I3-EB4BJ0Dan7D-g_OZ4fLoGd-sYYYvY,1557
+pymonctl/__init__.py,sha256=rDZL-y60d8ajQkJQV-EXuwxsSZPmko80NpuRSo3VJCo,1557
 pymonctl/_display_manager_lib.py,sha256=RNv26v7Ws4RUcA5FpUM3VOcqG_w9fCW_ViOHP_NLRxM,24917
 pymonctl/_main.py,sha256=N1rkxvC8ZokHw-ntvMAVp-dxNIGvkluOhBHFdRwWfjc,32376
-pymonctl/_pymonctl_linux.py,sha256=xKVsOvdF-jki4HTObLNq_aLfeoYf4G69LMaNEhWTdOY,33915
+pymonctl/_pymonctl_linux.py,sha256=x4hFwsvrTa8HhQJ13DN3QC7oiB67xznMC0jnprCA_xU,34678
 pymonctl/_pymonctl_macos.py,sha256=tn9IxUW7aTXCNf5PGN0GSifYeYvcmPbWeCeLM1q_nEo,27716
 pymonctl/_pymonctl_win.py,sha256=M2LZOvl7d_KrBvH_nKRY5G6J2XJIQezYuOIv9GipFhM,41089
 pymonctl/_structs.py,sha256=hJ2NPhdXnlopclKX7tHdohJPndSmQv9II2pL7X330HE,8900
 pymonctl/py.typed,sha256=ZP8cu6_5o1f0WVmLlrBtTf-U63xl66Bs1AwvdxfRYbw,67
-PyMonCtl-0.6.dist-info/AUTHORS.txt,sha256=S38i1sfZWUInPdEs9f5bVig_Sr5i7Yk6Np7aYkBqlnM,200
-PyMonCtl-0.6.dist-info/LICENSE.txt,sha256=sGfwFFlJYQhsPvAMIPC8Lb2n62iK6DOpK1ukP_8Pl1g,1543
-PyMonCtl-0.6.dist-info/METADATA,sha256=kxmczmwhq8tr19486tPwUxu2T9OiQOBsfR-lv9Yz_dI,11786
-PyMonCtl-0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyMonCtl-0.6.dist-info/top_level.txt,sha256=ISZRWgRKlonHlJZ6kweAq8F6Kbgy8-dwRcGnuGwWKHM,17
-PyMonCtl-0.6.dist-info/RECORD,,
+PyMonCtl-0.7.dist-info/AUTHORS.txt,sha256=S38i1sfZWUInPdEs9f5bVig_Sr5i7Yk6Np7aYkBqlnM,200
+PyMonCtl-0.7.dist-info/LICENSE.txt,sha256=sGfwFFlJYQhsPvAMIPC8Lb2n62iK6DOpK1ukP_8Pl1g,1543
+PyMonCtl-0.7.dist-info/METADATA,sha256=_04lxSOeyk2Fc3ZI-V6y6jC6o-90n4ZB8fcKQTcXsgU,11786
+PyMonCtl-0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PyMonCtl-0.7.dist-info/top_level.txt,sha256=ISZRWgRKlonHlJZ6kweAq8F6Kbgy8-dwRcGnuGwWKHM,17
+PyMonCtl-0.7.dist-info/RECORD,,
```

