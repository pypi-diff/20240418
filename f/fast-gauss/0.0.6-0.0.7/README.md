# Comparing `tmp/fast_gauss-0.0.6.tar.gz` & `tmp/fast_gauss-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gauss-0.0.6.tar", last modified: Fri Apr 12 07:52:37 2024, max compression
+gzip compressed data, was "fast_gauss-0.0.7.tar", last modified: Thu Apr 18 06:26:01 2024, max compression
```

## Comparing `fast_gauss-0.0.6.tar` & `fast_gauss-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/base_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26294 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/console_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/cuda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/egl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gaussian_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/gsplat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/sh_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss/shaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.frag
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.geom
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/fast_gauss/shaders/gsplat.vert
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/fast_gauss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 07:52:37.000000 fast_gauss-0.0.6/fast_gauss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/license
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:52:28.000000 fast_gauss-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:52:37.731333 fast_gauss-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/fast_gauss/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26525 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/console_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/cuda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19045 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/egl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/gaussian_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/gl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/gsplat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/sh_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/fast_gauss/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/shaders/gsplat.frag
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/shaders/gsplat.geom
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/fast_gauss/shaders/gsplat.vert
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/fast_gauss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-18 06:26:01.000000 fast_gauss-0.0.7/fast_gauss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 06:26:01.000000 fast_gauss-0.0.7/fast_gauss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:26:01.000000 fast_gauss-0.0.7/fast_gauss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 06:26:01.000000 fast_gauss-0.0.7/fast_gauss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 06:26:01.000000 fast_gauss-0.0.7/fast_gauss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/license
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:25:55.000000 fast_gauss-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:26:01.083616 fast_gauss-0.0.7/setup.cfg
```

### Comparing `fast_gauss-0.0.6/PKG-INFO` & `fast_gauss-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: fast_gauss
-Version: 0.0.6
+Version: 0.0.7
 Summary: A geometry-shader-based, global CUDA sorted high-performance 3D Gaussian Splatting rasterizer. Can achieve a 5-10x speedup in rendering compared to the vanialla diff-gaussian-rasterization.
 Author: Zhen Xu
 Author-email: zhenx@zju.edu.cn
-License: Copyright 2022-2023 3D Vision Group at the State Key Lab of CAD&CG,  
+License: Copyright 2022-2024 3D Vision Group at the State Key Lab of CAD&CG,  
         Zhejiang University. All Rights Reserved. 
         
-        For more information see <https://github.com/dendenxu/fast-gaussian-splatting> 
+        For more information see <https://github.com/dendenxu/fast-gaussian-rasterization> 
         If you use this software, please cite the corresponding publications   
         listed on the above website. 
         
         Permission to use, copy, modify and distribute this software and its 
         documentation for educational, research and non-profit purposes only. 
         Any modification based on this work must be open-source and prohibited 
         for commercial use. 
         You must retain, in the source form of any derivative works that you  
         distribute, all copyright, patent, trademark, and attribution notices  
         from the source form of this work. 
          
         For commercial uses of this software, please send email to xwzhou@zju.edu.cn
+        
 Project-URL: homepage, https://github.com/dendenxu/fast-gaussian-rasterization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: cuda-python
 Requires-Dist: PyGLM
-Requires-Dist: PyOpenGL
+Requires-Dist: PyOpenGL>=3.1.7
 
 # Fast Gaussian Rasterization
 
 - **Can be 5-10x faster than the original software CUDA rasterizer ([diff-gaussian-rasterization](https://github.com/graphdeco-inria/diff-gaussian-rasterization)).**
 - **Can be 2-3x faster if using offline rendering. (Bottleneck: copying rendered images around, thinking about improvements.)**
 - **Speedup most visible with high pixel-to-point ratio (large Gaussians, small point count, high-res rendering).**
```

### Comparing `fast_gauss-0.0.6/fast_gauss/__init__.py` & `fast_gauss-0.0.7/fast_gauss/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch import nn
-from typing import NamedTuple
+from typing import NamedTuple, List, Dict
 
 from .gsplat_utils import GSplatContextManager
 
 raster_context = None
 
 
 class GaussianRasterizationSettings(NamedTuple):
@@ -19,21 +19,28 @@
     sh_degree: int
     campos: torch.Tensor
     prefiltered: bool
     debug: bool
 
 
 class GaussianRasterizer:
-    def __init__(self, raster_settings: GaussianRasterizationSettings, dtype=torch.float, tex_dtype=torch.half):
+    def __init__(self,
+                 raster_settings: GaussianRasterizationSettings,
+                 init_buffer_size: int = 32768,
+                 init_texture_size: List[int] = [512, 512],
+                 dtype=torch.float,
+                 tex_dtype=torch.half):
         super().__init__()
         self.raster_settings = raster_settings
 
         global raster_context
+        dtype = getattr(torch, dtype) if isinstance(dtype, str) else dtype
+        tex_dtype = getattr(torch, tex_dtype) if isinstance(tex_dtype, str) else tex_dtype
         if raster_context is None or raster_context.dtype != dtype or raster_context.tex_dtype != tex_dtype:
-            raster_context = GSplatContextManager(dtype=dtype, tex_dtype=tex_dtype)  # only created once
+            raster_context = GSplatContextManager(init_buffer_size=init_buffer_size, init_texture_size=init_texture_size, dtype=dtype, tex_dtype=tex_dtype)  # only created once
 
     def __call__(self,
                  means3D: torch.Tensor,
                  means2D: torch.Tensor,  # only to match the api, can be none, not used
                  opacities: torch.Tensor,
                  shs: torch.Tensor = None,
                  colors_precomp: torch.Tensor = None,
```

### Comparing `fast_gauss-0.0.6/fast_gauss/base_utils.py` & `fast_gauss-0.0.7/fast_gauss/base_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/console_utils.py` & `fast_gauss-0.0.7/fast_gauss/console_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,25 +96,33 @@
         return buf.getvalue().decode(encoding='utf-8', errors='strict')[:-1]  # remove \n
 
 
 yaml = MyYAML()
 yaml.default_flow_style = None
 
 warnings.filterwarnings("ignore")  # ignore disturbing warnings
-os.environ["PYTHONBREAKPOINT"] = "easyvolcap.utils.console_utils.set_trace"
+os.environ["PYTHONBREAKPOINT"] = "fast_gauss.console_utils.set_trace"
 
 slim_width = None
 verbose_width = None
 slim_log_time = True
 slim_log_path = True
 slim_time_format = '%H:%M:%S'
 # slim_time_format = ''
 verbose_time_format = '%Y-%m-%d %H:%M:%S.%f'
-do_nothing_console = Console(file=StringIO(), stderr=StringIO())
-console = Console(soft_wrap=True, tab_size=4, log_time_format=slim_time_format, width=slim_width, log_time=slim_log_time, log_path=slim_log_path)  # shared
+
+# fmt: off
+if 'easyvolcap.utils.console_utils' in sys.modules:
+    console = sys.modules['easyvolcap.utils.console_utils'].console
+    do_nothing_console = sys.modules['easyvolcap.utils.console_utils'].do_nothing_console
+else:
+    do_nothing_console = Console(file=StringIO(), stderr=StringIO())
+    console = Console(soft_wrap=True, tab_size=4, log_time_format=slim_time_format, width=slim_width, log_time=slim_log_time, log_path=slim_log_path)
+# fmt: on
+
 progress = Progress(console=console, expand=True)  # destroyed
 live = Live(console=console, refresh_per_second=10)  # destroyed
 traceback.install(console=console, width=slim_width)  # for colorful tracebacks
 pretty.install(console=console)
 
 NoneType = type(None)
```

### Comparing `fast_gauss-0.0.6/fast_gauss/cuda_utils.py` & `fast_gauss-0.0.7/fast_gauss/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/data_utils.py` & `fast_gauss-0.0.7/fast_gauss/data_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/egl_utils.py` & `fast_gauss-0.0.7/fast_gauss/egl_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/gaussian_utils.py` & `fast_gauss-0.0.7/fast_gauss/gaussian_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/gl_utils.py` & `fast_gauss-0.0.7/fast_gauss/gl_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/gsplat_utils.py` & `fast_gauss-0.0.7/fast_gauss/gsplat_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.resize_buffers(init_buffer_size)
         self.resize_textures(*init_texture_size)
 
         log(green_slim(f'GSplatContextManager initialized with attribute dtype: {self.dtype}, texture dtype: {self.tex_dtype}, offline rendering: {self.offline_rendering}, buffer size: {init_buffer_size}, texture size: {init_texture_size}'))
 
         if not self.offline_rendering:
             log(green_slim('Using online rendering mode, in this mode, calling the rendering function of fast_gauss will write directly to the currently bound framebuffer'))
-            log(green_slim('In this mode, the output of all rasterization calls will be None (same output count). Please do not perform further processing on them.'))
+            log(green_slim('In this mode, the output of all rasterization calls will be None (same output count). Please do not perform further processing on them'))
             log(green_slim('Please make sure to set up the correct GUI environment before calling the rasterization function, see more in readme.md'))
 
     def opengl_options(self):
         # Performs face culling
         gl.glDisable(gl.GL_CULL_FACE)
 
         # Performs z-buffer testing
@@ -208,25 +208,29 @@
         gl.glBindFramebuffer(gl.GL_FRAMEBUFFER, 0)
 
         # Register image to read from
         flags = cudart.cudaGraphicsRegisterFlags.cudaGraphicsRegisterFlagsReadOnly
         self.cu_tex = CHECK_CUDART_ERROR(cudart.cudaGraphicsGLRegisterImage(self.tex_rgba, gl.GL_TEXTURE_2D, flags))
 
     def resize_textures(self, H: int, W: int):  # analogy to update_gl_buffers
-        if not hasattr(self, 'max_H'): self.max_H = 0
-        if not hasattr(self, 'max_W'): self.max_W = 0
+        init = False
+        if not hasattr(self, 'max_H'): self.max_H = 0; init = True
+        if not hasattr(self, 'max_W'): self.max_W = 0; init = True
         if H > self.max_H or W > self.max_W:  # max got updated
             if H > self.max_H: self.max_H = int(H * 1.05)
             if W > self.max_W: self.max_W = int(W * 1.05)
+            if not init: log(green_slim('Resizing textures to:'), int(H), int(W))
             self.init_textures(self.max_H, self.max_W)
 
     def resize_buffers(self, v: int = 0):
-        if not hasattr(self, 'max_verts'): self.max_verts = 0
+        init = False
+        if not hasattr(self, 'max_verts'): self.max_verts = 0; init = True;
         if v > self.max_verts:
             if v > self.max_verts: self.max_verts = int(v * 1.05)
+            if not init: log(green_slim('Resizing buffers to:'), int(v))
             self.init_gl_buffers(self.max_verts)
 
     @torch.no_grad()
     def render(self, xyz3: torch.Tensor, cov6: torch.Tensor, rgb3: torch.Tensor, occ1: torch.Tensor, raster_settings: 'GaussianRasterizationSettings'):
         if xyz3.dtype != self.dtype:
             warn_once(yellow(f'Input tensors has dtype {xyz3.dtype}, expected {self.dtype}, will cast to {self.dtype}'))
             xyz3, cov6, rgb3, occ1 = xyz3.to(self.dtype), cov6.to(self.dtype), rgb3.to(self.dtype), occ1.to(self.dtype)
```

### Comparing `fast_gauss-0.0.6/fast_gauss/math_utils.py` & `fast_gauss-0.0.7/fast_gauss/math_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/sh_utils.py` & `fast_gauss-0.0.7/fast_gauss/sh_utils.py`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.frag` & `fast_gauss-0.0.7/fast_gauss/shaders/gsplat.frag`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.geom` & `fast_gauss-0.0.7/fast_gauss/shaders/gsplat.geom`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss/shaders/gsplat.vert` & `fast_gauss-0.0.7/fast_gauss/shaders/gsplat.vert`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/fast_gauss.egg-info/PKG-INFO` & `fast_gauss-0.0.7/fast_gauss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: fast_gauss
-Version: 0.0.6
+Version: 0.0.7
 Summary: A geometry-shader-based, global CUDA sorted high-performance 3D Gaussian Splatting rasterizer. Can achieve a 5-10x speedup in rendering compared to the vanialla diff-gaussian-rasterization.
 Author: Zhen Xu
 Author-email: zhenx@zju.edu.cn
-License: Copyright 2022-2023 3D Vision Group at the State Key Lab of CAD&CG,  
+License: Copyright 2022-2024 3D Vision Group at the State Key Lab of CAD&CG,  
         Zhejiang University. All Rights Reserved. 
         
-        For more information see <https://github.com/dendenxu/fast-gaussian-splatting> 
+        For more information see <https://github.com/dendenxu/fast-gaussian-rasterization> 
         If you use this software, please cite the corresponding publications   
         listed on the above website. 
         
         Permission to use, copy, modify and distribute this software and its 
         documentation for educational, research and non-profit purposes only. 
         Any modification based on this work must be open-source and prohibited 
         for commercial use. 
         You must retain, in the source form of any derivative works that you  
         distribute, all copyright, patent, trademark, and attribution notices  
         from the source form of this work. 
          
         For commercial uses of this software, please send email to xwzhou@zju.edu.cn
+        
 Project-URL: homepage, https://github.com/dendenxu/fast-gaussian-rasterization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: cuda-python
 Requires-Dist: PyGLM
-Requires-Dist: PyOpenGL
+Requires-Dist: PyOpenGL>=3.1.7
 
 # Fast Gaussian Rasterization
 
 - **Can be 5-10x faster than the original software CUDA rasterizer ([diff-gaussian-rasterization](https://github.com/graphdeco-inria/diff-gaussian-rasterization)).**
 - **Can be 2-3x faster if using offline rendering. (Bottleneck: copying rendered images around, thinking about improvements.)**
 - **Speedup most visible with high pixel-to-point ratio (large Gaussians, small point count, high-res rendering).**
```

### Comparing `fast_gauss-0.0.6/fast_gauss.egg-info/SOURCES.txt` & `fast_gauss-0.0.7/fast_gauss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_gauss-0.0.6/license` & `fast_gauss-0.0.7/license`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Copyright 2022-2023 3D Vision Group at the State Key Lab of CAD&CG,  
+Copyright 2022-2024 3D Vision Group at the State Key Lab of CAD&CG,  
 Zhejiang University. All Rights Reserved. 
 
-For more information see <https://github.com/dendenxu/fast-gaussian-splatting> 
+For more information see <https://github.com/dendenxu/fast-gaussian-rasterization> 
 If you use this software, please cite the corresponding publications   
 listed on the above website. 
 
 Permission to use, copy, modify and distribute this software and its 
 documentation for educational, research and non-profit purposes only. 
 Any modification based on this work must be open-source and prohibited 
 for commercial use. 
 You must retain, in the source form of any derivative works that you  
 distribute, all copyright, patent, trademark, and attribution notices  
 from the source form of this work. 
  
-For commercial uses of this software, please send email to xwzhou@zju.edu.cn
+For commercial uses of this software, please send email to xwzhou@zju.edu.cn
```

### Comparing `fast_gauss-0.0.6/pyproject.toml` & `fast_gauss-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_gauss"
-version = "0.0.6"
+version = "0.0.7"
 description = "A geometry-shader-based, global CUDA sorted high-performance 3D Gaussian Splatting rasterizer. Can achieve a 5-10x speedup in rendering compared to the vanialla diff-gaussian-rasterization."
 readme = "readme.md"
 license = { file = "license" }
 authors = [{ email = "zhenx@zju.edu.cn" }, { name = "Zhen Xu" }]
 requires-python = ">=3.9"
 dynamic = ["dependencies"]
```

### Comparing `fast_gauss-0.0.6/readme.md` & `fast_gauss-0.0.7/readme.md`

 * *Files identical despite different names*

