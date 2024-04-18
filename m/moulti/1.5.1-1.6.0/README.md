# Comparing `tmp/moulti-1.5.1.tar.gz` & `tmp/moulti-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moulti-1.5.1.tar", last modified: Sun Mar 31 14:47:03 2024, max compression
+gzip compressed data, was "moulti-1.6.0.tar", last modified: Thu Apr 18 14:41:10 2024, max compression
```

## Comparing `moulti-1.5.1.tar` & `moulti-1.6.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.472310 moulti-1.5.1/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.5.1/LICENSE
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3888 2024-03-31 14:47:03.468310 moulti-1.5.1/PKG-INFO
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2899 2024-03-15 01:21:38.000000 moulti-1.5.1/README.md
--rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.5.1/pyproject.toml
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-03-31 14:47:03.472310 moulti-1.5.1/setup.cfg
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1497 2024-03-31 14:43:59.000000 moulti-1.5.1/setup.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/
--rw-r--r--   0 xavier    (1000) xavier    (1000)       76 2024-03-31 14:44:02.000000 moulti-1.5.1/src/moulti/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.5.1/src/moulti/__main__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.5.1/src/moulti/ansi.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    20997 2024-03-31 10:37:09.000000 moulti-1.5.1/src/moulti/app.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6677 2024-03-15 00:47:42.000000 moulti-1.5.1/src/moulti/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1064 2024-03-15 00:47:42.000000 moulti-1.5.1/src/moulti/helpers.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.5.1/src/moulti/precli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.5.1/src/moulti/protocol.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/
--rw-r--r--   0 xavier    (1000) xavier    (1000)      165 2024-02-16 23:41:25.000000 moulti-1.5.1/src/moulti/widgets/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/abstractquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.5.1/src/moulti/widgets/abstractquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      600 2024-02-16 15:33:17.000000 moulti-1.5.1/src/moulti/widgets/abstractquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2785 2024-03-12 15:58:46.000000 moulti-1.5.1/src/moulti/widgets/abstractquestion/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/abstractstep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.5.1/src/moulti/widgets/abstractstep/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      891 2024-03-15 00:04:02.000000 moulti-1.5.1/src/moulti/widgets/abstractstep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5823 2024-03-12 22:56:22.000000 moulti-1.5.1/src/moulti/widgets/abstractstep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/buttonquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.5.1/src/moulti/widgets/buttonquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.5.1/src/moulti/widgets/buttonquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.5.1/src/moulti/widgets/buttonquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.5.1/src/moulti/widgets/cli.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/inputquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.5.1/src/moulti/widgets/inputquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.5.1/src/moulti/widgets/inputquestion/cli.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-03-11 11:06:29.000000 moulti-1.5.1/src/moulti/widgets/inputquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.5.1/src/moulti/widgets/moulticonsole.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.5.1/src/moulti/widgets/moultilog.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.5.1/src/moulti/widgets/quitdialog.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti/widgets/step/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.5.1/src/moulti/widgets/step/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4541 2024-02-24 00:23:06.000000 moulti-1.5.1/src/moulti/widgets/step/cli.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     7207 2024-03-04 03:59:15.000000 moulti-1.5.1/src/moulti/widgets/step/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.5.1/src/moulti/widgets/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-02-03 20:43:48.000000 moulti-1.5.1/src/moulti/widgets/vertscroll.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-03-31 14:47:03.468310 moulti-1.5.1/src/moulti.egg-info/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3888 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/PKG-INFO
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1238 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/SOURCES.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/dependency_links.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       46 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/entry_points.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       36 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/requires.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-03-31 14:47:03.000000 moulti-1.5.1/src/moulti.egg-info/top_level.txt
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.6.0/LICENSE
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4241 2024-04-18 14:41:10.850919 moulti-1.6.0/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3252 2024-04-18 01:55:09.000000 moulti-1.6.0/README.md
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.6.0/pyproject.toml
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-18 14:41:10.850919 moulti-1.6.0/setup.cfg
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1497 2024-04-18 14:38:53.000000 moulti-1.6.0/setup.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.846919 moulti-1.6.0/src/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.846919 moulti-1.6.0/src/moulti/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       76 2024-04-18 14:38:56.000000 moulti-1.6.0/src/moulti/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.6.0/src/moulti/__main__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.6.0/src/moulti/ansi.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    21830 2024-04-17 16:17:33.000000 moulti-1.6.0/src/moulti/app.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7395 2024-04-15 23:17:12.000000 moulti-1.6.0/src/moulti/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/helpers.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.6.0/src/moulti/precli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.6.0/src/moulti/protocol.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      165 2024-02-16 23:41:25.000000 moulti-1.6.0/src/moulti/widgets/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/abstractquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      600 2024-02-16 15:33:17.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2785 2024-03-12 15:58:46.000000 moulti-1.6.0/src/moulti/widgets/abstractquestion/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/abstractstep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1123 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6555 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/abstractstep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/buttonquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.6.0/src/moulti/widgets/buttonquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.6.0/src/moulti/widgets/cli.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/inputquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/cli.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-03-11 11:06:29.000000 moulti-1.6.0/src/moulti/widgets/inputquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.6.0/src/moulti/widgets/moulticonsole.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.6.0/src/moulti/widgets/moultilog.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.6.0/src/moulti/widgets/quitdialog.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti/widgets/step/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.6.0/src/moulti/widgets/step/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4541 2024-02-24 00:23:06.000000 moulti-1.6.0/src/moulti/widgets/step/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7225 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/step/tui.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.6.0/src/moulti/widgets/stepcontainer.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.6.0/src/moulti/widgets/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.6.0/src/moulti/widgets/vertscroll.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-18 14:41:10.850919 moulti-1.6.0/src/moulti.egg-info/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4241 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/PKG-INFO
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1274 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/SOURCES.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/dependency_links.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       46 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/entry_points.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       36 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/requires.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-04-18 14:41:10.000000 moulti-1.6.0/src/moulti.egg-info/top_level.txt
```

### Comparing `moulti-1.5.1/LICENSE` & `moulti-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/PKG-INFO` & `moulti-1.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.5.1
+Version: 1.6.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
 Classifier: Environment :: Console :: Curses
@@ -27,14 +27,16 @@
 Moulti changes the way your shell scripts (bash, zsh, etc.) display their output in your terminal.
 Moulti enables you to assign the numerous lines emitted by your scripts to "steps", i.e. visual, collapsible blocks featuring their own title and color.
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
+Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
+
 Moulti is a tool meant for people who write and execute shell scripts.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 ## How?
 
 Synopsis:
 
@@ -49,18 +51,21 @@
 
 As shown in the demo, Moulti enables user interactions through **questions**:
 
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
-Moulti also features a **progress bar**: [documentation](Documentation.md#progress-bar)
+Moulti also features:
+- a **progress bar**: [documentation](Documentation.md#progress-bar)
+- programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 
 When it comes to look and feel, Moulti can be customised:
 
+- through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
 
 ## Implementation
 
 Moulti is written in Python and leverages [Textual](https://textual.textualize.io/), along with [Pyperclip](https://pypi.org/project/pyperclip/) and [argcomplete](https://kislyuk.github.io/argcomplete/).
```

### Comparing `moulti-1.5.1/README.md` & `moulti-1.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Moulti changes the way your shell scripts (bash, zsh, etc.) display their output in your terminal.
 Moulti enables you to assign the numerous lines emitted by your scripts to "steps", i.e. visual, collapsible blocks featuring their own title and color.
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
+Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
+
 Moulti is a tool meant for people who write and execute shell scripts.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 ## How?
 
 Synopsis:
 
@@ -25,18 +27,21 @@
 
 As shown in the demo, Moulti enables user interactions through **questions**:
 
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
-Moulti also features a **progress bar**: [documentation](Documentation.md#progress-bar)
+Moulti also features:
+- a **progress bar**: [documentation](Documentation.md#progress-bar)
+- programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 
 When it comes to look and feel, Moulti can be customised:
 
+- through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
 
 ## Implementation
 
 Moulti is written in Python and leverages [Textual](https://textual.textualize.io/), along with [Pyperclip](https://pypi.org/project/pyperclip/) and [argcomplete](https://kislyuk.github.io/argcomplete/).
```

### Comparing `moulti-1.5.1/pyproject.toml` & `moulti-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/setup.py` & `moulti-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 short_description += 'lines emitted by your scripts to visual, collapsible blocks called steps.'
 
 with open('README.md', 'r') as readme:
 	long_description = readme.read()
 
 setup(
 	name='moulti',
-	version='1.5.1',
+	version='1.6.0',
 	description=short_description,
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Xavier G.',
 	author_email='xavier.moulti@kindwolf.org',
 	url='https://github.com/xavierog/moulti',
 	packages=[
```

### Comparing `moulti-1.5.1/src/moulti/ansi.py` & `moulti-1.6.0/src/moulti/ansi.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/app.py` & `moulti-1.6.0/src/moulti/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .ansi import AnsiThemePolicy, dump_filters
 from .helpers import call_all
 from .protocol import PRINTABLE_MOULTI_SOCKET, clean_socket, current_instance
 from .protocol import moulti_listen, get_unix_credentials, send_json_message
 from .protocol import MoultiConnectionClosedException, MoultiProtocolException, Message, FDs
 from .protocol import MoultiTLVReader, data_to_message, getraddr
 from .widgets.tui import MoultiWidgets
-from .widgets.vertscroll import VertScroll
+from .widgets.stepcontainer import StepContainer
 from .widgets.abstractstep.tui import AbstractStep
 from .widgets.moulticonsole import MoultiConsole
 from .widgets.quitdialog import QuitDialog
 
 def timestamp() -> str:
 	timestamp_ns = time_ns()
 	timestamp_s = timestamp_ns//10**9
@@ -87,15 +87,15 @@
 		# Make this behaviour configurable through environment variables:
 		self.allowed_uids.extend(ids_from_env('MOULTI_ALLOWED_UID'))
 		self.allowed_gids.extend(ids_from_env('MOULTI_ALLOWED_GID'))
 
 	def init_widgets(self) -> None:
 		self.title_label = Label('Moulti', id='header')
 		self.title_label.tooltip = f'Instance name: {current_instance()}'
-		self.steps_container = VertScroll(id='steps_container')
+		self.steps_container = StepContainer()
 		self.progress_bar = ProgressBar(id='progress_bar', show_eta=False)
 		self.footer = Footer()
 
 	def setup_ansi_behavior(self) -> None:
 		"""
 		By default and by design, Textual strives to avoid outputting ANSI colors (i.e. the 16 colors that have no
 		official value). This makes perfect sense for most applications. Moulti is special because its users expect
@@ -171,19 +171,24 @@
 					process.terminate()
 				# else just leave the process running in the background and exit.
 		except Exception as exc:
 			self.logconsole(f'exec: error running {command}: {exc}')
 			self.init_command_running = False
 
 	def all_steps(self) -> Iterator[AbstractStep]:
-		return self.query('#steps_container AbstractStep').results(AbstractStep)
+		return self.steps_container.ordered_steps()
 
 	def export_properties(self) -> dict[str, Any]:
-		prop = {}
+		prop: dict[str, Any] = {}
 		prop['title'] = str(self.title_label.renderable)
+		prop['progress_bar'] = self.progress_bar.styles.display == 'block'
+		prop['progress_target'] = self.progress_bar.total
+		prop['progress'] = self.progress_bar.progress
+		prop['step_position'] = 'bottom' if self.steps_container.has_class('bottom') else 'top'
+		prop['step_direction'] = 'down' if self.steps_container.layout_direction_is_down else 'up'
 		return prop
 
 	def logconsole(self, line: str) -> None:
 		line = timestamp() + line
 		if self._thread_id == get_ident():
 			self.end_user_console.write(line)
 		else:
@@ -319,15 +324,15 @@
 				action = str(message.get('action'))
 				# add/update/delete actions are considered common/standard and are thus handled here:
 				if action == 'add':
 					if step:
 						raise MoultiMessageException(f'id {message.get("id")} already in use')
 					if 'id' not in message:
 						raise MoultiMessageException('missing id')
-					calls.append((self.steps_container.mount, command_class(**message)))
+					calls.append((self.steps_container.add_step, command_class(**message)))
 				else:
 					# All other actions require an existing step:
 					if not step:
 						raise MoultiMessageException(f'unknown id: {message.get("id")}')
 					if not isinstance(step, command_class):
 						raise MoultiMessageException(f'{message.get("id")} is not a {command}')
 					if action == 'update':
@@ -358,28 +363,42 @@
 						if call:
 							calls.append(call)
 						else:
 							finally_reply = False
 			elif command == 'set':
 				if message.get('title') is not None:
 					calls.append((self.title_label.update, str(message['title'])))
+				if message.get('step_position') is not None:
+					calls.append((self.steps_container.set_class, message['step_position'] == 'bottom', 'bottom'))
+				if message.get('step_direction') is not None:
+					is_down = bool(message['step_direction'] != 'up')
+					calls.append((setattr, self.steps_container, 'layout_direction_is_down', is_down))
 				if message.get('progress_bar') is not None:
 					display_progress_bar = 'block' if bool(message['progress_bar']) else 'none'
 					calls.append((setattr, self.progress_bar.styles, 'display', display_progress_bar))
 				if message.get('progress_target') is not None:
 					progress_target = float(message['progress_target'])
 					final_progress_target: float|None = None if progress_target <= 0 else progress_target
 					calls.append((setattr, self.progress_bar, 'total', final_progress_target))
 				if message.get('progress') is not None:
 					progress_float = float(message['progress'])
 					progress_str = str(message['progress'])
 					if progress_str.startswith('+') or progress_str.startswith('-'):
 						calls.append((self.progress_bar.advance, progress_float))
 					else:
 						calls.append((setattr, self.progress_bar, 'progress', progress_float))
+			elif command == 'scroll':
+				step = self.step_from_message(message)
+				if step is None:
+					raise MoultiMessageException(f'unknown id: {message.get("id")}')
+				try:
+					offset = int(message['offset'])
+				except Exception:
+					offset = True
+				calls.append((self.steps_container.scroll_to_step, step, offset))
 			elif command == 'ping':
 				pass
 			else:
 				raise MoultiMessageException(f'unknown command {command}')
 			# At this stage, the analysis is complete; perform the required action and reply accordingly:
 			if calls:
 				self.call_from_thread(call_all, calls)
@@ -489,18 +508,14 @@
 		text-align: center;
 		/* For the title to appear centered, the widget must occupy all available width: */
 		width: 100%;
 		background: $accent;
 		color: auto;
 	}
 
-	/* Leave a thin space between steps and their container's vertical scrollbar: */
-	#steps_container.vertical_scrollbar_visible > Widget {
-		margin-right: 1;
-	}
 	/* Show the progress bar as a full-width extension of the footer: */
 	#progress_bar {
 		display: none; /* Do not display by default */
 		background: $accent;
 		padding-left: 1;
 		padding-right: 1;
 		width: 100%;
```

### Comparing `moulti-1.5.1/src/moulti/cli.py` & `moulti-1.6.0/src/moulti/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,24 +115,32 @@
 	wait_parser.add_argument('--delay', '-d', type=pint, default=500, help='number of milliseconds between two connection attempts')
 	wait_parser.add_argument('--max-attempts', '-m', type=pint, default=0, help='maximum number of attempts before giving up; 0 means "never give up"')
 
 	# moulti set
 	set_parser = subparsers.add_parser('set', help='Set Moulti options')
 	set_parser.set_defaults(func=send_to_moulti_and_handle_reply, command='set')
 	set_parser.add_argument('--title', '-t', default=None, type=str, help='title displayed at the top of the screen')
+	set_parser.add_argument('--step-position', default=None, type=str, choices=('top', 'bottom'), help='whether to display steps at the top (default) or bottom of the screen')
+	set_parser.add_argument('--step-direction', default=None, type=str, choices=('up', 'down'), help='whether to lay out steps up or down (default)')
 	set_parser.add_argument('--progress-bar', default=None, action=BooleanOptionalAction, help='whether to display the progress bar')
 	set_parser.add_argument('--progress-target', '-pt', default=None, type=float, help='total number of steps associated with the progress bar')
 	set_parser.add_argument('--progress', '-p', default=None, type=float_str, help='progress so far, in number of steps; accept absolute or relative values, e.g. 50, +1 or -5')
 
 	# moulti load
 	load_parser = subparsers.add_parser('load', help='Load a saved directory into Moulti')
 	load_parser.set_defaults(func=load, command='load')
 	arg = load_parser.add_argument('saved_directory', type=Path, help='path to a directory generated by Moulti\'s "Save" feature')
 	arg.completer = argcomplete.completers.DirectoriesCompleter()
 
+	# moulti scroll
+	scroll_parser = subparsers.add_parser('scroll', help='Scroll to make a specific step visible')
+	scroll_parser.set_defaults(func=send_to_moulti_and_handle_reply, command='scroll')
+	scroll_parser.add_argument('id', type=str, help='step identifier')
+	scroll_parser.add_argument('offset', type=int, nargs='?', default=None, help='-1: last line, 0: first line, 1: second line, etc.')
+
 def build_arg_parser() -> ArgumentParser:
 	arg_parser = ArgumentParser(prog='moulti', description='step-by-step logs')
 	arg_parser.add_argument('--version', action='version', version=moulti_version)
 	subparsers = arg_parser.add_subparsers(required=True)
 	# moulti init, moulti wait:
 	add_main_commands(subparsers)
 	# moulti <widget>:
```

### Comparing `moulti-1.5.1/src/moulti/helpers.py` & `moulti-1.6.0/src/moulti/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 		raise ArgumentTypeError('expected a positive integer')
 	return integer_value
 
 def float_str(value: str) -> str:
 	_ = float(value)
 	return value
 
+def bool_or_int(value: str) -> bool|int:
+	if value.lower() == 'false':
+		return False
+	if value.lower() == 'true':
+		return True
+	return int(value)
+
 def handle_reply(reply: Message) -> None:
 	success = reply.get('done') is True
 	if not success:
 		fallback = 'alas, no error message was provided.'
 		error_message = reply.get('error', fallback)
 		sys.stderr.write(f'Something went wrong: {error_message}\n')
 	sys.exit(0 if success else 1)
```

### Comparing `moulti-1.5.1/src/moulti/precli.py` & `moulti-1.6.0/src/moulti/precli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/protocol.py` & `moulti-1.6.0/src/moulti/protocol.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/abstractquestion/cli.py` & `moulti-1.6.0/src/moulti/widgets/abstractquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/abstractquestion/tui.py` & `moulti-1.6.0/src/moulti/widgets/abstractquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/abstractstep/cli.py` & `moulti-1.6.0/src/moulti/widgets/abstractstep/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from argparse import ArgumentParser, BooleanOptionalAction
+from moulti.helpers import bool_or_int
 
 def add_abstractstep_options(parser: ArgumentParser, none: bool = False) -> None:
 	"""Options common to step add (with actual default values) and step update (with None default values)."""
 	parser.add_argument('--title', type=str, default=None, help='step title, always visible')
 	parser.add_argument('--top-text', '-tt', type=str, default=None if none else '', help='line of text displayed above the content')
 	parser.add_argument('--bottom-text', '-bt', type=str, default=None if none else '', help='line of text displayed below the content')
 	parser.add_argument('--classes', '-c', type=str, default=None if none else 'standard', help='step class (color): standard, error, warning, success')
 	parser.add_argument('--collapsed', action=BooleanOptionalAction, default=None if none else False, help='whether to collapse the step')
+	parser.add_argument('--scroll-on-activity', type=bool_or_int, default=None if none else False, help='whether to scroll to this step upon activity', metavar='{true,false,...,-2,-1,0,1,2,...}')
```

### Comparing `moulti-1.5.1/src/moulti/widgets/abstractstep/tui.py` & `moulti-1.6.0/src/moulti/widgets/abstractstep/tui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 import json
+from operator import attrgetter
 from typing import Any, Callable
 from pyperclip import copy # type: ignore
 from rich.errors import MarkupError
 from textual.app import ComposeResult
 from textual.events import Click
+from textual.message import Message
 from textual.widgets import Static, Collapsible
 
 class AbstractStep(Static):
 	"""
 	This is the base class for all components end users may wish to add to Moulti.
 	"""
+
+	class StepActivity(Message):
+		def __init__(self, step: 'AbstractStep', *args: Any, **kwargs: Any):
+			self.step = step
+			super().__init__(*args, **kwargs)
+
 	def __init__(self, id: str, **kwargs: Any): # pylint: disable=redefined-builtin
 		self.collapsible = Collapsible(title=id)
 		self.top_label = Static('', classes='top_text')
 		self.bottom_label = Static('', classes='bottom_text')
 
 		self.top_text = ''
 		self.bottom_text = ''
 
 		# This attribute is meant to prevent deletion of a step while content
 		# is being appended to it:
 		self.prevent_deletion = 0
 
+		self.scroll_on_activity: bool|int = False
+
 		self.check_properties(kwargs)
 		self.init_kwargs = kwargs
 
 		step_classes = str(kwargs.get('classes', ''))
 		super().__init__(id='step_' + id, classes=step_classes)
 
 	def subcompose(self) -> ComposeResult:
@@ -51,15 +61,15 @@
 		self_id = str(self.id)
 		if '_' not in self_id:
 			return self_id
 		return self_id.split('_', 1)[1]
 
 	def index(self) -> int:
 		if self.parent is not None:
-			return self.parent.children.index(self) + 1
+			return sorted(self.parent.children, key=attrgetter('sort_order')).index(self) + 1
 		return -1
 
 	def check_markup(self, value: str|int|bool) -> None:
 		value = str(value)
 		text = self.render_str(value)
 		# Extra check to work around https://github.com/Textualize/textual/issues/4248:
 		for span in text.spans:
@@ -85,23 +95,30 @@
 			self.top_text = str(kwargs['top_text'])
 			self.top_label.update(self.top_text)
 		self.top_label.styles.display = 'block' if self.top_text else 'none'
 		if 'bottom_text' in kwargs:
 			self.bottom_text = str(kwargs['bottom_text'])
 			self.bottom_label.update(self.bottom_text)
 		self.bottom_label.styles.display = 'block' if self.bottom_text else 'none'
+		if 'scroll_on_activity' in kwargs:
+			scroll_on_activity = kwargs['scroll_on_activity']
+			if isinstance(scroll_on_activity, int):
+				self.scroll_on_activity = scroll_on_activity
+			else:
+				self.scroll_on_activity = bool(scroll_on_activity)
 
 	def export_properties(self) -> dict[str, Any]:
 		prop: dict[str, Any] = {}
 		prop['id'] = self.title_from_id()
 		prop['classes'] = ' '.join(self.classes)
 		prop['title'] = self.collapsible.title
 		prop['collapsed'] = self.collapsible.collapsed
 		prop['top_text'] = self.top_text
 		prop['bottom_text'] = self.bottom_text
+		prop['scroll_on_activity'] = self.scroll_on_activity
 		return prop
 
 	def save(self, opener: Callable[[str, int], int], filename: str, extra_properties: dict[str, Any]) -> None:
 		properties = {**extra_properties, **self.export_properties()}
 		with open(filename + '.properties.json', 'w', encoding='utf-8', opener=opener) as properties_filedesc:
 			json.dump(properties, properties_filedesc, indent=4)
 			properties_filedesc.write('\n')
@@ -125,14 +142,18 @@
 				if result:
 					copy(data)
 			except Exception as exc:
 				result, explanation = False, str(exc)
 			self.notify_copy_to_clipboard(result, explanation)
 		return wrapper
 
+	def activity(self) -> None:
+		msg = AbstractStep.StepActivity(self)
+		self.call_after_refresh(self.post_message, msg)
+
 	DEFAULT_COLORS = """
 	$step_default: $primary;
 	$step_success: ansi_bright_green;
 	$step_warning: orange;
 	$step_error: tomato;
 	"""
 	DEFAULT_CSS = DEFAULT_COLORS + """
```

### Comparing `moulti-1.5.1/src/moulti/widgets/buttonquestion/cli.py` & `moulti-1.6.0/src/moulti/widgets/buttonquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/buttonquestion/tui.py` & `moulti-1.6.0/src/moulti/widgets/buttonquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/inputquestion/cli.py` & `moulti-1.6.0/src/moulti/widgets/inputquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/inputquestion/tui.py` & `moulti-1.6.0/src/moulti/widgets/inputquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/moulticonsole.py` & `moulti-1.6.0/src/moulti/widgets/moulticonsole.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/moultilog.py` & `moulti-1.6.0/src/moulti/widgets/moultilog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/quitdialog.py` & `moulti-1.6.0/src/moulti/widgets/quitdialog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/step/cli.py` & `moulti-1.6.0/src/moulti/widgets/step/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti/widgets/step/tui.py` & `moulti-1.6.0/src/moulti/widgets/step/tui.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 			# Convert text and an extra character from ANSI to Rich Text
 			text_to_write = Text.from_ansi(text + '_')
 			# The extra character reflects the color the next line should inherit:
 			self.color = Step.last_character_color(text_to_write)
 			# Strip the extra character:
 			text_to_write.right_crop(1)
 		self.log_widget.write(text_to_write)
+		self.activity()
 
 	@classmethod
 	def last_character_color(cls, text: Text) -> str:
 		# If the last span (if any) covers the last character...
 		if text.spans and text.spans[-1].end == len(text):
 			# ... return the ANSI escape code for its color:
 			style = text.spans[-1].style
```

### Comparing `moulti-1.5.1/src/moulti/widgets/tui.py` & `moulti-1.6.0/src/moulti/widgets/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.5.1/src/moulti.egg-info/PKG-INFO` & `moulti-1.6.0/src/moulti.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.5.1
+Version: 1.6.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible
 Classifier: Environment :: Console :: Curses
@@ -27,14 +27,16 @@
 Moulti changes the way your shell scripts (bash, zsh, etc.) display their output in your terminal.
 Moulti enables you to assign the numerous lines emitted by your scripts to "steps", i.e. visual, collapsible blocks featuring their own title and color.
 
 Here is how [upgrading a Debian system](examples/upgrade-system.bash) looks like with Moulti:
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
+Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
+
 Moulti is a tool meant for people who write and execute shell scripts.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 ## How?
 
 Synopsis:
 
@@ -49,18 +51,21 @@
 
 As shown in the demo, Moulti enables user interactions through **questions**:
 
 ![Moulti input question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-input-question.png?20240218)
 
 ![Moulti button question](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-button-question.png?20240218)
 
-Moulti also features a **progress bar**: [documentation](Documentation.md#progress-bar)
+Moulti also features:
+- a **progress bar**: [documentation](Documentation.md#progress-bar)
+- programmatic scrolling: [documentation](Documentation.md#programmatically-scrolling-through-steps)
 
 When it comes to look and feel, Moulti can be customised:
 
+- through `moulti set`: define whether Moulti steps flow up or down: [documentation](Documentation.md#multiple-ways-to-display-steps)
 - through [Textual CSS (TCSS)](https://textual.textualize.io/guide/CSS/): [documentation](Documentation.md#how-to-define-my-own-step-classes-)
 - through ANSI themes: [documentation](Documentation.md#appearance-look-and-feel)
 
 ## Implementation
 
 Moulti is written in Python and leverages [Textual](https://textual.textualize.io/), along with [Pyperclip](https://pypi.org/project/pyperclip/) and [argcomplete](https://kislyuk.github.io/argcomplete/).
```

### Comparing `moulti-1.5.1/src/moulti.egg-info/SOURCES.txt` & `moulti-1.6.0/src/moulti.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/moulti.egg-info/requires.txt
 src/moulti.egg-info/top_level.txt
 src/moulti/widgets/__init__.py
 src/moulti/widgets/cli.py
 src/moulti/widgets/moulticonsole.py
 src/moulti/widgets/moultilog.py
 src/moulti/widgets/quitdialog.py
+src/moulti/widgets/stepcontainer.py
 src/moulti/widgets/tui.py
 src/moulti/widgets/vertscroll.py
 src/moulti/widgets/abstractquestion/__init__.py
 src/moulti/widgets/abstractquestion/cli.py
 src/moulti/widgets/abstractquestion/tui.py
 src/moulti/widgets/abstractstep/__init__.py
 src/moulti/widgets/abstractstep/cli.py
```

