# Comparing `tmp/xyz_py-5.9.3.tar.gz` & `tmp/xyz_py-5.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.9.3.tar", last modified: Thu Feb 22 11:31:11 2024, max compression
+gzip compressed data, was "xyz_py-5.9.4.tar", last modified: Thu Apr 18 16:39:31 2024, max compression
```

## Comparing `xyz_py-5.9.3.tar` & `xyz_py-5.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 11:31:11.051848 xyz_py-5.9.3/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2024-02-22 11:30:37.000000 xyz_py-5.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1391 2024-02-22 11:31:11.051848 xyz_py-5.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-02-22 11:30:37.000000 xyz_py-5.9.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-02-22 11:30:37.000000 xyz_py-5.9.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 11:31:11.051848 xyz_py-5.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-02-22 11:31:03.000000 xyz_py-5.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 11:31:11.049848 xyz_py-5.9.3/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-22 11:30:37.000000 xyz_py-5.9.3/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8117 2024-02-22 11:30:37.000000 xyz_py-5.9.3/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)    11935 2024-02-22 11:30:37.000000 xyz_py-5.9.3/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-22 11:31:03.000000 xyz_py-5.9.3/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    42666 2024-02-22 11:30:37.000000 xyz_py-5.9.3/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 11:31:11.050848 xyz_py-5.9.3/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1391 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-22 11:31:11.000000 xyz_py-5.9.3/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-18 16:39:31.139997 xyz_py-5.9.4/
+-rw-r--r--   0 jon       (1000) jon       (1000)    35072 2023-08-15 16:52:38.000000 xyz_py-5.9.4/LICENSE
+-rw-r--r--   0 jon       (1000) jon       (1000)     1391 2024-04-18 16:39:31.139997 xyz_py-5.9.4/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)      681 2023-08-15 16:52:38.000000 xyz_py-5.9.4/README.md
+-rw-r--r--   0 jon       (1000) jon       (1000)     1478 2024-01-24 10:54:08.000000 xyz_py-5.9.4/pyproject.toml
+-rw-r--r--   0 jon       (1000) jon       (1000)       38 2024-04-18 16:39:31.139997 xyz_py-5.9.4/setup.cfg
+-rw-r--r--   0 jon       (1000) jon       (1000)     1112 2024-04-04 16:19:36.000000 xyz_py-5.9.4/setup.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-18 16:39:31.139997 xyz_py-5.9.4/xyz_py/
+-rw-r--r--   0 jon       (1000) jon       (1000)       84 2023-08-15 16:52:38.000000 xyz_py-5.9.4/xyz_py/__init__.py
+-rw-r--r--   0 jon       (1000) jon       (1000)     8117 2023-08-15 16:52:38.000000 xyz_py-5.9.4/xyz_py/atomic.py
+-rw-r--r--   0 jon       (1000) jon       (1000)    11935 2024-01-24 10:37:56.000000 xyz_py-5.9.4/xyz_py/cli.py
+-rw-r--r--   0 jon       (1000) jon       (1000)       22 2024-04-04 16:19:36.000000 xyz_py-5.9.4/xyz_py/version.py
+-rw-r--r--   0 jon       (1000) jon       (1000)    43629 2024-04-18 14:03:53.000000 xyz_py-5.9.4/xyz_py/xyz_py.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-18 16:39:31.139997 xyz_py-5.9.4/xyz_py.egg-info/
+-rw-r--r--   0 jon       (1000) jon       (1000)     1391 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)      308 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)        1 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       43 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       28 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)        7 2024-04-18 16:39:31.000000 xyz_py-5.9.4/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.9.3/LICENSE` & `xyz_py-5.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.9.3/PKG-INFO` & `xyz_py-5.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz_py
-Version: 5.9.3
+Version: 5.9.4
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.9.3/README.md` & `xyz_py-5.9.4/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.9.3/pyproject.toml` & `xyz_py-5.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xyz_py-5.9.3/setup.py` & `xyz_py-5.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.9.3"
+__version__ = "5.9.4"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.9.3/xyz_py/atomic.py` & `xyz_py-5.9.4/xyz_py/atomic.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.9.3/xyz_py/cli.py` & `xyz_py-5.9.4/xyz_py/cli.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.9.3/xyz_py/xyz_py.py` & `xyz_py-5.9.4/xyz_py/xyz_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,44 +206,52 @@
 
     if verbose:
         print('New xyz file written to {}'.format(f_name))
 
     return
 
 
-def remove_label_indices(labels: ArrayLike) -> list[str]:
+def remove_label_indices(labels: ArrayLike | str) -> list[str]:
     '''
     Remove label indexing from atomic symbols\n
     indexing is either numbers or numbers followed by letters:\n
     e.g. H1, H2, H3\n
     or H1a, H2a, H3a
 
     Parameters
     ----------
-    labels: array_like
+    labels: array_like | str
         atomic labels
 
     Returns
     -------
-    list[str]
-        atomic labels without indexing
+    list[str] | str
+        atomic labels without indexing, type depends on input type
     '''
 
+    if isinstance(labels, str):
+        _labels = [labels]
+    else:
+        _labels = labels
+
     labels_nn = []
-    for label in labels:
+    for label in _labels:
         no_digits = []
         for i in label:
             if not i.isdigit():
                 no_digits.append(i)
             elif i.isdigit():
                 break
         result = ''.join(no_digits)
         labels_nn.append(result)
 
-    return labels_nn
+    if isinstance(labels, str):
+        return labels_nn[0]
+    else:
+        return labels_nn
 
 
 def add_label_indices(labels: ArrayLike, style: str = 'per_element',
                       start_index: int = 1) -> list[str]:
     '''
     Add label indexing to atomic symbols - either element or per atom.
 
@@ -635,15 +643,16 @@
 
 @deprecation.deprecated(
     deprecated_in='5.3.0', removed_in='6.3.0', current_version=__version__,
     details='Use find_bonds instead'
 )
 def get_bonds(labels: ArrayLike, coords: ArrayLike,
               neigh_list: neighborlist.NeighborList = None,
-              verbose: bool = True, style: str = 'indices') -> list[list[int | str]]:
+              verbose: bool = True,
+              style: str = 'indices') -> list[list[int | str]]:
     '''
     Calculate list of atoms between which there is a bond.\n
     Using ASE. Only unique bonds are retained.\n
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
@@ -671,17 +680,17 @@
         labels, coords, neigh_list=neigh_list, verbose=verbose, style=style
     )
 
     return bonds
 
 
 def find_bonds(labels: ArrayLike, coords: ArrayLike,
-              neigh_list: neighborlist.NeighborList = None,
-              verbose: bool = True,
-              style: str = 'labels') -> tuple[list[list[int | str]], NDArray]:
+               neigh_list: neighborlist.NeighborList = None,
+               verbose: bool = True,
+               style: str = 'labels') -> tuple[list[list[int | str]], NDArray]:
     '''
     Calculate list of atoms between which there is a bond.\n
     Using ASE. Only unique bonds are retained.\n
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
@@ -1033,34 +1042,42 @@
     # Print number of dihedrals to screen
     if verbose:
         print('{:d} dihedrals'.format(n_dihedrals))
 
     return dihedrals, values
 
 
-def lab_to_num(labels: ArrayLike) -> list[int]:
+def lab_to_num(labels: ArrayLike | str) -> list[int]:
     '''
     Convert atomic label to atomic number
 
     Parameters
     ----------
-    labels: array_like
+    labels: array_like | str
         Atomic labels
 
     Returns
     -------
-    list[int]
+    list[int] | int
         Atomic numbers
     '''
 
-    labels_nn = remove_label_indices(labels)
+    if isinstance(labels, str):
+        _labels = [labels]
+    else:
+        _labels = labels
+
+    labels_nn = remove_label_indices(_labels)
 
     numbers = [atomic.lab_num[lab] for lab in labels_nn]
 
-    return numbers
+    if isinstance(labels, str):
+        return numbers[0]
+    else:
+        return numbers
 
 
 def num_to_lab(numbers: ArrayLike, numbered: bool = True) -> list[str]:
     '''
     Convert atomic number to atomic labels
 
     Parameters
@@ -1124,16 +1141,16 @@
     # Apply operations
     coords = coords @ trans_mat
 
     return coords
 
 
 def find_entities(labels: ArrayLike, coords: ArrayLike,
-                  adjust_cutoff: dict[str, float ] = {},
-                  non_bond_labels: list[str] = []) -> dict[str, list[list[int]]]: # array_like
+                  adjust_cutoff: dict[str, float] = {},
+                  non_bond_labels: list[str] = []) -> dict[str, list[list[int]]]: # noqa
     '''
     Finds formulae of entities given in labels and coords using adjacency
     matrix
 
     Parameters
     ----------
     labels: array_like
@@ -1165,17 +1182,14 @@
     adjacency = get_adjacency(labels_nn, coords, adjust_cutoff=adjust_cutoff)
 
     no_bond_indices = [
         it for it, lab in enumerate(labels)
         if lab in non_bond_labels
     ]
 
-    if not len(no_bond_indices):
-        print('Cannot find specified no_bond atoms, perhaps try with index included?')
-
     for nbi in no_bond_indices:
         adjacency[nbi, :] = 0
         adjacency[:, nbi] = 0
 
     # Find entities
     entities = find_entities_from_adjacency(labels_nn, adjacency)
 
@@ -1355,18 +1369,55 @@
 
     # Calculate rmsd
     rmsd = _calculate_rmsd(_coords_1, _coords_2)
 
     return rmsd
 
 
+def build_rotation_matrix(alpha: float, beta: float, gamma: float) -> NDArray:
+    '''
+    Creates rotation matrix using euler angles alpha, beta, gamma
+    for the zyz convention\n
+    https://easyspin.org/easyspin/documentation/eulerangles.html
+
+    Parameters
+    ----------
+    alpha: float
+        alpha angle in radians
+    beta: float
+        beta  angle in radians
+    gamma: float
+        gamma angle in radians
+
+    Returns
+    -------
+    ndarray of floats
+        Rotation matrix R which is applied to a vector x as R dot x
+    '''
+    r_mat = np.zeros([3, 3])
+
+    # Build rotation matrix
+    r_mat[0, 0] = np.cos(gamma) * np.cos(beta) * np.cos(alpha) - np.sin(gamma) * np.sin(alpha) # noqa
+    r_mat[0, 1] = np.cos(gamma) * np.cos(beta) * np.sin(alpha) + np.sin(gamma) * np.cos(alpha) # noqa
+    r_mat[0, 2] = -np.cos(gamma) * np.sin(beta)
+    r_mat[1, 0] = -np.sin(gamma) * np.cos(beta) * np.cos(alpha) - np.cos(gamma) * np.sin(alpha) # noqa
+    r_mat[1, 1] = -np.sin(gamma) * np.cos(beta) * np.sin(alpha) + np.cos(gamma) * np.cos(alpha) # noqa
+    r_mat[1, 2] = np.sin(gamma) * np.sin(beta)
+    r_mat[2, 0] = np.sin(beta) * np.cos(alpha)
+    r_mat[2, 1] = np.sin(beta) * np.sin(alpha)
+    r_mat[2, 2] = np.cos(beta)
+
+    return r_mat
+
+
 def rotate_coords(coords: ArrayLike, alpha: float, beta: float,
                   gamma: float) -> NDArray:
     '''
-    Rotates coordinates by alpha, beta, gamma using the zyz convention\n
+    Rotates coordinates using euler angles alpha, beta, gamma
+    for the zyz convention\n
     https://easyspin.org/easyspin/documentation/eulerangles.html
 
     Parameters
     ----------
     coords: array_like
         xyz coordinates as (n_atoms, 3) array
     alpha: float
@@ -1380,26 +1431,15 @@
     -------
     ndarray of floats
         xyz coordinates as (n_atoms, 3) array after rotation\n
         in same order as input coordinates
     '''
     coords = np.asarray(coords)
 
-    R = np.zeros([3, 3])
-
-    # Build rotation matrix
-    R[0, 0] = np.cos(gamma) * np.cos(beta) * np.cos(alpha) - np.sin(gamma) * np.sin(alpha) # noqa
-    R[0, 1] = np.cos(gamma) * np.cos(beta) * np.sin(alpha) + np.sin(gamma) * np.cos(alpha) # noqa
-    R[0, 2] = -np.cos(gamma) * np.sin(beta)
-    R[1, 0] = -np.sin(gamma) * np.cos(beta) * np.cos(alpha) - np.cos(gamma) * np.sin(alpha) # noqa
-    R[1, 1] = -np.sin(gamma) * np.cos(beta) * np.sin(alpha) + np.cos(gamma) * np.cos(alpha) # noqa
-    R[1, 2] = np.sin(gamma) * np.sin(beta)
-    R[2, 0] = np.sin(beta) * np.cos(alpha)
-    R[2, 1] = np.sin(beta) * np.sin(alpha)
-    R[2, 2] = np.cos(beta)
+    R = build_rotation_matrix(alpha, beta, gamma)
 
     # Create (n,3) matrix from coords list
     _coords = coords.T
 
     # Apply rotation matrix
     rot_coords = R @ _coords
```

### Comparing `xyz_py-5.9.3/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.9.4/xyz_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz_py
-Version: 5.9.3
+Version: 5.9.4
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

