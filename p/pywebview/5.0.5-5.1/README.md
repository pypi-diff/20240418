# Comparing `tmp/pywebview-5.0.5.tar.gz` & `tmp/pywebview-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebview-5.0.5.tar", last modified: Thu Mar  7 15:11:52 2024, max compression
+gzip compressed data, was "pywebview-5.1.tar", last modified: Thu Apr 18 20:22:49 2024, max compression
```

## Comparing `pywebview-5.0.5.tar` & `pywebview-5.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.164972 pywebview-5.0.5/
--rw-r--r--   0 roman      (501) staff       (20)      138 2023-08-02 07:40:27.000000 pywebview-5.0.5/.editorconfig
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.144494 pywebview-5.0.5/.github/
--rw-r--r--   0 roman      (501) staff       (20)      544 2022-02-16 20:39:20.000000 pywebview-5.0.5/.github/funding.yml
--rw-r--r--   0 roman      (501) staff       (20)      330 2024-02-23 21:32:21.000000 pywebview-5.0.5/.github/issue_template.md
--rw-r--r--   0 roman      (501) staff       (20)      678 2022-02-16 20:39:20.000000 pywebview-5.0.5/.github/stale.yml
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.145012 pywebview-5.0.5/.github/workflows/
--rw-r--r--   0 roman      (501) staff       (20)      535 2024-03-06 20:39:27.000000 pywebview-5.0.5/.github/workflows/docs.yaml
--rw-r--r--   0 roman      (501) staff       (20)     1206 2023-08-02 07:40:27.000000 pywebview-5.0.5/.github/workflows/stale.yml
--rw-r--r--   0 roman      (501) staff       (20)      263 2024-03-06 20:39:27.000000 pywebview-5.0.5/.gitignore
--rw-r--r--   0 roman      (501) staff       (20)      389 2023-08-02 07:40:27.000000 pywebview-5.0.5/.pre-commit-config.yaml
--rw-r--r--   0 roman      (501) staff       (20)     1518 2024-03-02 13:52:16.000000 pywebview-5.0.5/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)      194 2024-03-06 20:39:27.000000 pywebview-5.0.5/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)     4115 2024-03-07 15:11:52.164604 pywebview-5.0.5/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     5167 2024-03-06 20:39:27.000000 pywebview-5.0.5/README.md
--rw-r--r--   0 roman      (501) staff       (20)      435 2023-08-02 07:40:27.000000 pywebview-5.0.5/SECURITY.md
--rw-r--r--   0 roman      (501) staff       (20)     2431 2024-03-06 20:39:27.000000 pywebview-5.0.5/pyproject.toml
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.163235 pywebview-5.0.5/pywebview.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)     4115 2024-03-07 15:11:51.000000 pywebview-5.0.5/pywebview.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     1595 2024-03-07 15:11:52.000000 pywebview-5.0.5/pywebview.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2024-03-07 15:11:51.000000 pywebview-5.0.5/pywebview.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)      424 2024-03-07 15:11:51.000000 pywebview-5.0.5/pywebview.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)        8 2024-03-07 15:11:51.000000 pywebview-5.0.5/pywebview.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)      490 2023-08-24 11:26:47.000000 pywebview-5.0.5/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2024-03-07 15:11:52.165043 pywebview-5.0.5/setup.cfg
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.148993 pywebview-5.0.5/webview/
--rwxr-xr-x   0 roman      (501) staff       (20)    13430 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)      411 2024-03-07 15:11:51.000000 pywebview-5.0.5/webview/_version.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.150828 pywebview-5.0.5/webview/dom/
--rw-r--r--   0 roman      (501) staff       (20)      987 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/dom/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     1397 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/dom/classlist.py
--rw-r--r--   0 roman      (501) staff       (20)     2533 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/dom/dom.py
--rw-r--r--   0 roman      (501) staff       (20)    14657 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/dom/element.py
--rw-r--r--   0 roman      (501) staff       (20)     1128 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/dom/event.py
--rw-r--r--   0 roman      (501) staff       (20)     5983 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/dom/propsdict.py
--rw-r--r--   0 roman      (501) staff       (20)       93 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/errors.py
--rw-r--r--   0 roman      (501) staff       (20)     2308 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/event.py
--rw-r--r--   0 roman      (501) staff       (20)     3811 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/guilib.py
--rw-r--r--   0 roman      (501) staff       (20)     7883 2023-10-10 21:24:25.000000 pywebview-5.0.5/webview/http.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.153335 pywebview-5.0.5/webview/js/
--rw-r--r--   0 roman      (501) staff       (20)      115 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/js/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)      164 2023-08-02 07:40:27.000000 pywebview-5.0.5/webview/js/alert.py
--rwxr-xr-x   0 roman      (501) staff       (20)     8014 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/js/api.py
--rw-r--r--   0 roman      (501) staff       (20)      515 2023-08-02 07:40:27.000000 pywebview-5.0.5/webview/js/css.py
--rw-r--r--   0 roman      (501) staff       (20)    26112 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/js/dom_json.py
--rw-r--r--   0 roman      (501) staff       (20)     1680 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/js/events.py
--rw-r--r--   0 roman      (501) staff       (20)     1678 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/js/mouse.py
--rw-r--r--   0 roman      (501) staff       (20)     8128 2023-08-02 07:40:27.000000 pywebview-5.0.5/webview/js/npo.py
--rw-r--r--   0 roman      (501) staff       (20)      514 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/js/polyfill.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.156993 pywebview-5.0.5/webview/lib/
--rw-r--r--   0 roman      (501) staff       (20)   500712 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.Core.dll
--rw-r--r--   0 roman      (501) staff       (20)     1608 2023-08-02 07:40:27.000000 pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.LICENSE.md
--rw-r--r--   0 roman      (501) staff       (20)    38376 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.WinForms.dll
--rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-5.0.5/webview/lib/WebBrowserInterop.x64.dll
--rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-5.0.5/webview/lib/WebBrowserInterop.x86.dll
--rw-r--r--   0 roman      (501) staff       (20)     9071 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/lib/pywebview-android.jar
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.141147 pywebview-5.0.5/webview/lib/runtimes/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.140907 pywebview-5.0.5/webview/lib/runtimes/win-arm64/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.157425 pywebview-5.0.5/webview/lib/runtimes/win-arm64/native/
--rw-r--r--   0 roman      (501) staff       (20)   137176 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.141052 pywebview-5.0.5/webview/lib/runtimes/win-x64/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.157835 pywebview-5.0.5/webview/lib/runtimes/win-x64/native/
--rw-r--r--   0 roman      (501) staff       (20)   161240 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/lib/runtimes/win-x64/native/WebView2Loader.dll
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.141209 pywebview-5.0.5/webview/lib/runtimes/win-x86/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.158528 pywebview-5.0.5/webview/lib/runtimes/win-x86/native/
--rw-r--r--   0 roman      (501) staff       (20)   116184 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/lib/runtimes/win-x86/native/WebView2Loader.dll
--rw-r--r--   0 roman      (501) staff       (20)      760 2023-10-01 10:46:15.000000 pywebview-5.0.5/webview/localization.py
--rw-r--r--   0 roman      (501) staff       (20)      669 2023-08-02 07:40:27.000000 pywebview-5.0.5/webview/menu.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-03-07 15:11:52.162771 pywebview-5.0.5/webview/platforms/
--rw-r--r--   0 roman      (501) staff       (20)        0 2022-02-16 20:39:21.000000 pywebview-5.0.5/webview/platforms/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)    12866 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/platforms/android.py
--rw-r--r--   0 roman      (501) staff       (20)    10840 2024-03-07 09:45:51.000000 pywebview-5.0.5/webview/platforms/cef.py
--rw-r--r--   0 roman      (501) staff       (20)    50676 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/platforms/cocoa.py
--rw-r--r--   0 roman      (501) staff       (20)    10276 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/platforms/edgechromium.py
--rwxr-xr-x   0 roman      (501) staff       (20)    29624 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/platforms/gtk.py
--rw-r--r--   0 roman      (501) staff       (20)     8727 2024-03-06 09:11:42.000000 pywebview-5.0.5/webview/platforms/mshtml.py
--rwxr-xr-x   0 roman      (501) staff       (20)    36443 2024-03-07 09:41:42.000000 pywebview-5.0.5/webview/platforms/qt.py
--rw-r--r--   0 roman      (501) staff       (20)    26722 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/platforms/winforms.py
--rw-r--r--   0 roman      (501) staff       (20)      329 2023-08-30 20:06:38.000000 pywebview-5.0.5/webview/screen.py
--rw-r--r--   0 roman      (501) staff       (20)    11889 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/util.py
--rw-r--r--   0 roman      (501) staff       (20)    16706 2024-03-06 20:39:27.000000 pywebview-5.0.5/webview/window.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.211437 pywebview-5.1/
+-rw-r--r--   0 roman      (501) staff       (20)      138 2024-04-16 08:32:51.000000 pywebview-5.1/.editorconfig
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.195873 pywebview-5.1/.github/
+-rw-r--r--   0 roman      (501) staff       (20)      544 2024-04-16 08:32:51.000000 pywebview-5.1/.github/funding.yml
+-rw-r--r--   0 roman      (501) staff       (20)      330 2024-04-16 08:32:51.000000 pywebview-5.1/.github/issue_template.md
+-rw-r--r--   0 roman      (501) staff       (20)      678 2024-04-16 08:32:51.000000 pywebview-5.1/.github/stale.yml
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.196411 pywebview-5.1/.github/workflows/
+-rw-r--r--   0 roman      (501) staff       (20)      535 2024-04-16 08:33:17.000000 pywebview-5.1/.github/workflows/docs.yaml
+-rw-r--r--   0 roman      (501) staff       (20)     1206 2024-04-16 08:32:51.000000 pywebview-5.1/.github/workflows/stale.yml
+-rw-r--r--   0 roman      (501) staff       (20)      263 2024-04-16 08:33:17.000000 pywebview-5.1/.gitignore
+-rw-r--r--   0 roman      (501) staff       (20)      389 2024-04-16 08:32:51.000000 pywebview-5.1/.pre-commit-config.yaml
+-rw-r--r--   0 roman      (501) staff       (20)     1518 2024-04-16 08:32:51.000000 pywebview-5.1/LICENSE
+-rw-r--r--   0 roman      (501) staff       (20)      194 2024-04-16 08:33:17.000000 pywebview-5.1/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)     4113 2024-04-18 20:22:49.211099 pywebview-5.1/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     5203 2024-04-16 08:33:17.000000 pywebview-5.1/README.md
+-rw-r--r--   0 roman      (501) staff       (20)      468 2024-04-16 08:33:17.000000 pywebview-5.1/SECURITY.md
+-rw-r--r--   0 roman      (501) staff       (20)     2431 2024-04-16 08:33:17.000000 pywebview-5.1/pyproject.toml
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.209662 pywebview-5.1/pywebview.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)     4113 2024-04-18 20:22:48.000000 pywebview-5.1/pywebview.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     1595 2024-04-18 20:22:49.000000 pywebview-5.1/pywebview.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2024-04-18 20:22:48.000000 pywebview-5.1/pywebview.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)      424 2024-04-18 20:22:48.000000 pywebview-5.1/pywebview.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)        8 2024-04-18 20:22:48.000000 pywebview-5.1/pywebview.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)      490 2024-04-16 08:32:51.000000 pywebview-5.1/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2024-04-18 20:22:49.211493 pywebview-5.1/setup.cfg
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.198978 pywebview-5.1/webview/
+-rwxr-xr-x   0 roman      (501) staff       (20)    13573 2024-04-16 08:33:17.000000 pywebview-5.1/webview/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)      406 2024-04-18 20:22:48.000000 pywebview-5.1/webview/_version.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.200239 pywebview-5.1/webview/dom/
+-rw-r--r--   0 roman      (501) staff       (20)      987 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     1397 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/classlist.py
+-rw-r--r--   0 roman      (501) staff       (20)     2533 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/dom.py
+-rw-r--r--   0 roman      (501) staff       (20)    14657 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/element.py
+-rw-r--r--   0 roman      (501) staff       (20)     1128 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/event.py
+-rw-r--r--   0 roman      (501) staff       (20)     5983 2024-04-16 08:33:17.000000 pywebview-5.1/webview/dom/propsdict.py
+-rw-r--r--   0 roman      (501) staff       (20)       93 2024-04-16 08:33:17.000000 pywebview-5.1/webview/errors.py
+-rw-r--r--   0 roman      (501) staff       (20)     2488 2024-04-16 08:33:17.000000 pywebview-5.1/webview/event.py
+-rw-r--r--   0 roman      (501) staff       (20)     3811 2024-04-16 08:33:17.000000 pywebview-5.1/webview/guilib.py
+-rw-r--r--   0 roman      (501) staff       (20)     7883 2024-04-16 08:32:51.000000 pywebview-5.1/webview/http.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.201835 pywebview-5.1/webview/js/
+-rw-r--r--   0 roman      (501) staff       (20)      115 2024-04-16 08:33:17.000000 pywebview-5.1/webview/js/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)      164 2024-04-16 08:32:51.000000 pywebview-5.1/webview/js/alert.py
+-rw-r--r--   0 roman      (501) staff       (20)     8100 2024-04-18 17:18:32.000000 pywebview-5.1/webview/js/api.py
+-rw-r--r--   0 roman      (501) staff       (20)      515 2024-04-16 08:32:51.000000 pywebview-5.1/webview/js/css.py
+-rw-r--r--   0 roman      (501) staff       (20)    26112 2024-04-16 08:33:17.000000 pywebview-5.1/webview/js/dom_json.py
+-rw-r--r--   0 roman      (501) staff       (20)     1680 2024-04-16 08:33:17.000000 pywebview-5.1/webview/js/events.py
+-rw-r--r--   0 roman      (501) staff       (20)     1678 2024-04-16 08:33:17.000000 pywebview-5.1/webview/js/mouse.py
+-rw-r--r--   0 roman      (501) staff       (20)     8128 2024-04-16 08:32:51.000000 pywebview-5.1/webview/js/npo.py
+-rw-r--r--   0 roman      (501) staff       (20)      514 2024-04-16 08:33:17.000000 pywebview-5.1/webview/js/polyfill.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.204727 pywebview-5.1/webview/lib/
+-rw-r--r--   0 roman      (501) staff       (20)   500712 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/Microsoft.Web.WebView2.Core.dll
+-rw-r--r--   0 roman      (501) staff       (20)     1608 2024-04-16 08:32:51.000000 pywebview-5.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md
+-rw-r--r--   0 roman      (501) staff       (20)    38376 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll
+-rw-r--r--   0 roman      (501) staff       (20)     7168 2024-04-16 08:32:51.000000 pywebview-5.1/webview/lib/WebBrowserInterop.x64.dll
+-rw-r--r--   0 roman      (501) staff       (20)     7168 2024-04-16 08:32:51.000000 pywebview-5.1/webview/lib/WebBrowserInterop.x86.dll
+-rw-r--r--   0 roman      (501) staff       (20)     9071 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/pywebview-android.jar
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.192273 pywebview-5.1/webview/lib/runtimes/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.192082 pywebview-5.1/webview/lib/runtimes/win-arm64/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.205034 pywebview-5.1/webview/lib/runtimes/win-arm64/native/
+-rw-r--r--   0 roman      (501) staff       (20)   137176 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.192205 pywebview-5.1/webview/lib/runtimes/win-x64/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.205817 pywebview-5.1/webview/lib/runtimes/win-x64/native/
+-rw-r--r--   0 roman      (501) staff       (20)   161240 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/runtimes/win-x64/native/WebView2Loader.dll
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.192323 pywebview-5.1/webview/lib/runtimes/win-x86/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.206578 pywebview-5.1/webview/lib/runtimes/win-x86/native/
+-rw-r--r--   0 roman      (501) staff       (20)   116184 2024-04-16 08:33:17.000000 pywebview-5.1/webview/lib/runtimes/win-x86/native/WebView2Loader.dll
+-rw-r--r--   0 roman      (501) staff       (20)      760 2024-04-16 08:32:51.000000 pywebview-5.1/webview/localization.py
+-rw-r--r--   0 roman      (501) staff       (20)      669 2024-04-16 08:32:51.000000 pywebview-5.1/webview/menu.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-18 20:22:49.209421 pywebview-5.1/webview/platforms/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2022-02-16 20:39:21.000000 pywebview-5.1/webview/platforms/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)    12993 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/android.py
+-rw-r--r--   0 roman      (501) staff       (20)    11094 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/cef.py
+-rw-r--r--   0 roman      (501) staff       (20)    51068 2024-04-18 20:14:10.000000 pywebview-5.1/webview/platforms/cocoa.py
+-rw-r--r--   0 roman      (501) staff       (20)    10433 2024-04-18 20:20:45.000000 pywebview-5.1/webview/platforms/edgechromium.py
+-rwxr-xr-x   0 roman      (501) staff       (20)    29936 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/gtk.py
+-rw-r--r--   0 roman      (501) staff       (20)     8727 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/mshtml.py
+-rwxr-xr-x   0 roman      (501) staff       (20)    36633 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/qt.py
+-rw-r--r--   0 roman      (501) staff       (20)    28205 2024-04-16 08:33:17.000000 pywebview-5.1/webview/platforms/winforms.py
+-rw-r--r--   0 roman      (501) staff       (20)      329 2024-04-16 08:32:52.000000 pywebview-5.1/webview/screen.py
+-rw-r--r--   0 roman      (501) staff       (20)    12033 2024-04-16 08:33:17.000000 pywebview-5.1/webview/util.py
+-rw-r--r--   0 roman      (501) staff       (20)    17044 2024-04-16 08:33:17.000000 pywebview-5.1/webview/window.py
```

### Comparing `pywebview-5.0.5/.github/funding.yml` & `pywebview-5.1/.github/funding.yml`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/.github/stale.yml` & `pywebview-5.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/.github/workflows/docs.yaml` & `pywebview-5.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/.github/workflows/stale.yml` & `pywebview-5.1/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/LICENSE` & `pywebview-5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/PKG-INFO` & `pywebview-5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebview
-Version: 5.0.5
+Version: 5.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS
 Author-email: Roman Sirokov <roman@flowrl.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `pywebview-5.0.5/README.md` & `pywebview-5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 <p align='center'><a href="https://opencollective.com/pywebview" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/pywebview/all/badge.svg?label=financial+contributors" /></a> <img src="https://badge.fury.io/py/pywebview.svg" alt="PyPI version" /> <img src="https://img.shields.io/pypi/dm/pywebview" alt="PyPI downloads" /> <a href="https://ci.appveyor.com/project/r0x0r/pywebview"><img src="https://ci.appveyor.com/api/projects/status/nu6mbhvbq03wudxd/branch/master?svg=true" alt="Build status" /></a>
 
 https://pywebview.flowrl.com
 </p>
 
 
-_pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you power of web technologies in your desktop application, hiding the fact that GUI is browser based. You can use pywebview either with a lightweight web framework like [Flask](http://flask.pocoo.org/) or on its own with a two way bridge between Python and DOM.
+_pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you the power of web technologies in your desktop application, hiding the fact that the GUI is browser based. Available for Windows, macOS, Linux and Android. You can use pywebview either with a 3rd party web framework or on its own with a two way bridge between Python and DOM.
 
-_pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it keeping the executable size small. _pywebview_ is compatible with Python 3.
+_pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS, QT or GTK on Linux and Kivy for Android. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it, keeping the executable size small. _pywebview_ is compatible with Python 3.
 
 _pywebview_ is created by [Roman Sirokov](https://github.com/r0x0r/).
 
 
 # Getting started
 
 ### Install
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
                                [pywebview logo]
                   _[_h_t_t_p_s_:_/_/_o_p_e_n_c_o_l_l_e_c_t_i_v_e_._c_o_m_/_p_y_w_e_b_v_i_e_w_/_a_l_l_/
   _b_a_d_g_e_._s_v_g_?_l_a_b_e_l_=_f_i_n_a_n_c_i_a_l_+_c_o_n_t_r_i_b_u_t_o_r_s_][PyPI version][PyPI downloads]_[_B_u_i_l_d
                       _s_t_a_t_u_s_]https://pywebview.flowrl.com
 _pywebview_ is a lightweight cross-platform wrapper around a webview component
 that allows to display HTML content in its own native GUI window. It gives you
-power of web technologies in your desktop application, hiding the fact that GUI
-is browser based. You can use pywebview either with a lightweight web framework
-like [Flask](http://flask.pocoo.org/) or on its own with a two way bridge
-between Python and DOM. _pywebview_ uses native GUI for creating a web
-component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux.
-If you choose to freeze your application, pywebview does not bundle a heavy GUI
-toolkit or web renderer with it keeping the executable size small. _pywebview_
-is compatible with Python 3. _pywebview_ is created by [Roman Sirokov](https://
-github.com/r0x0r/). # Getting started ### Install ``` bash pip install
-pywebview ``` - _On Linux you need additional libraries. Refer to the
-[installation](https://pywebview.flowrl.com/guide/installation.html) page for
-details._ ### Hello world ``` python import webview webview.create_window
-('Hello world', 'https://pywebview.flowrl.com/hello') webview.start() ```
-Explore _pywebview_ further by reading [documentation](https://
-pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/examples)
-or [contributing](https://pywebview.flowrl.com/contributing). If React is your
-thing, get started right away with [React boilerplate](https://github.com/
-r0x0r/pywebview-react-boilerplate). # Contribution ### Consulting services If
-your company is looking for support with _pywebview_ or needs a hand with full-
-stack development, the author of _pywebview_ is available for hire. As a VAT-
-registered EU based professional, I specialize in a wide range of technologies,
-including JavaScript/TypeScript, React/Vue, Python, GIS, SQL databases, API
-integration, CI/CD pipelines and cloud solutions. For inquiries about
-availability and pricing details, reach out to roman@maumau.fi. ### Code
+the power of web technologies in your desktop application, hiding the fact that
+the GUI is browser based. Available for Windows, macOS, Linux and Android. You
+can use pywebview either with a 3rd party web framework or on its own with a
+two way bridge between Python and DOM. _pywebview_ uses native GUI for creating
+a web component window: WinForms on Windows, Cocoa on macOS, QT or GTK on Linux
+and Kivy for Android. If you choose to freeze your application, pywebview does
+not bundle a heavy GUI toolkit or web renderer with it, keeping the executable
+size small. _pywebview_ is compatible with Python 3. _pywebview_ is created by
+[Roman Sirokov](https://github.com/r0x0r/). # Getting started ### Install ```
+bash pip install pywebview ``` - _On Linux you need additional libraries. Refer
+to the [installation](https://pywebview.flowrl.com/guide/installation.html)
+page for details._ ### Hello world ``` python import webview
+webview.create_window('Hello world', 'https://pywebview.flowrl.com/hello')
+webview.start() ``` Explore _pywebview_ further by reading [documentation]
+(https://pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/
+examples) or [contributing](https://pywebview.flowrl.com/contributing). If
+React is your thing, get started right away with [React boilerplate](https://
+github.com/r0x0r/pywebview-react-boilerplate). # Contribution ### Consulting
+services If your company is looking for support with _pywebview_ or needs a
+hand with full-stack development, the author of _pywebview_ is available for
+hire. As a VAT-registered EU based professional, I specialize in a wide range
+of technologies, including JavaScript/TypeScript, React/Vue, Python, GIS, SQL
+databases, API integration, CI/CD pipelines and cloud solutions. For inquiries
+about availability and pricing details, reach out to roman@maumau.fi. ### Code
 Contributors This project exists thanks to all the people who contribute. [
 [Contribute](docs/contributing/README.md)]. _[_h_t_t_p_s_:_/_/_o_p_e_n_c_o_l_l_e_c_t_i_v_e_._c_o_m_/
 _p_y_w_e_b_v_i_e_w_/_c_o_n_t_r_i_b_u_t_o_r_s_._s_v_g_?_w_i_d_t_h_=_8_9_0_&_b_u_t_t_o_n_=_f_a_l_s_e_]### Financial Contributors
 Become a financial contributor and help us sustain our community. More donation
 options are outlined on the [Donating](https://pywebview.flowrl.com/
 contributing/donating.html) page. #### Individuals _[_h_t_t_p_s_:_/_/_o_p_e_n_c_o_l_l_e_c_t_i_v_e_._c_o_m_/
 _p_y_w_e_b_v_i_e_w_/_i_n_d_i_v_i_d_u_a_l_s_._s_v_g_?_w_i_d_t_h_=_8_9_0_]_[_B_e_c_o_m_e_ _a_ _P_a_t_r_o_n_!_]#### Organizations
```

### Comparing `pywebview-5.0.5/pyproject.toml` & `pywebview-5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/pywebview.egg-info/PKG-INFO` & `pywebview-5.1/pywebview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebview
-Version: 5.0.5
+Version: 5.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS
 Author-email: Roman Sirokov <roman@flowrl.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2014-2017, Roman Sirokov
         All rights reserved.
```

### Comparing `pywebview-5.0.5/pywebview.egg-info/SOURCES.txt` & `pywebview-5.1/pywebview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/__init__.py` & `pywebview-5.1/webview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     screen: Screen = None,
     resizable: bool = True,
     fullscreen: bool = False,
     min_size: tuple[int, int] = (200, 100),
     hidden: bool = False,
     frameless: bool = False,
     easy_drag: bool = True,
+    shadow: bool = True,
     focus: bool = True,
     minimized: bool = False,
     maximized: bool = False,
     on_top: bool = False,
     confirm_close: bool = False,
     background_color: str = '#FFFFFF',
     transparent: bool = False,
@@ -255,14 +256,15 @@
     :param screen: Screen to display the window on.
     :param resizable: True if window can be resized, False otherwise. Default is True
     :param fullscreen: True if start in fullscreen mode. Default is False
     :param min_size: a (width, height) tuple that specifies a minimum window size. Default is 200x100
     :param hidden: Whether the window should be hidden.
     :param frameless: Whether the window should have a frame.
     :param easy_drag: Easy window drag mode when window is frameless.
+    :param shadow: Whether the window should have a frame border (shadows and Windows rounded edges).
     :param focus: Whether to activate the window when user opens it. Window can be controlled with mouse but keyboard input will go to another (active) window and not this one.
     :param minimized: Display window minimized
     :param maximized: Display window maximized
     :param on_top: Keep window above other windows (required OS: Windows)
     :param confirm_close: Display a window close confirmation dialog. Default is False
     :param background_color: Background color as a hex string that is displayed before the content of webview is loaded. Default is white.
     :param text_select: Allow text selection on page. Default is False.
@@ -289,14 +291,15 @@
         y,
         resizable,
         fullscreen,
         min_size,
         hidden,
         frameless,
         easy_drag,
+        shadow,
         focus,
         minimized,
         maximized,
         on_top,
         confirm_close,
         background_color,
         js_api,
```

### Comparing `pywebview-5.0.5/webview/dom/__init__.py` & `pywebview-5.1/webview/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/dom/classlist.py` & `pywebview-5.1/webview/dom/classlist.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/dom/dom.py` & `pywebview-5.1/webview/dom/dom.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/dom/element.py` & `pywebview-5.1/webview/dom/element.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/dom/event.py` & `pywebview-5.1/webview/dom/event.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/dom/propsdict.py` & `pywebview-5.1/webview/dom/propsdict.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/event.py` & `pywebview-5.1/webview/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,25 +24,29 @@
 
         @type_check_only
         def __setattr__(self, __name: str, __value: Event) -> None:
             ...
 
 
 class Event:
-    def __init__(self, should_lock: bool = False) -> None:
+    def __init__(self, window, should_lock: bool = False) -> None:
         self._items: list[Callable[..., Any]] = []
         self._should_lock = should_lock
         self._event = threading.Event()
+        self._window = window
 
     def set(self, *args: Any, **kwargs: Any) -> bool:
         def execute():
             for func in self._items:
                 try:
+
                     if len(inspect.signature(func).parameters.values()) == 0:
                         value = func()
+                    elif 'window' in inspect.signature(func).parameters:
+                        value = func(self._window, *args, **kwargs)
                     else:
                         value = func(*args, **kwargs)
                     return_values.add(value)
 
                 except Exception as e:
                     logger.exception(e)
```

### Comparing `pywebview-5.0.5/webview/guilib.py` & `pywebview-5.1/webview/guilib.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/http.py` & `pywebview-5.1/webview/http.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/api.py` & `pywebview-5.1/webview/js/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,56 +111,62 @@
                 a != null &&
                 typeof(a[Symbol.iterator]) === 'function' &&
                 typeof(a.length) === 'number' &&
                 typeof(a) !== 'string'
             )
         }
 
-        function serialize(obj, depth=0, visited=new WeakSet()) {
+        function serialize(obj, ancestors=[]) {
             try {
                 if (obj instanceof Node) return pywebview.domJSON.toJSON(obj, { metadata: false, serialProperties: true });
                 if (obj instanceof Window) return 'Window';
 
-                if (visited.has(obj)) {
-                    return '[Circular Reference]';
+                var boundSerialize = serialize.bind(obj);
+
+                if (typeof obj !== "object" || obj === null) {
+                    return obj;
                 }
 
-                if (typeof obj === 'object' && obj !== null) {
-                    visited.add(obj);
+                while (ancestors.length > 0 && ancestors[ancestors.length - 1] !== this) {
+                    ancestors.pop();
+                }
 
-                    if (isArrayLike(obj)) {
-                        obj = tryConvertToArray(obj);
-                    }
+                if (ancestors.includes(obj)) {
+                    return "[Circular Reference]";
+                }
+                ancestors.push(obj);
 
-                    if (Array.isArray(obj)) {
-                        const arr = obj.map(value => serialize(value, depth + 1, visited));
-                        visited.delete(obj);
-                        return arr;
-                    }
+                if (isArrayLike(obj)) {
+                    obj = tryConvertToArray(obj);
+                }
 
-                    const newObj = {};
-                    for (const key in obj) {
-                        if (typeof obj === 'function') {
-                            continue;
-                        }
-                        newObj[key] = serialize(obj[key], depth + 1, visited);
+                if (Array.isArray(obj)) {
+                    const arr = obj.map(value => boundSerialize(value, ancestors));
+                    return arr;
+                }
+
+                const newObj = {};
+                for (const key in obj) {
+                    if (typeof obj === 'function') {
+                        continue;
                     }
-                    visited.delete(obj);
-                    return newObj;
+                    newObj[key] = boundSerialize(obj[key], ancestors);
                 }
+                return newObj;
 
-                return obj;
             } catch (e) {
                 console.error(e)
                 return e.toString();
             }
         }
 
-        return JSON.stringify(serialize(obj));
-    },
+      var _serialize = serialize.bind(null);
+
+      return JSON.stringify(_serialize(obj));
+  },
 
     _getNodeId: function (element) {
         if (!element) {
             return null;
         }
         var pywebviewId = element.getAttribute('data-pywebview-id') || Math.random().toString(36).substr(2, 11);
         if (!element.hasAttribute('data-pywebview-id')) {
@@ -215,9 +221,8 @@
     new QWebChannel(qt.webChannelTransport, function(channel) {
         window.pywebview._QWebChannel = channel;
         window.dispatchEvent(new CustomEvent('pywebviewready'));
     });
 } else {
     window.dispatchEvent(new CustomEvent('pywebviewready'));
 }
-
 """
```

### Comparing `pywebview-5.0.5/webview/js/css.py` & `pywebview-5.1/webview/js/css.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/dom_json.py` & `pywebview-5.1/webview/js/dom_json.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/events.py` & `pywebview-5.1/webview/js/events.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/mouse.py` & `pywebview-5.1/webview/js/mouse.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/npo.py` & `pywebview-5.1/webview/js/npo.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/js/polyfill.py` & `pywebview-5.1/webview/js/polyfill.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.Core.dll` & `pywebview-5.1/webview/lib/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.LICENSE.md` & `pywebview-5.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/Microsoft.Web.WebView2.WinForms.dll` & `pywebview-5.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/WebBrowserInterop.x64.dll` & `pywebview-5.1/webview/lib/WebBrowserInterop.x64.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/WebBrowserInterop.x86.dll` & `pywebview-5.1/webview/lib/WebBrowserInterop.x86.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/pywebview-android.jar` & `pywebview-5.1/webview/lib/pywebview-android.jar`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll` & `pywebview-5.1/webview/lib/runtimes/win-arm64/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/runtimes/win-x64/native/WebView2Loader.dll` & `pywebview-5.1/webview/lib/runtimes/win-x64/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/lib/runtimes/win-x86/native/WebView2Loader.dll` & `pywebview-5.1/webview/lib/runtimes/win-x86/native/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/localization.py` & `pywebview-5.1/webview/localization.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/menu.py` & `pywebview-5.1/webview/menu.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/platforms/android.py` & `pywebview-5.1/webview/platforms/android.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,19 @@
     lock = Semaphore(0)
     js_result = None
 
     Runnable(_evaluate_js)()
     lock.acquire()
     return js_result
 
+def clear_cookies(_):
+    def _cookies():
+        CookieManager.getInstance().removeAllCookies(None)
+
+    Runnable(_cookies)()
 
 def get_cookies(_):
     def _cookies():
         nonlocal cookies
 
         raw_cookies = app.view._cookies
         full_url = app.view.webview.getUrl()
```

### Comparing `pywebview-5.0.5/webview/platforms/cef.py` & `pywebview-5.1/webview/platforms/cef.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,19 @@
         result = copy(self.js_bridge.results[unique_id])
 
         del self.eval_events[unique_id]
         del self.js_bridge.results[unique_id]
 
         return result
 
+    def clear_cookies(self):
+        self.loaded.wait()
+        self.cookie_manager.DeleteCookies('', '')
+        self.cookie_manager.FlushStore()
+
     def get_cookies(self):
         self.loaded.wait()
         self.cookie_visitor.cookies = []
         self.cookie_visitor.lock = Event()
         self.cookie_manager.VisitUrlCookies(self.browser.GetUrl(), True, self.cookie_visitor)
         self.cookie_visitor.lock.wait()
 
@@ -233,15 +238,15 @@
 
 def _cef_call(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         uid = args[-1]
 
         if uid not in instances:
-            logger.error('CEF window with uid {0} does not exist'.format(uid))
+            logger.error(f'CEF window with uid {uid} does not exist with {func}')
             return
 
         return func(*args, **kwargs)
 
     return wrapper
 
 
@@ -347,14 +352,20 @@
 @_cef_call
 def evaluate_js(code, result, uid):
     instance = instances[uid]
     return instance.evaluate_js(code, result)
 
 
 @_cef_call
+def clear_cookies(uid):
+    instance = instances[uid]
+    return instance.clear_cookies()
+
+
+@_cef_call
 def get_cookies(uid):
     instance = instances[uid]
     return instance.get_cookies()
 
 
 @_cef_call
 def get_current_url(uid):
```

### Comparing `pywebview-5.0.5/webview/platforms/cocoa.py` & `pywebview-5.1/webview/platforms/cocoa.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,31 +520,30 @@
         self.webkit.setNavigationDelegate_(self._browserDelegate)
         self.window.setDelegate_(self._windowDelegate)
 
         config = self.webkit.configuration()
         config.userContentController().addScriptMessageHandler_name_(
             self._browserDelegate, 'browserDelegate'
         )
+        self.datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
 
         if _settings['private_mode']:
             # nonPersisentDataStore preserves cookies for some unknown reason. For this reason we use default datastore
             # and clear all the cookies beforehand
-            self.datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
 
             def dummy_completion_handler():
                 pass
 
             data_types = WebKit.WKWebsiteDataStore.allWebsiteDataTypes()
             from_start = WebKit.NSDate.dateWithTimeIntervalSince1970_(0)
             config.setWebsiteDataStore_(self.datastore)
             self.datastore.removeDataOfTypes_modifiedSince_completionHandler_(
                 data_types, from_start, dummy_completion_handler
             )
         else:
-            self.datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
             config.setWebsiteDataStore_(self.datastore)
 
         try:
             config.preferences().setValue_forKey_(False, 'backspaceKeyNavigationEnabled')
         except KeyError:
             pass  # backspaceKeyNavigationEnabled does not exist prior to macOS Mojave
 
@@ -627,16 +626,14 @@
         if window.fullscreen:
             self.toggle_fullscreen()
         self.shown.set()
 
     def first_show(self):
         if not self.hidden:
             self.window.makeKeyAndOrderFront_(self.window)
-        else:
-            self.hidden = False
 
         if self.maximized:
             self.maximize()
         elif self.minimized:
             self.minimize()
 
         if not BrowserView.app.isRunning():
@@ -647,14 +644,15 @@
             BrowserView.app.activateIgnoringOtherApps_(Foundation.YES)
             AppHelper.installMachInterrupt()
             BrowserView.app.run()
 
     def show(self):
         def _show():
             self.window.makeKeyAndOrderFront_(self.window)
+            BrowserView.app.activateIgnoringOtherApps_(Foundation.YES)
 
         AppHelper.callAfter(_show)
 
     def hide(self):
         def _hide():
             self.window.orderOut_(self.window)
 
@@ -724,14 +722,24 @@
         window_frame = self.window.frame()
 
         window_frame.origin.x = self.screen.origin.x + (self.screen.size.width - window_frame.size.width) / 2
         window_frame.origin.y = self.screen.origin.y + (self.screen.size.height - window_frame.size.height) / 2
 
         self.window.setFrameOrigin_(window_frame.origin)
 
+    def clear_cookies(self):
+        def clear():
+            self.datastore.removeDataOfTypes_modifiedSince_completionHandler_(
+                WebKit.WKWebsiteDataStore.allWebsiteDataTypes(),
+                Foundation.NSDate.dateWithTimeIntervalSince1970_(0),
+                lambda: None,
+            )
+
+        AppHelper.callAfter(clear)
+
     def get_cookies(self):
         def handler(cookies):
             for c in cookies:
                 domain = c.domain()[1:] if c.domain().startswith('.') else c.domain()
                 if domain not in self.url:
                     continue
 
@@ -1304,14 +1312,20 @@
 
 def get_current_url(uid):
     i = BrowserView.instances.get(uid)
     if i:
         return i.get_current_url()
 
 
+def clear_cookies(uid):
+    i = BrowserView.instances.get(uid)
+    if i:
+        i.clear_cookies()
+
+
 def get_cookies(uid):
     i = BrowserView.instances.get(uid)
     if i:
         return i.get_cookies()
 
 
 def evaluate_js(script, uid):
```

### Comparing `pywebview-5.0.5/webview/platforms/edgechromium.py` & `pywebview-5.1/webview/platforms/edgechromium.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,17 @@
                 self.syncContextTaskScheduler,
             )
         except Exception:
             logger.exception('Error occurred in script')
             js_result.append(None)
             semaphore.release()
 
+    def clear_cookies(self):
+        self.web_view.CoreWebView2.CookieManager.DeleteAllCookies()
+
     def get_cookies(self, cookies, semaphore):
         def _callback(task):
             for c in task.Result:
                 _cookies.append(c)
 
             self.web_view.Invoke(Func[Type](_parse_cookies))
 
@@ -221,14 +224,16 @@
             sender.CoreWebView2.CookieManager.DeleteAllCookies()
 
         if self.pywebview_window.real_url:
             self.load_url(self.pywebview_window.real_url)
         elif self.pywebview_window.html:
             self.html = self.pywebview_window.html
             self.load_html(self.pywebview_window.html, '')
+        else:
+            self.load_html(DEFAULT_HTML, '')
 
         if _settings['debug'] and webview_settings['OPEN_DEVTOOLS_IN_DEBUG']:
             sender.CoreWebView2.OpenDevToolsWindow()
 
     def on_download_starting(self, sender, args):
         if not webview_settings['ALLOW_DOWNLOADS']:
             args.Cancel = True
```

### Comparing `pywebview-5.0.5/webview/platforms/gtk.py` & `pywebview-5.1/webview/platforms/gtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             'GtkWindow {{ background-color: {}; }}'.format(window.background_color).encode()
         )
         gtk.StyleContext.add_provider_for_screen(
             Gdk.Screen.get_default(), style_provider, gtk.STYLE_PROVIDER_PRIORITY_APPLICATION
         )
 
         scrolled_window = gtk.ScrolledWindow()
+        scrolled_window.set_policy(gtk.PolicyType.NEVER, gtk.PolicyType.NEVER)
         self.window.add(scrolled_window)
 
         self.window.connect('delete-event', self.close_window)
 
         self.window.connect('window-state-event', self.on_window_state_change)
         self.window.connect('size-allocate', self.on_window_resize)
         self.window.connect('configure-event', self.on_window_configure)
@@ -302,15 +303,15 @@
                 webview.evaluate_javascript(
                     script=disable_text_select,
                     length=len(disable_text_select),
                     world_name=None,
                     source_uri=None,
                     cancellable=None,
                     callback=None)
-                
+
             self._set_js_api()
 
     def on_download_started(self, session, download):
         download.connect('decide-destination', self.on_download_decide_destination)
 
     def on_download_decide_destination(self, download, suggested_filename):
         destination = self.create_file_dialog(
@@ -489,14 +490,20 @@
             f = gtk.FileFilter()
             f.set_name(description)
             for e in extensions.split(';'):
                 f.add_pattern(e)
 
             dialog.add_filter(f)
 
+    def clear_cookies(self):
+        def _clear_cookies():
+            self.cookie_manager.delete_all_cookies()
+
+        glib.idle_add(_clear_cookies)
+
     def get_cookies(self):
         def _get_cookies():
             self.cookie_manager.get_cookies(self.webview.get_uri(), None, callback, None)
 
         def callback(source, task, data):
             results = source.get_cookies_finish(task)
 
@@ -574,15 +581,15 @@
             self.webview.evaluate_javascript(
                     script=script,
                     length=len(script),
                     world_name=None,
                     source_uri=None,
                     cancellable=None,
                     callback=None)
-    
+
             self.loaded.set()
 
         glib.idle_add(create_bridge)
 
 
 def setup_app():
     # MUST be called before create_window and set_app_menu
@@ -697,14 +704,20 @@
 
 def restore(uid):
     i = BrowserView.instances.get(uid)
     if i:
         glib.idle_add(i.restore)
 
 
+def clear_cookies(uid):
+    i = BrowserView.instances.get(uid)
+    if i:
+        i.clear_cookies()
+
+
 def get_cookies(uid):
     i = BrowserView.instances.get(uid)
     if i:
         cookies = i.get_cookies()
         return cookies
```

### Comparing `pywebview-5.0.5/webview/platforms/mshtml.py` & `pywebview-5.1/webview/platforms/mshtml.py`

 * *Files identical despite different names*

### Comparing `pywebview-5.0.5/webview/platforms/qt.py` & `pywebview-5.1/webview/platforms/qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from PyQt5 import QtWebKitWidgets
     from PyQt5.QtNetwork import QSslCertificate, QSslConfiguration
     from PyQt5.QtWebKitWidgets import QWebPage, QWebView
 
     is_webengine = False
     renderer = 'qtwebkit'
 
-if is_webengine and QtCore.QSysInfo.productType() in ['arch', 'manjaro', 'nixos','rhel']:
+if is_webengine and QtCore.QSysInfo.productType() in ['arch', 'manjaro', 'nixos', 'rhel', 'pop']:
     # I don't know why, but it's a common solution for #890 (White screen displayed)
     # such as:
     # - https://github.com/LCA-ActivityBrowser/activity-browser/pull/954/files
     # - https://bugs.archlinux.org/task/73957
     # - https://www.google.com/search?q=arch+rstudio+no+sandbox
     # And sometimes it needs two "--no-sandbox" flags
 
@@ -219,15 +219,14 @@
                 return False
             else:
                 self.parent.load_url(url.toString())
                 return True
 
     class WebPage(QWebPage):
         def __init__(self, parent=None, profile=None):
-            print(profile)
             if is_webengine and profile:
                 super(BrowserView.WebPage, self).__init__(profile, parent.view)
             else:
                 super(BrowserView.WebPage, self).__init__(parent.view)
 
             if is_webengine:
                 self.featurePermissionRequested.connect(self.onFeaturePermissionRequested)
@@ -366,24 +365,26 @@
                 BrowserView.inspector_port = BrowserView._get_debug_port()
                 os.environ['QTWEBENGINE_REMOTE_DEBUGGING'] = BrowserView.inspector_port
         else:
             self.view.setContextMenuPolicy(
                 QtCore.Qt.NoContextMenu
             )  # disable right click context menu
 
+        self.cookies = {}
+
         if is_webengine:
             if _settings['private_mode']:
                 self.profile = QWebEngineProfile()
             else:
                 self.profile = QWebEngineProfile('pywebview')
                 self.profile.setPersistentStoragePath(_profile_storage_path)
-                self.cookies = {}
-                cookie_store = self.profile.cookieStore()
-                cookie_store.cookieAdded.connect(self.on_cookie_added)
-                cookie_store.cookieRemoved.connect(self.on_cookie_removed)
+                
+            cookie_store = self.profile.cookieStore()
+            cookie_store.cookieAdded.connect(self.on_cookie_added)
+            cookie_store.cookieRemoved.connect(self.on_cookie_removed)
 
             self.view.setPage(BrowserView.WebPage(self, profile=self.profile))
         elif not is_webengine and not _settings['private_mode']:
             logger.warning('qtwebkit does not support private_mode')
 
         if is_webengine:
             self.profile.settings().setAttribute(
@@ -682,14 +683,18 @@
 
     def set_title(self, title):
         self.set_title_trigger.emit(title)
 
     def get_cookies(self):
         return list(self.cookies.values())
 
+    def clear_cookies(self):
+        self.cookies = {}
+        self.profile.cookieStore().deleteAllCookies()
+
     def get_current_url(self):
         self.loaded.wait()
         self.current_url_trigger.emit()
         self._current_url_semaphore.acquire()
 
         return self._current_url
 
@@ -893,14 +898,20 @@
 
 def set_title(title, uid):
     i = BrowserView.instances.get(uid)
     if i:
         i.set_title(title)
 
 
+def clear_cookies(uid):
+    i = BrowserView.instances.get(uid)
+    if i:
+        i.clear_cookies()
+
+
 def get_cookies(uid):
     i = BrowserView.instances.get(uid)
     if i:
         return i.get_cookies()
 
 
 def get_current_url(uid):
```

### Comparing `pywebview-5.0.5/webview/platforms/winforms.py` & `pywebview-5.1/webview/platforms/winforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import sys
 import tempfile
 import threading
 import winreg
 from ctypes import windll
+from ctypes import wintypes
 from platform import machine
 from threading import Event, Semaphore
 
 import clr
 
 from webview import FOLDER_DIALOG, OPEN_DIALOG, SAVE_DIALOG, _settings, windows
 from webview.guilib import forced_gui_
@@ -117,21 +118,44 @@
 
     logger.debug('Using WinForms / Chromium')
     renderer = 'edgechromium'
 else:
     from . import mshtml as IE
 
     logger.warning(
-        'MSHTML is deprecated. See https://pywebview.flowrl.com/guide/renderer.html#web-engine on details how to use Edge Chromium'
+        'MSHTML is deprecated. See https://pywebview.flowrl.com/guide/web_engine.html on details how to use Edge Chromium'
     )
     logger.debug('Using WinForms / MSHTML')
     IE._set_ie_mode()
     renderer = 'mshtml'
 
 
+def DwmSetWindowAttribute(hwnd, attr, value, size=4):
+    DwmSetWindowAttribute = ctypes.windll.dwmapi.DwmSetWindowAttribute
+    DwmSetWindowAttribute.argtypes = [wintypes.HWND, wintypes.DWORD, ctypes.c_void_p, wintypes.DWORD]
+    return DwmSetWindowAttribute(hwnd, attr, ctypes.byref(ctypes.c_int(value)), size)
+
+
+def ExtendFrameIntoClientArea(hwnd):
+    class _MARGINS(ctypes.Structure):
+        _fields_ = [("cxLeftWidth", ctypes.c_int),
+                    ("cxRightWidth", ctypes.c_int),
+                    ("cyTopHeight", ctypes.c_int),
+                    ("cyBottomHeight", ctypes.c_int)
+                    ]
+
+    DwmExtendFrameIntoClientArea = ctypes.windll.dwmapi.DwmExtendFrameIntoClientArea
+    m = _MARGINS()
+    m.cxLeftWidth = 1
+    m.cxRightWidth = 1
+    m.cyTopHeight = 1
+    m.cyBottomHeight = 1
+    return DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(m))
+
+
 class BrowserView:
     instances = {}
 
     app_menu_list = None
 
     class BrowserForm(WinForms.Form):
         def __init__(self, window, cache_dir):
@@ -191,14 +215,19 @@
             self.text_select = window.text_select
             self.TopMost = window.on_top
 
             self.is_fullscreen = False
             if window.fullscreen:
                 self.toggle_fullscreen()
 
+            if window.shadow:
+                # Should do this before set frameless
+                ExtendFrameIntoClientArea(self.Handle.ToInt32())
+                DwmSetWindowAttribute(self.Handle.ToInt32(), 2, 2, 4)
+
             if window.frameless:
                 self.frameless = window.frameless
                 self.FormBorderStyle = getattr(WinForms.FormBorderStyle, 'None')
 
             if BrowserView.app_menu_list:
                 self.set_window_menu(BrowserView.app_menu_list)
 
@@ -232,17 +261,14 @@
 
             self.localization = window.localization
 
         def on_activated(self, *_):
             if not self.pywebview_window.focus:
                 windll.user32.SetWindowLongW(self.Handle.ToInt32(), -20, windll.user32.GetWindowLongW(self.Handle.ToInt32(), -20) | 0x8000000)
 
-            if is_cef and self.pywebview_window.focus:
-                CEF.focus(self.uid)
-
         def on_shown(self, *_):
             if not is_cef:
                 self.shown.set()
                 self.browser.web_view.Focus()
 
         def on_close(self, *_):
             def _shutdown():
@@ -323,14 +349,24 @@
 
             if is_chromium:
                 result = js_result.pop()
                 return result
 
             return self.browser.js_result
 
+        def clear_cookies(self):
+            def _clear_cookies():
+                self.browser.clear_cookies()
+
+            if not is_chromium:
+                logger.error('clear_cookies() is not implemented for this platform')
+                return
+
+            self.Invoke(Func[Type](_clear_cookies))
+
         def get_cookies(self):
             def _get_cookies():
                 self.browser.get_cookies(cookies, semaphore)
 
             cookies = []
             if not is_chromium:
                 logger.error('get_cookies() is not implemented for this platform')
@@ -669,14 +705,23 @@
 
         return file_path
     except:
         logger.exception('Error invoking %s dialog', dialog_type)
         return None
 
 
+def clear_cookies(uid):
+    if is_cef:
+        CEF.clear_cookies(uid)
+    i = BrowserView.instances.get(uid)
+
+    if i:
+        i.clear_cookies()
+
+
 def get_cookies(uid):
     if is_cef:
         return CEF.get_cookies(uid)
     i = BrowserView.instances.get(uid)
 
     if i:
         return i.get_cookies()
```

### Comparing `pywebview-5.0.5/webview/util.py` & `pywebview-5.1/webview/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
     if hasattr(sys, '_MEIPASS'):  # Pyinstaller
         return sys._MEIPASS
 
     if getattr(sys, 'frozen', False):  # cx_freeze
         return os.path.dirname(sys.executable)
 
     if 'pytest' in sys.modules:
+        root_dir = [arg.split('=')[1] for arg in sys.argv if arg.startswith('--rootdir')]
+
+        if root_dir:
+            return root_dir[0]
+
         for arg in reversed(sys.argv):
             path = os.path.realpath(arg.split('::')[0])
             if os.path.exists(path):
                 return path if os.path.isdir(path) else os.path.dirname(path)
 
     if hasattr(sys, 'getandroidapilevel'):
         return os.getenv('ANDROID_APP_PATH')
```

### Comparing `pywebview-5.0.5/webview/window.py` & `pywebview-5.1/webview/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         y: int | None = None,
         resizable: bool = True,
         fullscreen: bool = False,
         min_size: tuple[int, int] = (200, 100),
         hidden: bool = False,
         frameless: bool = False,
         easy_drag: bool = True,
+        shadow: bool = True,
         focus: bool = True,
         minimized: bool = False,
         maximized: bool = False,
         on_top: bool = False,
         confirm_close: bool = False,
         background_color: str = '#FFFFFF',
         js_api: Any = None,
@@ -117,14 +118,15 @@
         self.fullscreen = fullscreen
         self.min_size = min_size
         self.confirm_close = confirm_close
         self.background_color = background_color
         self.text_select = text_select
         self.frameless = frameless
         self.easy_drag = easy_drag
+        self.shadow = shadow
         self.focus = focus
         self.hidden = hidden
         self.on_top = on_top
         self.minimized = minimized
         self.maximized = maximized
         self.transparent = transparent
         self.zoomable = zoomable
@@ -144,23 +146,23 @@
         self._server = None
 
         self._js_api = js_api
         self._functions: dict[str, Callable[..., Any]] = {}
         self._callbacks: dict[str, Callable[..., Any] | None] = {}
 
         self.events = EventContainer()
-        self.events.closed = Event()
-        self.events.closing = Event(True)
-        self.events.loaded = Event()
-        self.events.shown = Event()
-        self.events.minimized = Event()
-        self.events.maximized = Event()
-        self.events.restored = Event()
-        self.events.resized = Event()
-        self.events.moved = Event()
+        self.events.closed = Event(self)
+        self.events.closing = Event(self, True)
+        self.events.loaded = Event(self)
+        self.events.shown = Event(self)
+        self.events.minimized = Event(self)
+        self.events.maximized = Event(self)
+        self.events.restored = Event(self)
+        self.events.resized = Event(self)
+        self.events.moved = Event(self)
 
         self.dom = DOM(self)
         self.gui = None
 
     def _initialize(self, gui, server: http.BottleServer | None = None):
         self.gui = gui
 
@@ -275,14 +277,21 @@
         """
         Set a new title of the window
         """
         self._title = title
         self.gui.set_title(title, self.uid)
 
     @_loaded_call
+    def clear_cookies(self):
+        """
+        Clear all the cookies
+        """
+        return self.gui.clear_cookies(self.uid)
+
+    @_loaded_call
     def get_cookies(self):
         """
         Get cookies for the current website
         """
         return self.gui.get_cookies(self.uid)
 
     @_loaded_call
@@ -374,15 +383,15 @@
         Move Window
         :param x: desired x coordinate of target window
         :param y: desired y coordinate of target window
         """
         self.gui.move(x, y, self.uid)
 
     @_loaded_call
-    def evaluate_js(self, script: str, callback: Callable[..., Any] | None = None) -> Any:
+    def evaluate_js(self, script: str, callback: Callable[..., Any] | None = None, raw=False) -> Any:
         """
         Evaluate given JavaScript code and return the result
         :param script: The JavaScript code to be evaluated
         :return: Return value of the evaluated code
         :callback: Optional callback function that will be called for resolved promises
         """
         unique_id = uuid1().hex
@@ -393,15 +402,17 @@
                 unique_id,
             )
         elif self.gui.renderer == 'android-webkit':
             sync_eval = 'return pywebview._stringify(value);'
         else:
             sync_eval = 'pywebview._stringify(value);'
 
-        if callback:
+        if raw:
+            escaped_script = escape_string(script)
+        elif callback:
             escaped_script = """
                 var value = eval("{0}");
                 if (pywebview._isPromise(value)) {{
                     value.then(function evaluate_async(result) {{
                         pywebview._asyncCallback(pywebview._stringify(result), "{1}")
                     }}).catch(function evaluate_async(error) {{
                         pywebview._asyncCallback(pywebview._stringify(error), "{1}")
@@ -425,15 +436,15 @@
                     keys.forEach(function(key) {{ value[key] = e[key] }})
                 }}
                 {sync_eval};
             """
 
         if self.gui.renderer == 'cef':
             result = self.gui.evaluate_js(escaped_script, self.uid, unique_id)
-        elif self.gui.renderer == 'android-webkit':
+        elif self.gui.renderer == 'android-webkit' and not raw:
             escaped_script = f"""
                 (function() {{
                     {escaped_script}
                 }})()
             """
             result = self.gui.evaluate_js(escaped_script, self.uid)
         else:
```

