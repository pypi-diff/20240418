# Comparing `tmp/apimanager_dm_2024-0.0.6.tar.gz` & `tmp/apimanager_dm_2024-0.0.7.tar.gz`

## Comparing `apimanager_dm_2024-0.0.6.tar` & `apimanager_dm_2024-0.0.7.tar`

### file list

```diff
@@ -1,1746 +1,1746 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/requirements.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/.gitignore
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/pyvenv.cfg
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/__init__.py
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/__main__.py
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_builder.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_ctx.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_exceptions.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_types.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_util.py
--rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/py.typed
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_compat/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_compat/importlib.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_compat/tarfile.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_compat/tomllib.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/LICENSE
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/__main__.py
--rw-r--r--   0        0        0    21723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    42476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/legacy.py
--rw-r--r--   0        0        0    20239 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/md.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/cli/__main__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/__main__.py
--rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/core.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/docutils.conf
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/examples.py
--rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/frontend.py
--rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/io.py
--rw-r--r--   0        0        0    80628 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/nodes.py
--rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/statemachine.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/af.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ar.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ca.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/cs.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/da.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/de.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/en.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/eo.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/es.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fa.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fi.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fr.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/gl.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/he.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/it.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ja.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ka.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ko.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/lt.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/lv.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/nl.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/pl.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/pt_br.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ru.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/sk.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/sv.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/uk.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/zh_cn.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/zh_tw.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/null.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/__init__.py
--rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-r--r--   0        0        0   133123 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/states.py
--rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
--rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-r--r--   0        0        0    26700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
--rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ka.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/doctree.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/pep.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/standalone.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/components.py
--rw-r--r--   0        0        0    20809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/misc.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/parts.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/peps.py
--rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/references.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/universal.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/writer_aux.py
--rw-r--r--   0        0        0    30381 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/__init__.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/error_reporting.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/roman.py
--rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/smartquotes.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/urischemes.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/__init__.py
--rw-r--r--   0        0        0    46961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-r--r--   0        0        0   107808 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/math2html.py
--rw-r--r--   0        0        0    56217 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/mathalphabet2unichar.py
--rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/mathml_elements.py
--rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/__init__.py
--rw-r--r--   0        0        0    75401 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/_html_base.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/docutils_xml.py
--rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/manpage.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/null.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pseudoxml.py
--rw-r--r--   0        0        0    38125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html4css1/template.txt
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/italic-field-names.css
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
--rw-r--r--   0        0        0   138165 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/default.tex
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
--rw-r--r--   0        0        0   132081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/pep.css
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/template.txt
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/xetex/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/COPYING.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/METADATA
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/WHEEL
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/core.py
--rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/WHEEL
--rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_text.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/diagnose.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/compat/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/compat/py39.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/__init__.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/ancestry.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/meta.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/properties.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/py.typed
--rw-r--r--   0        0        0    16642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/functools/__init__.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/functools/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/functools/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/METADATA
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/METADATA
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/__main__.py
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backend.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backend_complete.bash
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backend_complete.zsh
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/cli.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/completion.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/core.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/credentials.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/devpi_client.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/errors.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/http.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/py.typed
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/SecretService.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/Windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/chainer.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/fail.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/kwallet.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/libsecret.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/null.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/macOS/api.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/compat/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/compat/properties.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/compat/py312.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/compat/py38.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/testing/__init__.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/testing/backend.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/testing/util.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/util/__init__.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/util/platform_.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/_compat.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/_punycode.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/main.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_block.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/port.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/py.typed
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/renderer.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/ruler.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/token.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/tree.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/zero.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/text_join.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/linkify.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_decode.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_encode.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_format.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_parse.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_url.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   143045 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/more.py
--rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/py.typed
--rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/recipes.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/recipes.pyi
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/INSTALLER
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/METADATA
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/RECORD
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/WHEEL
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    78960 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/__init__.pyi
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/bdist.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/bdist.pyi
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/commandline.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/commandline.pyi
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/develop.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/develop.pyi
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/distribution.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/distribution.pyi
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/index.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/index.pyi
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/installed.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/installed.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/py.typed
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/sdist.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/sdist.pyi
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/utils.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/utils.pyi
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/wheel.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/wheel.pyi
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_index.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/__main__.py
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/filter.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatter.py
--rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/modeline.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/scanner.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/sphinxext.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/style.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/util.py
--rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/html.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/img.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/other.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/actionscript.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ada.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/agile.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/algebra.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ambient.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ampl.py
--rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/apl.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/archetype.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/arrow.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/arturo.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asc.py
--rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asm.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asn1.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/automation.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bare.py
--rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/basic.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bdd.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/berry.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bibtex.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/blueprint.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/boa.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bqn.py
--rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/business.py
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/c_like.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/capnproto.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/carbon.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/cddl.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/chapel.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/clean.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/comal.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/compiled.py
--rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/configs.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/console.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/cplint.py
--rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/crystal.py
--rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/csound.py
--rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/css.py
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/d.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dalvik.py
--rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/data.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dax.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/devicetree.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/diff.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dns.py
--rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dotnet.py
--rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dsls.py
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dylan.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ecl.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/eiffel.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/elm.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/elpi.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/email.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/erlang.py
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/esoteric.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ezhil.py
--rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/factor.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fantom.py
--rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/felix.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fift.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/floscript.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/forth.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fortran.py
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/foxpro.py
--rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/freefem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/func.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/functional.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/futhark.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gdscript.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/go.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graph.py
--rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphics.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphql.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphviz.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gsql.py
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/haskell.py
--rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/haxe.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/hdl.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/hexdump.py
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/html.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/idl.py
--rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/igor.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/inferno.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/installers.py
--rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/iolang.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/j.py
--rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/javascript.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jmespath.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jslt.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jsx.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/julia.py
--rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jvm.py
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/kuin.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/kusto.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ldap.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lean.py
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lilypond.py
--rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lisp.py
--rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/make.py
--rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/markup.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/math.py
--rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/matlab.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/maxima.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/meson.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mime.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/minecraft.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mips.py
--rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ml.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/modeling.py
--rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/modula2.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/monte.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mosel.py
--rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ncl.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nimrod.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nit.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nix.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/oberon.py
--rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/objective.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ooc.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/openscad.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/other.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/parasail.py
--rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/parsers.py
--rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pascal.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pawn.py
--rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/perl.py
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/phix.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/php.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pointless.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pony.py
--rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/praat.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/procfile.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/prolog.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/promql.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/prql.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ptx.py
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/python.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/q.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/qlik.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/qvt.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/r.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rdf.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rebol.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/resource.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ride.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rita.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rnc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/roboconf.py
--rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/robotframework.py
--rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ruby.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rust.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sas.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/savi.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/scdoc.py
--rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/scripting.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sgf.py
--rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/shell.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sieve.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/slash.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smithy.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smv.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/snobol.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/solidity.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sophia.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/special.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/spice.py
--rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sql.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/stata.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/supercollider.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tal.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tcl.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/teal.py
--rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/templates.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/teraterm.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/testing.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/text.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/textedit.py
--rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/textfmts.py
--rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/theorem.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tlb.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tls.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tnt.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/typoscript.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ul4.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/unicon.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/urbi.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/usd.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/varnish.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/verification.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/verifpal.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/vip.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/vyper.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/web.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webassembly.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webidl.py
--rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webmisc.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wgsl.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/whiley.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wren.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/x10.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/xorg.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/yang.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/yara.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/zig.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/__init__.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/_mapping.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/abap.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/algol.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/algol_nu.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/arduino.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/autumn.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/borland.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/bw.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/colorful.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/default.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/dracula.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/emacs.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/friendly.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/fruity.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/gh_dark.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/gruvbox.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/igor.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/inkpot.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lightbulb.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lilypond.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lovelace.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/manni.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/material.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/monokai.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/murphy.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/native.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/nord.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/onedark.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/pastie.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/perldoc.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/rrt.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/sas.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/solarized.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/staroffice.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/stata_dark.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/stata_light.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/tango.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/trac.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/vim.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/vs.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/xcode.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/zenburn.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/METADATA
--rw-r--r--   0        0        0    45069 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/__init__.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/__main__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/clean.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/py.typed
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/rst.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/txt.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/WHEEL
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/METADATA
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/_compat.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/exceptions.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/sessions.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/__init__.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/_mixin.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/api.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/builder.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/compat.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/exceptions.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/iri.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/misc.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/normalizers.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/parseresult.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/uri.py
--rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/validators.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/__init__.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/__main__.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_export_format.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_inspect.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_pick.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_timer.py
--rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_win32_console.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_windows.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_windows_renderer.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_wrap.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/abc.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/ansi.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/bar.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/box.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/cells.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/columns.py
--rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/constrain.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/containers.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/control.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/default_styles.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/diagnose.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/highlighter.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/json.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/jupyter.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/layout.py
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/live.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/live_render.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/logging.py
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/markdown.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/measure.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/pager.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/palette.py
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/panel.py
--rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/pretty.py
--rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/progress.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/progress_bar.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/prompt.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/region.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/repr.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/rule.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/scope.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/screen.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/spinner.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/style.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/styled.py
--rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/syntax.py
--rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/terminal_theme.py
--rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/themes.py
--rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/traceback.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/tree.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/METADATA
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/RECORD
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/__main__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/auth.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/cli.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/exceptions.py
--rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/py.typed
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/repository.py
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/settings.py
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/utils.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/wheel.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/wininst.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/__init__.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/check.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/register.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/upload.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_base_connection.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/http2.py
--rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/py.typed
--rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/__init__.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/connection.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/fetch.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/request.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/response.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywintypes.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/version.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/win32api.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/win32cred.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/_winerrors.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/compat.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_backends.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/glob.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/compat/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/compat/py310.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/METADATA
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/top_level.txt
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate.bat
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate.fish
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate.nu
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate.ps1
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/activate_this.py
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/docutils.exe
--rwxr-xr-x   0        0        0   108421 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/keyring.exe
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/markdown-it.exe
--rwxr-xr-x   0        0        0   108444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pip3.12.exe
--rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pkginfo.exe
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pydoc.bat
--rwxr-xr-x   0        0        0   108426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pygmentize.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0   274712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/python.exe
--rwxr-xr-x   0        0        0   263448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/pythonw.exe
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html.exe
--rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html4.exe
--rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html5.exe
--rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2latex.exe
--rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2man.exe
--rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2odt.exe
--rwxr-xr-x   0        0        0   108441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2pseudoxml.exe
--rwxr-xr-x   0        0        0   108427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2s5.exe
--rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2xetex.exe
--rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/rst2xml.exe
--rwxr-xr-x   0        0        0   108424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.venv/Scripts/twine.exe
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/APIManager/APIManager.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/APIManager/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/.gitignore
--rw-r--r--   0        0        0    35801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/LICENSE
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/.gitignore
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/__init__.py
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/__main__.py
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_builder.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_ctx.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_exceptions.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_types.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_util.py
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/py.typed
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_compat/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_compat/importlib.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_compat/tarfile.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_compat/tomllib.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/__main__.py
+-rw-r--r--   0        0        0    21723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    42476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/legacy.py
+-rw-r--r--   0        0        0    20239 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/md.py
+-rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/cli/__main__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/__main__.py
+-rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/core.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/docutils.conf
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/examples.py
+-rw-r--r--   0        0        0    44396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/frontend.py
+-rw-r--r--   0        0        0    22583 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/io.py
+-rw-r--r--   0        0        0    80628 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/nodes.py
+-rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/statemachine.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/af.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ar.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ca.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/cs.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/da.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/de.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/en.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/eo.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/es.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fa.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fi.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fr.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/gl.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/he.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/it.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ja.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ka.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ko.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/lt.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/lv.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/nl.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/pl.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/pt_br.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ru.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/sk.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/sv.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/uk.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/zh_cn.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/zh_tw.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/null.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/__init__.py
+-rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/roles.py
+-rw-r--r--   0        0        0   133123 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/states.py
+-rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/tableparser.py
+-rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/body.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/html.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/images.py
+-rw-r--r--   0        0        0    26700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/references.py
+-rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/README.txt
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
+-rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/af.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/da.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/de.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/en.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/es.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/he.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/it.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ka.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/doctree.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/pep.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/standalone.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/components.py
+-rw-r--r--   0        0        0    20809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/frontmatter.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/misc.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/parts.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/peps.py
+-rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/references.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/universal.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/writer_aux.py
+-rw-r--r--   0        0        0    30381 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/__init__.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/code_analyzer.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/error_reporting.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/punctuation_chars.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/roman.py
+-rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/smartquotes.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/urischemes.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/__init__.py
+-rw-r--r--   0        0        0    46961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/latex2mathml.py
+-rw-r--r--   0        0        0   107808 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/math2html.py
+-rw-r--r--   0        0        0    56217 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/mathalphabet2unichar.py
+-rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/mathml_elements.py
+-rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/tex2unichar.py
+-rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/unichar2tex.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/__init__.py
+-rw-r--r--   0        0        0    75401 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/_html_base.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/docutils_xml.py
+-rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/manpage.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/null.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pseudoxml.py
+-rw-r--r--   0        0        0    38125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html4css1/__init__.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html4css1/template.txt
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/italic-field-names.css
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
+-rw-r--r--   0        0        0   138165 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/default.tex
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
+-rw-r--r--   0        0        0   132081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/pep.css
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/template.txt
+-rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/xetex/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/COPYING.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/METADATA
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/core.py
+-rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/WHEEL
+-rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/diagnose.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/compat/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/compat/py39.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/__init__.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/ancestry.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/meta.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/properties.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/py.typed
+-rw-r--r--   0        0        0    16642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/functools/__init__.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/functools/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/functools/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/__main__.py
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backend.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backend_complete.bash
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backend_complete.zsh
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/cli.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/completion.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/core.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/credentials.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/devpi_client.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/errors.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/http.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/py.typed
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/SecretService.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/Windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/chainer.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/fail.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/kwallet.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/libsecret.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/null.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/macOS/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/macOS/api.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/compat/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/compat/properties.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/compat/py312.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/compat/py38.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/testing/__init__.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/testing/backend.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/testing/util.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/util/__init__.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/util/platform_.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/_punycode.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/main.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_block.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/port.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/py.typed
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/renderer.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/ruler.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/token.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/tree.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/text_join.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/linkify.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_decode.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_encode.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_format.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_parse.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_url.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   143045 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/more.py
+-rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/py.typed
+-rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/METADATA
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/RECORD
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/WHEEL
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    78960 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/__init__.pyi
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/bdist.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/bdist.pyi
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/commandline.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/commandline.pyi
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/develop.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/develop.pyi
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/distribution.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/distribution.pyi
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/index.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/index.pyi
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/installed.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/installed.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/py.typed
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/sdist.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/sdist.pyi
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/utils.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/utils.pyi
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/wheel.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/wheel.pyi
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_bdist.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_commandline.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_develop.py
+-rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_distribution.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_index.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_installed.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_sdist.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_utils.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_wheel.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/__main__.py
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/filter.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatter.py
+-rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/modeline.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/scanner.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/style.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/util.py
+-rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/html.py
+-rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_ada_builtins.py
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_css_builtins.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_julia_builtins.py
+-rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_php_builtins.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/actionscript.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ada.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/agile.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/algebra.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ambient.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/amdgpu.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ampl.py
+-rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/apdlexer.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/apl.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/archetype.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/arrow.py
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/arturo.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asc.py
+-rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asm.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asn1.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/automation.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bare.py
+-rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/basic.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bdd.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/berry.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bibtex.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/blueprint.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/boa.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bqn.py
+-rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/business.py
+-rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/c_cpp.py
+-rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/c_like.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/capnproto.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/carbon.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/cddl.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/chapel.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/clean.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/comal.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/compiled.py
+-rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/configs.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/console.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/cplint.py
+-rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/crystal.py
+-rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/csound.py
+-rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/css.py
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/d.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dalvik.py
+-rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/data.py
+-rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dax.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/devicetree.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/diff.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dns.py
+-rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dotnet.py
+-rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dsls.py
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dylan.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ecl.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/eiffel.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/elm.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/elpi.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/email.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/erlang.py
+-rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/esoteric.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ezhil.py
+-rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/factor.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fantom.py
+-rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/felix.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fift.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/floscript.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/forth.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fortran.py
+-rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/foxpro.py
+-rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/freefem.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/func.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/functional.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/futhark.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gcodelexer.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gdscript.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/go.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/grammar_notation.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graph.py
+-rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphics.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphql.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphviz.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gsql.py
+-rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/haskell.py
+-rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/haxe.py
+-rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/hdl.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/hexdump.py
+-rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/html.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/idl.py
+-rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/igor.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/inferno.py
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/installers.py
+-rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/int_fiction.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/iolang.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/j.py
+-rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/javascript.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jmespath.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jslt.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jsonnet.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jsx.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/julia.py
+-rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jvm.py
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/kuin.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/kusto.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ldap.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lean.py
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lilypond.py
+-rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lisp.py
+-rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/macaulay2.py
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/make.py
+-rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/markup.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/math.py
+-rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/matlab.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/maxima.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/meson.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mime.py
+-rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/minecraft.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mips.py
+-rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ml.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/modeling.py
+-rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/modula2.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/monte.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mosel.py
+-rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ncl.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nimrod.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nit.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nix.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/oberon.py
+-rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/objective.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ooc.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/openscad.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/other.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/parasail.py
+-rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/parsers.py
+-rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pascal.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pawn.py
+-rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/perl.py
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/phix.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/php.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pointless.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pony.py
+-rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/praat.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/procfile.py
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/prolog.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/promql.py
+-rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/prql.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ptx.py
+-rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/python.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/q.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/qlik.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/qvt.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/r.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rdf.py
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rebol.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/resource.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ride.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rita.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rnc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/roboconf.py
+-rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/robotframework.py
+-rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ruby.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rust.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sas.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/savi.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/scdoc.py
+-rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/scripting.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sgf.py
+-rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/shell.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sieve.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/slash.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smalltalk.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smithy.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smv.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/snobol.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/solidity.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sophia.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/special.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/spice.py
+-rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sql.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/srcinfo.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/stata.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/supercollider.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tal.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tcl.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/teal.py
+-rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/templates.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/teraterm.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/testing.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/text.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/textedit.py
+-rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/textfmts.py
+-rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/theorem.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/thingsdb.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tlb.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tls.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tnt.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/trafficscript.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/typoscript.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ul4.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/unicon.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/urbi.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/usd.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/varnish.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/verification.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/verifpal.py
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/vip.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/vyper.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/web.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webassembly.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webidl.py
+-rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webmisc.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wgsl.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/whiley.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wowtoc.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wren.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/x10.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/xorg.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/yang.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/yara.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/zig.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/_mapping.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/abap.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/algol.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/algol_nu.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/arduino.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/autumn.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/borland.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/bw.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/colorful.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/default.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/dracula.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/emacs.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/friendly.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/friendly_grayscale.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/fruity.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/gh_dark.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/gruvbox.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/igor.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/inkpot.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lightbulb.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lilypond.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lovelace.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/manni.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/material.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/monokai.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/murphy.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/native.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/nord.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/onedark.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/paraiso_dark.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/paraiso_light.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/pastie.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/perldoc.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/rainbow_dash.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/rrt.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/sas.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/solarized.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/staroffice.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/stata_dark.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/stata_light.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/tango.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/trac.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/vim.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/vs.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/xcode.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/zenburn.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/METADATA
+-rw-r--r--   0        0        0    45069 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/__init__.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/__main__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/clean.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/py.typed
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/rst.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/txt.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/_compat.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/exceptions.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/sessions.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/__init__.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/source.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/x509.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/guess.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/handler.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/cookies/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py
+-rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/pool.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/thread.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/dump.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/formdata.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/__init__.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/_mixin.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/abnf_regexp.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/api.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/builder.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/compat.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/exceptions.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/iri.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/misc.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/normalizers.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/parseresult.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/uri.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/validators.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/__init__.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/__main__.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_export_format.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_inspect.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_pick.py
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_timer.py
+-rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_win32_console.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_windows.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/abc.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/ansi.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/bar.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/box.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/cells.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/columns.py
+-rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/constrain.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/containers.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/control.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/default_styles.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/diagnose.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/highlighter.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/json.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/jupyter.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/layout.py
+-rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/live.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/live_render.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/logging.py
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/markdown.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/measure.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/pager.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/palette.py
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/panel.py
+-rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/pretty.py
+-rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/progress.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/progress_bar.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/prompt.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/region.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/repr.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/rule.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/scope.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/screen.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/spinner.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/style.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/styled.py
+-rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/syntax.py
+-rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/terminal_theme.py
+-rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/themes.py
+-rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/traceback.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/tree.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/__main__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/auth.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/cli.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/exceptions.py
+-rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/py.typed
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/repository.py
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/settings.py
+-rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/utils.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/wheel.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/wininst.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/__init__.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/check.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/register.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/upload.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/http2.py
+-rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/py.typed
+-rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/__init__.py
+-rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/connection.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/fetch.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/request.py
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/response.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywintypes.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/version.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/win32api.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/win32cred.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/_winerrors.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/compat.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/__init__.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_common.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_time.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_util.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_time.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/win32api.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/__init__.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_backends.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_win32api.py
+-rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/glob.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/compat/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/compat/py310.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/METADATA
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate
+-rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate.bat
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate.fish
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate.nu
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate.ps1
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/activate_this.py
+-rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/docutils.exe
+-rwxr-xr-x   0        0        0   108421 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/keyring.exe
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/markdown-it.exe
+-rwxr-xr-x   0        0        0   108444 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/normalizer.exe
+-rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pip3.12.exe
+-rwxr-xr-x   0        0        0   108432 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pkginfo.exe
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pydoc.bat
+-rwxr-xr-x   0        0        0   108426 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pygmentize.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pyproject-build.exe
+-rwxr-xr-x   0        0        0   274712 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/python.exe
+-rwxr-xr-x   0        0        0   263448 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/pythonw.exe
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html.exe
+-rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html4.exe
+-rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html5.exe
+-rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2latex.exe
+-rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2man.exe
+-rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2odt.exe
+-rwxr-xr-x   0        0        0   108441 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2pseudoxml.exe
+-rwxr-xr-x   0        0        0   108427 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2s5.exe
+-rwxr-xr-x   0        0        0   108433 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2xetex.exe
+-rwxr-xr-x   0        0        0   108429 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/rst2xml.exe
+-rwxr-xr-x   0        0        0   108424 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.venv/Scripts/twine.exe
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/api_manager/APIManager.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/api_manager/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35801 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/LICENSE
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/README.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 apimanager_dm_2024-0.0.7/PKG-INFO
```

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/_virtualenv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_builder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_builder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_ctx.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_ctx.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/env.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/env.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build/_compat/tarfile.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build/_compat/tarfile.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/build-1.2.1.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/build-1.2.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/cacert.pem` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/cd.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/constant.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/legacy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/md.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/models.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer/cli/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/ansi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/ansitowin32.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/initialise.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/win32.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/winterm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/ansi_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/ansitowin32_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/initialise_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/isatty_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama/tests/winterm_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/examples.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/examples.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/frontend.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/frontend.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/io.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/io.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/nodes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/nodes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/statemachine.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/statemachine.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/af.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/af.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ca.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ca.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/cs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/cs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/da.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/da.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/de.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/de.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/en.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/en.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/eo.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/eo.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/es.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/es.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fa.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fa.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/fr.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/fr.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/gl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/gl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/he.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/he.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/it.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/it.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ja.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ja.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ka.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ka.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ko.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ko.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/lt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/lt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/lv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/lv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/nl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/nl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/pl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/pl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/pt_br.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/ru.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/ru.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/sk.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/sk.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/sv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/sv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/uk.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/uk.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/zh_cn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/languages/zh_tw.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/commonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/roles.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/roles.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/states.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/states.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/tableparser.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/tableparser.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/body.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/body.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/html.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/html.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/images.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/images.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/misc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/parts.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/references.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/references.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/directives/tables.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/README.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/README.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isobox.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isodia.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isonum.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isopub.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/isotech.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/af.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/af.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ca.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/cs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/da.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/da.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/de.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/de.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/en.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/en.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/eo.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/es.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/es.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fa.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/fr.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/gl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/he.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/he.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/it.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/it.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ja.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ka.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ka.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ko.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/lt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/lv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/nl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/pl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/ru.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/sk.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/sv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/uk.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/doctree.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/doctree.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/pep.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/pep.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/readers/standalone.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/readers/standalone.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/components.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/components.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/frontmatter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/frontmatter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/misc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/parts.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/parts.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/peps.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/peps.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/references.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/references.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/universal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/universal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/transforms/writer_aux.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/transforms/writer_aux.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/code_analyzer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/error_reporting.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/error_reporting.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/punctuation_chars.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/punctuation_chars.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/roman.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/roman.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/smartquotes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/smartquotes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/urischemes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/urischemes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/latex2mathml.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/math2html.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/math2html.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/mathalphabet2unichar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/mathalphabet2unichar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/mathml_elements.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/mathml_elements.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/tex2unichar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/tex2unichar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/utils/math/unichar2tex.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/utils/math/unichar2tex.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/_html_base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/_html_base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/docutils_xml.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/docutils_xml.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/manpage.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/null.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/null.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pseudoxml.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pseudoxml.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html4css1/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html4css1/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html4css1/html4css1.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/italic-field-names.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/italic-field-names.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/math.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/plain.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/docutils.sty`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/latex2e/xelatex.tex`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/odf_odt/styles.odt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/pep.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/pep.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/pep_html/template.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/pep_html/template.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils/writers/xetex/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils/writers/xetex/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/COPYING.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/COPYING.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/docutils-0.21.1.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/docutils-0.21.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/codec.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/idnadata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/intranges.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna/uts46data.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/LICENSE.md` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/idna-3.7.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/idna-3.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_adapters.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_collections.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_functools.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_itertools.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_meta.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/_text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata/compat/py39.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata/compat/py39.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/context.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/ancestry.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/ancestry.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/meta.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/meta.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/classes/properties.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/classes/properties.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/functools/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/functools/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco/functools/__init__.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco/functools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.context-5.3.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/jaraco.functools-4.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backend.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backend.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/cli.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/cli.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/completion.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/completion.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/credentials.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/credentials.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/devpi_client.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/devpi_client.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/errors.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/errors.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/http.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/http.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/SecretService.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/SecretService.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/Windows.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/Windows.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/chainer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/chainer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/fail.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/fail.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/kwallet.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/kwallet.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/libsecret.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/libsecret.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/macOS/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/macOS/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/backends/macOS/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/backends/macOS/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/compat/properties.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/compat/properties.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/testing/backend.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/testing/backend.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/testing/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/testing/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring/util/platform_.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring/util/platform_.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/keyring-25.1.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/keyring-25.1.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/_punycode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/main.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_block.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/parser_inline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/port.yaml` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/renderer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/ruler.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/token.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/tree.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/cli/parse.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/html_blocks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/html_re.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/normalize_url.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/common/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/commonmark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/default.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/presets/zero.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/blockquote.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/code.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/fence.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/heading.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/hr.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/html_block.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/lheading.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/list.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/paragraph.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/reference.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/state_block.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_block/table.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/linkify.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/replacements.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/state_core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_core/text_join.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_core/text_join.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/autolink.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/backticks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/entity.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/escape.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/fragments_join.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/image.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/link.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/linkify.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/linkify.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/newline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it/rules_inline/text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_decode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_decode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_encode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_encode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_format.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_format.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl/_parse.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl/_parse.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/more.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/more.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/recipes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools/recipes.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3/__init__.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/nh3-0.2.17.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/nh3-0.2.17.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_elffile.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_manylinux.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_musllinux.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_parser.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_structures.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/_tokenizer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/markers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/metadata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/requirements.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/specifiers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/tags.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging/version.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging/version.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/packaging-24.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/packaging-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/__pip-runner__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/build_env.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/configuration.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/pyproject.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/main.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/parser.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/check.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/completion.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/debug.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/download.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/hash.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/help.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/index.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/install.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/list.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/search.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/show.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/collector.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/index/sources.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/locations/base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/candidate.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/format_control.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/index.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/link.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/scheme.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/target_python.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/models/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/auth.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/download.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/session.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/check.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/constructors.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_file.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_install.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_set.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/_log.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/logging.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/misc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/models.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/urls.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/git.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/six.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/help.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/models.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/align.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/box.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/color.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/control.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/json.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/live.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/status.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/style.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/table.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_macos.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/truststore/_windows.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/AUTHORS.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/LICENSE.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pip-24.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pip-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/bdist.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/bdist.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/commandline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/commandline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/commandline.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/commandline.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/develop.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/develop.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/distribution.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/distribution.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/distribution.pyi` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/distribution.pyi`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/index.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/index.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/installed.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/installed.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/sdist.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/sdist.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_bdist.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_bdist.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_commandline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_develop.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_distribution.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_index.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_installed.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_sdist.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo/tests/test_wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/cmdline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/filter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/modeline.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/plugin.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/regexopt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/scanner.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/sphinxext.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/style.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/token.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/unistring.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/filters/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/_mapping.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/bbcode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/groff.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/html.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/img.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/irc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/latex.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/other.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/pangomarkup.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/rtf.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/svg.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/terminal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/formatters/terminal256.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_ada_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_asy_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_cl_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_csound_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_css_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_julia_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_lua_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mapping.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mql_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_php_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_qlik_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_stan_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_stata_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_usd_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/_vim_builtins.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/actionscript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ada.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/agile.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/algebra.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ambient.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/amdgpu.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ampl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/apdlexer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/apl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/archetype.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/arrow.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/arturo.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/asn1.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/asn1.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/automation.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bare.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/basic.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bdd.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bdd.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/berry.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/berry.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bibtex.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/blueprint.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/blueprint.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/boa.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/bqn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/bqn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/business.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/c_cpp.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/c_like.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/capnproto.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/carbon.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/carbon.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/cddl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/chapel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/clean.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/comal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/compiled.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/configs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/cplint.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/crystal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/csound.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/css.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/d.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dalvik.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/data.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dax.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dax.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/devicetree.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/diff.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dns.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dns.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dotnet.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dsls.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/dylan.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ecl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/eiffel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/elm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/elpi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/email.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/erlang.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/esoteric.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ezhil.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/factor.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fantom.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/felix.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fift.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/floscript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/forth.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/fortran.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/foxpro.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/freefem.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/func.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/functional.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/futhark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gcodelexer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gdscript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/go.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/grammar_notation.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graph.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphics.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphql.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphql.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/graphviz.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/gsql.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/haskell.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/haxe.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/hdl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/hexdump.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/html.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/idl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/igor.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/inferno.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/installers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/int_fiction.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/iolang.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/j.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/javascript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jmespath.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jslt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jsonnet.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jsx.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jsx.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/julia.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/jvm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/kuin.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/kusto.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/kusto.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ldap.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ldap.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lean.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lean.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lilypond.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lilypond.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/lisp.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/macaulay2.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/make.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/markup.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/math.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/matlab.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/maxima.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/meson.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mime.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/minecraft.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mips.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ml.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/modeling.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/modula2.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/monte.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/mosel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ncl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nimrod.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nit.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/nix.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/oberon.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/objective.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ooc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/openscad.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/openscad.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/other.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/parasail.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/parsers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pascal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pawn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/perl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/phix.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/php.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pointless.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/pony.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/praat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/procfile.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/prolog.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/promql.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/prql.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/prql.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ptx.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ptx.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/python.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/q.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/q.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/qlik.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/qlik.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/qvt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/r.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rdf.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rebol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/resource.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ride.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rita.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rnc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/roboconf.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/robotframework.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ruby.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/rust.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sas.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/savi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/scdoc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/scripting.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sgf.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/shell.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sieve.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/slash.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smalltalk.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smithy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/smv.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/snobol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/solidity.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sophia.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/special.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/spice.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/sql.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/srcinfo.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/srcinfo.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/stata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/supercollider.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tcl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/teal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/templates.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/teraterm.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/testing.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/textedit.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/textfmts.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/theorem.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/thingsdb.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tlb.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tls.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tls.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/tnt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/trafficscript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/typoscript.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/ul4.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/unicon.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/urbi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/usd.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/varnish.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/verification.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/verifpal.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/verifpal.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/vip.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/vip.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/vyper.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/vyper.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/web.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webassembly.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webidl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/webmisc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wgsl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wgsl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/whiley.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wowtoc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/wren.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/x10.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/xorg.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/yang.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/yara.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/yara.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/lexers/zig.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/_mapping.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/_mapping.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/abap.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/algol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/algol_nu.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/arduino.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/autumn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/borland.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/bw.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/colorful.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/default.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/dracula.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/dracula.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/emacs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/friendly.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/friendly_grayscale.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/friendly_grayscale.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/fruity.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/gh_dark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/gh_dark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/gruvbox.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/gruvbox.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/igor.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/inkpot.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lightbulb.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lightbulb.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lilypond.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lilypond.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/lovelace.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/manni.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/material.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/material.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/monokai.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/murphy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/native.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/nord.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/nord.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/onedark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/onedark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/paraiso_dark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/paraiso_light.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/pastie.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/perldoc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/rainbow_dash.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/rrt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/sas.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/solarized.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/staroffice.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/staroffice.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/stata_dark.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/stata_light.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/tango.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/trac.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/vim.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/vs.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/xcode.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments/styles/zenburn.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments/styles/zenburn.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_impl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/clean.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/clean.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/markdown.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/markdown.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/rst.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/rst.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer/txt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer/txt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/_internal_utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/adapters.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/auth.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/cookies.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/help.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/hooks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/models.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/packages.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/sessions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/status_codes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/structures.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests-2.31.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests-2.31.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/_compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/_compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/sessions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/sessions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/appengine.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/socket_options.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/source.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/source.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/ssl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/adapters/x509.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/adapters/x509.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/guess.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/guess.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/handler.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/handler.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/downloadutils/stream.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/downloadutils/tee.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/pool.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/pool.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/threaded/thread.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/threaded/thread.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/dump.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/dump.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/formdata.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/formdata.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/_mixin.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/_mixin.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/abnf_regexp.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/abnf_regexp.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/builder.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/builder.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/compat.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/compat.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/iri.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/iri.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/misc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/misc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/normalizers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/normalizers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/parseresult.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/parseresult.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/uri.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/uri.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986/validators.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986/validators.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_cell_widths.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_emoji_codes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_emoji_replace.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_export_format.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_fileno.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_inspect.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_log_render.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_loop.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_null_file.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_palettes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_ratio.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_spinners.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_win32_console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_windows.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_windows_renderer.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/_wrap.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/abc.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/align.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/ansi.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/bar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/box.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/cells.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/color.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/color_triplet.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/columns.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/console.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/constrain.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/containers.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/control.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/default_styles.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/diagnose.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/emoji.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/errors.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/file_proxy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/filesize.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/highlighter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/json.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/jupyter.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/layout.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/live.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/live_render.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/logging.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/markdown.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/markup.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/measure.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/padding.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/pager.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/palette.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/panel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/pretty.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/progress.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/progress_bar.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/prompt.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/protocol.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/repr.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/rule.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/scope.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/screen.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/segment.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/spinner.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/status.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/style.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/styled.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/syntax.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/table.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/terminal_theme.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/text.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/theme.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/traceback.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich/tree.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/rich-13.7.1.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/rich-13.7.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/__main__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/__main__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/auth.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/auth.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/cli.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/cli.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/package.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/package.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/repository.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/repository.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/settings.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/settings.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/utils.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/utils.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/wheel.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/wheel.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/wininst.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/wininst.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/check.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/check.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/register.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/register.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine/commands/upload.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine/commands/upload.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/twine-5.0.0.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/twine-5.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_base_connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_collections.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/_request_methods.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/connectionpool.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/exceptions.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/fields.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/filepost.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/http2.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/http2.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/poolmanager.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/response.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/pyopenssl.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/socks.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/fetch.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/fetch.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/request.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/request.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/contrib/emscripten/response.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/contrib/emscripten/response.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/connection.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/proxy.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/request.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/response.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/retry.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssl_.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/ssltransport.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/timeout.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/url.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3/util/wait.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_authentication.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_common.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_common.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_dll.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_resource.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_system_information.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/cffi/_util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/cffi/_util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_common.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_dll.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_resource.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/core/ctypes/_util.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/pywintypes.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/win32api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/win32api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/pywin32/win32cred.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_backends.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_win32api.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_win32api.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/win32ctypes/tests/test_win32cred.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/__init__.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp/glob.py` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp/glob.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/METADATA` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Lib/site-packages/zipp-3.18.1.dist-info/RECORD` & `apimanager_dm_2024-0.0.7/.venv/Lib/site-packages/zipp-3.18.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate.bat` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate.fish` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate.fish`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate.nu` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate.nu`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate.ps1` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate.ps1`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/activate_this.py` & `apimanager_dm_2024-0.0.7/.venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/deactivate.bat` & `apimanager_dm_2024-0.0.7/.venv/Scripts/deactivate.bat`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/docutils.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/docutils.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/keyring.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/keyring.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/markdown-it.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/markdown-it.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/normalizer.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/normalizer.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pip.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pip3.12.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pip3.12.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pip3.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pkginfo.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pkginfo.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pygmentize.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pygmentize.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pyproject-build.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pyproject-build.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/python.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/pythonw.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html4.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html4.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2html5.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2html5.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2latex.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2latex.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2man.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2man.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2odt.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2odt.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2pseudoxml.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2pseudoxml.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2s5.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2s5.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2xetex.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2xetex.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/rst2xml.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/rst2xml.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/.venv/Scripts/twine.exe` & `apimanager_dm_2024-0.0.7/.venv/Scripts/twine.exe`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/APIManager/APIManager.py` & `apimanager_dm_2024-0.0.7/api_manager/APIManager.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,26 +24,26 @@
             response_object.raise_for_status()
 
 
 def test(text):
     print(text)
 
 
-if __name__ == "__main__":
-    api_manager = APIManager("https://fakestoreapi.com")
-    response = api_manager.request_get("users")
-    response_json = response.json()
-
-    # for item in response_json:
-    #     print(item)
-
-    send_obj_status = api_manager.request_post("users", {
-        "name": "David",
-        "age": 20,
-    })
-
-    # send_obj_status = requests.post("https://fakestoreapi.com/users", json={
-    #     "name": "David",
-    #     "age": 20,
-    # })
-
-    print(send_obj_status)
+# if __name__ == "__main__":
+#     api_manager = APIManipulator("https://fakestoreapi.com")
+#     response = api_manager.request_get("users")
+#     response_json = response.json()
+#
+#     # for item in response_json:
+#     #     print(item)
+#
+#     send_obj_status = api_manager.request_post("users", {
+#         "name": "David",
+#         "age": 20,
+#     })
+#
+#     # send_obj_status = requests.post("https://fakestoreapi.com/users", json={
+#     #     "name": "David",
+#     #     "age": 20,
+#     # })
+#
+#     print(send_obj_status)
```

### Comparing `apimanager_dm_2024-0.0.6/LICENSE` & `apimanager_dm_2024-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apimanager_dm_2024-0.0.6/pyproject.toml` & `apimanager_dm_2024-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "APIManager_DM_2024"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "David", email = "movsis.david@gmail.com" },
 ]
 description = "A small http(s) requests package"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -17,8 +17,8 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["APIManager"]
+packages = ["api_manager"]
```

