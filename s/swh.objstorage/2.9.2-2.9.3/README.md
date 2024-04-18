# Comparing `tmp/swh.objstorage-2.9.2.tar.gz` & `tmp/swh_objstorage-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.objstorage-2.9.2.tar", last modified: Tue Apr  2 15:01:08 2024, max compression
+gzip compressed data, was "swh_objstorage-2.9.3.tar", last modified: Thu Apr 18 13:06:38 2024, max compression
```

## Comparing `swh.objstorage-2.9.2.tar` & `swh_objstorage-2.9.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/bin/swh-objstorage-azure
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.746988 swh.objstorage-2.9.2/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11190 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8317 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14679 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14565 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18323 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/sleep.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7079 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12577 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      547 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/interface.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/multiplexer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/read_write_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10925 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/multiplexer_objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.766988 swh.objstorage-2.9.2/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2322 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5672 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    38512 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20137 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6707 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      541 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4097 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.750988 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.150711 swh_objstorage-2.9.3/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.154711 swh_objstorage-2.9.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-04-18 13:06:38.182711 swh_objstorage-2.9.3/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.142711 swh_objstorage-2.9.3/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.158711 swh_objstorage-2.9.3/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11190 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8317 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14679 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14565 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18323 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/sleep.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7079 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12577 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      547 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/interface.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.162711 swh_objstorage-2.9.3/swh/objstorage/multiplexer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.166711 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/read_write_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11782 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/multiplexer/multiplexer_objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.170711 swh_objstorage-2.9.3/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3747 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5672 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    38512 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20137 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6707 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.178711 swh_objstorage-2.9.3/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4097 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-18 13:06:38.000000 swh_objstorage-2.9.3/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.142711 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.174711 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:38.178711 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-18 13:06:32.000000 swh_objstorage-2.9.3/winery-test-environment/tests.yml
```

### Comparing `swh.objstorage-2.9.2/.pre-commit-config.yaml` & `swh_objstorage-2.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/CODE_OF_CONDUCT.md` & `swh_objstorage-2.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/LICENSE` & `swh_objstorage-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/PKG-INFO` & `swh_objstorage-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.2
+Version: 2.9.3
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh.objstorage-2.9.2/README.rst` & `swh_objstorage-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/bin/swh-objstorage-azure` & `swh_objstorage-2.9.3/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/conftest.py` & `swh_objstorage-2.9.3/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/docs/winery.rst` & `swh_objstorage-2.9.3/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/mypy.ini` & `swh_objstorage-2.9.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/pyproject.toml` & `swh_objstorage-2.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/api/client.py` & `swh_objstorage-2.9.3/swh/objstorage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/api/server.py` & `swh_objstorage-2.9.3/swh/objstorage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/azure.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/azure.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/generator.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/http.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/http.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/in_memory.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/libcloud.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/libcloud.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/noop.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/pathslicing.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/http.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/database.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/objstorage.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/roshard.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/roshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/rwshard.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/sharedbase.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/sleep.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/stats.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/backends/winery/throttler.py` & `swh_objstorage-2.9.3/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/cli.py` & `swh_objstorage-2.9.3/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/constants.py` & `swh_objstorage-2.9.3/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/exc.py` & `swh_objstorage-2.9.3/swh/objstorage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/factory.py` & `swh_objstorage-2.9.3/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/interface.py` & `swh_objstorage-2.9.3/swh/objstorage/interface.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/__init__.py` & `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/filter.py` & `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/read_write_filter.py` & `swh_objstorage-2.9.3/swh/objstorage/multiplexer/filter/read_write_filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/multiplexer/multiplexer_objstorage.py` & `swh_objstorage-2.9.3/swh/objstorage/multiplexer/multiplexer_objstorage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+import logging
 import queue
 import threading
 from typing import Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
 
 from swh.model.model import Sha1
 from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import ObjStorage
+from swh.objstorage.utils import format_obj_id
+
+logger = logging.getLogger(__name__)
 
 
 class ObjStorageThread(threading.Thread):
     def __init__(self, storage):
         super().__init__(daemon=True)
         self.storage = storage
         self.commands = queue.Queue()
@@ -280,21 +284,39 @@
             self.get_write_threads(obj_id),
             "restore",
             content,
             obj_id=obj_id,
         ).pop()
 
     def get(self, obj_id: ObjId) -> bytes:
+        corrupted_exc: Optional[ObjCorruptedError] = None
         for storage in self.get_read_threads(obj_id):
             try:
                 return storage.get(obj_id)
             except ObjNotFoundError:
                 continue
-        # If no storage contains this content, raise the error
-        raise ObjNotFoundError(obj_id)
+            except ObjCorruptedError as exc:
+                logger.warning(
+                    "Object %s was reported as corrupted by %s: %s",
+                    format_obj_id(obj_id),
+                    storage.storage.__class__.__name__,
+                    str(exc),
+                )
+                # Hoist exception, mypy doesn't like when we directly use
+                # `except ObjCorruptedError as corrupted_exc`
+                corrupted_exc = exc
+                # Try reading from another storage
+                continue
+
+        if corrupted_exc:
+            # The only objects we've found were corrupted, raise that exception
+            raise corrupted_exc
+        else:
+            # No storage contains this content, raise the error
+            raise ObjNotFoundError(obj_id)
 
     def check(self, obj_id: ObjId) -> None:
         nb_present = 0
         nb_corrupted = 0
         exception: Optional[Exception] = None
         for storage in self.get_read_threads(obj_id):
             try:
```

### Comparing `swh.objstorage-2.9.2/swh/objstorage/objstorage.py` & `swh_objstorage-2.9.3/swh/objstorage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/pytest_plugin.py` & `swh_objstorage-2.9.3/swh/objstorage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/objstorage_testing.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/objstorage_testing.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_interface.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_api.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_azure.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_cloud.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_http.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_http.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_noop.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_winery.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_pathslicer.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_readonly_filter.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_readonly_filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/test_server.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/winery_benchmark.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh/objstorage/tests/winery_testing_helpers.py` & `swh_objstorage-2.9.3/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/swh.objstorage.egg-info/PKG-INFO` & `swh_objstorage-2.9.3/swh.objstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.2
+Version: 2.9.3
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh.objstorage-2.9.2/swh.objstorage.egg-info/SOURCES.txt` & `swh_objstorage-2.9.3/swh.objstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/tox.ini` & `swh_objstorage-2.9.3/tox.ini`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/README.md` & `swh_objstorage-2.9.3/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/bootstrap.yml` & `swh_objstorage-2.9.3/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/build-vms.sh` & `swh_objstorage-2.9.3/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/ceph.yml` & `swh_objstorage-2.9.3/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/fed4fire.rspec` & `swh_objstorage-2.9.3/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/fed4fire.sh` & `swh_objstorage-2.9.3/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/grid5000.yml` & `swh_objstorage-2.9.3/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/inventory/hosts.yml` & `swh_objstorage-2.9.3/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen.py` & `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh_objstorage-2.9.3/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/osd.yml` & `swh_objstorage-2.9.3/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/remote-tox.sh` & `swh_objstorage-2.9.3/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/render-stats.py` & `swh_objstorage-2.9.3/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/rw.yml` & `swh_objstorage-2.9.3/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.2/winery-test-environment/tests.yml` & `swh_objstorage-2.9.3/winery-test-environment/tests.yml`

 * *Files identical despite different names*

