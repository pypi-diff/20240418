# Comparing `tmp/PyQtUIkit-2.7.1.tar.gz` & `tmp/PyQtUIkit-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.7.1.tar", last modified: Wed Apr 17 09:37:45 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.7.2.tar", last modified: Wed Apr 17 12:00:36 2024, max compression
```

## Comparing `PyQtUIkit-2.7.1.tar` & `PyQtUIkit-2.7.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.076212 PyQtUIkit-2.7.1/
--rw-rw-rw-   0        0        0     1090 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-17 09:37:45.076212 PyQtUIkit-2.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.044964 PyQtUIkit-2.7.1/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3325 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.044964 PyQtUIkit-2.7.1/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.044964 PyQtUIkit-2.7.1/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.060592 PyQtUIkit-2.7.1/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.060592 PyQtUIkit-2.7.1/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     3173 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1762 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/local.py
--rw-rw-rw-   0        0        0     1470 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.076212 PyQtUIkit-2.7.1/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1654 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7885 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2739 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11101 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     2280 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5174 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4336 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13972 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2370 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16164 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:37:45.044964 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2575 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 09:37:44.000000 PyQtUIkit-2.7.1/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 09:37:45.076212 PyQtUIkit-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-04-17 09:37:00.000000 PyQtUIkit-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.692237 PyQtUIkit-2.7.2/
+-rw-rw-rw-   0        0        0     1090 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-17 12:00:36.692237 PyQtUIkit-2.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.660533 PyQtUIkit-2.7.2/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3325 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.661054 PyQtUIkit-2.7.2/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.661054 PyQtUIkit-2.7.2/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.676580 PyQtUIkit-2.7.2/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.676580 PyQtUIkit-2.7.2/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     3173 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1828 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/local.py
+-rw-rw-rw-   0        0        0     1470 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.692237 PyQtUIkit-2.7.2/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1654 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7885 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2739 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11294 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     2280 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5174 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4948 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13972 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2370 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16743 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:36.661054 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2575 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 12:00:36.000000 PyQtUIkit-2.7.2/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:00:36.692237 PyQtUIkit-2.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-17 12:00:03.000000 PyQtUIkit-2.7.2/setup.py
```

### Comparing `PyQtUIkit-2.7.1/LICENSE` & `PyQtUIkit-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PKG-INFO` & `PyQtUIkit-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.1
+Version: 2.7.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/_icons.py` & `PyQtUIkit-2.7.2/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/_translate.py` & `PyQtUIkit-2.7.2/PyQtUIkit/_translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,23 +53,24 @@
             pass
         except AttributeError:
             pass
     if dst_local is None:
         dst_local = KitLocal(lang, translate(LANGUAGES[lang].capitalize(), lang), dict())
 
     print(f"Translating to {lang.capitalize()}...")
+    res = ["from PyQtUIkit.themes.local import KitLocal\n",
+           f"local = KitLocal('{lang}', '{dst_local.name}', {{"]
+    for key, item in src_local.items():
+        try:
+            res.append(f"    '{key}': \"{dst_local.get(key)}\",")
+        except Exception:
+            res.append(f"    '{key}': \"{translate(item, lang)}\",")
+    res.append("})\n")
     with open(f"{os.path.dirname(filename)}/{lang}.py", mode='w', encoding='utf-8') as f:
-        f.write(f"from PyQtUIkit.themes.local import KitLocal\n\n"
-                f"local = KitLocal('{lang}', '{dst_local.name}', {{\n")
-        for key, item in src_local.items():
-            try:
-                f.write(f"    '{key}': \"{dst_local.get(key)}\",\n")
-            except Exception:
-                f.write(f"    '{key}': \"{translate(item, lang)}\",\n")
-        f.write("})\n")
+        f.write('\n'.join(res))
 
 
 def main():
     _parser = argparse.ArgumentParser(prog="PyQtUIkit auto translator")
 
     _parser.add_argument('filename', help="Путь к файлу")
     _parser.add_argument('langs', nargs='*', help="Код(ы) языка(ов)")
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.7.2/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.7.2/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.7.2/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/core/font.py` & `PyQtUIkit-2.7.2/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.7.2/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.7.2/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.7.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/local.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,9 +59,12 @@
         return _KitLocalStringArray(other, *self.__args)
 
 
 class _KitLocalStringClass:
     def __getattr__(self, item):
         return _KitLocalString(item)
 
+    def get(self, item):
+        return _KitLocalString(item)
+
 
 KitLocalString = _KitLocalStringClass()
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.7.2/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/combo_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,14 +144,20 @@
         if self.__current is not None:
             self.setText(self.__widgets[self.__current].text)
             if self.__widgets[self.__current].icon is not None and self._tm and self._tm.active:
                 self.setIcon(self.__widgets[self.__current].icon.icon(self.main_palette.text))
         self.currentValueChanged.emit(self.currentValue())
         self.currentIndexChanged.emit(self.__current)
 
+    def setCurrentValue(self, value):
+        for i, item in enumerate(self.__widgets):
+            if item.value == value:
+                self.setCurrentIndex(i)
+                break
+
     def _show_menu(self):
         pos = QPoint(0, self.height() if self.type == 1 else self.height() // 2)
         self.__menu.open(self.mapToGlobal(pos), self.type)
 
     def _on_item_selected(self, item: KitComboBoxItem):
         self.setCurrentIndex(self.__widgets.index(item))
         self.__menu.close()
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/menu_bar.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitMenuBar(QMenuBar, _KitWidget):
     class Action(QAction):
         def __init__(self, name, icon, func=None, shortcut=None):
             super().__init__()
-            self.setText(name)
+            self._name = name
+            if isinstance(name, str):
+                self.setText(name)
             if shortcut:
                 self.setShortcut(shortcut)
             self._icon = icon
             self._func = func
             if self._func:
                 self.triggered.connect(self._func)
 
         def _apply_styles(self, tm, main_palette, *args):
             if self._icon:
                 self.setIcon(tm.icon(self._icon, main_palette.text))
+            if isinstance(self._name, str):
+                self.setText(self._name)
+            else:
+                self.setText(self._name.get(tm))
 
     class Menu(QMenu):
         def __init__(self, name, icon, *args):
             super().__init__()
-            self.setTitle(name)
+            self._name = name
             self._icon = icon
             self.setMinimumWidth(160)
             self._children = []
             for el in args:
                 if isinstance(el, QMenu):
                     self.addMenu(el)
                 elif isinstance(el, QAction):
@@ -45,14 +51,18 @@
         def clear(self) -> None:
             self._children.clear()
 
         def _apply_styles(self, tm, main_palette, border_palette, font):
             if self._icon:
                 self.setIcon(tm.icon(self._icon, main_palette.text))
             self.setFont(font)
+            if isinstance(self._name, str):
+                self.setTitle(self._name)
+            else:
+                self.setTitle(self._name.get(tm))
             self.setStyleSheet(f"""
 QMenu {{
     color: {main_palette.text};
     background-color: {main_palette.main};
     border: 1px solid {border_palette.main};
     border-radius: 6px;
     spacing: 4px;
@@ -128,7 +138,12 @@
 }}
 QMenuBar::item:pressed {{
     background: {self.main_palette.selected};
 }}""")
         for el in self._children:
             if hasattr(el, '_apply_styles'):
                 el._apply_styles(self._tm, self.main_palette, self.border_palette, self.font.get(self.font_size))
+
+    def _apply_lang(self):
+        for el in self._children:
+            if hasattr(el, '_apply_styles'):
+                el._apply_styles(self._tm, self.main_palette, self.border_palette, self.font.get(self.font_size))
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.7.2/PyQtUIkit/widgets/tree_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,28 @@
     PaletteProperty, FontProperty
 from PyQtUIkit.widgets.dialog import KitDialog
 from PyQtUIkit.widgets.layout import KitVBoxLayout, KitHBoxLayout
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.button import KitLayoutButton, KitIconButton
+from PyQtUIkit.widgets.checkbox import KitCheckBox
 
 
 class KitTreeWidgetItem(KitVBoxLayout):
     name = StringProperty('name', '')
     radius = IntProperty('radius', 4)
     icon = IconProperty('icon')
     text_palette = PaletteProperty('text_palette', 'Main')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     always_expandable = BoolProperty('always_expandable', False)
+    checkable = BoolProperty('checkable', False)
+
+    stateEdited = pyqtSignal(bool)
 
     def __init__(self, name='', icon=''):
         super().__init__()
         self._name = name
         self._icon = icon
         self._main_palette = 'Main'
         self._text_palette = 'Main'
@@ -62,14 +66,18 @@
         self.__arrow_down = KitIconButton('line-chevron-down')
         self.__arrow_down.setFixedSize(20, 20)
         self.__arrow_down.border = 0
         self.__arrow_down.hide()
         self.__arrow_down.clicked.connect(self.collapse)
         self.__button.addWidget(self.__arrow_down)
 
+        self.__checkbox = KitCheckBox()
+        self.__checkbox.on_state_edited = self.stateEdited.emit
+        self.__button.addWidget(self.__checkbox)
+
         self.__icon_widget = KitIconWidget()
         self.__button.addWidget(self.__icon_widget)
 
         self.__label = KitLabel(self._name)
         self.__button.addWidget(self.__label)
 
         self.__layout = KitVBoxLayout()
@@ -231,17 +239,25 @@
             for i, el in enumerate(self.__children):
                 res, h = el._find_by_pos(pos - QPoint(0, height))
                 if res:
                     return res, 0
                 height += h
         return None, height
 
+    @property
+    def checked(self):
+        return self.checkable and self.__checkbox.state
+
+    def setChecked(self, state):
+        self.__checkbox.state = state
+
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
+        self.__checkbox.setHidden(not self.checkable)
         for el in self.__children:
             el._height = self._height
             el.main_palette = self._main_palette
             el.text_palette = self._text_palette
         self.__button.setFixedHeight(self._height)
         self.__icon_widget.setFixedSize(self._height - 4, self._height - 4)
         self.__icon_widget._icon = self._icon
@@ -431,14 +447,17 @@
     def keyReleaseEvent(self, a0) -> None:
         super().keyReleaseEvent(a0)
         if a0.key() == Qt.Key.Key_Shift:
             self.__shift = False
         elif a0.key() == Qt.Key.Key_Control:
             self.__control = False
 
+    def clear(self):
+        self.__tree.clear()
+
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__tree._set_tm(tm)
 
     def _apply_theme(self):
         self.__tree.main_palette = self._main_palette
         self.__tree._main_palette = self._main_palette
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.7.2/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.1
+Version: 2.7.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.1/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.7.2/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.1/setup.py` & `PyQtUIkit-2.7.2/setup.py`

 * *Files identical despite different names*

