# Comparing `tmp/jupytercad_lab-2.0.0a4.tar.gz` & `tmp/jupytercad_lab-2.0.0a5.tar.gz`

## Comparing `jupytercad_lab-2.0.0a4.tar` & `jupytercad_lab-2.0.0a5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/.prettierignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/install.json
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/setup.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/tsconfig.json
--rw-r--r--   0        0        0    94325 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/_version.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/package.json
--rw-r--r--   0        0        0    21253 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/484.089536e1111cc88eba58.js
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/remoteEntry.68c1f5b29c2496eda7bd.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/style.js
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/__init__.py
--rw-r--r--   0        0        0    26535 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/cad_document.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/utils.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/y_connector.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/any.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/box.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/chamfer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cone.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cut.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cylinder.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/extrusion.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/fillet.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/fuse.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/geomCircle.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/intersection.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/jcad.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/placement.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/postOperator.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/sketch.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/sphere.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/torus.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/lib/index.d.ts
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/lib/index.js
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/lib/notebookrenderer.d.ts
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/lib/notebookrenderer.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/scripts/bump-version.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/src/index.ts
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/src/notebookrenderer.ts
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/style/index.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/README.md
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/.prettierignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/install.json
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/setup.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/tsconfig.json
+-rw-r--r--   0        0        0    94325 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/_version.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/package.json
+-rw-r--r--   0        0        0    21253 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/484.fd86346ab6e7cf5a316f.js
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/remoteEntry.47f30ab005e91facf7aa.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/style.js
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/__init__.py
+-rw-r--r--   0        0        0    29682 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/utils.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/y_connector.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/any.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/box.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/chamfer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cone.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cut.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cylinder.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/extrusion.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/fillet.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/fuse.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomCircle.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/intersection.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/jcad.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/placement.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/postOperator.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sketch.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sphere.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/torus.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/index.d.ts
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/index.js
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/notebookrenderer.d.ts
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/notebookrenderer.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/scripts/bump-version.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/src/index.ts
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/src/notebookrenderer.ts
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/index.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/README.md
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/PKG-INFO
```

### Comparing `jupytercad_lab-2.0.0a4/package.json` & `jupytercad_lab-2.0.0a5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9729166666666668%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.5', '@jupytercad/jupytercad-core': "*

 * *                   "'^2.0.0-alpha.5', '@jupytercad/schema': '^2.0.0-alpha.5'}",*

 * * "'version'": "'2.0.0-alpha.5'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.4",
-        "@jupytercad/jupytercad-core": "^2.0.0-alpha.4",
-        "@jupytercad/schema": "^2.0.0-alpha.4",
+        "@jupytercad/base": "^2.0.0-alpha.5",
+        "@jupytercad/jupytercad-core": "^2.0.0-alpha.5",
+        "@jupytercad/schema": "^2.0.0-alpha.5",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -114,9 +114,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.4"
+    "version": "2.0.0-alpha.5"
 }
```

### Comparing `jupytercad_lab-2.0.0a4/tsconfig.tsbuildinfo` & `jupytercad_lab-2.0.0a5/tsconfig.tsbuildinfo`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7498026445628577%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(57, "*

 * *              "'b3acb8cca3bb941863d23a16608f14d915fed250d9546f9470a125b41d851c62'), (226, "*

 * *              "'6c65bb162afacd744d370a05e51ec8702247f44d5ef4f39a398ef6f0239a1758'), (396, "*

 * *              "'e87bf3a17f2ba157837dfdd8f2a8ab67be222ea362c9e87447b1cf07b686bb37'), (418, "*

 * *              "'f5183d41c569ee9a2b8ba82a97a85cc59c24f6ac33901592116ce958be4f399d')], delete: [418, "*

 * *              '396, 226, 57]}}',*

 * * "'version'": "'5.4.5'"}*

```diff
@@ -5420,15 +5420,15 @@
             "61741e2c709c1d72f9c660ec77f556e3a7fd8af77728ebd11869c3129fd5c8d9",
             "ff96c4fb5269f72c178fffba25e6b912eb4a36f9758b24b35125636632cf2735",
             "2156b45e8b99f7f94e9237e2f4d4cd81a9e1f60c0c16a073b36aa830f4b82c80",
             "9826749f0fb0f2a74fe86fff797d9f474782bf866eaa7bf147098c133630780f",
             "67c666167a27fca8f28fa669ff00fc9085827ee6167856ddc2fd70cb7a8a0b31",
             "829aa8761c31f10764c72b9e9844d55d77dbe89ca2c2737d13814d6c93279d27",
             "89a7322545ab0c9e2440540e17083ed2bd400c895647dbeb6a2d9d680d687970",
-            "0c7801df7b6e27533410ad69d7dff2eeadc04dfd7d027a5745c2e83163cf8364",
+            "b3acb8cca3bb941863d23a16608f14d915fed250d9546f9470a125b41d851c62",
             "25e0956c4ecb076e6e1ed4607e898dbecbc79551543b174f64816073bcde52c0",
             "37dda729690e6b57c21a8bea72b412fd9421222f35751deacace3d12c5e6b6fb",
             "493db46a04b3b004f0fe57a44923a7cc9c886fb584e6530d6ec400b672c5379c",
             "13e57fa6546f53a980a612a6bd05bfccf10f3d3cbf955b3db89801f65200e8e6",
             "ea59d5da25758b3768cadc246bb6d761e8eb67708f6f31d89f8569b792ad329e",
             "3c4e68d898f52428b058d1fdde23afcfbfa46a3d935a1392b97b0e5f2ba13b1a",
             "0a6d24bacaebb1d29d4d5f933a6f542e3319a0b78230fe79e33c62552afbdc45",
@@ -5595,15 +5595,15 @@
             "c9f5e2d2807cbed36a170a7303be9e9c6a02d8f0e717f228e50afb50aec96ed7",
             "cd334ab582785166eb6470f13dca713125cb4142aae22f1335a36a6ce61aa639",
             "60396ddfdb23d5c538b0c8fdf76963721d7bb895a3ad9bd32ea74be48a5c1cfd",
             "3479943e26fe617c803016fab3a72583a51e20931a9d52701d7c19e1970fb38f",
             "841e4238dccc7d5e200f80b6f33abdc0955460b5d3c196d2fa7907d0a646d80c",
             "e503f183c0ac702838dc0f60bd2e01bffb344426dd2dc40369740a7ae0430574",
             "8ed3c4c1c117c587a4cfd55b150cb2aa76ecdf6d5af9a3b2d5a3dc2fec4519b4",
-            "79cc6f202a16c08ec89f326a2a62cd9cc3f033966a427d4c8e86c4cd022fe8a1",
+            "6c65bb162afacd744d370a05e51ec8702247f44d5ef4f39a398ef6f0239a1758",
             "894019192babee30c70051ebce3559fbe33e8264d7fc2a52a9190bfdfa3d350e",
             "e922c742d7406e0621aec3bf16b20df3a4628f6215098952e43d33967cce5bb7",
             "7f3ceccbbe3ee8208a62f938b28ca1934f573e37b06f7b9df71f5714212daac1",
             "4ec14d99c2c75e1f468340425b3484d412f2ad2a8da986c26b71b019e8d0e1e3",
             "e11fe83b5ba519fcc10f62bd672b3f1083117c794fc6f0df2c3125e000574f31",
             "fd7fe51baa9c4dc58bcb3674a262f3ec43a783833b82e6d09a8da02505121d62",
             "2b99ca04a544be690e8ff5e80dfc26e59f1088fb18e9fe71eb39e716c9317465",
@@ -5765,15 +5765,15 @@
             "1b162dfbafe3d183e089c97e1105ec93f9f102517977d0ef2322c32fb1ae69b3",
             "25fdcfcf217efc4a1ce16b1b87ba4b9de850706512f038a286cd00da9aee0c9b",
             "e087fcd41297b51f643ec14daed135350edd42517292c172837d3bb0f445a001",
             "4ed051e63cb4e713c8629ddb425b61b4acaac453183994a78187346f86f5c635",
             "1d24d23d670fbc3763013f9341a7a376499e8a4f2a35f24b008535d133101cd6",
             "15301c8c565b8581e9fd2b5524f4562ac204ad3e939125a850a8ba98aa151be0",
             "dc63de5eb376f0d81b06149ccb2da01a3a5a21cc3eca641ff5319ca6c048672e",
-            "0a4eb63454d4ebf328fdd2b0f5e296867ee4f64a528473f4bbef9dc78b2411f9",
+            "e87bf3a17f2ba157837dfdd8f2a8ab67be222ea362c9e87447b1cf07b686bb37",
             "e44a13a7be4eed59adc9bd3a26167425df44e45cd3a7cef0ad18b9d9d3d4bf87",
             "fe6c594baff933c3d6f1cb80d0db05bab273b61ce8cf39e03d9d87ced00efb1b",
             "81d2576b03c68c38c81c7d2a1cd5c8ad3b1683298bfb703a8c4dd2b31fa0e1e2",
             "3daafd119d681097f0172dd4defb4e46fc687a0b3f9ad8840b632f55421e06f1",
             "cc23b64f3b0537182c2680649eaea5c01b6763016ec25e6dd948720823cc2592",
             "319a51c73fff9bcb6e1c1533d5bbf7639950f8334a919a499e7931a6f97ae8ce",
             "0aea94afe7b180955d57572d7a6af45e8ad38c476234f76fb7f178ba64f7cb69",
@@ -5787,15 +5787,15 @@
             "becb1ba9752bab39612cd77eaf3140cca067ff0a1e651dc2b1242caf007e08b0",
             "9c554facd42b92c91cba6e487e9b9f6d012a1ea61a6d64096748e38f0946e7a7",
             "c9258d5692cbee696190eb474b532ac5069011d13f7be2ffa9af1f72f20afb5a",
             "cf3cbaee880ea25a8440feb8c49554e4d656ec003e2a7d82799a811c91bc920d",
             "9b09f3820a22f432dd59a447574b6e29aa27b24efc817024f40404c315300c4d",
             "86fbc20c92f731d0493b083291601491a93e73a3fdff9e4d25ade2458572c21e",
             "9f021433d0dcf255a95c0ccd312a6b7ea32458365dbc30d2390257cfad374630",
-            "53fd058f48b9f20010d5fce6404eb518bc5eef93f0c7091d4fabb430a6968219",
+            "f5183d41c569ee9a2b8ba82a97a85cc59c24f6ac33901592116ce958be4f399d",
             "967b1bfbb1eaa1d394465232c542bae781dcbd1aa9865a9da753c3c0ca51f032",
             "f0c4d7cd3054bf45245ab53a73336311100707472665c5b7fc90e5df7c7e795f",
             "aff801ef4268090333d6907db4fb1e1d286fbf8467283d4ee58f78d3f805c3b3",
             "43e7862403a3a325288bd4108fcb1d76d42c57fefb2a660eb46d1c1df356dbb4",
             "a81498798cca946eeaec5844059412baaca219eee731de4bb054b02faa26b8f5",
             "64a8c63ee138480e609ef6c9579c010dc0a902b61085a40f77a78b3f316cac78",
             "15afdb5ca062ea5473867906de2944f3ed87a8621e428ca60ea3a19075903cf9",
@@ -9361,9 +9361,9 @@
             398,
             400,
             401,
             472,
             471
         ]
     },
-    "version": "5.4.4"
+    "version": "5.4.5"
 }
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/__init__.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/package.json` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725000000000001%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.5', '@jupytercad/jupytercad-core': "*

 * *                   "'^2.0.0-alpha.5', '@jupytercad/schema': '^2.0.0-alpha.5'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.47f30ab005e91facf7aa.js'}}",*

 * * "'version'": "'2.0.0-alpha.5'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.4",
-        "@jupytercad/jupytercad-core": "^2.0.0-alpha.4",
-        "@jupytercad/schema": "^2.0.0-alpha.4",
+        "@jupytercad/base": "^2.0.0-alpha.5",
+        "@jupytercad/jupytercad-core": "^2.0.0-alpha.5",
+        "@jupytercad/schema": "^2.0.0-alpha.5",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -37,15 +37,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupytercad/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.68c1f5b29c2496eda7bd.js",
+            "load": "static/remoteEntry.47f30ab005e91facf7aa.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupytercad_lab"
                 },
@@ -119,9 +119,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.4"
+    "version": "2.0.0-alpha.5"
 }
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/484.089536e1111cc88eba58.js` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/484.fd86346ab6e7cf5a316f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_jupytercad_jupytercad_lab = self.webpackChunk_jupytercad_jupytercad_lab || []).push([
     [484], {
         484: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => m
             });
-            var o = a(139),
-                r = a(345),
+            var o = a(244),
+                r = a(266),
                 d = a(465),
                 n = a(381),
                 s = a(714),
                 i = a(796),
                 l = a(597),
                 c = a(486),
                 u = a(230),
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/remoteEntry.68c1f5b29c2496eda7bd.js` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/remoteEntry.47f30ab005e91facf7aa.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, u, l, d, s, f, c, p, h, b, v, y, m, g, j = {
+    var e, r, t, a, n, o, i, u, l, d, f, s, c, p, h, b, v, y, m, g, j = {
             913: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(256), t.e(484)]).then((() => () => t(484))),
                         "./extension": () => Promise.all([t.e(256), t.e(484)]).then((() => () => t(484))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -45,21 +45,21 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         256: "08612c5ea708c7e41bc6",
         432: "99819ec4f414dbcd800e",
-        484: "089536e1111cc88eba58",
+        484: "fd86346ab6e7cf5a316f",
         767: "88bd72c65e1bf31130e2",
         829: "a15a497a850dc99c9a70"
     } [e] + ".js?v=" + {
         256: "08612c5ea708c7e41bc6",
         432: "99819ec4f414dbcd800e",
-        484: "089536e1111cc88eba58",
+        484: "fd86346ab6e7cf5a316f",
         767: "88bd72c65e1bf31130e2",
         829: "a15a497a850dc99c9a70"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -67,31 +67,31 @@
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupytercad/jupytercad-lab:", S.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, u;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        i = s;
+                    var f = l[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var f = (r, a) => {
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@jupytercad/jupytercad-lab", "2.0.0-alpha.4", (() => Promise.all([S.e(256), S.e(484)]).then((() => () => S(484))))), u("yjs-widgets", "0.3.4", (() => Promise.all([S.e(829), S.e(767), S.e(256)]).then((() => () => S(829)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupytercad/jupytercad-lab", "2.0.0-alpha.5", (() => Promise.all([S.e(256), S.e(484)]).then((() => () => S(484))))), u("yjs-widgets", "0.3.4", (() => Promise.all([S.e(829), S.e(767), S.e(256)]).then((() => () => S(829)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,33 +171,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > a && !n : "" == f != n);
-                if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == s ? u > a && !n : "" == s != n);
+                if ("u" == f) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (f == s)
+                    if (s == f)
                         if (u <= a) {
                             if (d != e[u]) return !1
                         } else {
                             if (n ? d > e[u] : d < e[u]) return !1;
                             d != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= a || s < f != n) return !1;
+                    if (u <= a || f < s != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -208,46 +208,46 @@
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
         var n = u(e, t);
-        return o(a, n) || f(l(e, t, n, a)), c(e[t][n])
-    }, s = (e, r, t) => {
+        return o(a, n) || s(l(e, t, n, a)), c(e[t][n])
+    }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, f = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
-        var o = r && S.o(r, t) && s(r, t, a);
+        var o = r && S.o(r, t) && f(r, t, a);
         return o ? c(o) : n()
     })), v = {}, y = {
         256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         78: () => b("default", "yjs-widgets", [2, 0, 3, 3], (() => Promise.all([S.e(829), S.e(767)]).then((() => () => S(829))))),
-        139: () => h("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 4]),
         230: () => h("default", "@lumino/messaging", [1, 2, 0, 0]),
-        345: () => h("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 4]),
+        244: () => h("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 5]),
+        266: () => h("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 5]),
         381: () => h("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         465: () => h("default", "@jupyterlab/application", [1, 4, 1, 6]),
         486: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
         597: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
         714: () => h("default", "@jupyterlab/translation", [1, 4, 1, 6]),
         796: () => h("default", "@jupyter/docprovider", [1, 2, 0, 0]),
         206: () => h("default", "yjs", [1, 13, 5, 40]),
         262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         372: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
         602: () => h("default", "@lumino/signaling", [1, 2, 0, 0]),
         723: () => h("default", "@jupyterlab/rendermime", [1, 4, 1, 6])
     }, m = {
         256: [256],
-        484: [78, 139, 230, 345, 381, 465, 486, 597, 714, 796],
+        484: [78, 230, 244, 266, 381, 465, 486, 597, 714, 796],
         767: [206, 262, 372, 602, 723]
     }, g = {}, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(v, e)) return r.push(v[e]);
             if (!g[e]) {
                 var t = r => {
                     v[e] = 0, S.m[e] = t => {
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/labextension/static/third-party-licenses.json` & `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/cad_document.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/cad_document.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     ICone,
     ICut,
     ICylinder,
     IExtrusion,
     IFuse,
     IIntersection,
     ISphere,
+    IChamfer,
+    IFillet,
     ITorus,
     Parts,
     ShapeMetadata,
 )
 from .utils import normalize_path
 
 logger = logging.getLogger(__file__)
@@ -589,37 +591,109 @@
                 "Placement": {"Position": [0, 0, 0], "Axis": [0, 0, 1], "Angle": 0},
             },
         }
         self.set_visible(shape1, False)
         self.set_visible(shape2, False)
         return self.add_object(OBJECT_FACTORY.create_object(data, self))
 
-    def _get_boolean_operands(self, shape1: str | int | None, shape2: str | int | None):
-        objects = self.objects
+    def chamfer(
+        self,
+        name: str = "",
+        shape: str | int = None,
+        edge: int = 0,
+        dist: float = 0.1,
+        position: List[float] = [0, 0, 0],
+        rotation_axis: List[float] = [0, 0, 1],
+        rotation_angle: float = 0,
+    ) -> CadDocument:
+        """
+        Apply a chamfer operation on an object.
+        If no objects are provided as input, the last created object will be used as operand.
 
+        :param name: The name that will be used for the object in the document.
+        :param shape: The input object used for the chamfer. Can be the name of the object or its index in the objects list.
+        :param edge: The edge index where to apply chamfer.
+        :param dist: The distance of the chamfer.
+        :param position: The shape 3D position.
+        :param rotation_axis: The 3D axis used for the rotation.
+        :param rotation_angle: The shape rotation angle, in degrees.
+        :return: The document itself.
+        """  # noqa E501
+        shape = self._get_operand(shape)
+
+        data = {
+            "shape": Parts.Part__Chamfer.value,
+            "name": name if name else self._new_name("Chamfer"),
+            "parameters": {
+                "Base": shape,
+                "Edge": edge,
+                "Dist": dist,
+                "Placement": {"Position": [0, 0, 0], "Axis": [0, 0, 1], "Angle": 0},
+            },
+        }
+        self.set_visible(shape, False)
+        return self.add_object(OBJECT_FACTORY.create_object(data, self))
+
+    def fillet(
+        self,
+        name: str = "",
+        shape: str | int = None,
+        edge: int = 0,
+        radius: float = 0.1,
+        position: List[float] = [0, 0, 0],
+        rotation_axis: List[float] = [0, 0, 1],
+        rotation_angle: float = 0,
+    ) -> CadDocument:
+        """
+        Apply a fillet operation on an object.
+        If no objects are provided as input, the last created object will be used as operand.
+
+        :param name: The name that will be used for the object in the document.
+        :param shape: The input object used for the fillet. Can be the name of the object or its index in the objects list.
+        :param edge: The edge index where to apply fillet.
+        :param radius: The radius of the fillet.
+        :param position: The shape 3D position.
+        :param rotation_axis: The 3D axis used for the rotation.
+        :param rotation_angle: The shape rotation angle, in degrees.
+        :return: The document itself.
+        """  # noqa E501
+        shape = self._get_operand(shape)
+
+        data = {
+            "shape": Parts.Part__Fillet.value,
+            "name": name if name else self._new_name("Fillet"),
+            "parameters": {
+                "Base": shape,
+                "Edge": edge,
+                "Radius": radius,
+                "Placement": {"Position": [0, 0, 0], "Axis": [0, 0, 1], "Angle": 0},
+            },
+        }
+        self.set_visible(shape, False)
+        return self.add_object(OBJECT_FACTORY.create_object(data, self))
+
+    def _get_operand(self, shape: str | int | None, default_idx: int = -1):
+        if isinstance(shape, str):
+            if shape not in self.objects:
+                raise ValueError(f"Unknown object {shape}")
+        elif isinstance(shape, int):
+            shape = self.objects[shape]
+        else:
+            shape = self.objects[default_idx]
+
+        return shape
+
+    def _get_boolean_operands(self, shape1: str | int | None, shape2: str | int | None):
         if len(self.objects) < 2:
             raise ValueError(
                 "Cannot apply boolean operator if there are less than two objects in the document."  # noqa E501
             )
 
-        if isinstance(shape1, str):
-            if shape1 not in objects:
-                raise ValueError(f"Unknown object {shape1}")
-        elif isinstance(shape1, int):
-            shape1 = objects[shape1]
-        else:
-            shape1 = objects[-2]
-
-        if isinstance(shape2, str):
-            if shape2 not in objects:
-                raise ValueError(f"Unknown object {shape2}")
-        elif isinstance(shape2, int):
-            shape2 = objects[shape2]
-        else:
-            shape2 = objects[-1]
+        shape1 = self._get_operand(shape1, -2)
+        shape2 = self._get_operand(shape2, -1)
 
         return shape1, shape2
 
     def set_visible(self, name: str, value):
         obj: Optional[Map] = self._get_yobject_by_name(name)
 
         if obj is None:
@@ -672,14 +746,16 @@
         ICut,
         ICylinder,
         IExtrusion,
         IIntersection,
         IFuse,
         ISphere,
         ITorus,
+        IFillet,
+        IChamfer,
     ]
     metadata: Optional[ShapeMetadata]
     _caddoc = Optional[CadDocument]
     _parent = Optional[CadDocument]
 
     def __init__(__pydantic_self__, parent, **data: Any) -> None:  # noqa
         super().__init__(**data)
@@ -738,7 +814,9 @@
 OBJECT_FACTORY.register_factory(Parts.Part__Cut.value, ICut)
 OBJECT_FACTORY.register_factory(Parts.Part__Cylinder.value, ICylinder)
 OBJECT_FACTORY.register_factory(Parts.Part__Extrusion.value, IExtrusion)
 OBJECT_FACTORY.register_factory(Parts.Part__MultiCommon.value, IIntersection)
 OBJECT_FACTORY.register_factory(Parts.Part__MultiFuse.value, IFuse)
 OBJECT_FACTORY.register_factory(Parts.Part__Sphere.value, ISphere)
 OBJECT_FACTORY.register_factory(Parts.Part__Torus.value, ITorus)
+OBJECT_FACTORY.register_factory(Parts.Part__Chamfer.value, IChamfer)
+OBJECT_FACTORY.register_factory(Parts.Part__Fillet.value, IFillet)
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/y_connector.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/y_connector.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/any.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/any.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  any.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/box.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/placement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # generated by datamodel-codegen:
-#   filename:  box.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   filename:  placement.json
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
-from pydantic import BaseModel, ConfigDict, Field
+from typing import List
 
-from . import placement
+from pydantic import BaseModel, ConfigDict, Field
 
 
-class IBox(BaseModel):
+class Model(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Length: float = Field(..., description='The length of the box')
-    Width: float = Field(..., description='The width of the box')
-    Height: float = Field(..., description='The height of the box')
-    Placement: placement.Model
+    Position: List[float] = Field(..., description='Position of the Placement')
+    Axis: List[float] = Field(..., description='Axis of the Placement')
+    Angle: float = Field(..., description='Angle of the Placement')
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/chamfer.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/chamfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  chamfer.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cone.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  cone.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   filename:  sphere.json
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
 
 
-class ICone(BaseModel):
+class ISphere(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Radius1: float = Field(..., description='The bottom radius of the cone')
-    Radius2: float = Field(..., description='The top radius of the cone')
-    Height: float = Field(..., description='The height of the cone')
-    Angle: float = Field(..., description='The angle of the cone')
+    Radius: float = Field(..., description='The radius of the sphere')
+    Angle1: float = Field(..., description='The angle of the sphere')
+    Angle2: float = Field(..., description='The angle of the sphere')
+    Angle3: float = Field(..., description='The angle of the sphere')
     Placement: placement.Model
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cut.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # generated by datamodel-codegen:
-#   filename:  cut.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   filename:  geomLineSegment.json
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
+from typing_extensions import Literal
 
-from . import placement
 
-
-class ICut(BaseModel):
+class IGeomLineSegment(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Base: str = Field(..., description='The base of the cut operator')
-    Tool: str = Field(..., description='The tool of the cut operator')
-    Refine: bool = Field(..., description='Refine shape')
-    Placement: placement.Model
+    TypeId: Literal['Part::GeomLineSegment'] = Field(..., description='Geometry type')
+    StartX: float = Field(..., description='StartX')
+    StartY: float = Field(..., description='StartY')
+    StartZ: float = Field(..., description='StartZ')
+    EndX: float = Field(..., description='EndX')
+    EndY: float = Field(..., description='EndY')
+    EndZ: float = Field(..., description='EndZ')
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/cylinder.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cylinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  cylinder.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/extrusion.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/extrusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  extrusion.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/fillet.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomCircle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # generated by datamodel-codegen:
-#   filename:  fillet.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   filename:  geomCircle.json
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
+from typing_extensions import Literal
 
-from . import placement
 
-
-class IFillet(BaseModel):
+class IGeomCircle(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Base: str = Field(..., description='The name of input object')
-    Edge: float = Field(..., description='The edge index')
-    Radius: float = Field(..., description='The radius for the fillet')
-    Placement: placement.Model
+    TypeId: Literal['Part::GeomCircle'] = Field(..., description='Geometry type')
+    CenterX: float = Field(..., description='CenterX')
+    CenterY: float = Field(..., description='CenterY')
+    CenterZ: float = Field(..., description='CenterZ')
+    NormalX: float = Field(..., description='NormalX')
+    NormalY: float = Field(..., description='NormalY')
+    NormalZ: float = Field(..., description='NormalZ')
+    AngleXU: float = Field(..., description='AngleXU')
+    Radius: float = Field(..., description='Radius')
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/jcad.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/jcad.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  jcad.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel, constr
@@ -27,17 +27,19 @@
     Post__Operator = 'Post::Operator'
 
 
 class ShapeMetadata(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    mass: float
-    centerOfMass: List[float]
-    matrixOfInertia: List[List[float]]
+    shapeFormat: Optional[str] = None
+    workerId: Optional[str] = None
+    mass: Optional[float] = None
+    centerOfMass: Optional[List[float]] = None
+    matrixOfInertia: Optional[List[List[float]]] = None
 
 
 class JcadObject(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
     name: str
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/placement.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cone.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  placement.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   filename:  cone.json
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import BaseModel, ConfigDict, Field
 
+from . import placement
+
 
-class Model(BaseModel):
+class ICone(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Position: List[float] = Field(..., description='Position of the Placement')
-    Axis: List[float] = Field(..., description='Axis of the Placement')
-    Angle: float = Field(..., description='Angle of the Placement')
+    Radius1: float = Field(..., description='The bottom radius of the cone')
+    Radius2: float = Field(..., description='The top radius of the cone')
+    Height: float = Field(..., description='The height of the cone')
+    Angle: float = Field(..., description='The angle of the cone')
+    Placement: placement.Model
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/sketch.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sketch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  sketch.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a4/jupytercad_lab/notebook/objects/_schema/torus.py` & `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/torus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  torus.json
-#   timestamp: 2024-04-10T13:27:47+00:00
+#   timestamp: 2024-04-18T14:32:47+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a4/lib/index.js` & `jupytercad_lab-2.0.0a5/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/lib/notebookrenderer.d.ts` & `jupytercad_lab-2.0.0a5/lib/notebookrenderer.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/lib/notebookrenderer.js` & `jupytercad_lab-2.0.0a5/lib/notebookrenderer.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/src/index.ts` & `jupytercad_lab-2.0.0a5/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/src/notebookrenderer.ts` & `jupytercad_lab-2.0.0a5/src/notebookrenderer.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/style/base.css` & `jupytercad_lab-2.0.0a5/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/LICENSE` & `jupytercad_lab-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/pyproject.toml` & `jupytercad_lab-2.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a4/PKG-INFO` & `jupytercad_lab-2.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupytercad_lab
-Version: 2.0.0a4
+Version: 2.0.0a5
 Dynamic: Keywords
 Summary: JupyterCad Lab extension.
 Project-URL: Homepage, https://github.com/jupytercad/jupytercad
 Project-URL: Bug Tracker, https://github.com/jupytercad/jupytercad/issues
 Project-URL: Repository, https://github.com/jupytercad/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
```

