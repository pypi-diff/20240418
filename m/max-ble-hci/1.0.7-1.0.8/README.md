# Comparing `tmp/max_ble_hci-1.0.7.tar.gz` & `tmp/max_ble_hci-1.0.8.tar.gz`

## Comparing `max_ble_hci-1.0.7.tar` & `max_ble_hci-1.0.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/install.bat
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/install.sh
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/black-format-check.yml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/black-format-run.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/pypi-deploy.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.github/workflows/test-installer.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/make.bat
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/ble_hci.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/ble_standard.rst
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/constants.rst
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/controller_cmds.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/data_params.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/examples.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/hci_packets.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/hci_reference.rst
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/index.rst
--rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/informational_cmds.rst
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/installation.rst
--rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/le_controller_cmds.rst
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/link_control_cmds.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/modules.rst
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/overview.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/packet_codes.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/packet_defs.rst
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/status_cmds.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/utils.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/vendor_spec.rst
--rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/vendor_spec_cmds.rst
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/examples/dtm.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/examples/hello_hci.py
--rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/docs/source/images/ble_stack_diagram.jpeg
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/examples/dtm.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/examples/hello_hci.py
--rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci_cli.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/__init__.py
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/_hci_logger.py
--rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/_transport.py
--rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/ble_hci.py
--rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/ble_standard_cmds.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/constants.py
--rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/data_params.py
--rw-r--r--   0        0        0    19495 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/hci_packets.py
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/packet_codes.py
--rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/packet_defs.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/utils.py
--rw-r--r--   0        0        0    56095 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/src/max_ble_hci/vendor_spec_cmds.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/tests/test.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/LICENSE
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/install.bat
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/install.sh
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/black-format-check.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/black-format-run.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.github/workflows/test-installer.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/make.bat
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/ble_hci.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/ble_standard.rst
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/constants.rst
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/controller_cmds.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/data_params.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/examples.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/hci_packets.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/hci_reference.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/index.rst
+-rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/informational_cmds.rst
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/installation.rst
+-rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/le_controller_cmds.rst
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/link_control_cmds.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/modules.rst
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/overview.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/packet_codes.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/packet_defs.rst
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/status_cmds.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/utils.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/vendor_spec.rst
+-rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/vendor_spec_cmds.rst
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/examples/dtm.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/examples/hello_hci.py
+-rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/docs/source/images/ble_stack_diagram.jpeg
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/examples/dtm.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/examples/hello_hci.py
+-rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci_cli.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/__init__.py
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/_hci_logger.py
+-rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/_transport.py
+-rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/ble_hci.py
+-rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/ble_standard_cmds.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/constants.py
+-rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/data_params.py
+-rw-r--r--   0        0        0    19495 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/hci_packets.py
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/packet_codes.py
+-rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/packet_defs.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/utils.py
+-rw-r--r--   0        0        0    56077 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/src/max_ble_hci/vendor_spec_cmds.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/tests/test.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/LICENSE
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.0.8/PKG-INFO
```

### Comparing `max_ble_hci-1.0.7/.github/workflows/black-format-run.yml` & `max_ble_hci-1.0.8/.github/workflows/black-format-run.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/.github/workflows/documentation.yml` & `max_ble_hci-1.0.8/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/.github/workflows/pylint.yml` & `max_ble_hci-1.0.8/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/.github/workflows/pypi-deploy.yml` & `max_ble_hci-1.0.8/.github/workflows/pypi-deploy.yml`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - run: |
           set -e
+          python3 -m pip install --upgrade twine
           sudo chmod +x install.sh
           ./install.sh
           python3 -m twine upload --repository testpypi dist/*
           python3 -m twine upload --repository pypi dist/*
           set +e
```

### Comparing `max_ble_hci-1.0.7/.github/workflows/python-package-conda.yml` & `max_ble_hci-1.0.8/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/.github/workflows/test-installer.yml` & `max_ble_hci-1.0.8/.github/workflows/test-installer.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/Makefile` & `max_ble_hci-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/make.bat` & `max_ble_hci-1.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/conf.py` & `max_ble_hci-1.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/controller_cmds.rst` & `max_ble_hci-1.0.8/docs/source/controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/examples.rst` & `max_ble_hci-1.0.8/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/index.rst` & `max_ble_hci-1.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/informational_cmds.rst` & `max_ble_hci-1.0.8/docs/source/informational_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/installation.rst` & `max_ble_hci-1.0.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/le_controller_cmds.rst` & `max_ble_hci-1.0.8/docs/source/le_controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/link_control_cmds.rst` & `max_ble_hci-1.0.8/docs/source/link_control_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/overview.rst` & `max_ble_hci-1.0.8/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/status_cmds.rst` & `max_ble_hci-1.0.8/docs/source/status_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/vendor_spec_cmds.rst` & `max_ble_hci-1.0.8/docs/source/vendor_spec_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/examples/connection.py` & `max_ble_hci-1.0.8/docs/source/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/examples/dtm.py` & `max_ble_hci-1.0.8/docs/source/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/examples/hello_hci.py` & `max_ble_hci-1.0.8/docs/source/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/docs/source/images/ble_stack_diagram.jpeg` & `max_ble_hci-1.0.8/docs/source/images/ble_stack_diagram.jpeg`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/examples/connection.py` & `max_ble_hci-1.0.8/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/examples/dtm.py` & `max_ble_hci-1.0.8/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/examples/hello_hci.py` & `max_ble_hci-1.0.8/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci_cli.py` & `max_ble_hci-1.0.8/src/max_ble_hci_cli.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/__init__.py` & `max_ble_hci-1.0.8/src/max_ble_hci/__init__.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/_hci_logger.py` & `max_ble_hci-1.0.8/src/max_ble_hci/_hci_logger.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/_transport.py` & `max_ble_hci-1.0.8/src/max_ble_hci/_transport.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/ble_hci.py` & `max_ble_hci-1.0.8/src/max_ble_hci/ble_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/ble_standard_cmds.py` & `max_ble_hci-1.0.8/src/max_ble_hci/ble_standard_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/constants.py` & `max_ble_hci-1.0.8/src/max_ble_hci/constants.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/data_params.py` & `max_ble_hci-1.0.8/src/max_ble_hci/data_params.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/hci_packets.py` & `max_ble_hci-1.0.8/src/max_ble_hci/hci_packets.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/packet_codes.py` & `max_ble_hci-1.0.8/src/max_ble_hci/packet_codes.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/packet_defs.py` & `max_ble_hci-1.0.8/src/max_ble_hci/packet_defs.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/utils.py` & `max_ble_hci-1.0.8/src/max_ble_hci/utils.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/src/max_ble_hci/vendor_spec_cmds.py` & `max_ble_hci-1.0.8/src/max_ble_hci/vendor_spec_cmds.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             )
 
         if isinstance(payload, PayloadOption):
             payload = payload.value
         if isinstance(phy, PhyOption):
             phy = phy.value
 
-        params = [channel, packet_len, payload.value, phy.value]
+        params = [channel, packet_len, payload, phy]
         params.extend(to_le_nbyte_list(num_packets, 2))
         return self.send_vs_command(OCF.VENDOR_SPEC.TX_TEST, params=params)
 
     def rx_test_vs(
         self,
         channel: int = 0,
         phy: Union[PhyOption, int] = PhyOption.PHY_1M,
@@ -372,15 +372,15 @@
             raise ValueError(
                 f"Num packets too large ({num_packets}), must be 65535 or less."
             )
 
         if isinstance(phy, PhyOption):
             phy = phy.value
 
-        params = [channel, phy.value, modulation_idx]
+        params = [channel, phy, modulation_idx]
         params.extend(to_le_nbyte_list(num_packets, 2))
         return self.send_vs_command(OCF.VENDOR_SPEC.RX_TEST, params=params)
 
     def reset_test_stats(self) -> StatusCode:
         """Reset accumulated test stats.
 
         Sends a vendor-specific command to the DUT, telling it to
```

### Comparing `max_ble_hci-1.0.7/tests/test.py` & `max_ble_hci-1.0.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/LICENSE` & `max_ble_hci-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/README.md` & `max_ble_hci-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.0.7/pyproject.toml` & `max_ble_hci-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/max_ble_hci", "src/max_ble_hci_cli.py"]
 
 [project]
 name = "max_ble_hci"
-version = "1.0.7"
+version = "1.0.8"
 dependencies = [
     "pyserial",
     "pyreadline3 ; platform_system == 'Windows'",
     "gnureadline ; platform_system == 'Darwin'",
     "colorlog"
 ]
 requires-python = ">=3.8"
```

### Comparing `max_ble_hci-1.0.7/PKG-INFO` & `max_ble_hci-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: max_ble_hci
-Version: 1.0.7
+Version: 1.0.8
 Summary: BLE HCI Test interface for controllers capable of the UART transport
 Project-URL: Homepage, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Repository, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Documentation, https://analog-devices-msdk.github.io/MAX-BLE-HCI/
 Project-URL: Bug Tracker, https://github.com/Analog-Devices-MSDK/BLE-HCI/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
```

