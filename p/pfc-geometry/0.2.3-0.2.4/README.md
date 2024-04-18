# Comparing `tmp/pfc_geometry-0.2.3.tar.gz` & `tmp/pfc_geometry-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.2.3.tar", last modified: Wed Mar 20 17:20:00 2024, max compression
+gzip compressed data, was "pfc_geometry-0.2.4.tar", last modified: Thu Apr 18 11:54:31 2024, max compression
```

## Comparing `pfc_geometry-0.2.3.tar` & `pfc_geometry-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/LICENSE
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1557 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1191 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/geometry/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1253 2024-01-27 20:36:36.000000 pfc_geometry-0.2.3/geometry/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    11179 2024-03-20 17:11:27.000000 pfc_geometry-0.2.3/geometry/base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3039 2023-09-25 07:48:56.000000 pfc_geometry-0.2.3/geometry/coordinate_frame.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3381 2023-11-09 14:20:41.000000 pfc_geometry-0.2.3/geometry/gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1675 2023-12-22 19:42:33.000000 pfc_geometry-0.2.3/geometry/mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5025 2023-09-25 07:48:56.000000 pfc_geometry-0.2.3/geometry/point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     9418 2024-01-03 15:15:29.000000 pfc_geometry-0.2.3/geometry/quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      375 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/geometry/testing.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      995 2024-03-20 17:11:27.000000 pfc_geometry-0.2.3/geometry/time.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4701 2024-03-20 17:11:27.000000 pfc_geometry-0.2.3/geometry/transformation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/pfc_geometry.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)     1557 2024-03-20 17:20:00.000000 pfc_geometry-0.2.3/pfc_geometry.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      565 2024-03-20 17:20:00.000000 pfc_geometry-0.2.3/pfc_geometry.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-03-20 17:20:00.000000 pfc_geometry-0.2.3/pfc_geometry.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2024-03-20 17:20:00.000000 pfc_geometry-0.2.3/pfc_geometry.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        9 2024-03-20 17:20:00.000000 pfc_geometry-0.2.3/pfc_geometry.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      404 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      699 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 17:20:00.543844 pfc_geometry-0.2.3/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5532 2024-01-27 20:36:36.000000 pfc_geometry-0.2.3/tests/test_base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      875 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/tests/test_coord.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1240 2023-11-09 14:20:41.000000 pfc_geometry-0.2.3/tests/test_gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1163 2023-03-28 15:54:20.000000 pfc_geometry-0.2.3/tests/test_mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3274 2023-09-25 07:48:56.000000 pfc_geometry-0.2.3/tests/test_point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6256 2023-11-09 14:20:41.000000 pfc_geometry-0.2.3/tests/test_quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1659 2023-11-09 14:20:41.000000 pfc_geometry-0.2.3/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/coordinate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/geometry/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/pfc_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 11:54:31.000000 pfc_geometry-0.2.4/pfc_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:54:31.663937 pfc_geometry-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 11:54:11.000000 pfc_geometry-0.2.4/tests/test_transform.py
```

### Comparing `pfc_geometry-0.2.3/LICENSE` & `pfc_geometry-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/PKG-INFO` & `pfc_geometry-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
@@ -18,10 +18,13 @@
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
 
-now available on pypi:
+Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
-pip install pfc-geometry
+now available on pypi:
+```bash
+    pip install pfc-geometry
+```
```

### Comparing `pfc_geometry-0.2.3/README.md` & `pfc_geometry-0.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,10 +5,13 @@
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
 
-now available on pypi:
+Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
-pip install pfc-geometry
+now available on pypi:
+```bash
+    pip install pfc-geometry
+```
```

### Comparing `pfc_geometry-0.2.3/geometry/__init__.py` & `pfc_geometry-0.2.4/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/base.py` & `pfc_geometry-0.2.4/geometry/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
-from typing import Type, List, Self
+from typing import Self
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 from numbers import Number
 
 
 def dprep(func):
@@ -166,14 +166,18 @@
 
     def count(self) ->  int:
         return len(self)
 
     def __len__(self) -> int:
         return self.data.shape[0]
 
+    @property
+    def ends(self) -> Self:
+        return self.__class__(self.data[[0,-1], :])
+
     @dprep
     def __eq__(self, other):
         return np.all(self.data == other)
 
     @dprep
     def __add__(self, other) -> Self:
         return self.__class__(self.data + other)
@@ -229,15 +233,15 @@
         assert len(dt) == len(self)
         return self.__class__(
             np.gradient(self.data,axis=0) \
                 / \
                 np.tile(dt, (len(self.__class__.cols),1)).T)
 
     def to_pandas(self, prefix='', suffix='', columns=None, index=None):
-        if not columns is None:
+        if columns is not None:
             cols = columns
         else:
             cols = [prefix + col + suffix for col in self.__class__.cols]
         return pd.DataFrame(
             self.data, 
             columns=cols,
             index=index
@@ -313,18 +317,18 @@
 
         return self.__class__(filtfilt(b, a, self.data, axis=0))
     
     def fft(self, ts: np.ndarray=None):
         from scipy.fft import fft, fftfreq
         if ts is None:
             ts = np.array(range(len(self)))
-        N = len(self)
-        T = (ts[-1] - ts[0]) / N
+        N = len(self)*2
+        T = (ts[-1] - ts[0]) / len(self)
 
-        yf = fft(self.data, axis=0)
+        yf = fft(self.data, axis=0, n=N)
         xf = fftfreq(N, T)[:N//2]
 
         
         y=2.0/N * np.abs(yf[0:N//2, :])
 
         return pd.DataFrame(np.column_stack([xf, y]), columns=['freq'] + self.cols).set_index('freq')
```

### Comparing `pfc_geometry-0.2.3/geometry/coordinate_frame.py` & `pfc_geometry-0.2.4/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/gps.py` & `pfc_geometry-0.2.4/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/mass.py` & `pfc_geometry-0.2.4/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/point.py` & `pfc_geometry-0.2.4/geometry/point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/quaternion.py` & `pfc_geometry-0.2.4/geometry/quaternion.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import annotations
-from .point import Point, P0
+from .point import Point
 from .base import Base
 from geometry import PZ
-from typing import Union, Tuple
 import numpy as np
-import pandas as pd
 import numpy.typing as npt
+import pandas as pd
 from warnings import warn
 from numbers import Number
 
 
-
 class Quaternion(Base):
     cols=["w", "x", "y", "z"]
 
     @staticmethod
     def zero(count=1) -> Quaternion:
         return Quaternion(np.tile([1,0,0,0], (count,1)))
 
@@ -42,15 +40,15 @@
 
     def conjugate(self) -> Quaternion:
         return Quaternion(self.w, -self.x, -self.y, -self.z)
 
     def inverse(self):
         return self.conjugate().norm()
 
-    def __mul__(self, other: Union[Number, Quaternion, np.ndarray]) -> Quaternion:
+    def __mul__(self, other: Number | Quaternion | npt.NDArray) -> Quaternion:
         if isinstance(other, Quaternion):
             a, b = Quaternion.length_check(self, Quaternion.type_check(other))
             w = a.w * b.w - a.axis.dot(b.axis)
             xyz = a.w * b.axis + b.w * a.axis + a.axis.cross(b.axis)
             return Quaternion(np.column_stack([w, xyz.data]))
 
         elif isinstance(other, Number):
@@ -177,28 +175,28 @@
 
     def rotate(self, rate: Point) -> Quaternion:
         return (Quaternion.from_axis_angle(rate) * self).norm()
 
     def body_rotate(self, rate: Point) -> Quaternion:
         return (self * Quaternion.from_axis_angle(rate)).norm()
 
-    def diff(self, dt: Union[Number, np.ndarray]) -> Point:
+    def diff(self, dt: Number | npt.NDArray) -> Point:
         """differentiate in the world frame"""
         if not pd.api.types.is_list_like(dt):
             dt = np.full(len(self), dt)
         assert len(dt) == len(self)
         dt = dt * len(dt) / (len(dt) - 1)
 
         ps = Quaternion._axis_rates(
             Quaternion(self.data[:-1, :]),
             Quaternion(self.data[1:, :])
         ) / dt[:-1]
         return Point(np.vstack([ps.data, ps.data[-1,:]]))
 
-    def body_diff(self, dt: Union[Number, np.ndarray]) -> Point:
+    def body_diff(self, dt: Number | npt.NDArray) -> Point:
         """differentiate in the body frame"""
         if not pd.api.types.is_list_like(dt):
             dt = np.full(len(self), dt)
         assert len(dt) == len(self)
         dt = dt * len(dt) / (len(dt) - 1)
 
         ps = Quaternion.body_axis_rates(
```

### Comparing `pfc_geometry-0.2.3/geometry/time.py` & `pfc_geometry-0.2.4/geometry/time.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/geometry/transformation.py` & `pfc_geometry-0.2.4/geometry/transformation.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/pfc_geometry.egg-info/PKG-INFO` & `pfc_geometry-0.2.4/pfc_geometry.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
@@ -18,10 +18,13 @@
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
 
-now available on pypi:
+Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
-pip install pfc-geometry
+now available on pypi:
+```bash
+    pip install pfc-geometry
+```
```

### Comparing `pfc_geometry-0.2.3/pfc_geometry.egg-info/SOURCES.txt` & `pfc_geometry-0.2.4/pfc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/setup.py` & `pfc_geometry-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_base.py` & `pfc_geometry-0.2.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_coord.py` & `pfc_geometry-0.2.4/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_gps.py` & `pfc_geometry-0.2.4/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_mass.py` & `pfc_geometry-0.2.4/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_point.py` & `pfc_geometry-0.2.4/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.3/tests/test_quaternion.py` & `pfc_geometry-0.2.4/tests/test_quaternion.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from pytest import mark, approx, raises
 from geometry.quaternion import Quaternion, Q0
 from geometry.point import Point, PX, PY, PZ, P0
 from geometry import Euler, Euldeg
 from geometry.testing import assert_almost_equal
 import pandas as pd
 import numpy as np
-import quaternion
-from scipy.spatial.transform import Rotation as R
 
 
 
 def test_init():
     data = np.random.random((500,4))
     qs = Quaternion(data)
     np.testing.assert_array_equal(data, qs.data)
@@ -33,42 +31,23 @@
     
     np.testing.assert_array_almost_equal(
         check.data,
         check_npy,
         err_msg="failed to do Quaternions * Quaternions"
     )
 
-def test_from_euler():
-    parr = np.random.random((20, 3))
-
-    np.testing.assert_array_almost_equal(
-        Quaternion.from_euler(Point(parr)).xyzw,
-        R.from_euler('xyz', parr).as_quat()
-    )
-
 
 def test_from_euler_unwrap():    
     q = Q0(10).rotate(PZ()*np.radians(np.linspace(0,360, 10)))
     np.testing.assert_array_almost_equal(
         Quaternion.from_euler(q.to_euler()).diff(1).data, 
         q.diff(1).data
     )
 
 
-def test_to_euler():
-    qarr = Quaternion(np.random.random((2, 4))).norm()
-    eulers = qarr.to_euler()
-    
-    checks = np.array([R.from_euler("xyz", eul.data[0]).as_quat() for eul in eulers])
-    
-    np.testing.assert_array_almost_equal(
-        checks,
-        qarr.xyzw
-    )
-
 
 def test_norm():
     qarr = Quaternion(np.random.random( (2,4)))
 
     def npcheck(q1):
         res = np.quaternion(*q1.data[0]).normalized()
         return np.array([res.w, res.x, res.y, res.z])
```

### Comparing `pfc_geometry-0.2.3/tests/test_transform.py` & `pfc_geometry-0.2.4/tests/test_transform.py`

 * *Files identical despite different names*

