# Comparing `tmp/bbo-calibcamlib-0.3.5.tar.gz` & `tmp/bbo-calibcamlib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-calibcamlib-0.3.5.tar", last modified: Thu Feb  9 08:09:22 2023, max compression
+gzip compressed data, was "bbo-calibcamlib-0.3.7.tar", last modified: Thu Apr 18 13:33:56 2024, max compression
```

## Comparing `bbo-calibcamlib-0.3.5.tar` & `bbo-calibcamlib-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/
--rw-rw-r--   0 voit     (86501) voit     (86501)    35149 2022-06-21 07:05:21.000000 bbo-calibcamlib-0.3.5/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)      675 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)       65 2022-06-21 07:05:22.000000 bbo-calibcamlib-0.3.5/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)      675 2023-02-09 08:09:22.000000 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      463 2023-02-09 08:09:22.000000 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-02-09 08:09:22.000000 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       12 2023-02-09 08:09:22.000000 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       12 2023-02-09 08:09:22.000000 bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/top_level.txt
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/calibcamlib/
--rw-rw-r--   0 voit     (86501) voit     (86501)      191 2022-10-27 07:43:56.000000 bbo-calibcamlib-0.3.5/calibcamlib/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1836 2023-02-09 08:08:27.000000 bbo-calibcamlib-0.3.5/calibcamlib/camera.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     9350 2023-01-30 12:35:35.000000 bbo-calibcamlib-0.3.5/calibcamlib/camerasystem.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      408 2022-10-27 08:15:10.000000 bbo-calibcamlib-0.3.5/calibcamlib/dist_MaEtAl2003_model0.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      621 2022-10-27 07:43:56.000000 bbo-calibcamlib-0.3.5/calibcamlib/dist_MaEtAl2003_model3.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2176 2023-02-09 07:38:28.000000 bbo-calibcamlib-0.3.5/calibcamlib/dist_OpenCV.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1282 2022-06-21 07:05:22.000000 bbo-calibcamlib-0.3.5/calibcamlib/helper.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1023 2023-02-09 08:08:51.000000 bbo-calibcamlib-0.3.5/setup.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-09 08:09:22.110631 bbo-calibcamlib-0.3.5/test/
--rw-rw-r--   0 voit     (86501) voit     (86501)     3853 2023-01-27 08:40:16.000000 bbo-calibcamlib-0.3.5/test/test_camera.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     4688 2023-02-09 07:38:56.000000 bbo-calibcamlib-0.3.5/test/test_distortion.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    35149 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)      675 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)       65 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)      675 2024-04-18 13:33:56.000000 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      516 2024-04-18 13:33:56.000000 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-04-18 13:33:56.000000 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       19 2024-04-18 13:33:56.000000 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       12 2024-04-18 13:33:56.000000 bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/top_level.txt
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/calibcamlib/
+-rw-rw-r--   0 voit     (86501) voit     (86501)      191 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/calibcamlib/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1836 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/calibcamlib/camera.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)    10686 2024-04-16 08:52:52.000000 bbo-calibcamlib-0.3.7/calibcamlib/camerasystem.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      408 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/calibcamlib/dist_MaEtAl2003_model0.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      621 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/calibcamlib/dist_MaEtAl2003_model3.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2180 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/calibcamlib/dist_OpenCV.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1891 2024-03-11 13:51:02.000000 bbo-calibcamlib-0.3.7/calibcamlib/helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1798 2024-04-03 12:41:22.000000 bbo-calibcamlib-0.3.7/calibcamlib/yaml_helper.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1033 2024-04-18 13:33:38.000000 bbo-calibcamlib-0.3.7/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:33:56.571788 bbo-calibcamlib-0.3.7/test/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4250 2024-03-11 13:51:02.000000 bbo-calibcamlib-0.3.7/test/test_camera.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      474 2024-03-11 13:51:02.000000 bbo-calibcamlib-0.3.7/test/test_camerasystem.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4688 2023-11-13 15:21:50.000000 bbo-calibcamlib-0.3.7/test/test_distortion.py
```

### Comparing `bbo-calibcamlib-0.3.5/LICENSE` & `bbo-calibcamlib-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-calibcamlib-0.3.5/PKG-INFO` & `bbo-calibcamlib-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcamlib
-Version: 0.3.5
+Version: 0.3.7
 Summary: Library to work with calibration from bbo-calibcam
 Home-page: https://github.com/bbo-lab/calibcamlib
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcamlib-0.3.5/bbo_calibcamlib.egg-info/PKG-INFO` & `bbo-calibcamlib-0.3.7/bbo_calibcamlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-calibcamlib
-Version: 0.3.5
+Version: 0.3.7
 Summary: Library to work with calibration from bbo-calibcam
 Home-page: https://github.com/bbo-lab/calibcamlib
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-calibcamlib-0.3.5/calibcamlib/camera.py` & `bbo-calibcamlib-0.3.7/calibcamlib/camera.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcamlib-0.3.5/calibcamlib/camerasystem.py` & `bbo-calibcamlib-0.3.7/calibcamlib/camerasystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import numpy as np
 from scipy.spatial.transform import Rotation as R
+from scipy.optimize import least_squares
+import yaml
 from calibcamlib import Camera
 from calibcamlib.helper import intersect, get_line_dist
+from calibcamlib.yaml_helper import collection_to_array
 
 
 # R,t are world->cam
 class Camerasystem:
     def __init__(self):
         self.cameras = list()
 
@@ -88,23 +91,48 @@
 
         for i, Xp in enumerate(X):
             if np.sum(~np.isnan(V[:, i, 1])) > 1:
                 X[i] = intersect(P[:, i, :], V[:, i, :]).T
 
         return X.reshape(x_shape[1:-1] + (3,))
 
-    def triangulate(self, x, offsets):
+    def triangulate_repro(self, x, offsets=None):
+        X = self.triangulate_3derr(x, offsets)
+
+        x_shape = x.shape
+        x = x.reshape((x_shape[0], -1, 2))
+        X = X.reshape(-1, 3)
+
+        for i_point in range(x.shape[1]):
+            if np.any(np.isnan(X[i_point])):
+                X[i_point] = np.nan
+            else:
+                res = least_squares(self.repro_error, X[i_point],
+                              method='lm',
+                              verbose=0,
+                              args=[x[:,i_point]],
+                              kwargs={'offsets': offsets, "ravel": True, "nan_to_zero": True})
+                X[i_point] = res.x
+
+        return X.reshape(x_shape[1:-1] + (3,))
+
+    def repro_error(self, X, x_orig, offsets=None, ravel=False, nan_to_zero=False):
+        err = self.project(X, offsets)-x_orig
+        if nan_to_zero:
+            err[np.isnan(err)] = 0
+        if ravel:
+            err = err.ravel()
+        return err
+
+    def triangulate(self, x, offsets=None):
         # Triangulate image coordinates in shape np.array((N_CAMS, ..., 2)).
         # Returns 3d points np.array((..., 3)) in world coordinates.
-        # TODO: Implement triangulation by reprojection error (minimizing distance of original and reprojected image coordinates)
-        #  This will be changed to reprojection error in the future!
-        #  Use this function only if that is desired, else use triangulate_3derr
-        return self.triangulate_3derr(x, offsets)
+        return self.triangulate_repro(x, offsets)
 
-    def triangulate_nopointcorr(self, AB, offsets, linedist_thres, max_points=12):
+    def triangulate_nopointcorr(self, AB, offsets=None, linedist_thres=0.2, discard_ambiguities=True, max_points=12):
         # Tries to triangulate image coordinates in shape np.array((N_CAMS, M, 2)) even if image coordinate order does
         # not match between cameras, i.e. AB is shuffled in the second dimension for each camera independently.
         # linedist_thres: distance between camera lines that is still counted as a correspondance
         # max_points: limits number of points on which this is tried
         # Returns 3d points np.array((..., 3)) in world coordinates.
         n_AB = np.array([ab.shape[0] for ab in AB])
         if np.sum(n_AB > 0) < 2:
@@ -140,20 +168,21 @@
 
             cam_bases[iC] = cb[0]
 
             distances = np.array([[get_line_dist(cam_bases[main_cam_idx], full_dirs[main_cam_idx, i, :], cam_bases[iC],
                                                  dirs[j]) for j in range(dirs.shape[0])] for i in
                                   range(full_dirs.shape[1])])
 
-            np.equal(distances, np.min(distances, axis=0)[np.newaxis, :])
             connectmat = np.all([distances < linedist_thres,
                                  np.equal(distances, np.min(distances, axis=1)[:, np.newaxis]),
                                  # np.equal(distances,np.min(distances,axis=0)[np.newaxis,:])
                                  ], axis=0)
-            connectmat[:, np.sum(connectmat, axis=0) > 1] = False  # Discard ambiguities
+            if discard_ambiguities:
+                connectmat[:, np.sum(connectmat, axis=0) > 1] = False  # Discard ambiguities
+
             corrs = np.array(np.where(connectmat))
 
             if corrs.shape[1] == 0:
                 continue
 
             full_ab[iC, corrs[0], :] = ab[corrs[1]]
             # print(full_ab[iC])
@@ -163,14 +192,29 @@
 
         points = np.array([intersect(cam_bases, full_dirs[:, i, :]) for i in range(full_dirs.shape[1])])
         points = points[~np.any(np.isnan(points), axis=1)]
 
         return points
 
     @staticmethod
+    def load(filename: str):
+        calibs = Camerasystem.load_dict(filename)
+        return Camerasystem.from_calibs(calibs)
+
+    @staticmethod
+    def load_dict(filename):
+        if filename.endswith('.npy'):
+            calibs = np.load(filename, allow_pickle=True)[()]["calibs"]
+        elif filename.endswith('.yml'):
+            with open(filename, 'r') as stream:
+                calibs = yaml.safe_load(stream)["calibs"]
+                calibs = collection_to_array(calibs)
+        return calibs
+
+    @staticmethod
     def from_calibcam_file(filename: str):
         cs = Camerasystem()
         calib = np.load(filename, allow_pickle=True)[()]
 
         for i in range(len(calib['RX1_fit'])):
             A = np.array([
                 [calib['A_fit'][i][0], 0, calib['A_fit'][i][1]],
```

### Comparing `bbo-calibcamlib-0.3.5/calibcamlib/dist_MaEtAl2003_model3.py` & `bbo-calibcamlib-0.3.7/calibcamlib/dist_MaEtAl2003_model3.py`

 * *Files identical despite different names*

### Comparing `bbo-calibcamlib-0.3.5/calibcamlib/dist_OpenCV.py` & `bbo-calibcamlib-0.3.7/calibcamlib/dist_OpenCV.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         # Warning: There is no closed-form solution for tangential + radial distortion. Thus, we use a solver from
         #  scipy.optimize. If this function is used within a time-critical scope, this is probably slow
         from scipy.optimize import fsolve
 
         ab_ud = []
         for p_o, p_d in zip(ab, ab_dist):
             sol = fsolve(lambda p: dist_opt_func(p, p_d, k), p_o, full_output=True, maxfev=1000, xtol=1e-6)
-            if not sol[2] == 1:
-                print(sol[3])
+            # if not sol[2] == 1:
+            #     print(sol[3])
             ab_ud.append(sol[0])
 
         return np.array(ab_ud)
 
 
 def dist_opt_func(ab, ab_d, k):
     # This function is included in the unit tests and tested correct
```

### Comparing `bbo-calibcamlib-0.3.5/setup.py` & `bbo-calibcamlib-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bbo-calibcamlib",
-    version="0.3.5",
+    version="0.3.7",
     description="Library to work with calibration from bbo-calibcam",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/calibcamlib",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@caesar.de",
     license="BSD",
@@ -23,9 +23,9 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     packages=['calibcamlib'],
     include_package_data=True,
-    install_requires=["numpy", "scipy"],
+    install_requires=["numpy", "scipy", "pyyaml"],
 )
```

### Comparing `bbo-calibcamlib-0.3.5/test/test_camera.py` & `bbo-calibcamlib-0.3.7/test/test_camera.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import pathlib
 import unittest
+
 import numpy as np
-from calibcamlib import distortion as dist, Camera
-import pathlib
+
+from calibcamlib import Camera, helper
 
 
 class TestCameraClass(unittest.TestCase):
     def test_space_to_sensor(self):
         ref_file = pathlib.Path(__file__).parent.resolve() / 'data' / 'camera_test_space_to_sensor.npy'
 
         # Build reference file
@@ -91,12 +93,21 @@
         # }
         # np.save(ref_file, data)
 
         # Test
         data = np.load(ref_file, allow_pickle=True).item()
         for n, cam in data['cams'].items():
             cam = Camera(cam['A'], cam['k'], xi=cam['xi'], offset=cam['offset'])
-            np.testing.assert_array_almost_equal(cam.space_to_sensor(cam.sensor_to_space(data['points'])), data['points'])
+            np.testing.assert_array_almost_equal(cam.space_to_sensor(cam.sensor_to_space(data['points'])),
+                                                 data['points'])
+
+    def test_point_line_dist(self):
+        points = np.array([[1, np.nan, -1],
+                           [2, 2, -2]]).astype(np.float64)
+        pt = np.zeros(3)
+        vec = np.array([0, 0, -1]).astype(np.float64)
+        dists = helper.calc_min_line_point_dist(points, pt, vec)
+        np.testing.assert_allclose(dists, np.array([np.nan, np.sqrt(8)]))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bbo-calibcamlib-0.3.5/test/test_distortion.py` & `bbo-calibcamlib-0.3.7/test/test_distortion.py`

 * *Files identical despite different names*

