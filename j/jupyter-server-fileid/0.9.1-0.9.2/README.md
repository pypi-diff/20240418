# Comparing `tmp/jupyter_server_fileid-0.9.1.tar.gz` & `tmp/jupyter_server_fileid-0.9.2.tar.gz`

## Comparing `jupyter_server_fileid-0.9.1.tar` & `jupyter_server_fileid-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.flake8
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.readthedocs.yaml
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/RELEASE.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/conftest.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.github/workflows/test-python.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/Makefile
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/conf.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/docs/user_guide/index.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter-config/jupyter_server_config.d/jupyter_server_fileid.json
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/cli.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/extension.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/handler.py
--rw-r--r--   0        0        0    34828 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/manager.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/jupyter_server_fileid/pytest_plugin.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/tests/test_handler.py
--rw-r--r--   0        0        0    20456 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/tests/test_manager.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/LICENSE
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/README.md
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.flake8
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    16548 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/RELEASE.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/conftest.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.github/workflows/test-python.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/Makefile
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/docs/user_guide/index.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter-config/jupyter_server_config.d/jupyter_server_fileid.json
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/cli.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/extension.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/handler.py
+-rw-r--r--   0        0        0    35464 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/manager.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/jupyter_server_fileid/pytest_plugin.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/tests/test_handler.py
+-rw-r--r--   0        0        0    20456 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/tests/test_manager.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/README.md
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 jupyter_server_fileid-0.9.2/PKG-INFO
```

### Comparing `jupyter_server_fileid-0.9.1/.pre-commit-config.yaml` & `jupyter_server_fileid-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/.readthedocs.yaml` & `jupyter_server_fileid-0.9.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/CHANGELOG.md` & `jupyter_server_fileid-0.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.9.2
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.9.1...501a1230ac2e934c70bbb7267144f16fe6ed3484))
+
+### Bugs fixed
+
+- Check for ID before creating a new record [#78](https://github.com/jupyter-server/jupyter_server_fileid/pull/78) ([@Zsailer](https://github.com/Zsailer))
+- Use a context manager for all write actions to prevent indefinite database locks [#77](https://github.com/jupyter-server/jupyter_server_fileid/pull/77) ([@Zsailer](https://github.com/Zsailer))
+
+### Maintenance and upkeep improvements
+
+- Update Release Scripts [#79](https://github.com/jupyter-server/jupyter_server_fileid/pull/79) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_server_fileid/graphs/contributors?from=2023-12-19&to=2024-04-18&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Ablink1073+updated%3A2023-12-19..2024-04-18&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Awelcome+updated%3A2023-12-19..2024-04-18&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3AZsailer+updated%3A2023-12-19..2024-04-18&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.9.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.9.0...a5e65c99791a20e4684c55f631d2d7fef3c3fdad))
 
 ### Bugs fixed
 
 - Add RTD config to fix CI [#73](https://github.com/jupyter-server/jupyter_server_fileid/pull/73) ([@dlqqq](https://github.com/dlqqq))
@@ -18,16 +39,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_server_fileid/graphs/contributors?from=2023-04-09&to=2023-12-19&type=c))
 
 [@cmd-ntrf](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Acmd-ntrf+updated%3A2023-04-09..2023-12-19&type=Issues) | [@codecov](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Acodecov+updated%3A2023-04-09..2023-12-19&type=Issues) | [@dlqqq](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Adlqqq+updated%3A2023-04-09..2023-12-19&type=Issues) | [@stonebig](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Astonebig+updated%3A2023-04-09..2023-12-19&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3Awelcome+updated%3A2023-04-09..2023-12-19&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_server_fileid+involves%3AZsailer+updated%3A2023-04-09..2023-12-19&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.9.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_server_fileid/compare/v0.8.0...505806162b4df60b4cbb461cfec1266b81df32ce))
 
 ### Enhancements made
 
 - add Jupyter Releaser workflows [#65](https://github.com/jupyter-server/jupyter_server_fileid/pull/65) ([@dlqqq](https://github.com/dlqqq))
```

### Comparing `jupyter_server_fileid-0.9.1/RELEASE.md` & `jupyter_server_fileid-0.9.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/.github/workflows/build.yml` & `jupyter_server_fileid-0.9.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/.github/workflows/check-release.yml` & `jupyter_server_fileid-0.9.2/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/.github/workflows/prep-release.yml` & `jupyter_server_fileid-0.9.2/.github/workflows/prep-release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,34 +8,42 @@
         required: false
       branch:
         description: "The branch to target"
         required: false
       post_version_spec:
         description: "Post Version Specifier"
         required: false
+      silent:
+        description: "Set a placeholder in the changelog and don't publish the release."
+        required: false
+        type: boolean
       since:
         description: "Use PRs with activity since this date or git reference"
         required: false
       since_last_stable:
         description: "Use PRs with activity since the last stable git tag"
         required: false
         type: boolean
 jobs:
   prep_release:
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Prep Release
         id: prep-release
         uses: jupyter-server/jupyter_releaser/.github/actions/prep-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
+          token: ${{ secrets.GITHUB_TOKEN }}
           version_spec: ${{ github.event.inputs.version_spec }}
+          silent: ${{ github.event.inputs.silent }}
           post_version_spec: ${{ github.event.inputs.post_version_spec }}
+          target: ${{ github.event.inputs.target }}
           branch: ${{ github.event.inputs.branch }}
           since: ${{ github.event.inputs.since }}
           since_last_stable: ${{ github.event.inputs.since_last_stable }}
 
       - name: "** Next Step **"
         run: |
           echo "Optional): Review Draft Release: ${{ steps.prep-release.outputs.release_url }}"
```

### Comparing `jupyter_server_fileid-0.9.1/.github/workflows/publish-release.yml` & `jupyter_server_fileid-0.9.2/.github/workflows/publish-release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,36 +11,40 @@
       steps_to_skip:
         description: "Comma separated list of steps to skip"
         required: false
 
 jobs:
   publish_release:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
+      - uses: actions/create-github-app-token@v1
+        id: app-token
+        with:
+          app-id: ${{ vars.APP_ID }}
+          private-key: ${{ secrets.APP_PRIVATE_KEY }}
+
       - name: Populate Release
         id: populate-release
         uses: jupyter-server/jupyter_releaser/.github/actions/populate-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
+          token: ${{ steps.app-token.outputs.token }}
           branch: ${{ github.event.inputs.branch }}
           release_url: ${{ github.event.inputs.release_url }}
           steps_to_skip: ${{ github.event.inputs.steps_to_skip }}
 
       - name: Finalize Release
         id: finalize-release
-        env:
-          PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
-          PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
-          TWINE_USERNAME: __token__
-          NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
-        uses: jupyter-server/jupyter-releaser/.github/actions/finalize-release@v2
+        uses: jupyter-server/jupyter_releaser/.github/actions/finalize-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
+          token: ${{ steps.app-token.outputs.token }}
           release_url: ${{ steps.populate-release.outputs.release_url }}
 
       - name: "** Next Step **"
         if: ${{ success() }}
         run: |
           echo "Verify the final release"
           echo ${{ steps.finalize-release.outputs.release_url }}
```

### Comparing `jupyter_server_fileid-0.9.1/.github/workflows/test-python.yml` & `jupyter_server_fileid-0.9.2/.github/workflows/test-python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,17 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
         with:
           python_version: "3.7"
-      - name: Install miniumum versions
-        uses: jupyterlab/maintainer-tools/.github/actions/install-minimums@v1
+          dependency_type: minimum
+      - name: Install
+        run: pip install -e ".[test]"
       - name: Run the unit tests
         run: |
           pytest -vv -W default || pytest -vv -W default --lf
 
   test_prereleases:
     name: Test Prereleases
     runs-on: ubuntu-latest
```

### Comparing `jupyter_server_fileid-0.9.1/docs/Makefile` & `jupyter_server_fileid-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/docs/conf.py` & `jupyter_server_fileid-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/docs/make.bat` & `jupyter_server_fileid-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/docs/_static/jupyter_logo.png` & `jupyter_server_fileid-0.9.2/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/docs/user_guide/index.md` & `jupyter_server_fileid-0.9.2/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/jupyter_server_fileid/extension.py` & `jupyter_server_fileid-0.9.2/jupyter_server_fileid/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/jupyter_server_fileid/handler.py` & `jupyter_server_fileid-0.9.2/jupyter_server_fileid/handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/jupyter_server_fileid/manager.py` & `jupyter_server_fileid-0.9.2/jupyter_server_fileid/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,73 +308,71 @@
             return None
 
         relpath = posixpath.relpath(path, self.root_dir)
         return relpath
 
     def _create(self, path: str) -> str:
         path = self._normalize_path(path)
-        id = self._uuid()
-        self.con.execute("INSERT INTO Files (id, path) VALUES (?, ?)", (id, path))
-        return id
-
-    def index(self, path: str) -> str:
-        path = self._normalize_path(path)
         row = self.con.execute("SELECT id FROM Files WHERE path = ?", (path,)).fetchone()
         existing_id = row and row[0]
 
         if existing_id:
             return existing_id
 
-        # create new record
-        id = self._create(path)
-        self.con.commit()
+        id = self._uuid()
+        self.con.execute("INSERT INTO Files (id, path) VALUES (?, ?)", (id, path))
         return id
 
+    def index(self, path: str) -> str:
+        # create new record
+        with self.con:
+            id = self._create(path)
+            return id
+
     def get_id(self, path: str) -> Optional[str]:
         path = self._normalize_path(path)
         row = self.con.execute("SELECT id FROM Files WHERE path = ?", (path,)).fetchone()
         return row and row[0]
 
     def get_path(self, id: str) -> Optional[str]:
         row = self.con.execute("SELECT path FROM Files WHERE id = ?", (id,)).fetchone()
         path = row and row[0]
         return self._from_normalized_path(path)
 
     def move(self, old_path: str, new_path: str) -> None:
-        old_path = self._normalize_path(old_path)
-        new_path = self._normalize_path(new_path)
-        row = self.con.execute("SELECT id FROM Files WHERE path = ?", (old_path,)).fetchone()
-        id = row and row[0]
-
-        if id:
-            self.con.execute("UPDATE Files SET path = ? WHERE path = ?", (new_path, old_path))
-            self._move_recursive(old_path, new_path, posixpath)
-        else:
-            id = self._create(new_path)
+        with self.con:
+            old_path = self._normalize_path(old_path)
+            new_path = self._normalize_path(new_path)
+            row = self.con.execute("SELECT id FROM Files WHERE path = ?", (old_path,)).fetchone()
+            id = row and row[0]
+
+            if id:
+                self.con.execute("UPDATE Files SET path = ? WHERE path = ?", (new_path, old_path))
+                self._move_recursive(old_path, new_path, posixpath)
+            else:
+                id = self._create(new_path)
 
-        self.con.commit()
-        return id
+            return id
 
     def copy(self, from_path: str, to_path: str) -> Optional[str]:
-        from_path = self._normalize_path(from_path)
-        to_path = self._normalize_path(to_path)
+        with self.con:
+            from_path = self._normalize_path(from_path)
+            to_path = self._normalize_path(to_path)
 
-        id = self._create(to_path)
-        self._copy_recursive(from_path, to_path, posixpath)
+            id = self._create(to_path)
+            self._copy_recursive(from_path, to_path, posixpath)
 
-        self.con.commit()
-        return id
+            return id
 
     def delete(self, path: str) -> None:
-        path = self._normalize_path(path)
+        with self.con:
+            path = self._normalize_path(path)
 
-        self.con.execute("DELETE FROM Files WHERE path = ?", (path,))
-        self._delete_recursive(path, posixpath)
-
-        self.con.commit()
+            self.con.execute("DELETE FROM Files WHERE path = ?", (path,))
+            self._delete_recursive(path, posixpath)
 
     def save(self, path: str) -> None:
         return
 
     def get_handlers_by_action(self) -> Dict[str, Optional[Callable[[Dict[str, Any]], Any]]]:
         return {
             "get": None,
@@ -622,14 +620,15 @@
         if crtime != stat_info.crtime:
             self.con.execute("DELETE FROM Files WHERE id = ?", (id,))
             return None
 
         # otherwise update existing record with new path, moving any indexed
         # children if necessary. then return its id
         self._update(id, path=path)
+
         if stat_info.is_dir and old_path != path:
             self._move_recursive(old_path, path)
             self._update_cursor = True
 
         return id
 
     def _parse_raw_stat(self, raw_stat):
@@ -668,14 +667,25 @@
 
         Notes
         -----
         - Because of the uniqueness constraint on `ino`, this method is
         dangerous and may throw a runtime error if the file is not guaranteed to
         have a unique `ino`.
         """
+        # If the path exists
+        existing_id, ino = None, None
+        row = self.con.execute("SELECT id, ino FROM Files WHERE path = ?", (path,)).fetchone()
+        if row:
+            existing_id, ino = row
+
+        # If the file ID already exists and the current file matches our records
+        # return the file ID instead of creating a new one.
+        if existing_id and stat_info.ino == ino:
+            return existing_id
+
         id = self._uuid()
         self.con.execute(
             "INSERT INTO Files (id, path, ino, crtime, mtime, is_dir) VALUES (?, ?, ?, ?, ?, ?)",
             (id, path, stat_info.ino, stat_info.crtime, stat_info.mtime, stat_info.is_dir),
         )
         return id
 
@@ -714,47 +724,46 @@
                 (path, id),
             )
             return
 
     def index(self, path, stat_info=None, commit=True):
         """Returns the file ID for the file at `path`, creating a new file ID if
         one does not exist. Returns None only if file does not exist at path."""
-        path = self._normalize_path(path)
-        stat_info = stat_info or self._stat(path)
-        if not stat_info:
-            return None
+        with self.con:
+            path = self._normalize_path(path)
+            stat_info = stat_info or self._stat(path)
+            if not stat_info:
+                return None
 
-        # if file is symlink, then index the path it refers to instead
-        if stat_info.is_symlink:
-            return self.index(os.path.realpath(path))
+            # if file is symlink, then index the path it refers to instead
+            if stat_info.is_symlink:
+                return self.index(os.path.realpath(path))
+
+            # sync file at path and return file ID if it exists
+            id = self._sync_file(path, stat_info)
+            if id is not None:
+                return id
 
-        # sync file at path and return file ID if it exists
-        id = self._sync_file(path, stat_info)
-        if id is not None:
+            # otherwise, create a new record and return the file ID
+            id = self._create(path, stat_info)
             return id
 
-        # otherwise, create a new record and return the file ID
-        id = self._create(path, stat_info)
-        if commit:
-            self.con.commit()
-        return id
-
     def get_id(self, path):
         """Retrieves the file ID associated with a file path. Returns None if
         the file has not yet been indexed or does not exist at the given
         path."""
-        path = self._normalize_path(path)
-        stat_info = self._stat(path)
-        if not stat_info:
-            return None
+        with self.con:
+            path = self._normalize_path(path)
+            stat_info = self._stat(path)
+            if not stat_info:
+                return None
 
-        # then sync file at path and retrieve id, if any
-        id = self._sync_file(path, stat_info)
-        self.con.commit()
-        return id
+            # then sync file at path and retrieve id, if any
+            id = self._sync_file(path, stat_info)
+            return id
 
     def get_path(self, id):
         """Retrieves the file path associated with a file ID. The file path is
         relative to `self.root_dir`. Returns None if the ID does not
         exist in the Files table, if the path no longer has a
         file, or if the path is not a child of `self.root_dir`.
 
@@ -791,34 +800,34 @@
     @log(
         lambda self, old_path, new_path: f"Updating index following move from {old_path} to {new_path}.",
         lambda self, old_path, new_path: f"Successfully updated index following move from {old_path} to {new_path}.",
     )
     def move(self, old_path, new_path):
         """Handles file moves by updating the file path of the associated file
         ID.  Returns the file ID. Returns None if file does not exist at new_path."""
-        old_path = self._normalize_path(old_path)
-        new_path = self._normalize_path(new_path)
+        with self.con:
+            old_path = self._normalize_path(old_path)
+            new_path = self._normalize_path(new_path)
 
-        # verify file exists at new_path
-        stat_info = self._stat(new_path)
-        if stat_info is None:
-            return None
+            # verify file exists at new_path
+            stat_info = self._stat(new_path)
+            if stat_info is None:
+                return None
 
-        # sync the file and see if it was already indexed
-        #
-        # originally this method did not call _sync_file() for performance
-        # reasons, but this is needed to handle an edge case:
-        # https://github.com/jupyter-server/jupyter_server_fileid/issues/62
-        id = self._sync_file(new_path, stat_info)
-        if id is None:
-            # if no existing record, create a new one
-            id = self._create(new_path, stat_info)
+            # sync the file and see if it was already indexed
+            #
+            # originally this method did not call _sync_file() for performance
+            # reasons, but this is needed to handle an edge case:
+            # https://github.com/jupyter-server/jupyter_server_fileid/issues/62
+            id = self._sync_file(new_path, stat_info)
+            if id is None:
+                # if no existing record, create a new one
+                id = self._create(new_path, stat_info)
 
-        self.con.commit()
-        return id
+            return id
 
     def _copy_recursive(self, from_path: str, to_path: str, _: str = "") -> None:
         """Copy all children of a given directory at `from_path` to a new
         directory at `to_path`. Inserts stat_info with record."""
         from_path_glob = os.path.join(from_path, "*")
         records = self.con.execute(
             "SELECT path FROM Files WHERE path GLOB ?", (from_path_glob,)
@@ -855,48 +864,48 @@
     @log(
         lambda self, path: f"Deleting index at {path}.",
         lambda self, path: f"Successfully deleted index at {path}.",
     )
     def delete(self, path):
         """Handles file deletions by deleting the associated record in the File
         table. Returns None."""
-        path = self._normalize_path(path)
+        with self.con:
+            path = self._normalize_path(path)
 
-        if os.path.isdir(path):
-            self._delete_recursive(path)
+            if os.path.isdir(path):
+                self._delete_recursive(path)
 
-        self.con.execute("DELETE FROM Files WHERE path = ?", (path,))
-        self.con.commit()
+            self.con.execute("DELETE FROM Files WHERE path = ?", (path,))
 
     def save(self, path):
         """Handles file saves (edits) by updating recorded stat info.
 
         Notes
         -----
         - This assumes that the file was present prior to the save event. That
         means it's technically possible to fool this method by deleting and
         creating a new file at the same path out-of-band, and then update it via
         JupyterLab.  This would (wrongly) preserve the association b/w the old
         file ID and the current path rather than create a new file ID.
         """
-        path = self._normalize_path(path)
+        with self.con:
+            path = self._normalize_path(path)
 
-        # look up record by ino and path
-        stat_info = self._stat(path)
-        row = self.con.execute(
-            "SELECT id FROM Files WHERE ino = ? AND path = ?", (stat_info.ino, path)
-        ).fetchone()
-        # if no record exists, return early
-        if row is None:
-            return
-
-        # otherwise, update the stat info
-        (id,) = row
-        self._update(id, stat_info)
-        self.con.commit()
+            # look up record by ino and path
+            stat_info = self._stat(path)
+            row = self.con.execute(
+                "SELECT id FROM Files WHERE ino = ? AND path = ?", (stat_info.ino, path)
+            ).fetchone()
+            # if no record exists, return early
+            if row is None:
+                return
+
+            # otherwise, update the stat info
+            (id,) = row
+            self._update(id, stat_info)
 
     def get_handlers_by_action(self) -> Dict[str, Optional[Callable[[Dict[str, Any]], Any]]]:
         return {
             "get": None,
             "save": lambda data: self.save(data["path"]),
             "rename": lambda data: self.move(data["source_path"], data["path"]),
             "copy": lambda data: self.copy(data["source_path"], data["path"]),
```

### Comparing `jupyter_server_fileid-0.9.1/jupyter_server_fileid/pytest_plugin.py` & `jupyter_server_fileid-0.9.2/jupyter_server_fileid/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/tests/test_handler.py` & `jupyter_server_fileid-0.9.2/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/tests/test_manager.py` & `jupyter_server_fileid-0.9.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/.gitignore` & `jupyter_server_fileid-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/LICENSE` & `jupyter_server_fileid-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/README.md` & `jupyter_server_fileid-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/pyproject.toml` & `jupyter_server_fileid-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_server_fileid-0.9.1/PKG-INFO` & `jupyter_server_fileid-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyter_server_fileid
-Version: 0.9.1
+Version: 0.9.2
 Summary: Jupyter Server extension providing an implementation of the File ID service.
 Project-URL: Home, https://github.com/jupyter-server/jupyter_server_fileid
 Author-email: "David L. Qiu" <david@qiu.dev>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, David L. Qiu
         All rights reserved.
```

