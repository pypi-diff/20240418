# Comparing `tmp/pyansys-2024.1rc1.tar.gz` & `tmp/pyansys-2024.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyansys-2024.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyansys-2024.2.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyansys-2024.1rc1.tar` & `pyansys-2024.2.0b1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1089 2023-09-25 07:03:41.439322 pyansys-2024.1rc1/LICENSE
--rw-r--r--   0        0        0    10719 2023-09-25 07:03:41.439322 pyansys-2024.1rc1/README.rst
--rw-r--r--   0        0        0     2988 2023-09-25 07:03:41.455322 pyansys-2024.1rc1/pyproject.toml
--rw-r--r--   0        0        0      287 2023-09-25 07:03:41.455322 pyansys-2024.1rc1/src/pyansys/__init__.py
--rw-r--r--   0        0        0    13856 1970-01-01 00:00:00.000000 pyansys-2024.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-15 13:17:47.237010 pyansys-2024.2.0b1/LICENSE
+-rw-r--r--   0        0        0    12171 2024-04-15 13:17:47.237010 pyansys-2024.2.0b1/README.rst
+-rw-r--r--   0        0        0     3265 2024-04-15 13:17:47.261010 pyansys-2024.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1353 2024-04-15 13:17:47.261010 pyansys-2024.2.0b1/src/pyansys/__init__.py
+-rw-r--r--   0        0        0    15282 1970-01-01 00:00:00.000000 pyansys-2024.2.0b1/PKG-INFO
```

### Comparing `pyansys-2024.1rc1/LICENSE` & `pyansys-2024.2.0b1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 ANSYS, Inc. All rights reserved.
+Copyright (c) 2024 ANSYS, Inc. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyansys-2024.1rc1/README.rst` & `pyansys-2024.2.0b1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,243 @@
-PyAnsys metapackage
-===================
-|pyansys| |python| |pypi| |GH-CI| |MIT| |black| |pre-commit|
-
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
-   :alt: PyAnsys
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/pyansys?logo=pypi
-   :target: https://pypi.org/project/pyansys/
-   :alt: Python
-
-.. |pypi| image:: https://img.shields.io/pypi/v/pyansys.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pyansys/
-   :alt: PyPI
-
-.. |GH-CI| image:: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml/badge.svg
-   :target: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml
-   :alt: GH-CI
-
-.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-   :alt: MIT
-
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
-   :target: https://github.com/psf/black
-   :alt: Black
-
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyansys/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyansys/main
-   :alt: pre-commit.ci status
-
-Welcome to the PyAnsys metapackage repository. The ``pyansys`` metapackage
-provides a single package of collected PyAnsys packages that ensures compatibility
-of these packages amongst themselves and the Ansys product release that they are linked to.
-
-The ``pyansys`` metapackage ensures compatibility between these PyAnsys packages:
-
-- `PyAEDT <https://aedt.docs.pyansys.com/>`_: Pythonic interface to AEDT (Ansys Electronics Desktop).
-- `PyAnsys Geometry <https://geometry.docs.pyansys.com/>`_: Pythonic interface to the Ansys Geometry service.
-- `PyAnsys Math <https://math.docs.pyansys.com/>`_: Pythonic interface to PyAnsys Math libraries.
-- `PyDPF - Core <https://dpf.docs.pyansys.com/>`_: Pythonic interface to Ansys DPF (Data Processing Framework) for building more advanced and customized workflows.
-- `PyDPF - Post <https://post.docs.pyansys.com/>`_: Pythonic interface to access and post process Ansys solver result files.
-- `PyDPF - Composites <https://composites.dpf.docs.pyansys.com/>`_: Pythonic interface for DPF's postprocessing of layered and short-fiber composite models.
-- `PyDyna <https://dyna.docs.pyansys.com/>`_: Pythonic interface to build the Ansys DYNA input deck, submit it to the Ansys LS-DYNA solver and postprocess its results.
-- `PyDynamicReporting <https://dynamicreporting.docs.pyansys.com/>`_: Pythonic interface to Ansys Dynamic Reporting for service and control of its database and reports.
-- `PyEnSight <https://ensight.docs.pyansys.com/>`_: Pythonic interface to EnSight, the Ansys simulation postprocessor.
-- `PyFluent <https://fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent.
-- `PyFluent - Parametric <https://parametric.fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent parametric workflows.
-- `PyFluent - Visualization <https://visualization.fluent.docs.pyansys.com/>`_: Pythonic interface to visualize Ansys Fluent simulations.
-- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APDL).
-- `PyMAPDL Reader <https://reader.docs.pyansys.com/>`_: Pythonic interface to read legacy MAPDL result files (MAPDL 14.5 and later).
-- `PyMechanical <https://mechanical.docs.pyansys.com/>`_: Pythonic interface to Ansys Mechanical.
-- `PyMotorCAD <https://motorcad.docs.pyansys.com/>`_: Pythonic interface to Ansys Motor-CAD.
-- `PyOptislang <https://optislang.docs.pyansys.com/>`_: Pythonic interface to Ansys Optislang.
-- `PyPIM <https://pypim.docs.pyansys.com/>`_: Pythonic interface to communicate with the Ansys PIM (Product Instance Management) API.
-- `PyPrimeMesh <https://prime.docs.pyansys.com/>`_: Pythonic interface to Ansys Prime Server, which delivers core Ansys meshing technology.
-- `PySeascape <https://seascape.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys RedHawkSC and TotemSC.
-- `PySherlock <https://sherlock.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys Sherlock.
-- `PySystemCoupling <https://systemcoupling.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys System Coupling.
-- `PyTwin <https://twin.docs.pyansys.com/>`_: Pythonic interface to communicate with consumption workflows for Ansys digital twins.
-- `Granta MI BoM Analytics <https://bomanalytics.grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI BoM Analytics services.
-- `Granta MI RecordLists <https://recordlists.grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI Lists API.
-- `Shared Components <https://shared.docs.pyansys.com/>`_: Shared Ansys software components to enable package interoperability and minimize maintenance.
-
-Other tools delivered as part of the metapackage are:
-
-- `Ansys Tools Path <https://path.tools.docs.pyansys.com/>`_: Library to locate Ansys products in a local machine.
-- `Ansys Tools Protobuf Compilation Helper <https://ansys.github.io/ansys-tools-protoc-helper/>`_: Utility library to compile ``.proto`` files to Python source when building the package wheel.
-- `PyAnsys Tools Report <https://report.tools.docs.pyansys.com/>`_:  Tool for reporting your Python environment's package versions and hardware resources in a standardized way.
-- `PyAnsys Tools Versioning <https://versioning.tools.docs.pyansys.com/>`_: Tool for backwards and forwards server support.
-- `PyAnsys Units <https://units.docs.pyansys.com/>`_: Pythonic interface for units, unit systems, and unit conversions.
-
-Much effort is underway to continue expanding and developing packages in the
-`PyAnsys GitHub <https://github.com/ansys/>`__ account. On the ``Issues`` page
-for each package, you can post issues and request new features. You can also feel
-free to post a question on the `Ansys Developer Forums <https://discuss.ansys.com/>`_.
-
-By default, the PyAnsys metapackage installs these core modules:
-
-- `PyAEDT`_
-- `PyAnsys Geometry`_
-- `PyAnsys Math`_
-- `PyDPF - Core`_
-- `PyDPF - Post`_
-- `PyDPF - Composites`_
-- `PyDyna`_
-- `PyDynamicReporting`_
-- `PyEnSight`_
-- `PyFluent`_
-- `PyMAPDL`_
-- `PyMechanical`_
-- `PyMotorCAD`_
-- `PyOptislang`_
-- `PyPIM`_
-- `PyPrimeMesh`_
-- `PySeascape`_
-- `PySherlock`_
-- `PySystemCoupling`_
-- `PyTwin`_
-- `Granta MI BoM Analytics`_
-- `Granta MI RecordLists`_
-- `Shared Components`_
-
-Additionally, the ``pyansys`` metapackage contains certain extra targets that
-can be installed upon request:
-
-- **mapdl-all**: This target installs the core packages and `PyMAPDL Reader`_.
-- **fluent-all**: This target installs the core packages, `PyFluent - Parametric`_, and `PyFluent - Visualization`_.
-- **tools**: This target installs the core packages, `Ansys Tools Path`_, `Ansys Tools Protobuf Compilation Helper`_, `PyAnsys Tools Versioning`_, `PyAnsys Tools Report`_, and `PyAnsys Units`_.
-- **all**: This target installs all extra ``pyansys`` packages.
-
-Package installation
---------------------
-
-Two installation modes are provided: user and offline.
-
-User mode installation
-^^^^^^^^^^^^^^^^^^^^^^
-
-Before installing the ``pyansys`` metapackage in user mode, ensure that you have
-the latest version of `pip <https://pypi.org/project/pip/>`_ with this command:
-
-.. code:: bash
-
-    python -m pip install -U pip
-
-Then, install the ``pyansys`` metapackage with this command:
-
-.. code:: bash
-
-   python -m pip install pyansys
-
-If you are interested in **installing an extra target** such as ``fluent-all``,
-you use a command like this:
-
-.. code:: bash
-
-   python -m pip install pyansys[fluent-all]
-
-If you are interested in **installing a specific version** such as ``2023.1.0``,
-you use a command like this:
-
-.. code:: bash
-
-   python -m pip install pyansys==2023.1.0
-
-Offline mode installation
-^^^^^^^^^^^^^^^^^^^^^^^^^
-
-If you lack an internet connection on your installation machine, the recommended way of installing
-the ``pyansys`` metapackage is downloading the wheelhouse archive from the
-`Releases Page <https://github.com/ansys/pyansys/releases>`_ for your corresponding machine architecture.
-
-Each wheelhouse archive contains all the Python wheels necessary to install the ``pyansys`` metapackage from
-scratch on Windows, Linux, and MacOS from Python 3.8 to 3.11. You can install this on an isolated system with
-a fresh Python installation or on a virtual environment.
-
-For example, on Linux with Python 3.8, unzip the wheelhouse archive and install it with the following
-commands:
-
-.. code:: bash
-
-    unzip pyansys-v2024.1rc1-wheelhouse-Linux-3.8-core.zip wheelhouse
-    pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
-
-If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
-the same ``pip`` command as in the previous example.
-
-Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
-
-Versioning system
------------------
-
-The ``pyansys`` metapackage follows a semantic-like versioning system, though it has been adapted to the
-Ansys product release mechanism. Thus, this kind of versioning system is followed:
-
-.. code:: bash
-
-   XXXX.Y.ZZ
-
-Where:
-
-- ``XXXX`` is the Ansys product release year (for example, 2022).
-- ``Y`` is the Ansys product release within the same year (for example, 1, which relates to R1).
-- ``ZZ`` is a patched version to the ``pyansys`` metapackage, if any.
-
-Consequently, the first ``pyansys`` metapackage compatible with the 2024 R2 release would be:
-
-.. code:: bash
-
-   2024.2.0
-
-Any subsequent patched version of this package would be:
-
-.. code:: bash
-
-   2024.2.1
-   2024.2.2
-   2024.2.3
-   ...
-
-You can request a specific version install when using ``pip`` to install
-your package:
-
-.. code:: bash
-
-   python -m pip install pyansys==2024.2.0
-
-License and acknowledgments
----------------------------
-All PyAnsys libraries are licensed under the MIT license.
-
-PyAnsys libraries make no commercial claim over Ansys whatsoever.
-These libraries extend the functionality of Ansys products by
-adding Python interfaces to legally obtained software products
-without changing the core behaviors or licenses of the original
-software.
-
-For more information on Ansys products, visit the `Ansys web site <https://www.ansys.com/>`_.
+PyAnsys metapackage
+===================
+|pyansys| |python| |pypi| |downloads| |GH-CI| |MIT| |black| |pre-commit|
+
+.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://docs.pyansys.com/
+   :alt: PyAnsys
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/pyansys?logo=pypi
+   :target: https://pypi.org/project/pyansys/
+   :alt: Python
+
+.. |pypi| image:: https://img.shields.io/pypi/v/pyansys.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/pyansys/
+   :alt: PyPI
+
+.. |downloads| image:: https://img.shields.io/pypi/dm/pyansys.svg
+   :target: https://pypi.org/project/pyansys/
+   :alt: PyPI Downloads
+
+.. |GH-CI| image:: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml/badge.svg
+   :target: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml
+   :alt: GH-CI
+
+.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: MIT
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyansys/main.svg
+   :target: https://results.pre-commit.ci/latest/github/pyansys/pyansys/main
+   :alt: pre-commit.ci status
+
+Welcome to the PyAnsys metapackage repository. The ``pyansys`` metapackage
+provides a single package of collected PyAnsys packages that ensures compatibility
+of these packages amongst themselves and the Ansys product release that they are linked to.
+
+.. image:: https://raw.githubusercontent.com/ansys/pyansys/main/doc/source/_static/pyansys_dark.png
+   :target: https://docs.pyansys.com
+   :alt: PyAnsys
+
+The ``pyansys`` metapackage ensures compatibility between these PyAnsys packages:
+
+- `PyACP <https://acp.docs.pyansys.com/>`_: Pythonic interface to Ansys Composite PrepPost (ACP).
+- `PyAdditive <https://additive.docs.pyansys.com/>`_: Pythonic interface to the Ansys Additive service.
+- `PyAEDT <https://aedt.docs.pyansys.com/>`_: Pythonic interface to AEDT (Ansys Electronics Desktop).
+- `PyAnsys Geometry <https://geometry.docs.pyansys.com/>`_: Pythonic interface to the Ansys Geometry service.
+- `PyAnsys Math <https://math.docs.pyansys.com/>`_: Pythonic interface to PyAnsys Math libraries.
+- `PyDPF - Core <https://dpf.docs.pyansys.com/>`_: Pythonic interface to Ansys DPF (Data Processing Framework) for building more advanced and customized workflows.
+- `PyDPF - Post <https://post.docs.pyansys.com/>`_: Pythonic interface to access and post process Ansys solver result files.
+- `PyDPF - Composites <https://composites.dpf.docs.pyansys.com/>`_: Pythonic interface for DPF's postprocessing of layered and short-fiber composite models.
+- `PyDyna <https://dyna.docs.pyansys.com/>`_: Pythonic interface to build the Ansys DYNA input deck, submit it to the Ansys LS-DYNA solver and postprocess its results.
+- `PyDynamicReporting <https://dynamicreporting.docs.pyansys.com/>`_: Pythonic interface to Ansys Dynamic Reporting for service and control of its database and reports.
+- `PyEDB <https://edb.docs.pyansys.com/>`_: Pythonic interface to use the Electronics Database (EDB) client library.
+- `PyEDB - Core <https://edb.core.docs.pyansys.com/>`_: Pythonic interface to the Electronics Database (EDB).
+- `PyEnSight <https://ensight.docs.pyansys.com/>`_: Pythonic interface to EnSight, the Ansys simulation postprocessor.
+- `PyFluent <https://fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent.
+- `PyFluent - Parametric <https://parametric.fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent parametric workflows.
+- `PyFluent - Visualization <https://visualization.fluent.docs.pyansys.com/>`_: Pythonic interface to visualize Ansys Fluent simulations.
+- `PyGranta <https://grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI services.
+- `PyHPS <https://hps.docs.pyansys.com/version/dev/>`_: A Python client for Ansys HPC Platform Services (HPS).
+- `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APDL).
+- `PyMAPDL Reader <https://reader.docs.pyansys.com/>`_: Pythonic interface to read legacy MAPDL result files (MAPDL 14.5 and later).
+- `PyMechanical <https://mechanical.docs.pyansys.com/>`_: Pythonic interface to Ansys Mechanical.
+- `PyModelCenter <https://modelcenter.docs.pyansys.com/version/stable/>`_: Pythonic interface for Ansys ModelCenter
+- `PyMotorCAD <https://motorcad.docs.pyansys.com/>`_: Pythonic interface to Ansys Motor-CAD.
+- `PyOptislang <https://optislang.docs.pyansys.com/>`_: Pythonic interface to Ansys Optislang.
+- `PyPIM <https://pypim.docs.pyansys.com/>`_: Pythonic interface to communicate with the Ansys PIM (Product Instance Management) API.
+- `PyPrimeMesh <https://prime.docs.pyansys.com/>`_: Pythonic interface to Ansys Prime Server, which delivers core Ansys meshing technology.
+- `PyRocky <https://rocky.docs.pyansys.com/>`_: Python library to communicate with Ansys Rocky using Rocky PrePost API.
+- `PySeascape <https://seascape.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys RedHawkSC and TotemSC.
+- `PySherlock <https://sherlock.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys Sherlock.
+- `PySimAI <https://simai.docs.pyansys.com/>`_: Pythonic interface to use SimAI.
+- `PySystemCoupling <https://systemcoupling.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys System Coupling.
+- `PyTurboGrid <https://turbogrid.docs.pyansys.com/>`_: Pythonic interface to Ansys TurboGrid, a high-quality turbomachinery meshing software app.
+- `PyTwin <https://twin.docs.pyansys.com/>`_: Pythonic interface to communicate with consumption workflows for Ansys digital twins.
+- `Shared Components <https://shared.docs.pyansys.com/>`_: Shared Ansys software components to enable package interoperability and minimize maintenance.
+
+Other tools delivered as part of the metapackage are:
+
+- `Ansys Tools Path <https://path.tools.docs.pyansys.com/>`_: Library to locate Ansys products in a local machine.
+- `Ansys Tools Protobuf Compilation Helper <https://ansys.github.io/ansys-tools-protoc-helper/>`_: Utility library to compile ``.proto`` files to Python source when building the package wheel.
+- `PyAnsys Tools Report <https://report.tools.docs.pyansys.com/>`_:  Tool for reporting your Python environment's package versions and hardware resources in a standardized way.
+- `PyAnsys Tools Versioning <https://versioning.tools.docs.pyansys.com/>`_: Tool for backwards and forwards server support.
+- `PyAnsys Units <https://units.docs.pyansys.com/>`_: Pythonic interface for units, unit systems, and unit conversions.
+
+Much effort is underway to continue expanding and developing packages in the
+`PyAnsys GitHub <https://github.com/ansys/>`__ account. On the ``Issues`` page
+for each package, you can post issues and request new features. You can also feel
+free to post a question on the `Ansys Developer Forums <https://discuss.ansys.com/>`_.
+
+By default, the PyAnsys metapackage installs these core modules:
+
+- `PyACP`_
+- `PyAdditive`_
+- `PyAEDT`_
+- `PyAnsys Geometry`_
+- `PyAnsys Math`_
+- `PyDPF - Core`_
+- `PyDPF - Post`_
+- `PyDPF - Composites`_
+- `PyDyna`_
+- `PyDynamicReporting`_
+- `PyEDB`_
+- `PyEDB - Core`_
+- `PyEnSight`_
+- `PyFluent`_
+- `PyGranta`_
+- `PyHPS`_
+- `PyMAPDL`_
+- `PyMechanical`_
+- `PyMotorCAD`_
+- `PyOptislang`_
+- `PyPIM`_
+- `PyPrimeMesh`_
+- `PyRocky`_
+- `PySeascape`_
+- `PySherlock`_
+- `PySimAI`_
+- `PySystemCoupling`_
+- `PyTurboGrid`_
+- `PyTwin`_
+- `Shared Components`_
+
+Additionally, the ``pyansys`` metapackage contains certain extra targets that
+can be installed upon request:
+
+- **mapdl-all**: This target installs the core packages and `PyMAPDL Reader`_.
+- **fluent-all**: This target installs the core packages, `PyFluent - Parametric`_, and `PyFluent - Visualization`_.
+- **tools**: This target installs the core packages, `Ansys Tools Path`_, `Ansys Tools Protobuf Compilation Helper`_, `PyAnsys Tools Versioning`_, `PyAnsys Tools Report`_, and `PyAnsys Units`_.
+- **all**: This target installs all extra ``pyansys`` packages.
+
+Package installation
+--------------------
+
+Two installation modes are provided: user and offline.
+
+User mode installation
+^^^^^^^^^^^^^^^^^^^^^^
+
+Before installing the ``pyansys`` metapackage in user mode, ensure that you have
+the latest version of `pip <https://pypi.org/project/pip/>`_ with this command:
+
+.. code:: bash
+
+    python -m pip install -U pip
+
+Then, install the ``pyansys`` metapackage with this command:
+
+.. code:: bash
+
+   python -m pip install pyansys
+
+If you are interested in **installing an extra target** such as ``fluent-all``,
+you use a command like this:
+
+.. code:: bash
+
+   python -m pip install pyansys[fluent-all]
+
+If you are interested in **installing a specific version** such as ``2023.1.0``,
+you use a command like this:
+
+.. code:: bash
+
+   python -m pip install pyansys==2023.1.0
+
+Offline mode installation
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you lack an internet connection on your installation machine, the recommended way of installing
+the ``pyansys`` metapackage is downloading the wheelhouse archive from the
+`Releases Page <https://github.com/ansys/pyansys/releases>`_ for your corresponding machine architecture.
+
+Each wheelhouse archive contains all the Python wheels necessary to install the ``pyansys`` metapackage from
+scratch on Windows, Linux, and MacOS from Python 3.9 to 3.11. You can install this on an isolated system with
+a fresh Python installation or on a virtual environment.
+
+For example, on Linux with Python 3.9, unzip the wheelhouse archive and install it with the following
+commands:
+
+.. code:: bash
+
+    unzip pyansys-v2024.2.0b1-wheelhouse-Linux-3.9-core.zip wheelhouse
+    pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
+
+If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
+the same ``pip`` command as in the previous example.
+
+Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
+
+Versioning system
+-----------------
+
+The ``pyansys`` metapackage follows a semantic-like versioning system, though it has been adapted to the
+Ansys product release mechanism. Thus, this kind of versioning system is followed:
+
+.. code:: bash
+
+   XXXX.Y.ZZ
+
+Where:
+
+- ``XXXX`` is the Ansys product release year (for example, 2022).
+- ``Y`` is the Ansys product release within the same year (for example, 1, which relates to R1).
+- ``ZZ`` is a patched version to the ``pyansys`` metapackage, if any.
+
+Consequently, the first ``pyansys`` metapackage compatible with the 2024 R2 release would be:
+
+.. code:: bash
+
+   2024.2.0
+
+Any subsequent patched version of this package would be:
+
+.. code:: bash
+
+   2024.2.1
+   2024.2.2
+   2024.2.3
+   ...
+
+You can request a specific version install when using ``pip`` to install
+your package:
+
+.. code:: bash
+
+   python -m pip install pyansys==2024.2.0
+
+License and acknowledgments
+---------------------------
+All PyAnsys libraries are licensed under the MIT license.
+
+PyAnsys libraries make no commercial claim over Ansys whatsoever.
+These libraries extend the functionality of Ansys products by
+adding Python interfaces to legally obtained software products
+without changing the core behaviors or licenses of the original
+software.
+
+For more information on Ansys products, visit the `Ansys web site <https://www.ansys.com/>`_.
```

### Comparing `pyansys-2024.1rc1/PKG-INFO` & `pyansys-2024.2.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,102 @@
 Metadata-Version: 2.1
 Name: pyansys
-Version: 2024.1rc1
+Version: 2024.2.0b1
 Summary: Pythonic interfaces to Ansys products
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
-Requires-Dist: ansys-dpf-composites==0.3.1
-Requires-Dist: ansys-dpf-core==0.9.0
-Requires-Dist: ansys-dpf-post==0.5.0
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ansys-acp-core==0.1b1
+Requires-Dist: ansys-additive-core==0.17.2
+Requires-Dist: ansys-dpf-composites==0.4.0
+Requires-Dist: ansys-dpf-core==0.12.0
+Requires-Dist: ansys-dpf-post==0.8.0
 Requires-Dist: ansys-dpf-gate==0.4.1
-Requires-Dist: ansys-dyna-core==0.4.2
-Requires-Dist: ansys-dynamicreporting-core==0.5.0
-Requires-Dist: ansys-geometry-core==0.4rc1
-Requires-Dist: ansys-grantami-bomanalytics==1.2.0
-Requires-Dist: ansys-grantami-recordlists==1.0.0.post1
-Requires-Dist: ansys-fluent-core==0.17.1
-Requires-Dist: ansys-mapdl-core==0.66.0
+Requires-Dist: ansys-dyna-core==0.4.15
+Requires-Dist: ansys-dynamicreporting-core==0.5.1
+Requires-Dist: ansys-edb-core==0.1.4
+Requires-Dist: ansys-fluent-core==0.20.0
+Requires-Dist: ansys-geometry-core==0.4.14
+Requires-Dist: ansys-hps-client==0.8.0
+Requires-Dist: ansys-mapdl-core==0.68.1
 Requires-Dist: ansys-math-core==0.1.3
-Requires-Dist: ansys-mechanical-core==0.10.2
-Requires-Dist: ansys-meshing-prime==0.5.0.dev6
-Requires-Dist: ansys-motorcad-core==0.2.0
+Requires-Dist: ansys-mechanical-core==0.10.9
+Requires-Dist: ansys-meshing-prime==0.5.1
+Requires-Dist: ansys-modelcenter-workflow==0.1.1
+Requires-Dist: ansys-motorcad-core==0.4.3
+Requires-Dist: ansys-openapi-common==1.5.1
+Requires-Dist: ansys-optislang-core==0.6.3
 Requires-Dist: ansys-platform-instancemanagement==1.1.2
-Requires-Dist: ansys-pyensight-core==0.6.0
-Requires-Dist: ansys-openapi-common==1.2.2
-Requires-Dist: ansys-optislang-core==0.4.0
+Requires-Dist: ansys-pyensight-core==0.7.11
+Requires-Dist: ansys-rocky-core==0.1.0
 Requires-Dist: ansys-seascape==0.2.0
-Requires-Dist: ansys-sherlock-core==0.4.0
-Requires-Dist: ansys-systemcoupling-core==0.3.0
-Requires-Dist: pyaedt==0.6.94
-Requires-Dist: pytwin==0.5.0
-Requires-Dist: ansys-mapdl-reader==0.52.20 ; extra == "all"
-Requires-Dist: ansys-fluent-visualization==0.7.1 ; extra == "all"
-Requires-Dist: ansys-fluent-parametric==0.8.1 ; extra == "all"
-Requires-Dist: ansys-units==0.1.0 ; extra == "all"
-Requires-Dist: ansys-tools-path==0.3.1 ; extra == "all"
-Requires-Dist: pyansys-tools-report==0.6.0 ; extra == "all"
-Requires-Dist: pyansys-tools-versioning==0.4.0 ; extra == "all"
+Requires-Dist: ansys-sherlock-core==0.5.0
+Requires-Dist: ansys-simai-core==0.1.4
+Requires-Dist: ansys-systemcoupling-core==0.4.1
+Requires-Dist: ansys-turbogrid-core==0.4.0
+Requires-Dist: pyaedt==0.8.7
+Requires-Dist: pyedb==0.7.1
+Requires-Dist: pygranta==2024.1.0
+Requires-Dist: pytwin==0.6.0
+Requires-Dist: ansys-mapdl-reader==0.53.0 ; extra == "all"
+Requires-Dist: ansys-fluent-visualization==0.9.0 ; extra == "all"
+Requires-Dist: ansys-fluent-parametric==0.10.0 ; extra == "all"
+Requires-Dist: ansys-units==0.3.2 ; extra == "all"
+Requires-Dist: ansys-tools-path==0.5.1 ; extra == "all"
+Requires-Dist: pyansys-tools-report==0.7.0 ; extra == "all"
+Requires-Dist: pyansys-tools-versioning==0.5.0 ; extra == "all"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.11.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
-Requires-Dist: ansys-fluent-visualization==0.7.1 ; extra == "fluent-all"
-Requires-Dist: ansys-fluent-parametric==0.8.1 ; extra == "fluent-all"
-Requires-Dist: ansys-mapdl-reader==0.52.20 ; extra == "mapdl-all"
-Requires-Dist: ansys-units==0.1.0 ; extra == "tools"
-Requires-Dist: ansys-tools-path==0.3.1 ; extra == "tools"
-Requires-Dist: pyansys-tools-report==0.6.0 ; extra == "tools"
-Requires-Dist: pyansys-tools-versioning==0.4.0 ; extra == "tools"
+Requires-Dist: ansys-fluent-visualization==0.9.0 ; extra == "fluent-all"
+Requires-Dist: ansys-fluent-parametric==0.10.0 ; extra == "fluent-all"
+Requires-Dist: ansys-mapdl-reader==0.53.0 ; extra == "mapdl-all"
+Requires-Dist: ansys-units==0.3.2 ; extra == "tools"
+Requires-Dist: ansys-tools-path==0.5.1 ; extra == "tools"
+Requires-Dist: pyansys-tools-report==0.7.0 ; extra == "tools"
+Requires-Dist: pyansys-tools-versioning==0.5.0 ; extra == "tools"
 Project-URL: Documentation, https://docs.pyansys.com
 Project-URL: Source, https://github.com/ansys/pyansys
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: fluent-all
 Provides-Extra: mapdl-all
 Provides-Extra: tools
 
 PyAnsys metapackage
 ===================
-|pyansys| |python| |pypi| |GH-CI| |MIT| |black| |pre-commit|
+|pyansys| |python| |pypi| |downloads| |GH-CI| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/pyansys?logo=pypi
    :target: https://pypi.org/project/pyansys/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/pyansys.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/pyansys/
    :alt: PyPI
 
+.. |downloads| image:: https://img.shields.io/pypi/dm/pyansys.svg
+   :target: https://pypi.org/project/pyansys/
+   :alt: PyPI Downloads
+
 .. |GH-CI| image:: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml/badge.svg
    :target: https://github.com/ansys/pyansys/actions/workflows/ci-build.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
@@ -98,41 +109,53 @@
    :target: https://results.pre-commit.ci/latest/github/pyansys/pyansys/main
    :alt: pre-commit.ci status
 
 Welcome to the PyAnsys metapackage repository. The ``pyansys`` metapackage
 provides a single package of collected PyAnsys packages that ensures compatibility
 of these packages amongst themselves and the Ansys product release that they are linked to.
 
+.. image:: https://raw.githubusercontent.com/ansys/pyansys/main/doc/source/_static/pyansys_dark.png
+   :target: https://docs.pyansys.com
+   :alt: PyAnsys
+
 The ``pyansys`` metapackage ensures compatibility between these PyAnsys packages:
 
+- `PyACP <https://acp.docs.pyansys.com/>`_: Pythonic interface to Ansys Composite PrepPost (ACP).
+- `PyAdditive <https://additive.docs.pyansys.com/>`_: Pythonic interface to the Ansys Additive service.
 - `PyAEDT <https://aedt.docs.pyansys.com/>`_: Pythonic interface to AEDT (Ansys Electronics Desktop).
 - `PyAnsys Geometry <https://geometry.docs.pyansys.com/>`_: Pythonic interface to the Ansys Geometry service.
 - `PyAnsys Math <https://math.docs.pyansys.com/>`_: Pythonic interface to PyAnsys Math libraries.
 - `PyDPF - Core <https://dpf.docs.pyansys.com/>`_: Pythonic interface to Ansys DPF (Data Processing Framework) for building more advanced and customized workflows.
 - `PyDPF - Post <https://post.docs.pyansys.com/>`_: Pythonic interface to access and post process Ansys solver result files.
 - `PyDPF - Composites <https://composites.dpf.docs.pyansys.com/>`_: Pythonic interface for DPF's postprocessing of layered and short-fiber composite models.
 - `PyDyna <https://dyna.docs.pyansys.com/>`_: Pythonic interface to build the Ansys DYNA input deck, submit it to the Ansys LS-DYNA solver and postprocess its results.
 - `PyDynamicReporting <https://dynamicreporting.docs.pyansys.com/>`_: Pythonic interface to Ansys Dynamic Reporting for service and control of its database and reports.
+- `PyEDB <https://edb.docs.pyansys.com/>`_: Pythonic interface to use the Electronics Database (EDB) client library.
+- `PyEDB - Core <https://edb.core.docs.pyansys.com/>`_: Pythonic interface to the Electronics Database (EDB).
 - `PyEnSight <https://ensight.docs.pyansys.com/>`_: Pythonic interface to EnSight, the Ansys simulation postprocessor.
 - `PyFluent <https://fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent.
 - `PyFluent - Parametric <https://parametric.fluent.docs.pyansys.com/>`_: Pythonic interface to Ansys Fluent parametric workflows.
 - `PyFluent - Visualization <https://visualization.fluent.docs.pyansys.com/>`_: Pythonic interface to visualize Ansys Fluent simulations.
+- `PyGranta <https://grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI services.
+- `PyHPS <https://hps.docs.pyansys.com/version/dev/>`_: A Python client for Ansys HPC Platform Services (HPS).
 - `PyMAPDL <https://mapdl.docs.pyansys.com/>`_: Pythonic interface to Ansys MAPDL (Mechanical APDL).
 - `PyMAPDL Reader <https://reader.docs.pyansys.com/>`_: Pythonic interface to read legacy MAPDL result files (MAPDL 14.5 and later).
 - `PyMechanical <https://mechanical.docs.pyansys.com/>`_: Pythonic interface to Ansys Mechanical.
+- `PyModelCenter <https://modelcenter.docs.pyansys.com/version/stable/>`_: Pythonic interface for Ansys ModelCenter
 - `PyMotorCAD <https://motorcad.docs.pyansys.com/>`_: Pythonic interface to Ansys Motor-CAD.
 - `PyOptislang <https://optislang.docs.pyansys.com/>`_: Pythonic interface to Ansys Optislang.
 - `PyPIM <https://pypim.docs.pyansys.com/>`_: Pythonic interface to communicate with the Ansys PIM (Product Instance Management) API.
 - `PyPrimeMesh <https://prime.docs.pyansys.com/>`_: Pythonic interface to Ansys Prime Server, which delivers core Ansys meshing technology.
+- `PyRocky <https://rocky.docs.pyansys.com/>`_: Python library to communicate with Ansys Rocky using Rocky PrePost API.
 - `PySeascape <https://seascape.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys RedHawkSC and TotemSC.
 - `PySherlock <https://sherlock.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys Sherlock.
+- `PySimAI <https://simai.docs.pyansys.com/>`_: Pythonic interface to use SimAI.
 - `PySystemCoupling <https://systemcoupling.docs.pyansys.com/>`_: Pythonic interface to communicate with Ansys System Coupling.
+- `PyTurboGrid <https://turbogrid.docs.pyansys.com/>`_: Pythonic interface to Ansys TurboGrid, a high-quality turbomachinery meshing software app.
 - `PyTwin <https://twin.docs.pyansys.com/>`_: Pythonic interface to communicate with consumption workflows for Ansys digital twins.
-- `Granta MI BoM Analytics <https://bomanalytics.grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI BoM Analytics services.
-- `Granta MI RecordLists <https://recordlists.grantami.docs.pyansys.com/>`_: Pythonic interface to Ansys Granta MI Lists API.
 - `Shared Components <https://shared.docs.pyansys.com/>`_: Shared Ansys software components to enable package interoperability and minimize maintenance.
 
 Other tools delivered as part of the metapackage are:
 
 - `Ansys Tools Path <https://path.tools.docs.pyansys.com/>`_: Library to locate Ansys products in a local machine.
 - `Ansys Tools Protobuf Compilation Helper <https://ansys.github.io/ansys-tools-protoc-helper/>`_: Utility library to compile ``.proto`` files to Python source when building the package wheel.
 - `PyAnsys Tools Report <https://report.tools.docs.pyansys.com/>`_:  Tool for reporting your Python environment's package versions and hardware resources in a standardized way.
@@ -142,36 +165,43 @@
 Much effort is underway to continue expanding and developing packages in the
 `PyAnsys GitHub <https://github.com/ansys/>`__ account. On the ``Issues`` page
 for each package, you can post issues and request new features. You can also feel
 free to post a question on the `Ansys Developer Forums <https://discuss.ansys.com/>`_.
 
 By default, the PyAnsys metapackage installs these core modules:
 
+- `PyACP`_
+- `PyAdditive`_
 - `PyAEDT`_
 - `PyAnsys Geometry`_
 - `PyAnsys Math`_
 - `PyDPF - Core`_
 - `PyDPF - Post`_
 - `PyDPF - Composites`_
 - `PyDyna`_
 - `PyDynamicReporting`_
+- `PyEDB`_
+- `PyEDB - Core`_
 - `PyEnSight`_
 - `PyFluent`_
+- `PyGranta`_
+- `PyHPS`_
 - `PyMAPDL`_
 - `PyMechanical`_
 - `PyMotorCAD`_
 - `PyOptislang`_
 - `PyPIM`_
 - `PyPrimeMesh`_
+- `PyRocky`_
 - `PySeascape`_
 - `PySherlock`_
+- `PySimAI`_
 - `PySystemCoupling`_
+- `PyTurboGrid`_
 - `PyTwin`_
-- `Granta MI BoM Analytics`_
-- `Granta MI RecordLists`_
 - `Shared Components`_
 
 Additionally, the ``pyansys`` metapackage contains certain extra targets that
 can be installed upon request:
 
 - **mapdl-all**: This target installs the core packages and `PyMAPDL Reader`_.
 - **fluent-all**: This target installs the core packages, `PyFluent - Parametric`_, and `PyFluent - Visualization`_.
@@ -217,23 +247,23 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you lack an internet connection on your installation machine, the recommended way of installing
 the ``pyansys`` metapackage is downloading the wheelhouse archive from the
 `Releases Page <https://github.com/ansys/pyansys/releases>`_ for your corresponding machine architecture.
 
 Each wheelhouse archive contains all the Python wheels necessary to install the ``pyansys`` metapackage from
-scratch on Windows, Linux, and MacOS from Python 3.8 to 3.11. You can install this on an isolated system with
+scratch on Windows, Linux, and MacOS from Python 3.9 to 3.11. You can install this on an isolated system with
 a fresh Python installation or on a virtual environment.
 
-For example, on Linux with Python 3.8, unzip the wheelhouse archive and install it with the following
+For example, on Linux with Python 3.9, unzip the wheelhouse archive and install it with the following
 commands:
 
 .. code:: bash
 
-    unzip pyansys-v2024.1rc1-wheelhouse-Linux-3.8-core.zip wheelhouse
+    unzip pyansys-v2024.2.0b1-wheelhouse-Linux-3.9-core.zip wheelhouse
     pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
 the same ``pip`` command as in the previous example.
 
 Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
```

