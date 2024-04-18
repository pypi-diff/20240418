# Comparing `tmp/pyfem-0.1.9.tar.gz` & `tmp/pyfem-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.1.9.tar", last modified: Thu Jan 11 09:03:42 2024, max compression
+gzip compressed data, was "pyfem-0.2.0.tar", last modified: Thu Apr 18 07:48:12 2024, max compression
```

## Comparing `pyfem-0.1.9.tar` & `pyfem-0.2.0.tar`

### file list

```diff
@@ -1,110 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.886269 pyfem-0.1.9/
--rw-rw-rw-   0        0        0    11525 2023-08-17 09:47:31.000000 pyfem-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     3579 2024-01-11 09:03:42.886269 pyfem-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3065 2024-01-11 09:00:02.000000 pyfem-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-01-11 09:03:42.886269 pyfem-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-08-17 09:47:32.000000 pyfem-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.817499 pyfem-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.824479 pyfem-0.1.9/src/pyfem/
--rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.1.9/src/pyfem/Job.py
--rw-rw-rw-   0        0        0       23 2024-01-11 08:53:01.000000 pyfem-0.1.9/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-11-02 07:31:58.000000 pyfem-0.1.9/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.831457 pyfem-0.1.9/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.1.9/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.833449 pyfem-0.1.9/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    13344 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.839429 pyfem-0.1.9/src/pyfem/bc/
--rw-rw-rw-   0        0        0     4133 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2748 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2729 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0    26790 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0    12770 2023-12-12 06:44:34.000000 pyfem-0.1.9/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/bc/derive_surface_integral.py
--rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.845410 pyfem-0.1.9/src/pyfem/elements/
--rw-rw-rw-   0        0        0    17767 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0    76446 2024-01-11 07:21:24.000000 pyfem-0.1.9/src/pyfem/elements/SolidFiniteStrain.py
--rw-rw-rw-   0        0        0    18244 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
--rw-rw-rw-   0        0        0    12457 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/elements/SolidSmallStrain.py
--rw-rw-rw-   0        0        0    16473 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/elements/SolidThermalSmallStrain.py
--rw-rw-rw-   0        0        0     8419 2023-11-02 07:24:23.000000 pyfem-0.1.9/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     3236 2023-11-08 09:42:50.000000 pyfem-0.1.9/src/pyfem/elements/get_element_data.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.847399 pyfem-0.1.9/src/pyfem/fem/
--rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.1.9/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0      324 2023-11-02 07:36:44.000000 pyfem-0.1.9/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.857369 pyfem-0.1.9/src/pyfem/io/
--rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     1781 2023-11-02 07:24:37.000000 pyfem-0.1.9/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     3033 2023-11-02 07:37:06.000000 pyfem-0.1.9/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0     1573 2023-09-19 07:05:17.000000 pyfem-0.1.9/src/pyfem/io/Module.py
--rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.1.9/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.1.9/src/pyfem/io/Parameter.py
--rw-rw-rw-   0        0        0    12038 2023-11-02 07:43:14.000000 pyfem-0.1.9/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.1.9/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.1.9/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5213 2023-11-03 06:49:39.000000 pyfem-0.1.9/src/pyfem/io/write_hdf5.py
--rw-rw-rw-   0        0        0     5230 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.862348 pyfem-0.1.9/src/pyfem/isoelements/
--rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/isoelements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    18630 2023-12-12 06:48:03.000000 pyfem-0.1.9/src/pyfem/isoelements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/isoelements/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/isoelements/derive_shape_functions.py
--rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.1.9/src/pyfem/isoelements/get_iso_element_type.py
--rw-rw-rw-   0        0        0    23679 2023-12-05 03:38:54.000000 pyfem-0.1.9/src/pyfem/isoelements/shape_functions.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.871319 pyfem-0.1.9/src/pyfem/materials/
--rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     8776 2024-01-11 07:39:35.000000 pyfem-0.1.9/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     3135 2023-11-02 07:24:49.000000 pyfem-0.1.9/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     2174 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0    79933 2023-09-21 06:19:10.000000 pyfem-0.1.9/src/pyfem/materials/PlasticCrystal.py
--rw-rw-rw-   0        0        0    91044 2023-09-26 03:15:28.000000 pyfem-0.1.9/src/pyfem/materials/PlasticCrystalGNDs.py
--rw-rw-rw-   0        0        0     8404 2023-09-21 06:20:49.000000 pyfem-0.1.9/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2773 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     6137 2023-09-19 06:25:05.000000 pyfem-0.1.9/src/pyfem/materials/UMAT.py
--rw-rw-rw-   0        0        0    10058 2023-10-27 05:19:05.000000 pyfem-0.1.9/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0    41881 2023-09-26 03:18:28.000000 pyfem-0.1.9/src/pyfem/materials/crystal_slip_system.py
--rw-rw-rw-   0        0        0     2478 2023-11-02 07:24:49.000000 pyfem-0.1.9/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.873315 pyfem-0.1.9/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     8176 2023-11-15 11:20:27.000000 pyfem-0.1.9/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.877299 pyfem-0.1.9/src/pyfem/quadrature/
--rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/BaseQuadrature.py
--rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/GaussLegendreQuadrature.py
--rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/PyramidQuadrature.py
--rw-rw-rw-   0        0        0    22830 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/TetrahedronQuadrature.py
--rw-rw-rw-   0        0        0    25688 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/TriangleQuadrature.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/quadrature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.880292 pyfem-0.1.9/src/pyfem/solvers/
--rw-rw-rw-   0        0        0     1450 2023-11-01 04:20:15.000000 pyfem-0.1.9/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     2225 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0    11206 2024-01-11 07:11:52.000000 pyfem-0.1.9/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-11-02 07:24:54.000000 pyfem-0.1.9/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.885273 pyfem-0.1.9/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      957 2023-11-02 07:37:35.000000 pyfem-0.1.9/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.1.9/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0    18413 2023-10-13 04:28:56.000000 pyfem-0.1.9/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.1.9/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1183 2023-11-01 09:41:59.000000 pyfem-0.1.9/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-01-11 09:03:42.829458 pyfem-0.1.9/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     3579 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2972 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-11 09:03:42.000000 pyfem-0.1.9/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.193787 pyfem-0.2.0/
+-rw-rw-rw-   0        0        0    11525 2023-08-17 09:47:31.000000 pyfem-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3579 2024-04-18 07:48:12.193287 pyfem-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-18 07:48:12.193787 pyfem-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-08-17 09:47:32.000000 pyfem-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.090787 pyfem-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.104787 pyfem-0.2.0/src/pyfem/
+-rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.0/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2024-04-18 07:25:48.000000 pyfem-0.2.0/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-11-02 07:31:58.000000 pyfem-0.2.0/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.115287 pyfem-0.2.0/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.0/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.117287 pyfem-0.2.0/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    14782 2024-04-18 07:46:32.000000 pyfem-0.2.0/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.124787 pyfem-0.2.0/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.0/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.0/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0    13073 2024-04-18 07:30:11.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/bc/derive_surface_integral.py
+-rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.133787 pyfem-0.2.0/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    20823 2024-04-17 06:35:13.000000 pyfem-0.2.0/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    10336 2024-04-18 04:21:42.000000 pyfem-0.2.0/src/pyfem/elements/Diffusion.py
+-rw-rw-rw-   0        0        0    76446 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/elements/SolidFiniteStrain.py
+-rw-rw-rw-   0        0        0    18380 2024-04-18 07:24:12.000000 pyfem-0.2.0/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    12457 2024-04-18 04:25:16.000000 pyfem-0.2.0/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16473 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8419 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3324 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.136287 pyfem-0.2.0/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.0/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.0/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.151287 pyfem-0.2.0/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     1781 2023-11-02 07:24:37.000000 pyfem-0.2.0/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     3071 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1573 2023-09-19 07:05:17.000000 pyfem-0.2.0/src/pyfem/io/Module.py
+-rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.0/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.0/src/pyfem/io/Parameter.py
+-rw-rw-rw-   0        0        0    12038 2024-04-11 06:14:41.000000 pyfem-0.2.0/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.0/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.0/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5213 2023-11-03 06:49:39.000000 pyfem-0.2.0/src/pyfem/io/write_hdf5.py
+-rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.0/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.156787 pyfem-0.2.0/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    21867 2024-03-28 07:30:52.000000 pyfem-0.2.0/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.0/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.0/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.169787 pyfem-0.2.0/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     3135 2024-04-17 07:21:32.000000 pyfem-0.2.0/src/pyfem/materials/DiffusionIsotropic.py
+-rw-rw-rw-   0        0        0     8776 2024-03-11 03:57:52.000000 pyfem-0.2.0/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3135 2023-11-02 07:24:49.000000 pyfem-0.2.0/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2174 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0    79933 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/materials/PlasticCrystal.py
+-rw-rw-rw-   0        0        0    91044 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/materials/PlasticCrystalGNDs.py
+-rw-rw-rw-   0        0        0     8404 2023-09-21 06:20:49.000000 pyfem-0.2.0/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2773 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0     6137 2023-09-19 06:25:05.000000 pyfem-0.2.0/src/pyfem/materials/UMAT.py
+-rw-rw-rw-   0        0        0    10058 2023-10-27 05:19:05.000000 pyfem-0.2.0/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0    41881 2023-09-26 03:18:28.000000 pyfem-0.2.0/src/pyfem/materials/crystal_slip_system.py
+-rw-rw-rw-   0        0        0     2613 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.171787 pyfem-0.2.0/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.0/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.179287 pyfem-0.2.0/src/pyfem/quadrature/
+-rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/BaseQuadrature.py
+-rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/GaussLegendreQuadrature.py
+-rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/PyramidQuadrature.py
+-rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadrature.py
+-rw-rw-rw-   0        0        0    27075 2024-03-28 07:27:55.000000 pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadrature.py
+-rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.185287 pyfem-0.2.0/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0    15033 2024-04-18 07:31:18.000000 pyfem-0.2.0/src/pyfem/solvers/ArcLengthSolver.py
+-rw-rw-rw-   0        0        0     1450 2023-11-01 04:20:15.000000 pyfem-0.2.0/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.0/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0    16306 2024-04-18 07:30:49.000000 pyfem-0.2.0/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0    17321 2024-04-18 07:30:42.000000 pyfem-0.2.0/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-04-15 07:19:03.000000 pyfem-0.2.0/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.191787 pyfem-0.2.0/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-11-02 07:37:35.000000 pyfem-0.2.0/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.0/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0    28928 2024-01-17 03:42:50.000000 pyfem-0.2.0/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1183 2023-11-01 09:41:59.000000 pyfem-0.2.0/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.111287 pyfem-0.2.0/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     3579 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3243 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.1.9/LICENSE` & `pyfem-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/PKG-INFO` & `pyfem-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.1.9/README.md` & `pyfem-0.2.0/src/pyfem.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pyfem
+Version: 0.2.0
+Summary: Python Finite Element Method
+Home-page: https://github.com/sunwhale/pyfem
+Author: Jingyu Sun
+Author-email: sun.jingyu@outlook.com
+Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyfem
 
 pyfem是一个完全基于python语言实现的极简有限元求解器。依赖的第三方库包括numpy、scipy和meshio等，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
 
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
```

### Comparing `pyfem-0.1.9/setup.py` & `pyfem-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/Job.py` & `pyfem-0.2.0/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/__main__.py` & `pyfem-0.2.0/src/pyfem/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.2.0/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.2.0/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.2.0/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/assembly/Assembly.py` & `pyfem-0.2.0/src/pyfem/assembly/Assembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 
 """
+import time
+
 from numpy import repeat, array, ndarray, empty, zeros
 from scipy.sparse import coo_matrix, csc_matrix  # type: ignore
 
 from pyfem.bc.get_bc_data import get_bc_data, BCData
 from pyfem.elements.get_element_data import get_element_data, ElementData
 from pyfem.fem.Timer import Timer
-from pyfem.fem.constants import DTYPE
+from pyfem.fem.constants import DTYPE, IS_PETSC
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.Material import Material
 from pyfem.io.Properties import Properties
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import iso_element_shape_dict
 from pyfem.isoelements.get_iso_element_type import get_iso_element_type
 from pyfem.materials.get_material_data import get_material_data
@@ -51,20 +53,26 @@
 
     :ivar bc_data_list: 边界条件数据对象列表
     :vartype bc_data_list: list[BCData]
 
     :ivar global_stiffness: 全局刚度矩阵
     :vartype global_stiffness: csc_matrix(total_dof_number, total_dof_number)
 
+    :ivar A: 全局刚度矩阵
+    :vartype A: petsc4py.PETSc.Mat(total_dof_number, total_dof_number)
+
     :ivar fext: 等式右边外力向量
     :vartype fext: ndarray(total_dof_number,)
 
     :ivar fint: 内力向量
     :vartype fint: ndarray(total_dof_number,)
 
+    :ivar ftime: 时间离散导致的等式右边外力向量
+    :vartype ftime: ndarray(total_dof_number,)
+
     :ivar dof_solution: 全局自由度的值
     :vartype dof_solution: ndarray(total_dof_number,)
 
     :ivar ddof_solution: 全局自由度增量的值
     :vartype ddof_solution: ndarray(total_dof_number,)
 
     :ivar bc_dof_ids: 边界自由度列表
@@ -81,20 +89,22 @@
         'materials_dict': ('dict[str, Material]', '材料字典：材料名称->材料属性对象'),
         'sections_dict': ('dict[str, Section]', '截面字典：截面名称->截面属性对象'),
         'amplitudes_dict': ('dict[str, Amplitude]', '幅值字典：幅值名称->幅值属性对象'),
         'section_of_element_set': ('dict[str, Section]', '单元集合截面字典：单元集合名称->截面属性对象'),
         'element_data_list': ('list[ElementData]', '单元数据对象列表'),
         'bc_data_list': ('list[BCData]', '边界条件数据对象列表'),
         'global_stiffness': ('csc_matrix(total_dof_number, total_dof_number)', '全局刚度矩阵'),
+        'A': ('petsc4py.PETSc.Mat(total_dof_number, total_dof_number)', '全局刚度矩阵'),
         'fext': ('ndarray(total_dof_number,)', '等式右边外力向量'),
         'fint': ('ndarray(total_dof_number,)', '内力向量'),
+        'ftime': ('ndarray(total_dof_number,)', '时间离散导致的等式右边外力向量'),
         'dof_solution': ('ndarray(total_dof_number,)', '全局自由度的值'),
         'ddof_solution': ('ndarray(total_dof_number,)', '全局自由度增量的值'),
         'bc_dof_ids': ('ndarray', '边界自由度列表'),
-        'field_variables': ('dict[str, ndarray]', '常变量字典')
+        'field_variables': ('dict[str, ndarray]', '常变量字典'),
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, props: Properties) -> None:
         self.total_dof_number: int = -1
         self.props: Properties = props
@@ -102,16 +112,24 @@
         self.materials_dict: dict[str, Material] = dict()
         self.sections_dict: dict[str, Section] = dict()
         self.amplitudes_dict: dict[str, Amplitude] = dict()
         self.section_of_element_set: dict[str, Section] = dict()
         self.element_data_list: list[ElementData] = list()
         self.bc_data_list: list[BCData] = list()
         self.global_stiffness: csc_matrix = csc_matrix(0)
+        if IS_PETSC:
+            try:
+                from petsc4py import PETSc  # type: ignore
+                from petsc4py.PETSc import Mat  # type: ignore
+            except:
+                raise ImportError(error_style('petsc4py can not be imported'))
+            self.A: Mat = PETSc.Mat()
         self.fext: ndarray = empty(0, dtype=DTYPE)
         self.fint: ndarray = empty(0, dtype=DTYPE)
+        self.ftime: ndarray = empty(0, dtype=DTYPE)
         self.dof_solution: ndarray = empty(0, dtype=DTYPE)
         self.ddof_solution: ndarray = empty(0, dtype=DTYPE)
         self.bc_dof_ids: ndarray = empty(0)
         self.field_variables: dict[str, ndarray] = dict()
         self.init()
         self.update_element_data()
         self.assembly_global_stiffness()
@@ -210,36 +228,47 @@
         self.fext = zeros(self.total_dof_number, dtype=DTYPE)
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         self.dof_solution = zeros(self.total_dof_number, dtype=DTYPE)
         self.ddof_solution = zeros(self.total_dof_number, dtype=DTYPE)
 
     # @show_running_time
     def assembly_global_stiffness(self) -> None:
-        val = []
-        row = []
-        col = []
+        if IS_PETSC:
+            self.A.createAIJ((self.total_dof_number, self.total_dof_number))
+            for element_data in self.element_data_list:
+                element_dof_ids = element_data.element_dof_ids
+                self.A.setValues(element_dof_ids, element_dof_ids, element_data.element_stiffness, addv=True)
+            self.A.assemble()
+
+        else:
+            val = []
+            row = []
+            col = []
+
+            for element_data in self.element_data_list:
+                element_dof_ids = element_data.element_dof_ids
+                element_dof_number = element_data.element_dof_number
+                row += [r for r in repeat(element_dof_ids, element_dof_number)]
+                for _ in range(element_dof_number):
+                    col += [c for c in element_dof_ids]
+                val += [v for v in element_data.element_stiffness.reshape(element_dof_number * element_dof_number)]
 
-        for element_data in self.element_data_list:
-            element_dof_ids = element_data.element_dof_ids
-            element_dof_number = element_data.element_dof_number
-            row += [r for r in repeat(element_dof_ids, element_dof_number)]
-            for _ in range(element_dof_number):
-                col += [c for c in element_dof_ids]
-            val += [v for v in element_data.element_stiffness.reshape(element_dof_number * element_dof_number)]
-
-        self.global_stiffness = coo_matrix(
-            (array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))),
-            shape=(self.total_dof_number, self.total_dof_number)).tocsc()
+            self.global_stiffness = coo_matrix((array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))), shape=(self.total_dof_number, self.total_dof_number)).tocsr()
 
     # @show_running_time
     def assembly_fint(self) -> None:
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         for element_data in self.element_data_list:
             self.fint[element_data.element_dof_ids] += element_data.element_fint
 
+    def assembly_ftime(self) -> None:
+        self.ftime = zeros(self.total_dof_number, dtype=DTYPE)
+        for element_data in self.element_data_list:
+            self.ftime[element_data.element_dof_ids] += element_data.element_ftime
+
     # @show_running_time
     def update_element_data(self) -> None:
         dof_solution = self.dof_solution
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/BaseBC.py` & `pyfem-0.2.0/src/pyfem/bc/BaseBC.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         else:
             self.amplitude_data = BaseAmplitude()
             self.amplitude_data.set_f_amplitude([0, solver.total_time], [0, 1])
         self.get_amplitude: Callable = self.amplitude_data.get_amplitude
         self.bc_node_ids: ndarray = empty(0)
         self.bc_element_ids: ndarray = empty(0)
         self.bc_surface: list[tuple[int, str]] = list()
-        self.bc_dof_ids: ndarray = empty(0)
+        self.bc_dof_ids: ndarray = empty(0, dtype='int32')
         self.bc_dof_values: ndarray = empty(0)
         self.bc_fext: ndarray = empty(0)
 
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/DirichletBC.py` & `pyfem-0.2.0/src/pyfem/bc/DirichletBC.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,32 +36,35 @@
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
         for bc_node_set in bc_node_sets:
             bc_node_ids += list(self.mesh_data.node_sets[bc_node_set])
 
         # 如果发现施加当前边界条件的点集中有重复的点则抛出异常
         if len(bc_node_ids) != len(set(bc_node_ids)):
-            error_msg = f'{type(self).__name__} {self.bc.name} contains repeat nodes\n'
+            error_msg = f'{type(self).__name__} \'{self.bc.name}\' contains repeat nodes\n'
             error_msg += f'Please check the input file'
             raise NotImplementedError(error_style(error_msg))
         else:
             self.bc_node_ids = array(bc_node_ids)
 
         # 确定施加的边界条件对应的全局自由度编号
         bc_dof_names = self.bc.dof
         dof_names = self.dof.names
         bc_dof_ids = []
         for node_index in self.bc_node_ids:
             for _, bc_dof_name in enumerate(bc_dof_names):
                 bc_dof_ids.append(node_index * len(dof_names) + dof_names.index(bc_dof_name))
-        self.bc_dof_ids = array(bc_dof_ids)
+        self.bc_dof_ids = array(bc_dof_ids, dtype='int32')
 
         bc_value = self.bc.value
-        if isinstance(bc_value, float):
+        if isinstance(bc_value, float) or isinstance(bc_value, int):
             self.bc_dof_values = array([bc_value for _ in self.bc_dof_ids])
+        else:
+            error_msg = f'in {type(self).__name__} \'{self.bc.name}\' the value of \'{bc_value}\' is not a float or int number'
+            raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.2.0/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,32 +36,35 @@
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
         for bc_node_set in bc_node_sets:
             bc_node_ids += list(self.mesh_data.node_sets[bc_node_set])
 
         # 如果发现施加当前边界条件的点集中有重复的点则抛出异常
         if len(bc_node_ids) != len(set(bc_node_ids)):
-            error_msg = f'{type(self).__name__} {self.bc.name} contains repeat nodes\n'
+            error_msg = f'{type(self).__name__} \'{self.bc.name}\' contains repeat nodes\n'
             error_msg += f'Please check the input file'
             raise NotImplementedError(error_style(error_msg))
         else:
             self.bc_node_ids = array(bc_node_ids)
 
         # 确定施加的边界条件对应的全局自由度编号
         bc_dof_names = self.bc.dof
         dof_names = self.dof.names
         bc_dof_ids = []
         for node_index in self.bc_node_ids:
             for _, bc_dof_name in enumerate(bc_dof_names):
                 bc_dof_ids.append(node_index * len(dof_names) + dof_names.index(bc_dof_name))
-        self.bc_dof_ids = array(bc_dof_ids)
+        self.bc_dof_ids = array(bc_dof_ids, dtype='int32')
 
         bc_value = self.bc.value
-        if isinstance(bc_value, float):
+        if isinstance(bc_value, float) or isinstance(bc_value, int):
             self.bc_fext = array([bc_value for _ in self.bc_dof_ids])
+        else:
+            error_msg = f'in {type(self).__name__} \'{self.bc.name}\' the value of \'{bc_value}\' is not a float or int number'
+            raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\quad8\Job-1.toml')
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.2.0/src/pyfem/bc/NeumannBCDistributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,17 @@
         elements = self.mesh_data.elements
         bc_elements = self.mesh_data.bc_elements
 
         node_sets = self.bc.node_sets
         element_sets = self.bc.element_sets
         bc_element_sets = self.bc.bc_element_sets
         bc_value = self.bc.value
+        if not (isinstance(bc_value, float) or isinstance(bc_value, int)):
+            error_msg = f'in {type(self).__name__} \'{self.bc.name}\' the value of \'{bc_value}\' is not a float or int number'
+            raise NotImplementedError(error_style(error_msg))
 
         if bc_element_sets is not None:
             bc_element_ids = []
             for bc_element_set in bc_element_sets:
                 bc_element_ids += list(self.mesh_data.bc_element_sets[bc_element_set])
             for bc_element_id in set(bc_element_ids):
                 self.bc_surface += self.get_surface_from_bc_element(bc_element_id, bc_elements[bc_element_id])
@@ -360,15 +363,15 @@
             surface_fext = []
             for fext in element_fext[surface_local_nodes]:
                 for _ in range(len(bc_dof_names)):
                     surface_fext.append(fext)
 
             bc_fext += list(surface_fext)
 
-        self.bc_dof_ids = array(bc_dof_ids)
+        self.bc_dof_ids = array(bc_dof_ids, dtype='int32')
         self.bc_fext = array(bc_fext)
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     # props = Properties()
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/NeumannBCPressure.py` & `pyfem-0.2.0/src/pyfem/bc/NeumannBCPressure.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         elements = self.mesh_data.elements
         bc_elements = self.mesh_data.bc_elements
 
         node_sets = self.bc.node_sets
         element_sets = self.bc.element_sets
         bc_element_sets = self.bc.bc_element_sets
         bc_value = self.bc.value
+        if not (isinstance(bc_value, float) or isinstance(bc_value, int)):
+            error_msg = f'in {type(self).__name__} \'{self.bc.name}\' the value of \'{bc_value}\' is not a float or int number'
+            raise NotImplementedError(error_style(error_msg))
 
         if bc_element_sets is not None:
             bc_element_ids = []
             for bc_element_set in bc_element_sets:
                 bc_element_ids += list(self.mesh_data.bc_element_sets[bc_element_set])
             for bc_element_id in set(bc_element_ids):
                 self.bc_surface += self.get_surface_from_bc_element(bc_element_id, bc_elements[bc_element_id])
@@ -172,22 +175,22 @@
             element_fext = zeros(nodes_number * len(self.bc.dof))
 
             for i in range(bc_qp_number):
                 bc_qp_jacobi = dot(bc_qp_shape_gradients[i], node_coords).transpose()  # 此处雅克比矩阵的行列式为体积比
                 bc_qp_jacobi_sub = delete(bc_qp_jacobi, bc_surface_coord[0], axis=1)
                 surface_weight = bc_surface_coord[3]
                 if dimension == 2:
-                    sigma = -array([[0, bc_value],
-                                    [-bc_value, 0]])
+                    sigma = -array([[0.0, bc_value],
+                                    [-bc_value, 0.0]])
                     sigma_times_jacobi = (dot(sigma, bc_qp_jacobi_sub)).transpose()
                     element_fext += (dot(bc_qp_shape_values[i].reshape(1, -1).transpose(), sigma_times_jacobi) *
                                      bc_qp_weights[i] * bc_surface_coord[2] * surface_weight * sign(det(bc_qp_jacobi))).reshape(-1)
 
                 elif dimension == 3:
-                    sigma = -bc_value
+                    sigma = -bc_value  # type: ignore
                     if surface_weight == 1:
                         for row in range(bc_qp_jacobi_sub.shape[0]):
                             s = det(delete(bc_qp_jacobi_sub, row, axis=0)) * (-1) ** row
                             qp_fext = (bc_qp_shape_values[i].reshape(1, -1).transpose() * bc_qp_weights[i] * sigma * s *
                                        bc_surface_coord[2] * surface_weight * sign(det(bc_qp_jacobi))).reshape(-1)
                             element_dof_ids = [i * len(dof_names) + row for i in range(nodes_number)]
                             element_fext[element_dof_ids] += qp_fext
@@ -215,15 +218,15 @@
 
             surface_fext = []
             for fext in element_fext[surface_local_dof_ids]:
                 surface_fext.append(fext)
 
             bc_fext += list(surface_fext)
 
-        self.bc_dof_ids = array(bc_dof_ids)
+        self.bc_dof_ids = array(bc_dof_ids, dtype='int32')
         self.bc_fext = array(bc_fext)
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     # props = Properties()
```

### Comparing `pyfem-0.1.9/src/pyfem/bc/derive_surface_integral.py` & `pyfem-0.2.0/src/pyfem/bc/derive_surface_integral.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/bc/get_bc_data.py` & `pyfem-0.2.0/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/elements/BaseElement.py` & `pyfem-0.2.0/src/pyfem/elements/BaseElement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
 
-from numpy import dot, ndarray
-from numpy.linalg import det
+from numpy import dot, ndarray, array, ones, concatenate, transpose, einsum
+from numpy.linalg import det, inv
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
@@ -24,14 +24,20 @@
 
     :ivar element_id: 单元序号
     :vartype element_id: int
 
     :ivar iso_element_shape: 等参元对象
     :vartype iso_element_shape: IsoElementShape
 
+    :ivar dimension: 单元空间维度
+    :vartype dimension: int
+
+    :ivar topological_dimension: 单元拓扑维度
+    :vartype topological_dimension: int
+
     :ivar connectivity: 单元节点序号列表
     :vartype connectivity: ndarray
 
     :ivar node_coords: 单元节点坐标列表
     :vartype node_coords: ndarray
 
     :ivar assembly_conn: 全局单元节点序号列表
@@ -54,14 +60,17 @@
 
     :ivar dof_names: 自由度名称列表
     :vartype dof_names: list[str]
 
     :ivar qp_number: 积分点个数
     :vartype qp_number: int
 
+    :ivar qp_dhdxes: 积分点处的全局坐标形函数梯度
+    :vartype qp_dhdxes: ndarray(qp_number, 空间维度, 单元节点数)
+
     :ivar qp_jacobis: 积分点处的雅克比矩阵列表
     :vartype qp_jacobis: ndarray(qp_number, 空间维度, 空间维度)
 
     :ivar qp_jacobi_invs: 积分点处的雅克比矩阵逆矩阵列表
     :vartype qp_jacobi_invs: ndarray(qp_number,)
 
     :ivar qp_jacobi_dets: 积分点处的雅克比矩阵行列式列表
@@ -93,14 +102,17 @@
 
     :ivar element_ddof_values: 单元全局自由度数值增量列表
     :vartype element_ddof_values: ndarray(element_dof_number,)
 
     :ivar element_fint: 单元内力列表
     :vartype element_fint: ndarray(element_dof_number,)
 
+    :ivar element_ftime: 单元时间离散外力列表
+    :vartype element_ftime: ndarray(element_dof_number,)
+
     :ivar element_stiffness: 单元刚度矩阵
     :vartype element_stiffness: ndarray(element_dof_number, element_dof_number)
 
     :ivar element_average_field_variables: 单元磨平后的场变量字典
     :vartype element_average_field_variables: dict[str, ndarray]
 
     :ivar allowed_material_data_list: 许可的单元材料数据类名列表
@@ -121,27 +133,29 @@
         'dof': ('Dof', 'io.Dof的自由度对象'),
         'materials': ('list[Material]', 'io.Material的材料对象列表'),
         'section': ('list[Section]', 'io.Section的截面对象列表'),
         'material_data_list': ('list[MaterialData]', '材料数据对象列表'),
         'timer': ('Timer', '计时器对象'),
         'dof_names': ('list[str]', '自由度名称列表'),
         'qp_number': ('int', '积分点个数'),
+        'qp_dhdxes': ('ndarray(qp_number, 空间维度, 单元节点数)', '积分点处的全局坐标形函数梯度'),
         'qp_jacobis': ('ndarray(qp_number, 空间维度, 空间维度)', '积分点处的雅克比矩阵列表'),
         'qp_jacobi_invs': ('ndarray(qp_number,)', '积分点处的雅克比矩阵逆矩阵列表'),
         'qp_jacobi_dets': ('ndarray(qp_number,)', '积分点处的雅克比矩阵行列式列表'),
         'qp_weight_times_jacobi_dets': ('ndarray(qp_number,)', '积分点处的雅克比矩阵行列式乘以积分权重列表'),
         'qp_ddsddes': ('ndarray', '积分点处的材料刚度矩阵列表'),
         'qp_state_variables': ('list[dict[str, ndarray]]', '积分点处的状态变量列表'),
         'qp_state_variables_new': ('list[dict[str, ndarray]]', '积分点处局部增量时刻的状态变量列表'),
         'qp_field_variables': ('dict[str, ndarray]', '积分点处场变量字典'),
         'element_dof_number': ('int', '单元自由度总数'),
         'element_dof_ids': ('list[int]', '单元全局自由度编号列表'),
         'element_dof_values': ('ndarray(element_dof_number,)', '单元全局自由度数值列表'),
         'element_ddof_values': ('ndarray(element_dof_number,)', '单元全局自由度数值增量列表'),
         'element_fint': ('ndarray(element_dof_number,)', '单元内力列表'),
+        'element_ftime': ('ndarray(element_dof_number,)', '单元时间离散外力列表'),
         'element_stiffness': ('ndarray(element_dof_number, element_dof_number)', '单元刚度矩阵'),
         'element_average_field_variables': ('dict[str, ndarray]', '单元磨平后的场变量字典'),
         'allowed_material_data_list': ('list[Tuple]', '许可的单元材料数据类名列表'),
         'allowed_material_number': ('int', '许可的单元材料数量')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
@@ -163,14 +177,15 @@
         self.section: Section = None  # type: ignore
         self.material_data_list: list[MaterialData] = None  # type: ignore
         self.timer: Timer = None  # type: ignore
 
         self.dof_names: list[str] = list()
 
         self.qp_number: int = self.iso_element_shape.qp_number
+        self.qp_dhdxes: ndarray = None  # type: ignore
         self.qp_jacobis: ndarray = None  # type: ignore
         self.qp_jacobi_invs: ndarray = None  # type: ignore
         self.qp_jacobi_dets: ndarray = None  # type: ignore
         self.qp_weight_times_jacobi_dets: ndarray = None  # type: ignore
         self.qp_ddsddes: list[ndarray] = list()
         self.qp_state_variables: list[dict[str, ndarray]] = [{} for _ in range(self.qp_number)]
         self.qp_state_variables_new: list[dict[str, ndarray]] = [{} for _ in range(self.qp_number)]
@@ -178,14 +193,15 @@
         self.cal_jacobi()
 
         self.element_dof_number: int = 0
         self.element_dof_ids: list[int] = list()
         self.element_dof_values: ndarray = None  # type: ignore
         self.element_ddof_values: ndarray = None  # type: ignore
         self.element_fint: ndarray = None  # type: ignore
+        self.element_ftime: ndarray = None  # type: ignore
         self.element_stiffness: ndarray = None  # type: ignore
         self.element_average_field_variables: dict[str, ndarray] = dict()
 
         self.allowed_material_data_list: list[tuple] = list()
         self.allowed_material_number: int = 0
 
     def to_string(self, level: int = 1) -> str:
@@ -261,34 +277,64 @@
               {{x_1}}&{{y_1}}&{{z_1}} \\
                \vdots & \vdots & \vdots  \\
               {{x_n}}&{{y_n}}&{{z_n}}
             \end{array}} \right]}_{{\text{node_coords}}}} \right)^T}
 
         """
 
-        # 以下代码为采用for循环的计算方法，结构清晰，但计算效率较低
-        # self.qp_jacobis = []
-        # self.qp_jacobi_invs = []
-        # self.qp_jacobi_dets = []
-        # for qp_shape_gradient in self.iso_element_shape.qp_shape_gradients:
-        #     jacobi = dot(qp_shape_gradient, self.node_coords).transpose()
-        #     self.qp_jacobis.append(jacobi)
-        #     self.qp_jacobi_invs.append(inv(jacobi))
-        #     self.qp_jacobi_dets.append(det(jacobi))
-        # self.qp_jacobis = array(self.qp_jacobis)
-        # self.qp_jacobi_invs = array(self.qp_jacobi_invs)
-        # self.qp_jacobi_dets = array(self.qp_jacobi_dets)
-
-        # 以下代码为采用numpy高维矩阵乘法的计算方法，计算效率高，但要注意矩阵维度的变化
-        self.qp_jacobis = dot(self.iso_element_shape.qp_shape_gradients, self.node_coords).swapaxes(1, 2)
-        self.qp_jacobi_dets = det(self.qp_jacobis)
-
-        # qp_jacobi通常为2×2或3×3的方阵，可以直接根据解析式求逆矩阵，计算效率比numpy.linalg.inv()函数更高
-        self.qp_jacobi_invs = inverse(self.qp_jacobis, self.qp_jacobi_dets)
-        self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets
+        if self.iso_element_shape.coord_type == 'cartesian':
+            # 以下代码为采用for循环的计算方法，结构清晰，但计算效率较低
+            # self.qp_jacobis = []
+            # self.qp_jacobi_invs = []
+            # self.qp_jacobi_dets = []
+            # for qp_shape_gradient in self.iso_element_shape.qp_shape_gradients:
+            #     print(qp_shape_gradient.shape, self.node_coords.shape)
+            #     jacobi = dot(qp_shape_gradient, self.node_coords).transpose()
+            #     self.qp_jacobis.append(jacobi)
+            #     self.qp_jacobi_invs.append(inv(jacobi))
+            #     self.qp_jacobi_dets.append(det(jacobi))
+            # self.qp_jacobis = array(self.qp_jacobis)
+            # self.qp_jacobi_invs = array(self.qp_jacobi_invs)
+            # self.qp_jacobi_dets = array(self.qp_jacobi_dets)
+
+            # 以下代码为采用numpy高维矩阵乘法的计算方法，计算效率高，但要注意矩阵维度的变化
+            # self.qp_jacobis = dot(self.iso_element_shape.qp_shape_gradients, self.node_coords).swapaxes(1, 2)
+
+            # 以下代码为采用numpy爱因斯坦求和约定函数einsum，更简洁明了
+            self.qp_jacobis = einsum('ijk,kl->ilj', self.iso_element_shape.qp_shape_gradients, self.node_coords)
+            self.qp_jacobi_dets = det(self.qp_jacobis)
+            # qp_jacobi通常为2×2或3×3的方阵，可以直接根据解析式求逆矩阵，计算效率比numpy.linalg.inv()函数更高
+            self.qp_jacobi_invs = inverse(self.qp_jacobis, self.qp_jacobi_dets)
+            self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets
+
+            # qp_dhdxes = []
+            # for iqp, (qp_shape_gradient, qp_jacobi_inv) in enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
+            #     qp_dhdxes.append(dot(qp_shape_gradient.transpose(), qp_jacobi_inv))
+            # self.qp_dhdxes = array(qp_dhdxes)
+            self.qp_dhdxes = einsum('...ij,...ik->...kj', self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)
+
+        elif self.iso_element_shape.coord_type == 'barycentric':
+            self.qp_jacobis = dot(self.iso_element_shape.qp_shape_gradients, self.node_coords).swapaxes(1, 2)
+            new_rows = ones((self.qp_jacobis.shape[0], 1, self.qp_jacobis.shape[2]))
+            self.qp_jacobis = concatenate((new_rows, self.qp_jacobis), axis=1)
+            if self.dimension == 2:
+                a = array([[0.0, 0.0], [1.0, 0.0], [0.0, 1.0]])
+            elif self.dimension == 3:
+                a = array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
+            else:
+                raise NotImplementedError(error_style(f'dimension {self.dimension} is not support for the barycentric coordinates'))
+            self.qp_jacobi_dets = det(self.qp_jacobis)
+            self.qp_jacobi_invs = inverse(self.qp_jacobis, self.qp_jacobi_dets)
+            self.qp_jacobi_invs = dot(self.qp_jacobi_invs, a)
+            if self.dimension == 2:
+                self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets / 2.0
+            elif self.dimension == 3:
+                self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets / 6.0
+            else:
+                raise NotImplementedError(error_style(f'dimension {self.dimension} is not support for the barycentric coordinates'))
 
     def create_element_dof_ids(self) -> None:
         for node_index in self.assembly_conn:
             for dof_id, _ in enumerate(self.dof_names):
                 self.element_dof_ids.append(node_index * len(self.dof_names) + dof_id)
 
     def check_materials(self) -> None:
```

### Comparing `pyfem-0.1.9/src/pyfem/elements/SolidFiniteStrain.py` & `pyfem-0.2.0/src/pyfem/elements/SolidFiniteStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1236,15 +1236,15 @@
                 self.qp_strains.append(qp_strain)
                 self.qp_stresses.append(qp_stress)
             else:
                 qp_ddsdde = self.qp_ddsddes[i]
                 qp_stress = self.qp_stresses[i]
 
             if is_update_stiffness:
-                qp_stress_matrix = self.vogit_to_block_diagonal_matrix(qp_stress)
+                qp_stress_matrix = self.voigt_to_block_diagonal_matrix(qp_stress)
                 if self.method == 'TL':
                     self.element_stiffness += dot(qp_b_matrix_transpose, dot(qp_ddsdde, qp_b_matrix)) * qp_weight_times_jacobi_det
                     self.element_stiffness += dot(qp_bnl_matrix_transpose, dot(qp_stress_matrix, qp_bnl_matrix)) * qp_weight_times_jacobi_det
                 elif self.method == 'UL':
                     self.element_stiffness += dot(qp_b_matrix_transpose, dot(qp_ddsdde, qp_b_matrix)) * self.qp_weight_times_jacobi_dets_t[i]
                     self.element_stiffness += dot(qp_bnl_matrix_transpose, dot(qp_stress_matrix, qp_bnl_matrix)) * self.qp_weight_times_jacobi_dets_t[i]
 
@@ -1282,15 +1282,15 @@
             self.element_average_field_variables['S11'] = average_stress[0]
             self.element_average_field_variables['S22'] = average_stress[1]
             self.element_average_field_variables['S33'] = average_stress[2]
             self.element_average_field_variables['S12'] = average_stress[3]
             self.element_average_field_variables['S13'] = average_stress[4]
             self.element_average_field_variables['S23'] = average_stress[5]
 
-    def vogit_to_block_diagonal_matrix(self, stress):
+    def voigt_to_block_diagonal_matrix(self, stress):
         T = zeros(shape=(self.dimension * self.dimension, self.dimension * self.dimension))
 
         if self.dimension == 2:
             T[0, 0] = stress[0]
             T[1, 1] = stress[1]
             T[0, 1] = stress[2]
             T[1, 0] = stress[2]
```

### Comparing `pyfem-0.1.9/src/pyfem/elements/SolidPhaseDamageSmallStrain.py` & `pyfem-0.2.0/src/pyfem/elements/SolidPhaseDamageSmallStrain.py`

 * *Files 12% similar despite different names*

```diff
@@ -152,29 +152,25 @@
                 self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1, len(self.dof_names) * i + 2]
                 self.dof_p += [len(self.dof_names) * i + 3]
         self.create_qp_b_matrices()
 
     def create_qp_b_matrices(self) -> None:
         if self.dimension == 2:
             self.qp_b_matrices = zeros(shape=(self.qp_number, 3, len(self.dof_u)), dtype=DTYPE)
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
                     self.qp_b_matrices[iqp, 0, i * 2 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 2 + 1] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 2 + 0] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 2 + 1] = val[0]
 
         elif self.dimension == 3:
-            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, len(self.dof_u)))
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
+            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, len(self.dof_u)), dtype=DTYPE)
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
                     self.qp_b_matrices[iqp, 0, i * 3 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 3 + 1] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 3 + 2] = val[2]
                     self.qp_b_matrices[iqp, 3, i * 3 + 0] = val[1]
                     self.qp_b_matrices[iqp, 3, i * 3 + 1] = val[0]
                     self.qp_b_matrices[iqp, 4, i * 3 + 0] = val[2]
                     self.qp_b_matrices[iqp, 4, i * 3 + 2] = val[0]
@@ -194,14 +190,16 @@
         nshr = self.nshr
 
         dimension = self.iso_element_shape.dimension
 
         qp_number = self.qp_number
         qp_shape_values = self.iso_element_shape.qp_shape_values
         qp_shape_gradients = self.iso_element_shape.qp_shape_gradients
+        qp_dhdxes = self.qp_dhdxes
+
         qp_b_matrices = self.qp_b_matrices
         qp_b_matrices_transpose = self.qp_b_matrices_transpose
         qp_jacobi_invs = self.qp_jacobi_invs
         qp_weight_times_jacobi_dets = self.qp_weight_times_jacobi_dets
 
         qp_state_variables = self.qp_state_variables
         qp_state_variables_new = self.qp_state_variables_new
@@ -237,28 +235,27 @@
             self.qp_energies = list()
 
         for i in range(qp_number):
             if is_update_material:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
                 qp_shape_gradient = qp_shape_gradients[i]
+                qp_dhdx = qp_dhdxes[i]
                 qp_b_matrix_transpose = qp_b_matrices_transpose[i]
                 qp_b_matrix = qp_b_matrices[i]
                 qp_strain = dot(qp_b_matrix, u)
                 qp_dstrain = dot(qp_b_matrix, du)
                 qp_phase = dot(qp_shape_value, phi)
                 qp_dphase = dot(qp_shape_value, dphi)
                 qp_phase_gradient = dot(qp_shape_gradient, phi)
                 qp_dphase_gradient = dot(qp_shape_gradient, dphi)
-                qp_jacobi_inv = qp_jacobi_invs[i]
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
 
-                degradation = (1.0 - qp_phase) ** 2 + 1.0e-7
-                degradation = min(degradation, 1.0)
-                degradation = max(degradation, 0.0)
+                qp_degradation = (1.0 - qp_phase) ** 2 + 1.0e-8
+                qp_degradation = min(qp_degradation, 1.0)
+                qp_degradation = max(qp_degradation, 0.0)
 
                 variable = {'strain': qp_strain, 'dstrain': qp_dstrain}
                 qp_ddsdde, qp_output = solid_material_data.get_tangent(variable=variable,
                                                                        state_variable=qp_state_variables[i],
                                                                        state_variable_new=qp_state_variables_new[i],
                                                                        element_id=element_id,
                                                                        iqp=i,
@@ -266,15 +263,15 @@
                                                                        ndi=ndi,
                                                                        nshr=nshr,
                                                                        timer=timer)
                 qp_stress = qp_output['stress']
                 qp_strain_energy = qp_output['strain_energy']
                 self.qp_ddsddes.append(qp_ddsdde)
                 self.qp_strains.append(qp_strain)
-                self.qp_stresses.append(qp_stress * degradation)
+                self.qp_stresses.append(qp_stress * qp_degradation)
                 self.qp_phases.append(qp_phase)
 
             else:
                 qp_b_matrix_transpose = qp_b_matrices_transpose[i]
                 qp_b_matrix = qp_b_matrices[i]
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
@@ -286,48 +283,52 @@
                 qp_phase = dot(qp_shape_value, phi)
                 qp_dphase = dot(qp_shape_value, dphi)
                 qp_phase_gradient = dot(qp_shape_gradient, phi)
                 qp_dphase_gradient = dot(qp_shape_gradient, dphi)
                 qp_jacobi_inv = qp_jacobi_invs[i]
                 qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
 
-                degradation = (1.0 - qp_phase) ** 2 + 1.0e-7
-                degradation = min(degradation, 1.0)
-                degradation = max(degradation, 0.0)
+                qp_degradation = (1.0 - qp_phase) ** 2 + 1.0e-8
+                qp_degradation = min(qp_degradation, 1.0)
+                qp_degradation = max(qp_degradation, 0.0)
 
-            energy_positive, energy_negative = get_decompose_energy(qp_strain + qp_dstrain, qp_stress, dimension)
+            # energy_positive, energy_negative = get_decompose_energy(qp_strain + qp_dstrain, qp_stress, dimension)
+            # energy_positive += qp_strain_energy
 
-            energy_positive += qp_strain_energy
+            energy_positive = 0.5 * sum((qp_strain + qp_dstrain) * qp_stress)
 
             if energy_positive < qp_state_variables[i]['history_energy'][0]:
                 energy_positive = qp_state_variables[i]['history_energy'][0]
 
+            if energy_positive < qp_state_variables_new[i]['history_energy'][0]:
+                energy_positive = qp_state_variables_new[i]['history_energy'][0]
+
             qp_state_variables_new[i]['history_energy'][0] = energy_positive
 
             self.qp_energies.append(energy_positive)
 
             if is_update_stiffness:
                 self.element_stiffness[ix_(self.dof_u, self.dof_u)] += qp_weight_times_jacobi_det * \
-                    dot(qp_b_matrix_transpose, dot(qp_ddsdde * degradation, qp_b_matrix))
+                                                                       dot(qp_b_matrix_transpose, dot(qp_ddsdde * qp_degradation, qp_b_matrix))
 
                 self.element_stiffness[ix_(self.dof_p, self.dof_p)] += qp_weight_times_jacobi_det * \
-                ((gc / lc + 2.0 * energy_positive) * outer(qp_shape_value, qp_shape_value) +
-                 gc * lc * dot(qp_shape_gradient.transpose(), qp_shape_gradient))
+                                                                       ((gc / lc + 2.0 * energy_positive) * outer(qp_shape_value, qp_shape_value) +
+                                                                        gc * lc * dot(qp_dhdx.transpose(), qp_dhdx))
 
-                # vecu = -2.0 * (1.0 - (qp_phase + qp_dphase)) * dot(qp_b_matrix_transpose, qp_stress * degradation) * qp_weight_times_jacobi_det
+                # vecu = -2.0 * (1.0 - (qp_phase + qp_dphase)) * dot(qp_b_matrix_transpose, qp_stress * qp_degradation) * qp_weight_times_jacobi_det
                 # self.element_stiffness[ix_(self.dof_u, self.dof_p)] += outer(vecu, qp_shape_value)
                 # self.element_stiffness[ix_(self.dof_p, self.dof_u)] += outer(qp_shape_value, vecu)
 
             if is_update_fint:
-                self.element_fint[self.dof_u] += dot(qp_b_matrix_transpose, qp_stress * degradation) * qp_weight_times_jacobi_det
+                self.element_fint[self.dof_u] += dot(qp_b_matrix_transpose, qp_stress * qp_degradation) * qp_weight_times_jacobi_det
 
                 self.element_fint[self.dof_p] += qp_weight_times_jacobi_det * \
-                    (gc * lc * dot(qp_shape_gradient.transpose(), (qp_phase_gradient + qp_dphase_gradient)) +
-                     gc / lc * (qp_phase + qp_dphase) * qp_shape_value +
-                     2.0 * ((qp_phase + qp_dphase) - 1.0) * energy_positive * qp_shape_value)
+                                                 (gc * lc * dot(qp_dhdx.transpose(), (qp_phase_gradient + qp_dphase_gradient)) +
+                                                  gc / lc * (qp_phase + qp_dphase) * qp_shape_value +
+                                                  2.0 * ((qp_phase + qp_dphase) - 1.0) * energy_positive * qp_shape_value)
 
     def update_element_field_variables(self) -> None:
         qp_stresses = self.qp_stresses
         qp_strains = self.qp_strains
         qp_energies = self.qp_energies
 
         average_strain = average(qp_strains, axis=0)
```

### Comparing `pyfem-0.1.9/src/pyfem/elements/SolidSmallStrain.py` & `pyfem-0.2.0/src/pyfem/elements/SolidSmallStrain.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/elements/SolidThermalSmallStrain.py` & `pyfem-0.2.0/src/pyfem/elements/SolidThermalSmallStrain.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/elements/Thermal.py` & `pyfem-0.2.0/src/pyfem/elements/Thermal.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/elements/get_element_data.py` & `pyfem-0.2.0/src/pyfem/elements/get_element_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,33 @@
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.SolidPhaseDamageSmallStrain import SolidPhaseDamageSmallStrain
 from pyfem.elements.SolidSmallStrain import SolidSmallStrain
 from pyfem.elements.SolidFiniteStrain import SolidFiniteStrain
 from pyfem.elements.SolidThermalSmallStrain import SolidThermalSmallStrain
 from pyfem.elements.Thermal import Thermal
+from pyfem.elements.Diffusion import Diffusion
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
 
 ElementData = Union[
-    BaseElement, SolidSmallStrain, SolidThermalSmallStrain, SolidPhaseDamageSmallStrain, Thermal]
+    BaseElement, SolidSmallStrain, SolidThermalSmallStrain, SolidPhaseDamageSmallStrain, Thermal, Diffusion]
 
 element_data_dict = {
     'SolidSmallStrain': SolidSmallStrain,
     'SolidFiniteStrain': SolidFiniteStrain,
     'SolidThermalSmallStrain': SolidThermalSmallStrain,
     'SolidPhaseDamageSmallStrain': SolidPhaseDamageSmallStrain,
     'Thermal': Thermal,
+    'Diffusion': Diffusion,
 }
 
 
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
```

### Comparing `pyfem-0.1.9/src/pyfem/fem/Timer.py` & `pyfem-0.2.0/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Amplitude.py` & `pyfem-0.2.0/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/BC.py` & `pyfem-0.2.0/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/BaseIO.py` & `pyfem-0.2.0/src/pyfem/io/BaseIO.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Dof.py` & `pyfem-0.2.0/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Material.py` & `pyfem-0.2.0/src/pyfem/io/Material.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     allowed_categories_types: dict = {
         None: [None],
         'Elastic': ['Isotropic'],
         'Plastic': ['KinematicHardening', 'Crystal', 'CrystalGNDs'],
         'ViscoElastic': ['Maxwell'],
         'Thermal': ['Isotropic'],
         'PhaseField': ['Damage'],
-        'MechanicalThermal': ['Expansion']
+        'MechanicalThermal': ['Expansion'],
+        'Diffusion': ['Isotropic'],
     }
 
     allowed_keys_values: dict = {
         'category': allowed_categories_types.keys(),
         'type': []
     }
```

### Comparing `pyfem-0.1.9/src/pyfem/io/Mesh.py` & `pyfem-0.2.0/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Module.py` & `pyfem-0.2.0/src/pyfem/io/Module.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Output.py` & `pyfem-0.2.0/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Parameter.py` & `pyfem-0.2.0/src/pyfem/io/Parameter.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Properties.py` & `pyfem-0.2.0/src/pyfem/io/Properties.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Section.py` & `pyfem-0.2.0/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/Solver.py` & `pyfem-0.2.0/src/pyfem/io/Solver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/arguments.py` & `pyfem-0.2.0/src/pyfem/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/write_hdf5.py` & `pyfem-0.2.0/src/pyfem/io/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/io/write_vtk.py` & `pyfem-0.2.0/src/pyfem/io/write_vtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,30 @@
                 disp.text += f"{u1} {u2} 0.0 \n"
         elif dimension == 3:
             for u1, u2, u3 in assembly.dof_solution.reshape(-1, len(props.dof.names))[:, 0:3]:
                 disp.text += f"{u1} {u2} {u3} \n"
         else:
             raise NotImplementedError
 
+        rf = SubElement(point_data, "DataArray", {
+            "type": "Float64",
+            "Name": "RF",
+            "NumberOfComponents": "3",
+            "format": "ascii"
+        })
+        rf.text = ""
+        if dimension == 2:
+            for rf1, rf2 in assembly.fint.reshape(-1, len(props.dof.names))[:, 0:2]:
+                rf.text += f"{rf1} {rf2} 0.0 \n"
+        elif dimension == 3:
+            for rf1, rf2, rf3 in assembly.fint.reshape(-1, len(props.dof.names))[:, 0:3]:
+                rf.text += f"{rf1} {rf2} {rf3} \n"
+        else:
+            raise NotImplementedError
+
     for field_name, field_values in assembly.field_variables.items():
         field = SubElement(point_data, "DataArray", {
             "type": "Float64",
             "Name": field_name,
             "NumberOfComponents": "1",
             "format": "ascii"
         })
```

### Comparing `pyfem-0.1.9/src/pyfem/isoelements/IsoElementDiagram.py` & `pyfem-0.2.0/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/isoelements/IsoElementShape.py` & `pyfem-0.2.0/src/pyfem/isoelements/IsoElementShape.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,39 +3,44 @@
 
 """
 from typing import Callable
 
 from numpy import empty, array, ndarray, insert, in1d, sqrt
 
 from pyfem.isoelements.IsoElementDiagram import IsoElementDiagram
-from pyfem.isoelements.shape_functions import get_shape_line2, get_shape_tetra4, get_shape_empty, get_shape_hex20, \
-    get_shape_quad4, get_shape_tria3, get_shape_line3, get_shape_quad8, get_shape_tria6, get_shape_hex8
+from pyfem.isoelements.shape_functions import get_shape_line2, get_shape_tetra4, get_shape_tetra4_barycentric, get_shape_empty, get_shape_hex20, get_shape_quad4, \
+    get_shape_tria3, get_shape_tria3_barycentric, get_shape_line3, get_shape_quad8, get_shape_tria6, get_shape_tria6_barycentric, get_shape_hex8
 from pyfem.quadrature.GaussLegendreQuadrature import GaussLegendreQuadrature
 from pyfem.quadrature.TetrahedronQuadrature import TetrahedronQuadrature
+from pyfem.quadrature.TetrahedronQuadratureBarycentric import TetrahedronQuadratureBarycentric
 from pyfem.quadrature.TriangleQuadrature import TriangleQuadrature
+from pyfem.quadrature.TriangleQuadratureBarycentric import TriangleQuadratureBarycentric
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class IsoElementShape:
     """
     等参单元类，设置等参单元的形函数和积分点等信息。
 
     当前支持的单元类型 ['empty', 'line2', 'line3', 'tria3', 'tria6', 'quad4', 'quad8', 'tetra4', 'hex8', 'hex20']
 
     :ivar element_type: 等参单元类型
     :vartype element_type: str
 
+    :ivar coord_type: 坐标类型
+    :vartype coord_type: str
+
     :ivar diagram: 等参单元示意图（字符串形式）
     :vartype diagram: str
 
     :ivar dimension: 等参单元空间维度
     :vartype dimension: int
 
-    :ivar topological_dimension: 等参单元拓扑维度
+    :ivar topological_dimension: 等参单元拓扑维度，有些情况下拓扑维度不等于空间维度，例如处理空间曲面单元时，空间维度为3，但是单元拓扑维度为2
     :vartype topological_dimension: int
 
     :ivar nodes_number: 等参单元节点数目
     :vartype nodes_number: int
 
     :ivar order: 等参单元插值阶次
     :vartype order: int
@@ -81,14 +86,15 @@
 
     :ivar nodes_on_surface_dict: 单元节点与等参单元边表面的映射字典
     :vartype nodes_on_surface_dict: dict[str, ndarray]
     """
 
     __slots_dict__: dict = {
         'element_type': ('str', '等参单元类型'),
+        'coord_type': ('str', '坐标类型'),
         'diagram': ('str', '等参单元示意图（字符串形式）'),
         'dimension': ('int', '等参单元空间维度'),
         'topological_dimension': ('int',
                                   '等参单元拓扑维度，有些情况下拓扑维度不等于空间维度，例如处理空间曲面单元时，空间维度为3，但是单元拓扑维度为2'),
         'nodes_number': ('int', '等参单元节点数目'),
         'order': ('int', '等参单元插值阶次'),
         'shape_function': ('Callable', '等参单元形函数'),
@@ -109,14 +115,15 @@
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     allowed_element_type = ['empty', 'line2', 'line3', 'tria3', 'tria6', 'quad4', 'quad8', 'tetra4', 'hex8', 'hex20']
 
     def __init__(self, element_type: str) -> None:
         self.element_type: str = ''
+        self.coord_type: str = ''
         self.diagram: str = ''
         self.dimension: int = 0
         self.topological_dimension: int = 0
         self.nodes_number: int = 0
         self.order: int = 0
         self.shape_function: Callable = get_shape_empty
         self.qp_number: int = 0
@@ -188,34 +195,37 @@
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def set_line2(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 1
         self.topological_dimension = 1
         self.nodes_number = 2
         self.order = 1
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_line2
         self.diagram = IsoElementDiagram.line2
 
     def set_line3(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 1
         self.topological_dimension = 1
         self.nodes_number = 3
         self.order = 2
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_line3
         self.diagram = IsoElementDiagram.line3
 
     def set_quad4(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 2
         self.topological_dimension = 2
         self.nodes_number = 4
         self.order = 2
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_quad4
@@ -232,14 +242,15 @@
                                       's3': (1, -1, 1, 1),
                                       's4': (1, 1, -1, 1)}
         self.bc_qp_coords_dict = {name: insert(bc_qp_coords, item[0], item[1], axis=1) for name, item in
                                   self.bc_surface_coord_dict.items()}
         self.diagram = IsoElementDiagram.quad4
 
     def set_quad8(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 2
         self.topological_dimension = 2
         self.nodes_number = 8
         self.order = 3
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_quad8
@@ -256,60 +267,108 @@
                                       's3': (1, -1, 1, 1),
                                       's4': (1, 1, -1, 1)}
         self.bc_qp_coords_dict = {name: insert(bc_qp_coords, item[0], item[1], axis=1) for name, item in
                                   self.bc_surface_coord_dict.items()}
         self.diagram = IsoElementDiagram.quad8
 
     def set_tria3(self) -> None:
+        # self.coord_type = 'cartesian'
+        # self.dimension = 2
+        # self.topological_dimension = 2
+        # self.nodes_number = 3
+        # self.order = 1
+        # quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension)
+        # self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
+        # self.shape_function = get_shape_tria3
+
+        self.coord_type = 'barycentric'
         self.dimension = 2
         self.topological_dimension = 2
         self.nodes_number = 3
         self.order = 1
-        quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension)
+        quadrature = TriangleQuadratureBarycentric(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
-        self.shape_function = get_shape_tria3
+        self.shape_function = get_shape_tria3_barycentric
+
         self.diagram = IsoElementDiagram.tria3
 
     def set_tria6(self) -> None:
+        # self.coord_type = 'cartesian'
+        # self.dimension = 2
+        # self.topological_dimension = 2
+        # self.nodes_number = 6
+        # self.order = 2
+        # quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension)
+        # self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
+        # self.shape_function = get_shape_tria6
+
+        self.coord_type = 'barycentric'
         self.dimension = 2
         self.topological_dimension = 2
         self.nodes_number = 6
         self.order = 2
-        quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension)
+        quadrature = TriangleQuadratureBarycentric(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
-        self.shape_function = get_shape_tria6
+        self.shape_function = get_shape_tria6_barycentric
+
         self.diagram = IsoElementDiagram.tria6
 
     def set_tetra4(self) -> None:
+        # self.coord_type = 'cartesian'
+        # self.dimension = 3
+        # self.topological_dimension = 3
+        # self.nodes_number = 4
+        # self.order = 1
+        # quadrature = TetrahedronQuadrature(order=self.order, dimension=self.dimension)
+        # self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
+        # self.shape_function = get_shape_tetra4
+        # self.bc_surface_number = 4
+        # bc_quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension - 1)
+        # bc_qp_coords, self.bc_qp_weights = bc_quadrature.get_quadrature_coords_and_weights()
+        # self.bc_surface_nodes_dict = {'s1': (0, 3, 2),
+        #                               's2': (0, 1, 3),
+        #                               's3': (0, 2, 1),
+        #                               's4': (1, 2, 3)}
+        # self.bc_surface_coord_dict = {'s1': (0, 0, -1, 1),
+        #                               's2': (1, 0, 1, 1),
+        #                               's3': (2, 0, -1, 1),
+        #                               's4': (0, 0, 1, sqrt(3))}
+        # self.bc_qp_coords_dict = {name: insert(bc_qp_coords, item[0], item[1], axis=1) for name, item in
+        #                           self.bc_surface_coord_dict.items()}
+        # s4_qp_coords = self.bc_qp_coords_dict['s4']
+        # s4_qp_coords[:, 0] = 1 - s4_qp_coords[:, 1] - s4_qp_coords[:, 2]
+
+        self.coord_type = 'barycentric'
         self.dimension = 3
         self.topological_dimension = 3
         self.nodes_number = 4
         self.order = 1
-        quadrature = TetrahedronQuadrature(order=self.order, dimension=self.dimension)
+        quadrature = TetrahedronQuadratureBarycentric(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
-        self.shape_function = get_shape_tetra4
-
+        self.shape_function = get_shape_tetra4_barycentric
         self.bc_surface_number = 4
-        bc_quadrature = TriangleQuadrature(order=self.order, dimension=self.dimension - 1)
+        bc_quadrature = TriangleQuadratureBarycentric(order=self.order, dimension=self.dimension - 1)
         bc_qp_coords, self.bc_qp_weights = bc_quadrature.get_quadrature_coords_and_weights()
         self.bc_surface_nodes_dict = {'s1': (0, 3, 2),
                                       's2': (0, 1, 3),
                                       's3': (0, 2, 1),
                                       's4': (1, 2, 3)}
         self.bc_surface_coord_dict = {'s1': (0, 0, -1, 1),
                                       's2': (1, 0, 1, 1),
                                       's3': (2, 0, -1, 1),
                                       's4': (0, 0, 1, sqrt(3))}
         self.bc_qp_coords_dict = {name: insert(bc_qp_coords, item[0], item[1], axis=1) for name, item in
                                   self.bc_surface_coord_dict.items()}
         s4_qp_coords = self.bc_qp_coords_dict['s4']
         s4_qp_coords[:, 0] = 1 - s4_qp_coords[:, 1] - s4_qp_coords[:, 2]
+
         self.diagram = IsoElementDiagram.tetra4
 
     def set_hex8(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 3
         self.topological_dimension = 3
         self.nodes_number = 8
         self.order = 2
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_hex8
@@ -330,14 +389,15 @@
                                       's5': (2, -1, -1, 1),
                                       's6': (2, 1, 1, 1)}
         self.bc_qp_coords_dict = {name: insert(bc_qp_coords, item[0], item[1], axis=1) for name, item in
                                   self.bc_surface_coord_dict.items()}
         self.diagram = IsoElementDiagram.hex8
 
     def set_hex20(self) -> None:
+        self.coord_type = 'cartesian'
         self.dimension = 3
         self.topological_dimension = 3
         self.nodes_number = 20
         self.order = 3
         quadrature = GaussLegendreQuadrature(order=self.order, dimension=self.dimension)
         self.qp_coords, self.qp_weights = quadrature.get_quadrature_coords_and_weights()
         self.shape_function = get_shape_hex20
@@ -377,14 +437,14 @@
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(IsoElementShape.__slots_dict__)
 
     # iso_element_shape_dict['line2'].show()
     # iso_element_shape_dict['line3'].show()
-    # iso_element_shape_dict['tria3'].show()
+    iso_element_shape_dict['tria3'].show()
     # iso_element_shape_dict['tria6'].show()
     # iso_element_shape_dict['quad4'].show()
     # iso_element_shape_dict['quad8'].show()
     # iso_element_shape_dict['tetra4'].show()
-    iso_element_shape_dict['hex8'].show()
+    # iso_element_shape_dict['hex8'].show()
     # iso_element_shape_dict['hex20'].show()
```

### Comparing `pyfem-0.1.9/src/pyfem/isoelements/derive_shape_functions.py` & `pyfem-0.2.0/src/pyfem/isoelements/derive_shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/isoelements/get_iso_element_type.py` & `pyfem-0.2.0/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/isoelements/shape_functions.py` & `pyfem-0.2.0/src/pyfem/isoelements/shape_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -133,14 +133,67 @@
     dNdxi[1, 0] = -1.0
     dNdxi[1, 1] = 0.0
     dNdxi[1, 2] = 1.0
 
     return N, dNdxi
 
 
+def get_shape_tria3_barycentric(xi: ndarray) -> tuple[ndarray, ndarray]:
+    r"""
+    三节点三角形单元。
+
+    节点序号及局部坐标方向如图所示::
+
+        2
+        * *
+        *   *
+        *     *
+        *       *
+        *         *
+        0 * * * * * 1
+
+    对应节点的形函数表达式如下：
+
+    .. math::
+        N_{ 0 } = \lambda_{0}
+
+    .. math::
+        N_{ 1 } = \lambda_{1}
+
+    .. math::
+        N_{ 2 } = \lambda_{2}
+
+    """
+
+    if len(xi) != 3:
+        raise NotImplementedError(error_style(f'barycentric coordinate {xi} must be dimension 3'))
+
+    N = empty(3)
+    dNdxi = empty(shape=(3, 3))
+    xi = xi
+
+    N[0] = xi[0]
+    N[1] = xi[1]
+    N[2] = xi[2]
+
+    dNdxi[0, 0] = 1.0
+    dNdxi[0, 1] = 0.0
+    dNdxi[0, 2] = 0.0
+
+    dNdxi[1, 0] = 0.0
+    dNdxi[1, 1] = 1.0
+    dNdxi[1, 2] = 0.0
+
+    dNdxi[2, 0] = 0.0
+    dNdxi[2, 1] = 0.0
+    dNdxi[2, 2] = 1.0
+
+    return N, dNdxi
+
+
 def get_shape_quad4(xi: ndarray) -> tuple[ndarray, ndarray]:
     r"""
     四节点四边形单元。
 
     节点序号及局部坐标方向如图所示::
 
         3---------------2
@@ -326,14 +379,80 @@
     dNdxi[2, 1] = 0.0
     dNdxi[2, 2] = 0.0
     dNdxi[2, 3] = 1.0
 
     return N, dNdxi
 
 
+def get_shape_tetra4_barycentric(xi: ndarray) -> tuple[ndarray, ndarray]:
+    r"""
+    四节点四面体单元。
+
+    节点序号及局部坐标方向如图所示::
+
+        3
+        * **
+        *   * *
+        *     *  *
+        *       *   2
+        *        **  *
+        *     *     * *
+        *  *          **
+        0 * * * * * * * 1
+
+    对应节点的形函数表达式如下：
+
+    .. math::
+        N_{ 0 } = - x_{0} - x_{1} - x_{2} + 1.0
+
+    .. math::
+        N_{ 1 } = x_{0}
+
+    .. math::
+        N_{ 2 } = x_{1}
+
+    .. math::
+        N_{ 3 } = x_{2}
+
+    """
+
+    if len(xi) != 4:
+        raise NotImplementedError(error_style(f'barycentric coordinate {xi} must be dimension 4'))
+
+    N = empty(4)
+    dNdxi = empty(shape=(4, 4))
+
+    N[0] = xi[0]
+    N[1] = xi[1]
+    N[2] = xi[2]
+    N[3] = xi[3]
+
+    dNdxi[0, 0] = 1.0
+    dNdxi[0, 1] = 0.0
+    dNdxi[0, 2] = 0.0
+    dNdxi[0, 3] = 0.0
+
+    dNdxi[1, 0] = 0.0
+    dNdxi[1, 1] = 1.0
+    dNdxi[1, 2] = 0.0
+    dNdxi[1, 3] = 0.0
+
+    dNdxi[2, 0] = 0.0
+    dNdxi[2, 1] = 0.0
+    dNdxi[2, 2] = 1.0
+    dNdxi[2, 3] = 0.0
+
+    dNdxi[3, 0] = 0.0
+    dNdxi[3, 1] = 0.0
+    dNdxi[3, 2] = 0.0
+    dNdxi[3, 3] = 1.0
+
+    return N, dNdxi
+
+
 def get_shape_hex8(xi: ndarray) -> tuple[ndarray, ndarray]:
     r"""
     八节点六面体单元。
 
     节点序号及局部坐标方向如图所示::
 
             7---------------6
@@ -458,36 +577,108 @@
     """
 
     if len(xi) != 2:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 2'))
 
     N = empty(6)
     dNdxi = empty(shape=(2, 6))
-    xi = xi
 
-    N[0] = - xi[0] + 2.0 * xi[0] * xi[0]
-    N[1] = - xi[1] + 2.0 * xi[1] * xi[1]
-    N[2] = - (1.0 - xi[0] - xi[1]) + 2.0 * (1.0 - xi[0] - xi[1]) * (1.0 - xi[0] - xi[1])
+    N[0] = 1.0 - xi[0] - xi[1] - 2.0 * xi[0] * (1.0 - xi[0] - xi[1]) - 2.0 * xi[1] * (1.0 - xi[0] - xi[1])
+    N[1] = xi[0] - 2.0 * xi[0] * (1.0 - xi[0] - xi[1]) - 2.0 * xi[0] * xi[1]
+    N[2] = xi[1] - 2.0 * xi[0] * xi[1] - 2.0 * xi[1] * (1.0 - xi[0] - xi[1])
+    N[3] = 4.0 * xi[0] * (1.0 - xi[0] - xi[1])
+    N[4] = 4.0 * xi[0] * xi[1]
+    N[5] = 4.0 * xi[1] * (1.0 - xi[0] - xi[1])
+
+    dNdxi[0, 0] = -1.0 - 2.0 * (1.0 - xi[0] - xi[1]) + 2.0 * xi[0] + 2.0 * xi[1]
+    dNdxi[0, 1] = 1.0 - 2.0 * (1.0 - xi[0] - xi[1]) + 2.0 * xi[0] - 2.0 * xi[1]
+    dNdxi[0, 2] = 0.0
+    dNdxi[0, 3] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[0]
+    dNdxi[0, 4] = 4.0 * xi[1]
+    dNdxi[0, 5] = -4.0 * xi[1]
+
+    dNdxi[1, 0] = -1.0 + 2.0 * xi[0] - 2.0 * (1.0 - xi[0] - xi[1]) + 2.0 * xi[1]
+    dNdxi[1, 1] = 0.0
+    dNdxi[1, 2] = 1.0 - 2.0 * xi[0] - 2.0 * (1.0 - xi[0] - xi[1]) + 2.0 * xi[1]
+    dNdxi[1, 3] = -4.0 * xi[0]
+    dNdxi[1, 4] = 4.0 * xi[0]
+    dNdxi[1, 5] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[1]
+
+    return N, dNdxi
+
+
+def get_shape_tria6_barycentric(xi: ndarray) -> tuple[ndarray, ndarray]:
+    r"""
+    六节点三角形单元。
+
+    节点序号及局部坐标方向如图所示::
+
+        2
+        * *
+        *   *
+        5     4
+        *       *
+        *         *
+        0 * * 3 * * 1
+
+    对应节点的形函数表达式如下：
+
+    .. math::
+        N_{ 0 } = 2.0 x_{0}^{2} - x_{0}
+
+    .. math::
+        N_{ 1 } = 2.0 x_{1}^{2} - x_{1}
+
+    .. math::
+        N_{ 2 } = x_{0} + x_{1} + \left(- 2.0 x_{0} - 2.0 x_{1} + 2.0\right) \left(- x_{0} - x_{1} + 1.0\right) - 1.0
+
+    .. math::
+        N_{ 3 } = 4.0 x_{0} x_{1}
+
+    .. math::
+        N_{ 4 } = 4.0 x_{1} \left(- x_{0} - x_{1} + 1.0\right)
+
+    .. math::
+        N_{ 5 } = 4.0 x_{0} \left(- x_{0} - x_{1} + 1.0\right)
+
+    """
+
+    if len(xi) != 3:
+        raise NotImplementedError(error_style(f'barycentric coordinate {xi} must be dimension 3'))
+
+    N = empty(6)
+    dNdxi = empty(shape=(3, 6))
+
+    N[0] = xi[0] * (2.0 * xi[0] - 1.0)
+    N[1] = xi[1] * (2.0 * xi[1] - 1.0)
+    N[2] = xi[2] * (2.0 * xi[2] - 1.0)
     N[3] = 4.0 * xi[0] * xi[1]
-    N[4] = 4.0 * xi[1] * (1.0 - xi[0] - xi[1])
-    N[5] = 4.0 * xi[0] * (1.0 - xi[0] - xi[1])
+    N[4] = 4.0 * xi[1] * xi[2]
+    N[5] = 4.0 * xi[2] * xi[0]
 
-    dNdxi[0, 0] = -1.0 + 4.0 * xi[0]
+    dNdxi[0, 0] = 4.0 * xi[0] - 1.0
     dNdxi[0, 1] = 0.0
-    dNdxi[0, 2] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
+    dNdxi[0, 2] = 0.0
     dNdxi[0, 3] = 4.0 * xi[1]
-    dNdxi[0, 4] = -4.0 * xi[1]
-    dNdxi[0, 5] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[0]
+    dNdxi[0, 4] = 0.0
+    dNdxi[0, 5] = 4.0 * xi[2]
 
     dNdxi[1, 0] = 0.0
-    dNdxi[1, 1] = -1.0 + 4.0 * xi[1]
-    dNdxi[1, 2] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
+    dNdxi[1, 1] = 4.0 * xi[1] - 1.0
+    dNdxi[1, 2] = 0.0
     dNdxi[1, 3] = 4.0 * xi[0]
-    dNdxi[1, 4] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[1]
-    dNdxi[1, 5] = -4.0 * xi[0]
+    dNdxi[1, 4] = 4.0 * xi[2]
+    dNdxi[1, 5] = 0.0
+
+    dNdxi[2, 0] = 0.0
+    dNdxi[2, 1] = 0.0
+    dNdxi[2, 2] = 4.0 * xi[2] - 1.0
+    dNdxi[2, 3] = 0.0
+    dNdxi[2, 4] = 4.0 * xi[1]
+    dNdxi[2, 5] = 4.0 * xi[0]
 
     return N, dNdxi
 
 
 def get_shape_hex20(xi: ndarray) -> tuple[ndarray, ndarray]:
     r"""
     二十节点六面体单元形函数。
@@ -658,8 +849,9 @@
     dNdxi[(2, 18)] = -0.5 * xi[2] * (xi[0] + 1) * (xi[1] + 1.0)
     dNdxi[(2, 19)] = 0.5 * xi[2] * (xi[0] - 1) * (xi[1] + 1.0)
 
     return N, dNdxi
 
 
 if __name__ == "__main__":
-    get_shape_line2(array([1]))
+    # get_shape_line2(array([1]))
+    print(get_shape_tria6(array([0, 0.5])))
```

### Comparing `pyfem-0.1.9/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.2.0/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.2.0/src/pyfem/materials/ElasticIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.2.0/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.2.0/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/PlasticCrystal.py` & `pyfem-0.2.0/src/pyfem/materials/PlasticCrystal.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
     :ivar w_grain: 晶粒坐标系下的3号矢量
     :vartype w_grain: ndarray
 
     :ivar T: 坐标变换矩阵
     :vartype T: ndarray
 
-    :ivar T_vogit: Vogit坐标变换矩阵
-    :vartype T_vogit: ndarray
+    :ivar T_voigt: Vogit坐标变换矩阵
+    :vartype T_voigt: ndarray
 
     :ivar m_s: 特征滑移系滑移方向
     :vartype m_s: ndarray
 
     :ivar n_s: 特征滑移系滑移面法向
     :vartype n_s: ndarray
 
@@ -126,15 +126,15 @@
         'u_global': ('ndarray', '全局坐标系下的1号矢量'),
         'v_global': ('ndarray', '全局坐标系下的2号矢量'),
         'w_global': ('ndarray', '全局坐标系下的3号矢量'),
         'u_grain': ('ndarray', '晶粒坐标系下的1号矢量'),
         'v_grain': ('ndarray', '晶粒坐标系下的2号矢量'),
         'w_grain': ('ndarray', '晶粒坐标系下的3号矢量'),
         'T': ('ndarray', '坐标变换矩阵'),
-        'T_vogit': ('ndarray', 'Vogit坐标变换矩阵'),
+        'T_voigt': ('ndarray', 'Vogit坐标变换矩阵'),
         'm_s': ('ndarray', '特征滑移系滑移方向'),
         'n_s': ('ndarray', '特征滑移系滑移面法向'),
         'MAX_NITER': ('ndarray', '硬化系数矩阵'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
@@ -207,20 +207,20 @@
         self.w_global: ndarray = array(section.data_dict['w_global'])
 
         self.u_grain: ndarray = array(section.data_dict['u_grain'])
         self.v_grain: ndarray = array(section.data_dict['v_grain'])
         self.w_grain: ndarray = array(section.data_dict['w_grain'])
 
         self.T: ndarray = get_transformation(self.u_grain, self.v_grain, self.w_grain, self.u_global, self.v_global, self.w_global)
-        self.T_vogit: ndarray = get_voigt_transformation(self.T)
+        self.T_voigt: ndarray = get_voigt_transformation(self.T)
 
         # 旋转至全局坐标系
         self.m_s = dot(self.m_s, self.T)
         self.n_s = dot(self.n_s, self.T)
-        self.C = dot(dot(self.T_vogit, self.C), transpose(self.T_vogit))
+        self.C = dot(dot(self.T_voigt, self.C), transpose(self.T_voigt))
 
     def create_elastic_stiffness(self, elastic: dict):
         r"""
         **定义局部晶系的弹性刚度矩阵**
 
         弹性刚度矩阵由弹性常数组成，对应的矩阵形式与弹性常数个数及材料对称性相关，相关参数由材料属性数据字典中的 :py:attr:`elastic` 字典给出。
```

### Comparing `pyfem-0.1.9/src/pyfem/materials/PlasticCrystalGNDs.py` & `pyfem-0.2.0/src/pyfem/materials/PlasticCrystalGNDs.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 
     :ivar w_grain: 晶粒坐标系下的3号矢量
     :vartype w_grain: ndarray
 
     :ivar T: 坐标变换矩阵
     :vartype T: ndarray
 
-    :ivar T_vogit: Vogit坐标变换矩阵
-    :vartype T_vogit: ndarray
+    :ivar T_voigt: Vogit坐标变换矩阵
+    :vartype T_voigt: ndarray
 
     :ivar m_s: 特征滑移系滑移方向
     :vartype m_s: ndarray
 
     :ivar n_s: 特征滑移系滑移面法向
     :vartype n_s: ndarray
 
@@ -155,15 +155,15 @@
         'u_global': ('ndarray', '全局坐标系下的1号矢量'),
         'v_global': ('ndarray', '全局坐标系下的2号矢量'),
         'w_global': ('ndarray', '全局坐标系下的3号矢量'),
         'u_grain': ('ndarray', '晶粒坐标系下的1号矢量'),
         'v_grain': ('ndarray', '晶粒坐标系下的2号矢量'),
         'w_grain': ('ndarray', '晶粒坐标系下的3号矢量'),
         'T': ('ndarray', '坐标变换矩阵'),
-        'T_vogit': ('ndarray', 'Vogit坐标变换矩阵'),
+        'T_voigt': ('ndarray', 'Vogit坐标变换矩阵'),
         'm_s': ('ndarray', '特征滑移系滑移方向'),
         'n_s': ('ndarray', '特征滑移系滑移面法向'),
         'MAX_NITER': ('ndarray', '最大迭代次数'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
@@ -253,20 +253,20 @@
         self.w_global: ndarray = array(section.data_dict['w_global'])
 
         self.u_grain: ndarray = array(section.data_dict['u_grain'])
         self.v_grain: ndarray = array(section.data_dict['v_grain'])
         self.w_grain: ndarray = array(section.data_dict['w_grain'])
 
         self.T: ndarray = get_transformation(self.u_grain, self.v_grain, self.w_grain, self.u_global, self.v_global, self.w_global)
-        self.T_vogit: ndarray = get_voigt_transformation(self.T)
+        self.T_voigt: ndarray = get_voigt_transformation(self.T)
 
         # 旋转至全局坐标系
         self.m_s = dot(self.m_s, self.T)
         self.n_s = dot(self.n_s, self.T)
-        self.C = dot(dot(self.T_vogit, self.C), transpose(self.T_vogit))
+        self.C = dot(dot(self.T_voigt, self.C), transpose(self.T_voigt))
 
     def create_elastic_stiffness(self, elastic: dict):
         r"""
         **定义局部晶系的弹性刚度矩阵**
 
         弹性刚度矩阵由弹性常数组成，对应的矩阵形式与弹性常数个数及材料对称性相关，相关参数由材料属性数据字典中的 :py:attr:`elastic` 字典给出。
```

### Comparing `pyfem-0.1.9/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.2.0/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.2.0/src/pyfem/materials/ThermalIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/UMAT.py` & `pyfem-0.2.0/src/pyfem/materials/UMAT.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.2.0/src/pyfem/materials/ViscoElasticMaxwell.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/crystal_slip_system.py` & `pyfem-0.2.0/src/pyfem/materials/crystal_slip_system.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/materials/get_material_data.py` & `pyfem-0.2.0/src/pyfem/materials/get_material_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,38 @@
 
 """
 from typing import Union
 
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
+from pyfem.materials.DiffusionIsotropic import DiffusionIsotropic
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
 from pyfem.materials.MechanicalThermalExpansion import MechanicalThermalExpansion
 from pyfem.materials.PhaseFieldDamage import PhaseFieldDamage
 from pyfem.materials.PlasticCrystal import PlasticCrystal
 from pyfem.materials.PlasticCrystalGNDs import PlasticCrystalGNDs
 from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
 from pyfem.materials.ThermalIsotropic import ThermalIsotropic
 from pyfem.materials.ViscoElasticMaxwell import ViscoElasticMaxwell
 from pyfem.utils.colors import error_style
 
 MaterialData = Union[
-    BaseMaterial, MechanicalThermalExpansion, PhaseFieldDamage, PlasticKinematicHardening, ThermalIsotropic, ViscoElasticMaxwell, ElasticIsotropic]
+    BaseMaterial, MechanicalThermalExpansion, PhaseFieldDamage, PlasticKinematicHardening, ThermalIsotropic, ViscoElasticMaxwell, ElasticIsotropic, DiffusionIsotropic]
 
 material_data_dict = {
     'ElasticIsotropic': ElasticIsotropic,
     'PlasticKinematicHardening': PlasticKinematicHardening,
     'PlasticCrystal': PlasticCrystal,
     'PlasticCrystalGNDs': PlasticCrystalGNDs,
     'ViscoElasticMaxwell': ViscoElasticMaxwell,
     'ThermalIsotropic': ThermalIsotropic,
     'MechanicalThermalExpansion': MechanicalThermalExpansion,
-    'PhaseFieldDamage': PhaseFieldDamage
+    'PhaseFieldDamage': PhaseFieldDamage,
+    'DiffusionIsotropic': DiffusionIsotropic,
 }
 
 
 def get_material_data(material: Material, dimension: int, section: Section) -> MaterialData:
     """
     工厂函数，用于根据材料属性生产不同的材料对象。
```

### Comparing `pyfem-0.1.9/src/pyfem/mesh/MeshData.py` & `pyfem-0.2.0/src/pyfem/mesh/MeshData.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pyfem.utils.colors import BLUE, END
 from pyfem.utils.colors import error_style, info_style
 from pyfem.utils.wrappers import show_running_time
 
 abaqus_to_meshio_type = meshio.abaqus._abaqus.abaqus_to_meshio_type
 abaqus_to_meshio_type['CPE4'] = 'quad'
 abaqus_to_meshio_type['CPE4R'] = 'quad'
+abaqus_to_meshio_type['CPS6'] = 'triangle6'
 
 
 class MeshData:
     """
     网格数据类。
 
     :ivar dimension: 空间维度
@@ -181,14 +182,10 @@
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(MeshData.__slots_dict__)
 
-    # mesh_data = MeshData()
-    # mesh_data.read_file(r'..\..\..\examples\mechanical\rectangle_hole\rectangle_hole_quad4.inp', 'abaqus')
-    # mesh_data.show()
-
     mesh_data = MeshData()
-    mesh_data.read_file(r'..\..\..\examples\mechanical\ansys\plate_45_solid.cdb', 'ansys')
+    mesh_data.read_file(r'..\..\..\examples\mechanical\rectangle_hole\rectangle_hole_quad4.inp', 'abaqus')
     mesh_data.show()
```

### Comparing `pyfem-0.1.9/src/pyfem/quadrature/BaseQuadrature.py` & `pyfem-0.2.0/src/pyfem/quadrature/BaseQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/quadrature/GaussLegendreQuadrature.py` & `pyfem-0.2.0/src/pyfem/quadrature/GaussLegendreQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/quadrature/PyramidQuadrature.py` & `pyfem-0.2.0/src/pyfem/quadrature/PyramidQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/quadrature/TetrahedronQuadrature.py` & `pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadrature.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 [0.5411844128002370, 0.2965010205431240, 0.1335581607035680, 0.0025991900130432],
                 [0.1335581607035680, 0.5411844128002370, 0.2965010205431240, 0.0025991900130432],
                 [0.2965010205431240, 0.1335581607035680, 0.5411844128002370, 0.0025991900130432]], dtype=DTYPE)
         else:
             raise NotImplementedError(error_style('order must be 1, 2, 3, 5, 6, 8 or 9'))
 
         self.qp_coords = qp_coords_and_weights[:, 0:3]
-        self.qp_weights = qp_coords_and_weights[:, 3:4]
+        self.qp_weights = qp_coords_and_weights[:, 3:4].reshape(-1)
         self.qp_number = len(self.qp_weights)
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(TetrahedronQuadrature.__slots_dict__)
```

### Comparing `pyfem-0.1.9/src/pyfem/quadrature/TriangleQuadrature.py` & `pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadrature.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 [0.4932203038571030, 0.0135593922857950, 0.0051060170945235],
                 [0.0135593922857950, 0.4932203038571030, 0.0051060170945235],
                 [0.4932203038571030, 0.4932203038571030, 0.0051060170945235]], dtype=DTYPE)
         else:
             raise NotImplementedError(error_style('order must be 1, 2, 4, 5, 7, 8, 10, 12, 14, 15 or 17'))
 
         self.qp_coords = qp_coords_and_weights[:, 0:2]
-        self.qp_weights = qp_coords_and_weights[:, 2:3]
+        self.qp_weights = qp_coords_and_weights[:, 2:3].reshape(-1)
         self.qp_number = len(self.qp_weights)
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(TriangleQuadrature.__slots_dict__)
```

### Comparing `pyfem-0.1.9/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.2.0/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.2.0/src/pyfem/solvers/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.2.0/src/pyfem/solvers/ArcLengthSolver.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 from scipy.sparse.linalg import splu  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
-from pyfem.utils.colors import info_style, warn_style, error_style
+from pyfem.utils.colors import error_style
 from pyfem.utils.logger import logger, logger_sta
 
 
-class NonlinearSolver(BaseSolver):
+class ArcLengthSolver(BaseSolver):
     r"""
     非线性求解器。
 
     :ivar PENALTY: 罚系数
     :vartype PENALTY: float
 
     :ivar FORCE_TOL: 残差容限
     :vartype FORCE_TOL: float
 
     :ivar MAX_NITER: 最大迭代次数
     :vartype MAX_NITER: int
 
+    :ivar BC_METHOD: 边界条件施加方式
+    :vartype BC_METHOD: str
+
     对于准静态过程，需要求解的线性系统可以表示为：
 
     .. math::
         {{\mathbf{f}}_{{\text{ext}}}} - {{\mathbf{f}}_{{\text{int}}}} = {\mathbf{0}}
 
     虽然在静态力学过程中，时间不再起作用，但是我们仍然需要一个参数来排列事件的顺序。出于这个原因，我们将继续在静态力学过程中使用“时间”的概念来表示加载顺序。特别地，时间的概念可以用来将完整的外部载荷分解为若干个增量加载步骤。这样做的原因如下：
 
@@ -45,38 +48,50 @@
 
     [1] Non‐Linear Finite Element Analysis of Solids and Structures, John Wiley & Sons, Ltd, 2012, 31-62, https://doi.org/10.1002/9781118375938.ch2
     """
 
     __slots_dict__: dict = {
         'PENALTY': ('float', '罚系数'),
         'FORCE_TOL': ('float', '残差容限'),
-        'MAX_NITER': ('int', '最大迭代次数')
+        'MAX_NITER': ('int', '最大迭代次数'),
+        'BC_METHOD': ('str', '边界条件施加方式'),
+        'lam': ('float', '求解器参数lambda'),
+        'da_old': ('float', '求解器参数lambda'),
+        'dlam_old': ('float', '求解器参数lambda'),
+        'factor': ('float', '求解器参数lambda'),
     }
 
     __slots__ = BaseSolver.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
         self.PENALTY: float = 1.0e128
         self.FORCE_TOL: float = 1.0e-3
         self.MAX_NITER: int = 16
+        self.BC_METHOD: str = '01'
+        self.lam: float = 1.0
+        self.da_old = None
+        self.dlam_old = None
+        self.factor = 1.0
 
     def run(self) -> int:
         if self.assembly.props.solver.option in [None, '', 'NR', 'NewtonRaphson']:
             return self.incremental_iterative_solve('NR')
         elif self.assembly.props.solver.option in ['IT', 'InitialTangent']:
             return self.incremental_iterative_solve('IT')
         else:
             raise NotImplementedError(error_style(
                 f'unsupported option \'{self.assembly.props.solver.option}\' of {self.assembly.props.solver.type}'))
 
     def incremental_iterative_solve(self, option: str) -> int:
+        import numpy as np
+        np.set_printoptions(precision=5, suppress=True, linewidth=10000)
         timer = self.assembly.timer
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
 
@@ -107,43 +122,87 @@
             self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
             self.assembly.update_element_data()
 
             is_convergence = False
 
             for niter in range(self.MAX_NITER):
                 self.assembly.assembly_global_stiffness()
-                fint = self.assembly.fint
+                fint = deepcopy(self.assembly.fint)
                 rhs = deepcopy(self.assembly.fext)
-                if niter == 0:
-                    for bc_data in self.assembly.bc_data_list:
-                        amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
-                        if bc_data.bc.category == 'DirichletBC':
-                            for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
-                                self.assembly.global_stiffness[bc_dof_id, bc_dof_id] += self.PENALTY
-                                rhs[bc_dof_id] += bc_dof_value * self.PENALTY * amplitude_increment
-                        elif bc_data.bc.category == 'NeumannBC':
-                            for bc_dof_id, bc_fext in zip(bc_data.bc_dof_ids, bc_data.bc_fext):
-                                rhs[bc_dof_id] += bc_fext * amplitude_increment
-                                self.assembly.fext[bc_dof_id] += bc_fext * amplitude_increment
-                else:
-                    for bc_data in self.assembly.bc_data_list:
-                        if bc_data.bc.category == 'DirichletBC':
-                            for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
-                                self.assembly.global_stiffness[bc_dof_id, bc_dof_id] += self.PENALTY
-                                rhs[bc_dof_id] = 0.0 * self.PENALTY
+                fhat = deepcopy(self.assembly.fext)
+
+                # 罚系数法施加边界条件
+                if self.BC_METHOD == 'PENALTY':
+                    if niter == 0:
+                        for bc_data in self.assembly.bc_data_list:
+                            amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
+                            if bc_data.bc.category == 'DirichletBC':
+                                for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
+                                    self.assembly.global_stiffness[bc_dof_id, bc_dof_id] += self.PENALTY
+                                    rhs[bc_dof_id] += bc_dof_value * self.PENALTY * amplitude_increment
+                            elif bc_data.bc.category == 'NeumannBC':
+                                for bc_dof_id, bc_fext in zip(bc_data.bc_dof_ids, bc_data.bc_fext):
+                                    rhs[bc_dof_id] += bc_fext * amplitude_increment
+                                    self.assembly.fext[bc_dof_id] += bc_fext * amplitude_increment
+                    else:
+                        for bc_data in self.assembly.bc_data_list:
+                            if bc_data.bc.category == 'DirichletBC':
+                                for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
+                                    self.assembly.global_stiffness[bc_dof_id, bc_dof_id] += self.PENALTY
+                                    rhs[bc_dof_id] = 0.0 * self.PENALTY
+
+                # 划0置1法
+                if self.BC_METHOD == '01':
+                    self.assembly.global_stiffness = self.assembly.global_stiffness.tolil()
+                    if niter == 0:
+                        for bc_data in self.assembly.bc_data_list:
+                            amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
+                            if bc_data.bc.category == 'DirichletBC':
+                                for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
+                                    rhs -= self.assembly.global_stiffness[:, bc_dof_id].toarray().reshape(-1) * bc_dof_value * amplitude_increment
+                                    self.assembly.global_stiffness[bc_dof_id, :] = 0.0
+                                    self.assembly.global_stiffness[:, bc_dof_id] = 0.0
+                                    self.assembly.global_stiffness[bc_dof_id, bc_dof_id] = 1.0
+                                    rhs[bc_dof_id] = bc_dof_value * amplitude_increment + fint[bc_dof_id]
+                            elif bc_data.bc.category == 'NeumannBC':
+                                for bc_dof_id, bc_fext in zip(bc_data.bc_dof_ids, bc_data.bc_fext):
+                                    rhs[bc_dof_id] += bc_fext * amplitude_increment
+                                    self.assembly.fext[bc_dof_id] += bc_fext * amplitude_increment
+                    else:
+                        for bc_data in self.assembly.bc_data_list:
+                            if bc_data.bc.category == 'DirichletBC':
+                                for bc_dof_id, bc_dof_value in zip(bc_data.bc_dof_ids, bc_data.bc_dof_values):
+                                    self.assembly.global_stiffness[bc_dof_id, :] = 0.0
+                                    self.assembly.global_stiffness[:, bc_dof_id] = 0.0
+                                    self.assembly.global_stiffness[bc_dof_id, bc_dof_id] = 1.0
+                                    rhs[bc_dof_id] = fint[bc_dof_id]
+                    self.assembly.global_stiffness = self.assembly.global_stiffness.tocsc()
+
+                # print(self.dof_solution)
 
                 try:
                     LU = splu(self.assembly.global_stiffness)
-                    da = LU.solve(rhs - fint)
+                    if timer.increment == 1:
+                        da1 = LU.solve(self.lam * rhs)
+                        dlam1 = self.lam
+                        print('rhs', rhs)
+                        print('da1', da1)
+                        print('dlam1', dlam1)
+                    else:
+                        da1 = self.factor * self.da_old
+                        dlam1 = self.factor * self.dlam_old
+                        self.lam += dlam1
+                    # da = LU.solve(rhs - fint)
                 except RuntimeError as e:
                     is_convergence = False
                     print(error_style(f"Catch RuntimeError exception: {e}"))
                     break
 
-                self.assembly.ddof_solution += da
+                self.assembly.ddof_solution += da1
+
                 if option == 'NR':
                     self.assembly.update_element_data()
                 elif option == 'IT':
                     self.assembly.update_element_data_without_stiffness()
                 self.assembly.assembly_fint()
 
                 f_residual = self.assembly.fext - self.assembly.fint
@@ -191,14 +250,15 @@
                     timer.dtime = self.solver.max_dtime
                 if timer.time0 + timer.dtime >= self.solver.total_time:
                     timer.dtime = self.solver.total_time - timer.time0
 
                 x.append(self.assembly.element_data_list[0].element_average_field_variables['E11'])
                 y.append(self.assembly.element_data_list[0].element_average_field_variables['S11'])
                 t.append(timer.time0)
+                print(self.assembly.dof_solution)
 
             else:
                 attempt += 1
                 timer.dtime *= 0.5
                 logger.warning(f'  increment {increment} is divergence, dtime is reduced to {timer.dtime}')
 
                 if timer.dtime <= self.assembly.props.solver.min_dtime:
@@ -211,14 +271,16 @@
 
                 self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
                 self.assembly.goback_element_state_variables()
                 self.assembly.update_element_data()
                 self.assembly.assembly_fint()
 
             if timer.is_done():
+                # plt.plot(x, y, marker='o')
+                # plt.show()
                 for output in self.assembly.props.outputs:
                     if output.is_save:
                         if output.type == 'vtk':
                             write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
@@ -227,14 +289,19 @@
         else:
             return 0
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
-    print_slots_dict(NonlinearSolver.__slots_dict__)
+    print_slots_dict(ArcLengthSolver.__slots_dict__)
 
     from pyfem.Job import Job
 
+    import numpy as np
+    np.set_printoptions(precision=5, suppress=True, linewidth=10000)
+
     job = Job(r'..\..\..\examples\mechanical\beam\Job-1.toml')
-    solver = NonlinearSolver(job.assembly, job.props.solver)
-    solver.show()
+    # job = Job(r'..\..\..\examples\mechanical\1element\quad4\Job-1.toml')
+    # solver = NonlinearSolver(job.assembly, job.props.solver)
+    # solver.show()
+    job.run()
```

### Comparing `pyfem-0.1.9/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.2.0/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/utils/colors.py` & `pyfem-0.2.0/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/utils/logger.py` & `pyfem-0.2.0/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/utils/visualization.py` & `pyfem-0.2.0/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem/utils/wrappers.py` & `pyfem-0.2.0/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.9/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.2.0/src/pyfem.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.md
+README
 setup.py
 src/pyfem/Job.py
 src/pyfem/__init__.py
 src/pyfem/__main__.py
 src/pyfem.egg-info/PKG-INFO
 src/pyfem.egg-info/SOURCES.txt
 src/pyfem.egg-info/dependency_links.txt
@@ -21,14 +21,15 @@
 src/pyfem/bc/NeumannBCConcentrated.py
 src/pyfem/bc/NeumannBCDistributed.py
 src/pyfem/bc/NeumannBCPressure.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/derive_surface_integral.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
+src/pyfem/elements/Diffusion.py
 src/pyfem/elements/SolidFiniteStrain.py
 src/pyfem/elements/SolidPhaseDamageSmallStrain.py
 src/pyfem/elements/SolidSmallStrain.py
 src/pyfem/elements/SolidThermalSmallStrain.py
 src/pyfem/elements/Thermal.py
 src/pyfem/elements/__init__.py
 src/pyfem/elements/get_element_data.py
@@ -54,14 +55,15 @@
 src/pyfem/isoelements/IsoElementDiagram.py
 src/pyfem/isoelements/IsoElementShape.py
 src/pyfem/isoelements/__init__.py
 src/pyfem/isoelements/derive_shape_functions.py
 src/pyfem/isoelements/get_iso_element_type.py
 src/pyfem/isoelements/shape_functions.py
 src/pyfem/materials/BaseMaterial.py
+src/pyfem/materials/DiffusionIsotropic.py
 src/pyfem/materials/ElasticIsotropic.py
 src/pyfem/materials/MechanicalThermalExpansion.py
 src/pyfem/materials/PhaseFieldDamage.py
 src/pyfem/materials/PlasticCrystal.py
 src/pyfem/materials/PlasticCrystalGNDs.py
 src/pyfem/materials/PlasticKinematicHardening.py
 src/pyfem/materials/ThermalIsotropic.py
@@ -72,19 +74,23 @@
 src/pyfem/materials/get_material_data.py
 src/pyfem/mesh/MeshData.py
 src/pyfem/mesh/__init__.py
 src/pyfem/quadrature/BaseQuadrature.py
 src/pyfem/quadrature/GaussLegendreQuadrature.py
 src/pyfem/quadrature/PyramidQuadrature.py
 src/pyfem/quadrature/TetrahedronQuadrature.py
+src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
 src/pyfem/quadrature/TriangleQuadrature.py
+src/pyfem/quadrature/TriangleQuadratureBarycentric.py
 src/pyfem/quadrature/__init__.py
+src/pyfem/solvers/ArcLengthSolver.py
 src/pyfem/solvers/BaseSolver.py
 src/pyfem/solvers/LinearSolver.py
 src/pyfem/solvers/NonlinearSolver.py
+src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
 src/pyfem/solvers/__init__.py
 src/pyfem/solvers/get_solver_data.py
 src/pyfem/utils/IntKeyDict.py
 src/pyfem/utils/__init__.py
 src/pyfem/utils/colors.py
 src/pyfem/utils/logger.py
 src/pyfem/utils/mechanics.py
```

