# Comparing `tmp/updes-1.0.0.tar.gz` & `tmp/updes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "updes-1.0.0.tar", last modified: Mon Apr 15 10:10:49 2024, max compression
+gzip compressed data, was "updes-1.0.1.tar", last modified: Thu Apr 18 13:06:52 2024, max compression
```

## Comparing `updes-1.0.0.tar` & `updes-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-15 10:10:49.260409 updes-1.0.0/
--rw-r--r--   0 ddrous     (501) staff       (20)    18092 2024-04-15 09:28:58.000000 updes-1.0.0/LICENSE
--rw-r--r--   0 ddrous     (501) staff       (20)     4733 2024-04-15 10:10:49.260200 updes-1.0.0/PKG-INFO
--rw-r--r--   0 ddrous     (501) staff       (20)     4127 2024-04-15 09:29:59.000000 updes-1.0.0/README.md
--rw-r--r--   0 ddrous     (501) staff       (20)      629 2024-04-15 10:10:44.000000 updes-1.0.0/pyproject.toml
--rw-r--r--   0 ddrous     (501) staff       (20)       38 2024-04-15 10:10:49.260449 updes-1.0.0/setup.cfg
-drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-15 10:10:49.259707 updes-1.0.0/updes.egg-info/
--rw-r--r--   0 ddrous     (501) staff       (20)     4733 2024-04-15 10:10:49.000000 updes-1.0.0/updes.egg-info/PKG-INFO
--rw-r--r--   0 ddrous     (501) staff       (20)      176 2024-04-15 10:10:49.000000 updes-1.0.0/updes.egg-info/SOURCES.txt
--rw-r--r--   0 ddrous     (501) staff       (20)        1 2024-04-15 10:10:49.000000 updes-1.0.0/updes.egg-info/dependency_links.txt
--rw-r--r--   0 ddrous     (501) staff       (20)       94 2024-04-15 10:10:49.000000 updes-1.0.0/updes.egg-info/requires.txt
--rw-r--r--   0 ddrous     (501) staff       (20)        6 2024-04-15 10:10:49.000000 updes-1.0.0/updes.egg-info/top_level.txt
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:06:52.807531 updes-1.0.1/
+-rw-r--r--   0 ddrous     (501) staff       (20)    18092 2024-04-15 09:28:58.000000 updes-1.0.1/LICENSE
+-rw-r--r--   0 ddrous     (501) staff       (20)      565 2024-04-18 13:06:52.807315 updes-1.0.1/PKG-INFO
+-rw-r--r--   0 ddrous     (501) staff       (20)     3753 2024-04-18 12:57:50.000000 updes-1.0.1/README.md
+-rw-r--r--   0 ddrous     (501) staff       (20)      646 2024-04-18 13:06:16.000000 updes-1.0.1/pyproject.toml
+-rw-r--r--   0 ddrous     (501) staff       (20)       38 2024-04-18 13:06:52.807577 updes-1.0.1/setup.cfg
+drwxr-xr-x   0 ddrous     (501) staff       (20)        0 2024-04-18 13:06:52.806910 updes-1.0.1/updes.egg-info/
+-rw-r--r--   0 ddrous     (501) staff       (20)      565 2024-04-18 13:06:52.000000 updes-1.0.1/updes.egg-info/PKG-INFO
+-rw-r--r--   0 ddrous     (501) staff       (20)      176 2024-04-18 13:06:52.000000 updes-1.0.1/updes.egg-info/SOURCES.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)        1 2024-04-18 13:06:52.000000 updes-1.0.1/updes.egg-info/dependency_links.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)       94 2024-04-18 13:06:52.000000 updes-1.0.1/updes.egg-info/requires.txt
+-rw-r--r--   0 ddrous     (501) staff       (20)        6 2024-04-18 13:06:52.000000 updes-1.0.1/updes.egg-info/top_level.txt
```

### Comparing `updes-1.0.0/LICENSE` & `updes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `updes-1.0.0/PKG-INFO` & `updes-1.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,117 +1,98 @@
-Metadata-Version: 2.1
-Name: updes
-Version: 1.0.0
-Summary: Universal Partial Differential Equations Simulator
-Author-email: Roussel Desmond Nzoyem <desmond.ngueguin@gmail.com>
-Keywords: differentiable-programming,radial-basis-function,meshfree,optimisation,differentiable-physics,PDEs
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jax>=0.3.4
-Requires-Dist: gmsh
-Requires-Dist: pytest
-Requires-Dist: matplotlib>=3.4.0
-Requires-Dist: scikit-learn
-Requires-Dist: seaborn
-Provides-Extra: dev
-Requires-Dist: pyvista[trame]; extra == "dev"
-Requires-Dist: quartodoc; extra == "dev"
-
 # 𝕌pdes
 
-𝕌pdes is a general-purpose library for mesh-free PDE simulation and control. __𝕌pdes__ stands for Universal(__𝕌__) Partial Differential Equations (__PDE__) Simulator(__S__). There is no faster way to run your PDE than to use Updes !
+𝕌pdes is a general-purpose library for mesh-free PDE simulation and control. There is no faster way to explore the realm of PDEs !
+
+<table>
+  <tr>
+    <th><img src="docs/assets/laplace.png" width="180"></th>
+    <th><img src="docs/assets/advection_diffusion.gif" width="350"></th>
+    <th><img src="docs/assets/burgers_u.gif" width="188"></th>
+  </tr>
+</table>
 
 
 ## Features
 𝕌pdes leverages Radial Basis Functions (RBFs) and JAX to provide the following features:
 - User-centric design: no need to re-implement a solver for each new PDE
 - Lightning fast mesh-free simulation via Radial Basis Functions
 - Robust differentiable simulation via JAX, and portable across CPU, GPU, and TPU
 - Support for Dirichlet, Neumann, Robin, and Periodic boundary conditions
 - Automatic generation of normals from 2D GMSH meshes
 
-𝕌pdes in incredibly extendable, and additional features will be added soon.
+𝕌pdes in incredibly extendable, with additional features added frequently.
 
 
 ## Getting started
 The package is available on PyPi. You can install it with
 ```
-pip install Updes OR pip install "git+https://github.com/user/project"
+pip install updes
 ```
 
 The example below illustrates how to solve the Laplace equation with Dirichlet and Neumann boundary conditions:
 ```python
-from updes import *
+import updes
 import jax.numpy as jnp
 
 # Create a mesh-free cloud of points on a unit square
 facet_types={"South":"n", "West":"d", "North":"d", "East":"d"}
-cloud = SquareCloud(Nx=30, Ny=20, facet_types=facet_types)
+cloud = updes.SquareCloud(Nx=30, Ny=20, facet_types=facet_types)
 
 # Define the differential operator (left-hand side of the PDE)
-def my_diff_operator(x, center=None, rbf=None, monomial=None, fields=None):
-    return nodal_laplacian(x, center, rbf, monomial)
+def my_diff_operator(x, center, rbf, monomial, fields):
+    return updes.nodal_laplacian(x, center, rbf, monomial)
 
 # Define the right-hand side of the PDE
-def my_rhs_operator(x, centers=None, rbf=None, fields=None):
+def my_rhs_operator(x, centers, rbf, fields):
     return 0.0
 
 # Set a sin function as the Dirichlet BC on the North, and zero everywhere else
-d_north = lambda coord: jnp.sin(jnp.pi * coord[0])
-d_zero = lambda coord: 0.0
-boundary_conditions = {"South":d_zero, "West":d_zero, "North":d_north, "East":d_zero}
+sine = lambda coord: jnp.sin(jnp.pi * coord[0])
+zero = lambda coord: 0.0
+boundary_conditions = {"South":zero, "West":zero, "North":sine, "East":zero}
 
 # Solve the Laplace equation with a JIT-compiled solver
-sol = pde_solver_jit(diff_operator=my_diff_operator, 
+sol = updes.pde_solver_jit(diff_operator=my_diff_operator, 
                     rhs_operator=my_rhs_operator, 
                     cloud=cloud, 
                     boundary_conditions=boundary_conditions, 
-                    rbf=polyharmonic,
+                    rbf=updes.polyharmonic,
                     max_degree=1)
 
 # Visualize the solution
-cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution");
+cloud.visualize_field(sol.vals, cmap="jet", projection="3d", title="RBF solution")
 ```
 
 𝕌pdes can handle much complicated cases with little to no modifications to the code above. Check out further notebooks and scripts in the documentation and the folder [`demos`](./demos)!
 
-<!-- | ![laplace](docs/assets/laplace.png) | ![Advection-Diffusion](![laplace](docs/assets/advection_diffusion.gif) | ![Burgers](docs/assets/burgers_rk4_u.gif) | -->
-
-<table>
-  <tr>
-    <th><img src="docs/assets/laplace.png" width="180"></th>
-    <th><img src="docs/assets/advection_diffusion.gif" width="350"></th>
-    <th><img src="docs/assets/burgers_u.gif" width="188"></th>
-  </tr>
-</table>
 
 
 
 ## To-Dos
-- Logo, licence, contributors guide, and developer documentation
-- Better introductory examples and user documentation for outreach
+- Logo, contributors guide, and developer documentation
+- Better introductory examples and user documentation for outreach:
     - Integration with Neural Networks and Equinox
     - Non-linear and multi-dimensional PDEs
     - Adjoint schemes for fluid flows
-- Better cloud points generation with accurate geometry and normals: 
+- Better point generation with accurate geometry and normals: 
     - USD format
     - Gmsh tutorial
 - Add support for 3D radial basis functions
 
 We welcome contributions from the community. Please feel free to open an issue or a pull request.
 
 
 ## Dependencies
 - **Core**: JAX - GMSH - Matplotlib - Seaborn - Scikit-Learn
 - **Optional**: PyVista - FFMPEG - QuartoDoc
 
 See the `pyproject.toml` file the specific versions of the dependencies.
 
 
-## Cite us
+## Cite us !
 If you use this software, please cite us with the following BibTeX entry:
 ```
 @inproceedings{nzoyem2023comparison,
   title={A comparison of mesh-free differentiable programming and data-driven strategies for optimal control under PDE constraints},
   author={Nzoyem Ngueguin, Roussel Desmond and Barton, David AW and Deakin, Tom},
   booktitle={Proceedings of the SC'23 Workshops of The International Conference on High Performance Computing, Network, Storage, and Analysis},
   pages={21--28},
```

### Comparing `updes-1.0.0/pyproject.toml` & `updes-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "updes"
 description = "Universal Partial Differential Equations Simulator"
-version = "1.0.0"
-readme = "README.md"
+version = "1.0.1"
+readme = "docs/assets/README_PyPI/md"
 authors = [
     { name = "Roussel Desmond Nzoyem", email = "desmond.ngueguin@gmail.com" }
 ]
 keywords = [
     "differentiable-programming",
     "radial-basis-function",
     "meshfree",
```

