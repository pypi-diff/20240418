# Comparing `tmp/sdss_cherno-0.6.8.tar.gz` & `tmp/sdss_cherno-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.6.8.tar", max compression
+gzip compressed data, was "sdss_cherno-0.6.9.tar", max compression
```

## Comparing `sdss_cherno-0.6.8.tar` & `sdss_cherno-0.6.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1504 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/LICENSE.md
--rw-r--r--   0        0        0     2723 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/README.md
--rw-r--r--   0        0        0     1251 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/__init__.py
--rw-r--r--   0        0        0     2188 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/__main__.py
--rw-r--r--   0        0        0      747 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4729 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/config.py
--rw-r--r--   0        0        0     8213 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1008 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3511 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10858 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2024-02-27 20:05:46.912063 sdss_cherno-0.6.8/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     2180 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     2145 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     5688 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/extraction.py
--rw-r--r--   0        0        0    42715 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/guider.py
--rw-r--r--   0        0        0     4175 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/maskbits.py
--rw-r--r--   0        0        0     4738 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2024-02-27 20:05:46.916063 sdss_cherno-0.6.8/cherno/utils.py
--rw-r--r--   0        0        0     2476 2024-02-27 20:05:46.920063 sdss_cherno-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 sdss_cherno-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/LICENSE.md
+-rw-r--r--   0        0        0     2723 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/README.md
+-rw-r--r--   0        0        0     1251 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/__init__.py
+-rw-r--r--   0        0        0     2188 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     4729 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0    10565 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1008 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3511 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10858 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     2210 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     2145 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/exceptions.py
+-rw-r--r--   0        0        0    14028 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/extraction.py
+-rw-r--r--   0        0        0    42948 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/utils.py
+-rw-r--r--   0        0        0     2476 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 sdss_cherno-0.6.9/PKG-INFO
```

### Comparing `sdss_cherno-0.6.8/LICENSE.md` & `sdss_cherno-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/README.md` & `sdss_cherno-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/__init__.py` & `sdss_cherno-0.6.9/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/__main__.py` & `sdss_cherno-0.6.9/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/__init__.py` & `sdss_cherno-0.6.9/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/actor.py` & `sdss_cherno-0.6.9/cherno/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/acquire.py` & `sdss_cherno-0.6.9/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/config.py` & `sdss_cherno-0.6.9/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/guide.py` & `sdss_cherno-0.6.9/cherno/actor/commands/guide.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # @Filename: guide.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
 from contextlib import suppress
-from functools import partial
 from types import SimpleNamespace
 
 from typing import Callable
 
 import click
 
 from cherno import config
@@ -42,14 +41,25 @@
         click.Option(
             ["--exposure-time", "-t"],
             type=float,
             default=None,
             help="Cameras exposure time.",
         ),
         click.Option(
+            ["--max-exposure-time", "-T"],
+            type=float,
+            default=30,
+            help="Maximum exposure time.",
+        ),
+        click.Option(
+            ["--dynamic-exposure-time", "-d"],
+            is_flag=True,
+            help="Increases the exposure time dynamically if failed to solve.",
+        ),
+        click.Option(
             ["--cameras", "-m"],
             type=str,
             help="Comma-separated cameras to expose.",
         ),
         click.Option(
             ["--count", "-n"],
             type=int,
@@ -80,15 +90,15 @@
             "-1 disables this feature and a full fit is allways performed.",
         ),
         click.Option(
             ["--wait", "-w"],
             type=float,
             default=15 if config["observatory"] == "LCO" else None,
             show_default=True,
-            help="Time to wait between iterations.",
+            help="Time to wait between iterations. Only applies to LCO.",
         ),
         click.Option(
             ["--mode"],
             type=click.Choice(
                 ["hybrid", "astrometrynet", "gaia"],
                 case_sensitive=False,
             ),
@@ -126,14 +136,16 @@
 
     return sorted(options, key=lambda opt: opt.name or "")
 
 
 class GuideParams(SimpleNamespace):
     command: ChernoCommandType
     exposure_time: float | None = None
+    max_exposure_time: float = 30.0
+    dynamic_exposure_time: bool = False
     continuous: bool = False
     count: int | None = None
     apply: bool = True
     full: bool = False
     only_radec: bool = False
     auto_radec_min: int = config["guider"]["auto_radec_min"]
     cameras: str | None = None
@@ -199,28 +211,68 @@
     guider = Guider(
         config["observatory"],
         target_rms=target_rms,
         command=params.command,
     )
     params.command.actor.state._guider_obj = guider  # To update PID coeffs.
 
-    return partial(
-        guider.process,
-        correct=params.apply,
-        full_correction=params.full,
-        wait_for_correction=(params.wait is None),
-        only_radec=params.only_radec,
-        auto_radec_min=params.auto_radec_min,
-        gaia_phot_g_mean_mag_max=params.gaia_max_mag,
-        gaia_cross_correlation_blur=params.cross_match_blur,
-        fit_all_detections=params.fit_all_detections,
-        plot=params.plot,
-        fit_focus=config["guider"].get("fit_focus", True),
-        **params.mode_kwargs,
-    )
+    async def process_callback(command: ChernoCommandType, images: list[str]):
+        ast_solution = await guider.process(
+            command,
+            images,
+            correct=params.apply,
+            full_correction=params.full,
+            offset=None,
+            wait_for_correction=False,  # This only applies to LCO.
+            only_radec=params.only_radec,
+            auto_radec_min=params.auto_radec_min,
+            gaia_phot_g_mean_mag_max=params.gaia_max_mag,
+            gaia_cross_correlation_blur=params.cross_match_blur,
+            fit_all_detections=params.fit_all_detections,
+            plot=params.plot,
+            fit_focus=config["guider"].get("fit_focus", True),
+            **params.mode_kwargs,
+        )
+
+        if params.dynamic_exposure_time:
+            max_exposure_time = params.max_exposure_time or 30.0
+            current_exposure_time = command.actor.state.exposure_time
+            if current_exposure_time >= max_exposure_time:
+                # This should only happen if the observer manually set the
+                # exposure time, in which case we accept it.
+                new_exposure_time = current_exposure_time
+            elif not ast_solution.valid_solution:
+                new_exposure_time = min(current_exposure_time * 2, max_exposure_time)
+            elif ast_solution.n_solved < 4:
+                new_exposure_time = max(current_exposure_time * 1.5, max_exposure_time)
+            else:
+                new_exposure_time = current_exposure_time
+
+            if new_exposure_time != round(current_exposure_time, 1):
+                command.actor.state.exposure_time = new_exposure_time
+                command.info(f"Exposure time updated to {new_exposure_time:.1f} s.")
+
+        if command.actor.observatory == "LCO":
+            rot_correction = ast_solution.correction_applied[2]
+            if abs(rot_correction) > 0:
+                # Do not add a delay if we applied a rotator correction. The
+                # rotator blocks until done, which means the RA/Dec corrections
+                # will probably have converged as well.
+                pass
+            elif (
+                any(ast_solution.correction_applied)
+                and params.wait is not None
+                and params.wait > 0.0
+            ):
+                command.debug(f"Waiting {params.wait:.1f} s for corrections.")
+                await asyncio.sleep(params.wait)
+
+        return ast_solution
+
+    return process_callback
 
 
 async def _guide(
     params: GuideParams,
     stop_condition: Callable[[], bool] | None = None,
     target_rms: float | None = None,
     max_iterations: int | None = None,
@@ -239,15 +291,15 @@
     command.actor.state._exposure_loop = asyncio.create_task(
         exposer.loop(
             None,
             count=params.count if params.continuous is False else None,
             max_iterations=max_iterations,
             timeout=25,
             names=params.names,
-            delay=params.wait or 0.0,
+            delay=0.0,
             stop_condition=stop_condition,
         )
     )
 
     try:
         await command.actor.state._exposure_loop
     except ExposerError as err:
```

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/offset.py` & `sdss_cherno-0.6.9/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/reprocess.py` & `sdss_cherno-0.6.9/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/scale.py` & `sdss_cherno-0.6.9/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/set.py` & `sdss_cherno-0.6.9/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/show.py` & `sdss_cherno-0.6.9/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/status.py` & `sdss_cherno-0.6.9/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/stop.py` & `sdss_cherno-0.6.9/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/commands/version.py` & `sdss_cherno-0.6.9/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/actor/exposer.py` & `sdss_cherno-0.6.9/cherno/actor/exposer.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/etc/cherno_APO.yml` & `sdss_cherno-0.6.9/cherno/etc/cherno_APO.yml`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,21 @@
 
 focus_sensitivity: 5.94
 
 guide_loop:
   ra:
     pid:
       k: 0.7
+      ti: 0.01
     min_correction: 0.05
     max_correction: 600
   dec:
     pid:
       k: 0.7
+      ti: 0.01
     min_correction: 0.05
     max_correction: 600
   rot:
     pid:
       k: 0.6
     min_correction: 3
     max_correction: 7200
```

### Comparing `sdss_cherno-0.6.8/cherno/etc/cherno_LCO.yml` & `sdss_cherno-0.6.9/cherno/etc/cherno_LCO.yml`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/etc/schema.json` & `sdss_cherno-0.6.9/cherno/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/exceptions.py` & `sdss_cherno-0.6.9/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/extraction.py` & `sdss_cherno-0.6.9/cherno/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/guider.py` & `sdss_cherno-0.6.9/cherno/guider.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,20 @@
     fwhm_median: float = -999.0
     fwhm_fit: float = -999.0
     focus_coeff: list[float] = field(default_factory=lambda: [-999.0] * 3)
     focus_r2: float = -999.0
     camera_rotation: float = -999.0
     correction_applied: list[float] = field(default_factory=lambda: [0.0] * 5)
 
+    @property
+    def n_solved(self):
+        """Returns the number of solved cameras."""
+
+        return len([gd for gd in self.guide_data if gd.solved])
+
 
 class AxesPID:
     """Store for the axis PID coefficient."""
 
     def __init__(self, actor: ChernoActor | None = None):
         self.actor = actor
 
@@ -504,19 +510,20 @@
             if guider_fit.only_radec:
                 ast_solution.fit_mode = "radec"
 
             # Report fit RMS. First value is the global fit RMS, then one for
             # each camera and a boolean indicating if that camera was used for the
             # global fit. If a camera was rejected the fit RMS is set to -999.
             fit_rms = guider_fit.fit_rms
-            fit_rms_camera = [numpy.round(fit_rms.loc[0].rms * mm_to_arcsec, 4)]
+            fit_rms_global = float(numpy.round(fit_rms.loc[0].rms * mm_to_arcsec, 4))
+            fit_rms_camera: list[int | float] = [fit_rms_global]
             for cid in range(1, 7):
                 if cid in fit_rms.index:
                     this_fit_rms = numpy.round(fit_rms.loc[cid].rms * mm_to_arcsec, 4)
-                    fit_rms_camera.append(this_fit_rms)
+                    fit_rms_camera.append(float(this_fit_rms))
                 else:
                     fit_rms_camera.append(-999.0)
                 fit_rms_camera.append(cid in guider_fit.cameras)
 
             self.command.info(fit_rms_camera=fit_rms_camera)
 
             # If the fit_rms of all the fit cameras is greater than a certain
```

### Comparing `sdss_cherno-0.6.8/cherno/lcotcc.py` & `sdss_cherno-0.6.9/cherno/lcotcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/maskbits.py` & `sdss_cherno-0.6.9/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/tcc.py` & `sdss_cherno-0.6.9/cherno/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/cherno/utils.py` & `sdss_cherno-0.6.9/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.8/pyproject.toml` & `sdss_cherno-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.6.8"
+version = "0.6.9"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
```

### Comparing `sdss_cherno-0.6.8/PKG-INFO` & `sdss_cherno-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.6.8
+Version: 0.6.9
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
```

