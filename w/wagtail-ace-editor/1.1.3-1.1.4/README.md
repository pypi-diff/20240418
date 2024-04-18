# Comparing `tmp/wagtail_ace_editor-1.1.3.tar.gz` & `tmp/wagtail_ace_editor-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_ace_editor-1.1.3.tar", last modified: Thu Apr 18 07:58:37 2024, max compression
+gzip compressed data, was "wagtail_ace_editor-1.1.4.tar", last modified: Thu Apr 18 08:00:53 2024, max compression
```

## Comparing `wagtail_ace_editor-1.1.3.tar` & `wagtail_ace_editor-1.1.4.tar`

### file list

```diff
@@ -1,527 +1,528 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:37.249942 wagtail_ace_editor-1.1.3/
--rw-rw-rw-   0        0        0    18429 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      282 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5371 2024-04-18 07:58:37.249942 wagtail_ace_editor-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4311 2024-02-19 22:06:30.000000 wagtail_ace_editor-1.1.3/README.md
--rw-rw-rw-   0        0        0       90 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1046 2024-04-18 07:58:37.262303 wagtail_ace_editor-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.085073 wagtail_ace_editor-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:25:26.000000 wagtail_ace_editor-1.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.093080 wagtail_ace_editor-1.1.3/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:25:26.000000 wagtail_ace_editor-1.1.3/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.107357 wagtail_ace_editor-1.1.3/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:28:25.000000 wagtail_ace_editor-1.1.3/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.108358 wagtail_ace_editor-1.1.3/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:28:25.000000 wagtail_ace_editor-1.1.3/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     2987 2024-03-16 15:01:57.000000 wagtail_ace_editor-1.1.3/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.3/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.156956 wagtail_ace_editor-1.1.3/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.3/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.3/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3523 2024-02-22 09:19:47.000000 wagtail_ace_editor-1.1.3/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.3/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.3/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.225496 wagtail_ace_editor-1.1.3/wagtail_ace_editor/
--rw-rw-rw-   0        0        0        0 2024-02-22 08:50:40.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/__init__.py
--rw-rw-rw-   0        0        0      172 2024-02-11 15:58:27.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/apps.py
--rw-rw-rw-   0        0        0     1932 2024-04-18 07:56:10.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/blocks.py
--rw-rw-rw-   0        0        0      990 2024-02-19 22:38:01.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/clean.py
--rw-rw-rw-   0        0        0     2742 2024-03-16 14:54:38.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.250854 wagtail_ace_editor-1.1.3/wagtail_ace_editor/migrations/
--rw-rw-rw-   0        0        0        0 2024-02-11 15:58:27.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.251863 wagtail_ace_editor-1.1.3/wagtail_ace_editor/migrations/__pycache__/
--rw-rw-rw-   0        0        0      216 2024-02-11 16:56:21.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.069646 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.069646 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.254811 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/css/
--rw-rw-rw-   0        0        0      350 2024-02-11 19:23:54.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-iframe.css
--rw-rw-rw-   0        0        0     1289 2024-02-11 19:28:54.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-widget.css
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:34.523126 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/
--rw-rw-rw-   0        0        0     1720 2024-02-11 18:47:49.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-controller.js
--rw-rw-rw-   0        0        0      600 2023-12-17 07:07:49.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-telepath.js
--rw-rw-rw-   0        0        0     5131 2024-02-11 19:05:28.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor.js
--rw-rw-rw-   0        0        0   444405 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace.js
--rw-rw-rw-   0        0        0     4502 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-beautify.js
--rw-rw-rw-   0        0        0     4166 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-code_lens.js
--rw-rw-rw-   0        0        0    12723 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-command_bar.js
--rw-rw-rw-   0        0        0     4093 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-elastic_tabstops_lite.js
--rw-rw-rw-   0        0        0    25711 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-emmet.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-error_marker.js
--rw-rw-rw-   0        0        0     1973 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-hardwrap.js
--rw-rw-rw-   0        0        0    76110 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-inline_autocomplete.js
--rw-rw-rw-   0        0        0     4422 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-keybinding_menu.js
--rw-rw-rw-   0        0        0    55365 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-language_tools.js
--rw-rw-rw-   0        0        0     1221 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-linking.js
--rw-rw-rw-   0        0        0     5170 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-modelist.js
--rw-rw-rw-   0        0        0    16364 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-options.js
--rw-rw-rw-   0        0        0    65922 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-prompt.js
--rw-rw-rw-   0        0        0     2586 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-rtl.js
--rw-rw-rw-   0        0        0    13594 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-searchbox.js
--rw-rw-rw-   0        0        0    16917 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-settings_menu.js
--rw-rw-rw-   0        0        0     1125 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-simple_tokenizer.js
--rw-rw-rw-   0        0        0     1588 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-spellcheck.js
--rw-rw-rw-   0        0        0     3866 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-split.js
--rw-rw-rw-   0        0        0     4358 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-static_highlight.js
--rw-rw-rw-   0        0        0     1276 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-statusbar.js
--rw-rw-rw-   0        0        0     6555 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-textarea.js
--rw-rw-rw-   0        0        0     1850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-themelist.js
--rw-rw-rw-   0        0        0     3245 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-whitespace.js
--rw-rw-rw-   0        0        0    25047 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-emacs.js
--rw-rw-rw-   0        0        0     7874 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-sublime.js
--rw-rw-rw-   0        0        0   118883 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vim.js
--rw-rw-rw-   0        0        0     5734 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vscode.js
--rw-rw-rw-   0        0        0     6198 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abap.js
--rw-rw-rw-   0        0        0     5098 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abc.js
--rw-rw-rw-   0        0        0    20926 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-actionscript.js
--rw-rw-rw-   0        0        0     2623 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ada.js
--rw-rw-rw-   0        0        0     5390 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-alda.js
--rw-rw-rw-   0        0        0    14242 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apache_conf.js
--rw-rw-rw-   0        0        0     8645 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apex.js
--rw-rw-rw-   0        0        0     5732 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-applescript.js
--rw-rw-rw-   0        0        0     4346 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-aql.js
--rw-rw-rw-   0        0        0     8479 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asciidoc.js
--rw-rw-rw-   0        0        0     8957 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asl.js
--rw-rw-rw-   0        0        0     4825 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_arm32.js
--rw-rw-rw-   0        0        0     9296 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_x86.js
--rw-rw-rw-   0        0        0    64708 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-astro.js
--rw-rw-rw-   0        0        0    63985 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-autohotkey.js
--rw-rw-rw-   0        0        0     5187 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-batchfile.js
--rw-rw-rw-   0        0        0     5230 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-bibtex.js
--rw-rw-rw-   0        0        0     4398 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c9search.js
--rw-rw-rw-   0        0        0    12181 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c_cpp.js
--rw-rw-rw-   0        0        0     3404 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cirru.js
--rw-rw-rw-   0        0        0     9017 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-clojure.js
--rw-rw-rw-   0        0        0     2634 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cobol.js
--rw-rw-rw-   0        0        0     7850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coffee.js
--rw-rw-rw-   0        0        0    64687 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coldfusion.js
--rw-rw-rw-   0        0        0    10342 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-crystal.js
--rw-rw-rw-   0        0        0     9120 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csharp.js
--rw-rw-rw-   0        0        0    76639 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_document.js
--rw-rw-rw-   0        0        0    42033 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_orchestra.js
--rw-rw-rw-   0        0        0     7960 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_score.js
--rw-rw-rw-   0        0        0     1568 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csp.js
--rw-rw-rw-   0        0        0    20931 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-css.js
--rw-rw-rw-   0        0        0    63176 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-curly.js
--rw-rw-rw-   0        0        0     1639 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cuttlefish.js
--rw-rw-rw-   0        0        0     9272 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-d.js
--rw-rw-rw-   0        0        0    15664 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dart.js
--rw-rw-rw-   0        0        0     2740 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-diff.js
--rw-rw-rw-   0        0        0    63520 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-django.js
--rw-rw-rw-   0        0        0     8538 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dockerfile.js
--rw-rw-rw-   0        0        0     7890 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dot.js
--rw-rw-rw-   0        0        0    12869 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-drools.js
--rw-rw-rw-   0        0        0     3190 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-edifact.js
--rw-rw-rw-   0        0        0     3166 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-eiffel.js
--rw-rw-rw-   0        0        0    82283 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ejs.js
--rw-rw-rw-   0        0        0    16143 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elixir.js
--rw-rw-rw-   0        0        0     5258 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elm.js
--rw-rw-rw-   0        0        0    30080 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-erlang.js
--rw-rw-rw-   0        0        0     3311 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-flix.js
--rw-rw-rw-   0        0        0     7316 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-forth.js
--rw-rw-rw-   0        0        0     8757 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fortran.js
--rw-rw-rw-   0        0        0     5765 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsharp.js
--rw-rw-rw-   0        0        0     5037 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsl.js
--rw-rw-rw-   0        0        0    36155 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ftl.js
--rw-rw-rw-   0        0        0     1785 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gcode.js
--rw-rw-rw-   0        0        0     2688 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gherkin.js
--rw-rw-rw-   0        0        0     1224 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gitignore.js
--rw-rw-rw-   0        0        0    14253 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-glsl.js
--rw-rw-rw-   0        0        0    31398 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gobstones.js
--rw-rw-rw-   0        0        0     7183 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-golang.js
--rw-rw-rw-   0        0        0     3815 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-graphqlschema.js
--rw-rw-rw-   0        0        0    26873 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-groovy.js
--rw-rw-rw-   0        0        0    49570 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haml.js
--rw-rw-rw-   0        0        0    64037 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-handlebars.js
--rw-rw-rw-   0        0        0    11851 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell.js
--rw-rw-rw-   0        0        0     2607 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell_cabal.js
--rw-rw-rw-   0        0        0     6801 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haxe.js
--rw-rw-rw-   0        0        0     6297 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-hjson.js
--rw-rw-rw-   0        0        0    62164 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html.js
--rw-rw-rw-   0        0        0    79426 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_elixir.js
--rw-rw-rw-   0        0        0    82614 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_ruby.js
--rw-rw-rw-   0        0        0     3025 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ini.js
--rw-rw-rw-   0        0        0     5666 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-io.js
--rw-rw-rw-   0        0        0     8067 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ion.js
--rw-rw-rw-   0        0        0     6033 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jack.js
--rw-rw-rw-   0        0        0    50973 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jade.js
--rw-rw-rw-   0        0        0    29040 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-java.js
--rw-rw-rw-   0        0        0    21785 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-javascript.js
--rw-rw-rw-   0        0        0     5109 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jexl.js
--rw-rw-rw-   0        0        0     5548 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json.js
--rw-rw-rw-   0        0        0     6193 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json5.js
--rw-rw-rw-   0        0        0   233671 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsoniq.js
--rw-rw-rw-   0        0        0    42635 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsp.js
--rw-rw-rw-   0        0        0     6220 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jssm.js
--rw-rw-rw-   0        0        0    22127 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsx.js
--rw-rw-rw-   0        0        0     7866 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-julia.js
--rw-rw-rw-   0        0        0     8389 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-kotlin.js
--rw-rw-rw-   0        0        0     5360 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latex.js
--rw-rw-rw-   0        0        0    65892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latte.js
--rw-rw-rw-   0        0        0    22922 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-less.js
--rw-rw-rw-   0        0        0    69494 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-liquid.js
--rw-rw-rw-   0        0        0     2281 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lisp.js
--rw-rw-rw-   0        0        0     5399 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-livescript.js
--rw-rw-rw-   0        0        0     6045 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logiql.js
--rw-rw-rw-   0        0        0    10989 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logtalk.js
--rw-rw-rw-   0        0        0    26892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lsl.js
--rw-rw-rw-   0        0        0     7905 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lua.js
--rw-rw-rw-   0        0        0    70900 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-luapage.js
--rw-rw-rw-   0        0        0     2763 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lucene.js
--rw-rw-rw-   0        0        0     6989 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-makefile.js
--rw-rw-rw-   0        0        0    73818 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-markdown.js
--rw-rw-rw-   0        0        0    45777 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mask.js
--rw-rw-rw-   0        0        0    20889 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-matlab.js
--rw-rw-rw-   0        0        0     5246 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-maze.js
--rw-rw-rw-   0        0        0     9691 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mediawiki.js
--rw-rw-rw-   0        0        0    25211 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mel.js
--rw-rw-rw-   0        0        0     5625 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mips.js
--rw-rw-rw-   0        0        0     3164 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mixal.js
--rw-rw-rw-   0        0        0     7032 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mushcode.js
--rw-rw-rw-   0        0        0     8218 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mysql.js
--rw-rw-rw-   0        0        0    10953 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nasal.js
--rw-rw-rw-   0        0        0    16214 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nginx.js
--rw-rw-rw-   0        0        0     6937 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nim.js
--rw-rw-rw-   0        0        0    14453 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nix.js
--rw-rw-rw-   0        0        0    10771 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nsis.js
--rw-rw-rw-   0        0        0    65602 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nunjucks.js
--rw-rw-rw-   0        0        0    68433 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-objectivec.js
--rw-rw-rw-   0        0        0    15910 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ocaml.js
--rw-rw-rw-   0        0        0     8326 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-odin.js
--rw-rw-rw-   0        0        0    13077 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-partiql.js
--rw-rw-rw-   0        0        0     4577 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pascal.js
--rw-rw-rw-   0        0        0     7743 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-perl.js
--rw-rw-rw-   0        0        0    63518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pgsql.js
--rw-rw-rw-   0        0        0   505292 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php.js
--rw-rw-rw-   0        0        0   509834 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php_laravel_blade.js
--rw-rw-rw-   0        0        0     6637 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pig.js
--rw-rw-rw-   0        0        0      836 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plain_text.js
--rw-rw-rw-   0        0        0     6198 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plsql.js
--rw-rw-rw-   0        0        0    84661 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-powershell.js
--rw-rw-rw-   0        0        0    10718 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-praat.js
--rw-rw-rw-   0        0        0     8573 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prisma.js
--rw-rw-rw-   0        0        0     8695 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prolog.js
--rw-rw-rw-   0        0        0     1425 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-properties.js
--rw-rw-rw-   0        0        0    13875 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-protobuf.js
--rw-rw-rw-   0        0        0     6017 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prql.js
--rw-rw-rw-   0        0        0     7373 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-puppet.js
--rw-rw-rw-   0        0        0     8294 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-python.js
--rw-rw-rw-   0        0        0    16414 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-qml.js
--rw-rw-rw-   0        0        0     5499 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-r.js
--rw-rw-rw-   0        0        0    17881 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-raku.js
--rw-rw-rw-   0        0        0    69959 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-razor.js
--rw-rw-rw-   0        0        0     5004 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rdoc.js
--rw-rw-rw-   0        0        0    12924 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-red.js
--rw-rw-rw-   0        0        0     8368 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-redshift.js
--rw-rw-rw-   0        0        0    67214 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rhtml.js
--rw-rw-rw-   0        0        0     4408 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-robot.js
--rw-rw-rw-   0        0        0     3381 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rst.js
--rw-rw-rw-   0        0        0    19951 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ruby.js
--rw-rw-rw-   0        0        0     8733 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rust.js
--rw-rw-rw-   0        0        0     7022 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sac.js
--rw-rw-rw-   0        0        0    16065 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sass.js
--rw-rw-rw-   0        0        0     6781 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scad.js
--rw-rw-rw-   0        0        0    27012 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scala.js
--rw-rw-rw-   0        0        0     3976 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scheme.js
--rw-rw-rw-   0        0        0     7485 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scrypt.js
--rw-rw-rw-   0        0        0    24109 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scss.js
--rw-rw-rw-   0        0        0     7501 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sh.js
--rw-rw-rw-   0        0        0    24930 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sjs.js
--rw-rw-rw-   0        0        0   113850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-slim.js
--rw-rw-rw-   0        0        0    65624 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smarty.js
--rw-rw-rw-   0        0        0     8959 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smithy.js
--rw-rw-rw-   0        0        0     4126 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-snippets.js
--rw-rw-rw-   0        0        0    70659 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-soy_template.js
--rw-rw-rw-   0        0        0     2625 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-space.js
--rw-rw-rw-   0        0        0     8183 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sparql.js
--rw-rw-rw-   0        0        0     5341 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sql.js
--rw-rw-rw-   0        0        0    16924 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sqlserver.js
--rw-rw-rw-   0        0        0    14831 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-stylus.js
--rw-rw-rw-   0        0        0    33722 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-svg.js
--rw-rw-rw-   0        0        0     7311 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-swift.js
--rw-rw-rw-   0        0        0     6516 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tcl.js
--rw-rw-rw-   0        0        0     7122 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-terraform.js
--rw-rw-rw-   0        0        0     3114 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tex.js
--rw-rw-rw-   0        0        0      328 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-text.js
--rw-rw-rw-   0        0        0     2448 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-textile.js
--rw-rw-rw-   0        0        0     2520 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-toml.js
--rw-rw-rw-   0        0        0    23807 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tsx.js
--rw-rw-rw-   0        0        0     5352 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-turtle.js
--rw-rw-rw-   0        0        0    65791 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-twig.js
--rw-rw-rw-   0        0        0    23506 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-typescript.js
--rw-rw-rw-   0        0        0    16781 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vala.js
--rw-rw-rw-   0        0        0    11995 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vbscript.js
--rw-rw-rw-   0        0        0    66939 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-velocity.js
--rw-rw-rw-   0        0        0     3223 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-verilog.js
--rw-rw-rw-   0        0        0     2518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vhdl.js
--rw-rw-rw-   0        0        0    64822 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-visualforce.js
--rw-rw-rw-   0        0        0    93195 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vue.js
--rw-rw-rw-   0        0        0    24740 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-wollok.js
--rw-rw-rw-   0        0        0    10202 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xml.js
--rw-rw-rw-   0        0        0   231054 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xquery.js
--rw-rw-rw-   0        0        0     6796 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-yaml.js
--rw-rw-rw-   0        0        0     9411 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zeek.js
--rw-rw-rw-   0        0        0    11929 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zig.js
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:37.243888 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abap.js
--rw-rw-rw-   0        0        0     1416 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abc.js
--rw-rw-rw-   0        0        0     3478 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/actionscript.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ada.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/alda.js
--rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/apache_conf.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/apex.js
--rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/applescript.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/aql.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/asciidoc.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/asl.js
--rw-rw-rw-   0        0        0      342 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/assembly_arm32.js
--rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/assembly_x86.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/astro.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/autohotkey.js
--rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/batchfile.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/bibtex.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c9search.js
--rw-rw-rw-   0        0        0     3140 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c_cpp.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cirru.js
--rw-rw-rw-   0        0        0     2525 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/clojure.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cobol.js
--rw-rw-rw-   0        0        0     2714 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coffee.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coldfusion.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/crystal.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csharp.js
--rw-rw-rw-   0        0        0      819 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_document.js
--rw-rw-rw-   0        0        0     1594 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_orchestra.js
--rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_score.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csp.js
--rw-rw-rw-   0        0        0    20119 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/css.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/curly.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cuttlefish.js
--rw-rw-rw-   0        0        0      329 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/d.js
--rw-rw-rw-   0        0        0     1792 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dart.js
--rw-rw-rw-   0        0        0     1024 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/diff.js
--rw-rw-rw-   0        0        0     4481 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/django.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dockerfile.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dot.js
--rw-rw-rw-   0        0        0      851 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/drools.js
--rw-rw-rw-   0        0        0     4802 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/edifact.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/eiffel.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ejs.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/elixir.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/elm.js
--rw-rw-rw-   0        0        0     4055 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/erlang.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/flix.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/forth.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fortran.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsharp.js
--rw-rw-rw-   0        0        0      814 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsl.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ftl.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gcode.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gherkin.js
--rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gitignore.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/glsl.js
--rw-rw-rw-   0        0        0    39601 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gobstones.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/golang.js
--rw-rw-rw-   0        0        0     1171 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/graphqlschema.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/groovy.js
--rw-rw-rw-   0        0        0      921 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haml.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/handlebars.js
--rw-rw-rw-   0        0        0     2460 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell.js
--rw-rw-rw-   0        0        0      341 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell_cabal.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haxe.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/hjson.js
--rw-rw-rw-   0        0        0    19629 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html.js
--rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html_elixir.js
--rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html_ruby.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ini.js
--rw-rw-rw-   0        0        0     1545 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/io.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ion.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jack.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jade.js
--rw-rw-rw-   0        0        0     4795 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/java.js
--rw-rw-rw-   0        0        0     4337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/javascript.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jexl.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/json.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/json5.js
--rw-rw-rw-   0        0        0     2197 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsoniq.js
--rw-rw-rw-   0        0        0     3247 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsp.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jssm.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsx.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/julia.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/kotlin.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/latex.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/latte.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/less.js
--rw-rw-rw-   0        0        0    20003 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/liquid.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lisp.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/livescript.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/logiql.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/logtalk.js
--rw-rw-rw-   0        0        0    35892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lsl.js
--rw-rw-rw-   0        0        0      977 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lua.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/luapage.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lucene.js
--rw-rw-rw-   0        0        0      687 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/makefile.js
--rw-rw-rw-   0        0        0     2462 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/markdown.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mask.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/matlab.js
--rw-rw-rw-   0        0        0      743 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/maze.js
--rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mediawiki.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mel.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mips.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mixal.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mushcode.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mysql.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nasal.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nginx.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nim.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nix.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nsis.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nunjucks.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/objectivec.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ocaml.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/odin.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/partiql.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pascal.js
--rw-rw-rw-   0        0        0     5986 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/perl.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pgsql.js
--rw-rw-rw-   0        0        0     7422 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php.js
--rw-rw-rw-   0        0        0      345 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php_laravel_blade.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pig.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/plain_text.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/plsql.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/powershell.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/praat.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prisma.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prolog.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/properties.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/protobuf.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prql.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/puppet.js
--rw-rw-rw-   0        0        0     4153 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/python.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/qml.js
--rw-rw-rw-   0        0        0     3091 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/r.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/raku.js
--rw-rw-rw-   0        0        0      641 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/razor.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rdoc.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/red.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/redshift.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rhtml.js
--rw-rw-rw-   0        0        0     2072 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/robot.js
--rw-rw-rw-   0        0        0      911 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rst.js
--rw-rw-rw-   0        0        0    21752 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ruby.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rust.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sac.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sass.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scad.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scala.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scheme.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scrypt.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scss.js
--rw-rw-rw-   0        0        0     2518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sh.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sjs.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/slim.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/smarty.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/smithy.js
--rw-rw-rw-   0        0        0      786 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/snippets.js
--rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/soy_template.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/space.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sparql.js
--rw-rw-rw-   0        0        0     1411 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sql.js
--rw-rw-rw-   0        0        0     2632 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sqlserver.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/stylus.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/svg.js
--rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/swift.js
--rw-rw-rw-   0        0        0     2159 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tcl.js
--rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/terraform.js
--rw-rw-rw-   0        0        0     4105 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tex.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/text.js
--rw-rw-rw-   0        0        0     1025 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/textile.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/toml.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tsx.js
--rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/turtle.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/twig.js
--rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/typescript.js
--rw-rw-rw-   0        0        0     3455 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vala.js
--rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vbscript.js
--rw-rw-rw-   0        0        0     1140 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/velocity.js
--rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/verilog.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vhdl.js
--rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/visualforce.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vue.js
--rw-rw-rw-   0        0        0     1744 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/wollok.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xml.js
--rw-rw-rw-   0        0        0     2197 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xquery.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/yaml.js
--rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/zeek.js
--rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/zig.js
--rw-rw-rw-   0        0        0    28712 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-ambiance.js
--rw-rw-rw-   0        0        0     3854 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chaos.js
--rw-rw-rw-   0        0        0     3872 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chrome.js
--rw-rw-rw-   0        0        0     4176 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_day.js
--rw-rw-rw-   0        0        0     4285 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night.js
--rw-rw-rw-   0        0        0     4306 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night_low_color.js
--rw-rw-rw-   0        0        0     5328 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor.js
--rw-rw-rw-   0        0        0     5876 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor_dark.js
--rw-rw-rw-   0        0        0     3126 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds.js
--rw-rw-rw-   0        0        0     3427 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds_midnight.js
--rw-rw-rw-   0        0        0     3359 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cobalt.js
--rw-rw-rw-   0        0        0     3985 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-crimson_editor.js
--rw-rw-rw-   0        0        0     3323 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dawn.js
--rw-rw-rw-   0        0        0     4821 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dracula.js
--rw-rw-rw-   0        0        0     4384 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dreamweaver.js
--rw-rw-rw-   0        0        0     3185 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-eclipse.js
--rw-rw-rw-   0        0        0     3516 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github.js
--rw-rw-rw-   0        0        0     3807 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github_dark.js
--rw-rw-rw-   0        0        0     3364 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gob.js
--rw-rw-rw-   0        0        0     2580 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox.js
--rw-rw-rw-   0        0        0     4060 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_dark_hard.js
--rw-rw-rw-   0        0        0     4412 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_light_hard.js
--rw-rw-rw-   0        0        0     3232 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-idle_fingers.js
--rw-rw-rw-   0        0        0     7616 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-iplastic.js
--rw-rw-rw-   0        0        0     4572 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-katzenmilch.js
--rw-rw-rw-   0        0        0     3286 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kr_theme.js
--rw-rw-rw-   0        0        0     3293 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kuroir.js
--rw-rw-rw-   0        0        0     3193 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore.js
--rw-rw-rw-   0        0        0     3432 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore_soft.js
--rw-rw-rw-   0        0        0     3820 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-mono_industrial.js
--rw-rw-rw-   0        0        0     3354 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-monokai.js
--rw-rw-rw-   0        0        0     2914 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-nord_dark.js
--rw-rw-rw-   0        0        0     3852 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-one_dark.js
--rw-rw-rw-   0        0        0     3667 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-pastel_on_dark.js
--rw-rw-rw-   0        0        0     3270 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_dark.js
--rw-rw-rw-   0        0        0     3434 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_light.js
--rw-rw-rw-   0        0        0     4196 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-sqlserver.js
--rw-rw-rw-   0        0        0     3923 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-terminal.js
--rw-rw-rw-   0        0        0      615 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-textmate.js
--rw-rw-rw-   0        0        0     3641 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow.js
--rw-rw-rw-   0        0        0     3836 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night.js
--rw-rw-rw-   0        0        0     4064 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_blue.js
--rw-rw-rw-   0        0        0     4593 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_bright.js
--rw-rw-rw-   0        0        0     4282 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_eighties.js
--rw-rw-rw-   0        0        0     3469 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-twilight.js
--rw-rw-rw-   0        0        0     3173 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-vibrant_ink.js
--rw-rw-rw-   0        0        0     3035 2024-02-11 16:53:43.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-wagtail.js
--rw-rw-rw-   0        0        0     3031 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-xcode.js
--rw-rw-rw-   0        0        0    21987 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-base.js
--rw-rw-rw-   0        0        0   323433 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-coffee.js
--rw-rw-rw-   0        0        0   151082 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-css.js
--rw-rw-rw-   0        0        0   208882 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-html.js
--rw-rw-rw-   0        0        0   514300 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-javascript.js
--rw-rw-rw-   0        0        0    24346 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-json.js
--rw-rw-rw-   0        0        0    48226 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-lua.js
--rw-rw-rw-   0        0        0    78734 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-php.js
--rw-rw-rw-   0        0        0    46914 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xml.js
--rw-rw-rw-   0        0        0  1624915 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xquery.js
--rw-rw-rw-   0        0        0    76731 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-yaml.js
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:24.071114 wagtail_ace_editor-1.1.3/wagtail_ace_editor/templates/
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:37.246796 wagtail_ace_editor-1.1.3/wagtail_ace_editor/templates/wagtail_ace_editor/
--rw-rw-rw-   0        0        0      888 2024-02-11 17:47:26.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/templates/wagtail_ace_editor/ace_editor.html
--rw-rw-rw-   0        0        0     2203 2024-02-19 21:47:41.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/util.py
--rw-rw-rw-   0        0        0      330 2024-02-11 17:27:32.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/wagtail_hooks.py
--rw-rw-rw-   0        0        0     2814 2024-03-16 14:35:46.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:58:37.247810 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/
--rw-rw-rw-   0        0        0     5371 2024-04-18 07:58:23.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    32108 2024-04-18 07:58:23.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:58:23.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-18 07:58:23.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-18 07:58:23.000000 wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.851687 wagtail_ace_editor-1.1.4/
+-rw-rw-rw-   0        0        0    18429 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      282 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5371 2024-04-18 08:00:53.851687 wagtail_ace_editor-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4311 2024-02-19 22:06:30.000000 wagtail_ace_editor-1.1.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1046 2024-04-18 08:00:53.865689 wagtail_ace_editor-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-02-11 20:18:05.000000 wagtail_ace_editor-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.409983 wagtail_ace_editor-1.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:25:26.000000 wagtail_ace_editor-1.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.410982 wagtail_ace_editor-1.1.4/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:25:26.000000 wagtail_ace_editor-1.1.4/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.411984 wagtail_ace_editor-1.1.4/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:28:25.000000 wagtail_ace_editor-1.1.4/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.412984 wagtail_ace_editor-1.1.4/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:28:25.000000 wagtail_ace_editor-1.1.4/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2987 2024-03-16 15:01:57.000000 wagtail_ace_editor-1.1.4/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.4/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.416046 wagtail_ace_editor-1.1.4/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.4/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.4/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3523 2024-02-22 09:19:47.000000 wagtail_ace_editor-1.1.4/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.4/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-02-22 08:27:45.000000 wagtail_ace_editor-1.1.4/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.422572 wagtail_ace_editor-1.1.4/wagtail_ace_editor/
+-rw-rw-rw-   0        0        0        0 2024-02-22 08:50:40.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-02-11 15:58:27.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/apps.py
+-rw-rw-rw-   0        0        0     1932 2024-04-18 07:56:10.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/blocks.py
+-rw-rw-rw-   0        0        0      990 2024-02-19 22:38:01.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/clean.py
+-rw-rw-rw-   0        0        0     2742 2024-03-16 14:54:38.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.453969 wagtail_ace_editor-1.1.4/wagtail_ace_editor/migrations/
+-rw-rw-rw-   0        0        0        0 2024-02-11 15:58:27.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.455522 wagtail_ace_editor-1.1.4/wagtail_ace_editor/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      216 2024-02-11 16:56:21.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.402978 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.403985 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.457534 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/css/
+-rw-rw-rw-   0        0        0      350 2024-02-11 19:23:54.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-iframe.css
+-rw-rw-rw-   0        0        0     1289 2024-02-11 19:28:54.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-widget.css
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.712473 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/
+-rw-rw-rw-   0        0        0     1512 2024-04-18 08:00:17.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/LICENSE
+-rw-rw-rw-   0        0        0     1720 2024-02-11 18:47:49.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-controller.js
+-rw-rw-rw-   0        0        0      600 2023-12-17 07:07:49.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-telepath.js
+-rw-rw-rw-   0        0        0     5131 2024-02-11 19:05:28.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor.js
+-rw-rw-rw-   0        0        0   444405 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace.js
+-rw-rw-rw-   0        0        0     4502 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-beautify.js
+-rw-rw-rw-   0        0        0     4166 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-code_lens.js
+-rw-rw-rw-   0        0        0    12723 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-command_bar.js
+-rw-rw-rw-   0        0        0     4093 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-elastic_tabstops_lite.js
+-rw-rw-rw-   0        0        0    25711 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-emmet.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-error_marker.js
+-rw-rw-rw-   0        0        0     1973 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-hardwrap.js
+-rw-rw-rw-   0        0        0    76110 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-inline_autocomplete.js
+-rw-rw-rw-   0        0        0     4422 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-keybinding_menu.js
+-rw-rw-rw-   0        0        0    55365 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-language_tools.js
+-rw-rw-rw-   0        0        0     1221 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-linking.js
+-rw-rw-rw-   0        0        0     5170 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-modelist.js
+-rw-rw-rw-   0        0        0    16364 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-options.js
+-rw-rw-rw-   0        0        0    65922 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-prompt.js
+-rw-rw-rw-   0        0        0     2586 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-rtl.js
+-rw-rw-rw-   0        0        0    13594 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-searchbox.js
+-rw-rw-rw-   0        0        0    16917 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-settings_menu.js
+-rw-rw-rw-   0        0        0     1125 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-simple_tokenizer.js
+-rw-rw-rw-   0        0        0     1588 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-spellcheck.js
+-rw-rw-rw-   0        0        0     3866 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-split.js
+-rw-rw-rw-   0        0        0     4358 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-static_highlight.js
+-rw-rw-rw-   0        0        0     1276 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-statusbar.js
+-rw-rw-rw-   0        0        0     6555 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-textarea.js
+-rw-rw-rw-   0        0        0     1850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-themelist.js
+-rw-rw-rw-   0        0        0     3245 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-whitespace.js
+-rw-rw-rw-   0        0        0    25047 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-emacs.js
+-rw-rw-rw-   0        0        0     7874 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-sublime.js
+-rw-rw-rw-   0        0        0   118883 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vim.js
+-rw-rw-rw-   0        0        0     5734 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vscode.js
+-rw-rw-rw-   0        0        0     6198 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abap.js
+-rw-rw-rw-   0        0        0     5098 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abc.js
+-rw-rw-rw-   0        0        0    20926 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-actionscript.js
+-rw-rw-rw-   0        0        0     2623 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ada.js
+-rw-rw-rw-   0        0        0     5390 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-alda.js
+-rw-rw-rw-   0        0        0    14242 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apache_conf.js
+-rw-rw-rw-   0        0        0     8645 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apex.js
+-rw-rw-rw-   0        0        0     5732 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-applescript.js
+-rw-rw-rw-   0        0        0     4346 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-aql.js
+-rw-rw-rw-   0        0        0     8479 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asciidoc.js
+-rw-rw-rw-   0        0        0     8957 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asl.js
+-rw-rw-rw-   0        0        0     4825 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_arm32.js
+-rw-rw-rw-   0        0        0     9296 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_x86.js
+-rw-rw-rw-   0        0        0    64708 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-astro.js
+-rw-rw-rw-   0        0        0    63985 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-autohotkey.js
+-rw-rw-rw-   0        0        0     5187 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-batchfile.js
+-rw-rw-rw-   0        0        0     5230 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-bibtex.js
+-rw-rw-rw-   0        0        0     4398 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c9search.js
+-rw-rw-rw-   0        0        0    12181 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c_cpp.js
+-rw-rw-rw-   0        0        0     3404 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cirru.js
+-rw-rw-rw-   0        0        0     9017 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-clojure.js
+-rw-rw-rw-   0        0        0     2634 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cobol.js
+-rw-rw-rw-   0        0        0     7850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coffee.js
+-rw-rw-rw-   0        0        0    64687 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coldfusion.js
+-rw-rw-rw-   0        0        0    10342 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-crystal.js
+-rw-rw-rw-   0        0        0     9120 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csharp.js
+-rw-rw-rw-   0        0        0    76639 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_document.js
+-rw-rw-rw-   0        0        0    42033 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_orchestra.js
+-rw-rw-rw-   0        0        0     7960 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_score.js
+-rw-rw-rw-   0        0        0     1568 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csp.js
+-rw-rw-rw-   0        0        0    20931 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-css.js
+-rw-rw-rw-   0        0        0    63176 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-curly.js
+-rw-rw-rw-   0        0        0     1639 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cuttlefish.js
+-rw-rw-rw-   0        0        0     9272 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-d.js
+-rw-rw-rw-   0        0        0    15664 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dart.js
+-rw-rw-rw-   0        0        0     2740 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-diff.js
+-rw-rw-rw-   0        0        0    63520 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-django.js
+-rw-rw-rw-   0        0        0     8538 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dockerfile.js
+-rw-rw-rw-   0        0        0     7890 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dot.js
+-rw-rw-rw-   0        0        0    12869 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-drools.js
+-rw-rw-rw-   0        0        0     3190 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-edifact.js
+-rw-rw-rw-   0        0        0     3166 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-eiffel.js
+-rw-rw-rw-   0        0        0    82283 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ejs.js
+-rw-rw-rw-   0        0        0    16143 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elixir.js
+-rw-rw-rw-   0        0        0     5258 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elm.js
+-rw-rw-rw-   0        0        0    30080 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-erlang.js
+-rw-rw-rw-   0        0        0     3311 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-flix.js
+-rw-rw-rw-   0        0        0     7316 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-forth.js
+-rw-rw-rw-   0        0        0     8757 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fortran.js
+-rw-rw-rw-   0        0        0     5765 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsharp.js
+-rw-rw-rw-   0        0        0     5037 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsl.js
+-rw-rw-rw-   0        0        0    36155 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ftl.js
+-rw-rw-rw-   0        0        0     1785 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gcode.js
+-rw-rw-rw-   0        0        0     2688 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gherkin.js
+-rw-rw-rw-   0        0        0     1224 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gitignore.js
+-rw-rw-rw-   0        0        0    14253 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-glsl.js
+-rw-rw-rw-   0        0        0    31398 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gobstones.js
+-rw-rw-rw-   0        0        0     7183 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-golang.js
+-rw-rw-rw-   0        0        0     3815 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-graphqlschema.js
+-rw-rw-rw-   0        0        0    26873 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-groovy.js
+-rw-rw-rw-   0        0        0    49570 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haml.js
+-rw-rw-rw-   0        0        0    64037 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-handlebars.js
+-rw-rw-rw-   0        0        0    11851 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell.js
+-rw-rw-rw-   0        0        0     2607 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell_cabal.js
+-rw-rw-rw-   0        0        0     6801 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haxe.js
+-rw-rw-rw-   0        0        0     6297 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-hjson.js
+-rw-rw-rw-   0        0        0    62164 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html.js
+-rw-rw-rw-   0        0        0    79426 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_elixir.js
+-rw-rw-rw-   0        0        0    82614 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_ruby.js
+-rw-rw-rw-   0        0        0     3025 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ini.js
+-rw-rw-rw-   0        0        0     5666 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-io.js
+-rw-rw-rw-   0        0        0     8067 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ion.js
+-rw-rw-rw-   0        0        0     6033 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jack.js
+-rw-rw-rw-   0        0        0    50973 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jade.js
+-rw-rw-rw-   0        0        0    29040 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-java.js
+-rw-rw-rw-   0        0        0    21785 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-javascript.js
+-rw-rw-rw-   0        0        0     5109 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jexl.js
+-rw-rw-rw-   0        0        0     5548 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json.js
+-rw-rw-rw-   0        0        0     6193 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json5.js
+-rw-rw-rw-   0        0        0   233671 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsoniq.js
+-rw-rw-rw-   0        0        0    42635 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsp.js
+-rw-rw-rw-   0        0        0     6220 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jssm.js
+-rw-rw-rw-   0        0        0    22127 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsx.js
+-rw-rw-rw-   0        0        0     7866 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-julia.js
+-rw-rw-rw-   0        0        0     8389 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-kotlin.js
+-rw-rw-rw-   0        0        0     5360 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latex.js
+-rw-rw-rw-   0        0        0    65892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latte.js
+-rw-rw-rw-   0        0        0    22922 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-less.js
+-rw-rw-rw-   0        0        0    69494 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-liquid.js
+-rw-rw-rw-   0        0        0     2281 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lisp.js
+-rw-rw-rw-   0        0        0     5399 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-livescript.js
+-rw-rw-rw-   0        0        0     6045 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logiql.js
+-rw-rw-rw-   0        0        0    10989 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logtalk.js
+-rw-rw-rw-   0        0        0    26892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lsl.js
+-rw-rw-rw-   0        0        0     7905 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lua.js
+-rw-rw-rw-   0        0        0    70900 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-luapage.js
+-rw-rw-rw-   0        0        0     2763 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lucene.js
+-rw-rw-rw-   0        0        0     6989 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-makefile.js
+-rw-rw-rw-   0        0        0    73818 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-markdown.js
+-rw-rw-rw-   0        0        0    45777 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mask.js
+-rw-rw-rw-   0        0        0    20889 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-matlab.js
+-rw-rw-rw-   0        0        0     5246 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-maze.js
+-rw-rw-rw-   0        0        0     9691 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mediawiki.js
+-rw-rw-rw-   0        0        0    25211 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mel.js
+-rw-rw-rw-   0        0        0     5625 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mips.js
+-rw-rw-rw-   0        0        0     3164 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mixal.js
+-rw-rw-rw-   0        0        0     7032 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mushcode.js
+-rw-rw-rw-   0        0        0     8218 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mysql.js
+-rw-rw-rw-   0        0        0    10953 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nasal.js
+-rw-rw-rw-   0        0        0    16214 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nginx.js
+-rw-rw-rw-   0        0        0     6937 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nim.js
+-rw-rw-rw-   0        0        0    14453 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nix.js
+-rw-rw-rw-   0        0        0    10771 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nsis.js
+-rw-rw-rw-   0        0        0    65602 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nunjucks.js
+-rw-rw-rw-   0        0        0    68433 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-objectivec.js
+-rw-rw-rw-   0        0        0    15910 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ocaml.js
+-rw-rw-rw-   0        0        0     8326 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-odin.js
+-rw-rw-rw-   0        0        0    13077 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-partiql.js
+-rw-rw-rw-   0        0        0     4577 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pascal.js
+-rw-rw-rw-   0        0        0     7743 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-perl.js
+-rw-rw-rw-   0        0        0    63518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pgsql.js
+-rw-rw-rw-   0        0        0   505292 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php.js
+-rw-rw-rw-   0        0        0   509834 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php_laravel_blade.js
+-rw-rw-rw-   0        0        0     6637 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pig.js
+-rw-rw-rw-   0        0        0      836 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plain_text.js
+-rw-rw-rw-   0        0        0     6198 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plsql.js
+-rw-rw-rw-   0        0        0    84661 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-powershell.js
+-rw-rw-rw-   0        0        0    10718 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-praat.js
+-rw-rw-rw-   0        0        0     8573 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prisma.js
+-rw-rw-rw-   0        0        0     8695 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prolog.js
+-rw-rw-rw-   0        0        0     1425 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-properties.js
+-rw-rw-rw-   0        0        0    13875 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-protobuf.js
+-rw-rw-rw-   0        0        0     6017 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prql.js
+-rw-rw-rw-   0        0        0     7373 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-puppet.js
+-rw-rw-rw-   0        0        0     8294 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-python.js
+-rw-rw-rw-   0        0        0    16414 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-qml.js
+-rw-rw-rw-   0        0        0     5499 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-r.js
+-rw-rw-rw-   0        0        0    17881 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-raku.js
+-rw-rw-rw-   0        0        0    69959 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-razor.js
+-rw-rw-rw-   0        0        0     5004 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rdoc.js
+-rw-rw-rw-   0        0        0    12924 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-red.js
+-rw-rw-rw-   0        0        0     8368 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-redshift.js
+-rw-rw-rw-   0        0        0    67214 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rhtml.js
+-rw-rw-rw-   0        0        0     4408 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-robot.js
+-rw-rw-rw-   0        0        0     3381 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rst.js
+-rw-rw-rw-   0        0        0    19951 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ruby.js
+-rw-rw-rw-   0        0        0     8733 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rust.js
+-rw-rw-rw-   0        0        0     7022 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sac.js
+-rw-rw-rw-   0        0        0    16065 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sass.js
+-rw-rw-rw-   0        0        0     6781 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scad.js
+-rw-rw-rw-   0        0        0    27012 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scala.js
+-rw-rw-rw-   0        0        0     3976 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scheme.js
+-rw-rw-rw-   0        0        0     7485 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scrypt.js
+-rw-rw-rw-   0        0        0    24109 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scss.js
+-rw-rw-rw-   0        0        0     7501 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sh.js
+-rw-rw-rw-   0        0        0    24930 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sjs.js
+-rw-rw-rw-   0        0        0   113850 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-slim.js
+-rw-rw-rw-   0        0        0    65624 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smarty.js
+-rw-rw-rw-   0        0        0     8959 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smithy.js
+-rw-rw-rw-   0        0        0     4126 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-snippets.js
+-rw-rw-rw-   0        0        0    70659 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-soy_template.js
+-rw-rw-rw-   0        0        0     2625 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-space.js
+-rw-rw-rw-   0        0        0     8183 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sparql.js
+-rw-rw-rw-   0        0        0     5341 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sql.js
+-rw-rw-rw-   0        0        0    16924 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sqlserver.js
+-rw-rw-rw-   0        0        0    14831 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-stylus.js
+-rw-rw-rw-   0        0        0    33722 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-svg.js
+-rw-rw-rw-   0        0        0     7311 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-swift.js
+-rw-rw-rw-   0        0        0     6516 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tcl.js
+-rw-rw-rw-   0        0        0     7122 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-terraform.js
+-rw-rw-rw-   0        0        0     3114 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tex.js
+-rw-rw-rw-   0        0        0      328 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-text.js
+-rw-rw-rw-   0        0        0     2448 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-textile.js
+-rw-rw-rw-   0        0        0     2520 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-toml.js
+-rw-rw-rw-   0        0        0    23807 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tsx.js
+-rw-rw-rw-   0        0        0     5352 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-turtle.js
+-rw-rw-rw-   0        0        0    65791 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-twig.js
+-rw-rw-rw-   0        0        0    23506 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-typescript.js
+-rw-rw-rw-   0        0        0    16781 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vala.js
+-rw-rw-rw-   0        0        0    11995 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vbscript.js
+-rw-rw-rw-   0        0        0    66939 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-velocity.js
+-rw-rw-rw-   0        0        0     3223 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-verilog.js
+-rw-rw-rw-   0        0        0     2518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vhdl.js
+-rw-rw-rw-   0        0        0    64822 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-visualforce.js
+-rw-rw-rw-   0        0        0    93195 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vue.js
+-rw-rw-rw-   0        0        0    24740 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-wollok.js
+-rw-rw-rw-   0        0        0    10202 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xml.js
+-rw-rw-rw-   0        0        0   231054 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xquery.js
+-rw-rw-rw-   0        0        0     6796 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-yaml.js
+-rw-rw-rw-   0        0        0     9411 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zeek.js
+-rw-rw-rw-   0        0        0    11929 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zig.js
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.848433 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abap.js
+-rw-rw-rw-   0        0        0     1416 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abc.js
+-rw-rw-rw-   0        0        0     3478 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/actionscript.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ada.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/alda.js
+-rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/apache_conf.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/apex.js
+-rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/applescript.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/aql.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/asciidoc.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/asl.js
+-rw-rw-rw-   0        0        0      342 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/assembly_arm32.js
+-rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/assembly_x86.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/astro.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/autohotkey.js
+-rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/batchfile.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/bibtex.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c9search.js
+-rw-rw-rw-   0        0        0     3140 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c_cpp.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cirru.js
+-rw-rw-rw-   0        0        0     2525 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/clojure.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cobol.js
+-rw-rw-rw-   0        0        0     2714 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coffee.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coldfusion.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/crystal.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csharp.js
+-rw-rw-rw-   0        0        0      819 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_document.js
+-rw-rw-rw-   0        0        0     1594 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_orchestra.js
+-rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_score.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csp.js
+-rw-rw-rw-   0        0        0    20119 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/css.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/curly.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/cuttlefish.js
+-rw-rw-rw-   0        0        0      329 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/d.js
+-rw-rw-rw-   0        0        0     1792 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dart.js
+-rw-rw-rw-   0        0        0     1024 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/diff.js
+-rw-rw-rw-   0        0        0     4481 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/django.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dockerfile.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dot.js
+-rw-rw-rw-   0        0        0      851 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/drools.js
+-rw-rw-rw-   0        0        0     4802 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/edifact.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/eiffel.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ejs.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/elixir.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/elm.js
+-rw-rw-rw-   0        0        0     4055 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/erlang.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/flix.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/forth.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fortran.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsharp.js
+-rw-rw-rw-   0        0        0      814 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsl.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ftl.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gcode.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gherkin.js
+-rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gitignore.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/glsl.js
+-rw-rw-rw-   0        0        0    39601 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gobstones.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/golang.js
+-rw-rw-rw-   0        0        0     1171 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/graphqlschema.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/groovy.js
+-rw-rw-rw-   0        0        0      921 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haml.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/handlebars.js
+-rw-rw-rw-   0        0        0     2460 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell.js
+-rw-rw-rw-   0        0        0      341 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell_cabal.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haxe.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/hjson.js
+-rw-rw-rw-   0        0        0    19629 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html.js
+-rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html_elixir.js
+-rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html_ruby.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ini.js
+-rw-rw-rw-   0        0        0     1545 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/io.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ion.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jack.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jade.js
+-rw-rw-rw-   0        0        0     4795 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/java.js
+-rw-rw-rw-   0        0        0     4337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/javascript.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jexl.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/json.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/json5.js
+-rw-rw-rw-   0        0        0     2197 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsoniq.js
+-rw-rw-rw-   0        0        0     3247 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsp.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jssm.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsx.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/julia.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/kotlin.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/latex.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/latte.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/less.js
+-rw-rw-rw-   0        0        0    20003 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/liquid.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lisp.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/livescript.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/logiql.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/logtalk.js
+-rw-rw-rw-   0        0        0    35892 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lsl.js
+-rw-rw-rw-   0        0        0      977 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lua.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/luapage.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lucene.js
+-rw-rw-rw-   0        0        0      687 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/makefile.js
+-rw-rw-rw-   0        0        0     2462 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/markdown.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mask.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/matlab.js
+-rw-rw-rw-   0        0        0      743 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/maze.js
+-rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mediawiki.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mel.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mips.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mixal.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mushcode.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/mysql.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nasal.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nginx.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nim.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nix.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nsis.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/nunjucks.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/objectivec.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ocaml.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/odin.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/partiql.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pascal.js
+-rw-rw-rw-   0        0        0     5986 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/perl.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pgsql.js
+-rw-rw-rw-   0        0        0     7422 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php.js
+-rw-rw-rw-   0        0        0      345 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php_laravel_blade.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/pig.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/plain_text.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/plsql.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/powershell.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/praat.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prisma.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prolog.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/properties.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/protobuf.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/prql.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/puppet.js
+-rw-rw-rw-   0        0        0     4153 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/python.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/qml.js
+-rw-rw-rw-   0        0        0     3091 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/r.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/raku.js
+-rw-rw-rw-   0        0        0      641 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/razor.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rdoc.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/red.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/redshift.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rhtml.js
+-rw-rw-rw-   0        0        0     2072 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/robot.js
+-rw-rw-rw-   0        0        0      911 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rst.js
+-rw-rw-rw-   0        0        0    21752 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ruby.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rust.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sac.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sass.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scad.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scala.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scheme.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scrypt.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/scss.js
+-rw-rw-rw-   0        0        0     2518 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sh.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sjs.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/slim.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/smarty.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/smithy.js
+-rw-rw-rw-   0        0        0      786 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/snippets.js
+-rw-rw-rw-   0        0        0      340 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/soy_template.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/space.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sparql.js
+-rw-rw-rw-   0        0        0     1411 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sql.js
+-rw-rw-rw-   0        0        0     2632 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sqlserver.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/stylus.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/svg.js
+-rw-rw-rw-   0        0        0      333 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/swift.js
+-rw-rw-rw-   0        0        0     2159 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tcl.js
+-rw-rw-rw-   0        0        0      337 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/terraform.js
+-rw-rw-rw-   0        0        0     4105 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tex.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/text.js
+-rw-rw-rw-   0        0        0     1025 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/textile.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/toml.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tsx.js
+-rw-rw-rw-   0        0        0      334 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/turtle.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/twig.js
+-rw-rw-rw-   0        0        0      338 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/typescript.js
+-rw-rw-rw-   0        0        0     3455 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vala.js
+-rw-rw-rw-   0        0        0      336 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vbscript.js
+-rw-rw-rw-   0        0        0     1140 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/velocity.js
+-rw-rw-rw-   0        0        0      335 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/verilog.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vhdl.js
+-rw-rw-rw-   0        0        0      339 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/visualforce.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vue.js
+-rw-rw-rw-   0        0        0     1744 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/wollok.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xml.js
+-rw-rw-rw-   0        0        0     2197 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xquery.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/yaml.js
+-rw-rw-rw-   0        0        0      332 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/zeek.js
+-rw-rw-rw-   0        0        0      331 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/zig.js
+-rw-rw-rw-   0        0        0    28712 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-ambiance.js
+-rw-rw-rw-   0        0        0     3854 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chaos.js
+-rw-rw-rw-   0        0        0     3872 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chrome.js
+-rw-rw-rw-   0        0        0     4176 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_day.js
+-rw-rw-rw-   0        0        0     4285 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night.js
+-rw-rw-rw-   0        0        0     4306 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night_low_color.js
+-rw-rw-rw-   0        0        0     5328 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor.js
+-rw-rw-rw-   0        0        0     5876 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor_dark.js
+-rw-rw-rw-   0        0        0     3126 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds.js
+-rw-rw-rw-   0        0        0     3427 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds_midnight.js
+-rw-rw-rw-   0        0        0     3359 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cobalt.js
+-rw-rw-rw-   0        0        0     3985 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-crimson_editor.js
+-rw-rw-rw-   0        0        0     3323 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dawn.js
+-rw-rw-rw-   0        0        0     4821 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dracula.js
+-rw-rw-rw-   0        0        0     4384 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dreamweaver.js
+-rw-rw-rw-   0        0        0     3185 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-eclipse.js
+-rw-rw-rw-   0        0        0     3516 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github.js
+-rw-rw-rw-   0        0        0     3807 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github_dark.js
+-rw-rw-rw-   0        0        0     3364 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gob.js
+-rw-rw-rw-   0        0        0     2580 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox.js
+-rw-rw-rw-   0        0        0     4060 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_dark_hard.js
+-rw-rw-rw-   0        0        0     4412 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_light_hard.js
+-rw-rw-rw-   0        0        0     3232 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-idle_fingers.js
+-rw-rw-rw-   0        0        0     7616 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-iplastic.js
+-rw-rw-rw-   0        0        0     4572 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-katzenmilch.js
+-rw-rw-rw-   0        0        0     3286 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kr_theme.js
+-rw-rw-rw-   0        0        0     3293 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kuroir.js
+-rw-rw-rw-   0        0        0     3193 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore.js
+-rw-rw-rw-   0        0        0     3432 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore_soft.js
+-rw-rw-rw-   0        0        0     3820 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-mono_industrial.js
+-rw-rw-rw-   0        0        0     3354 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-monokai.js
+-rw-rw-rw-   0        0        0     2914 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-nord_dark.js
+-rw-rw-rw-   0        0        0     3852 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-one_dark.js
+-rw-rw-rw-   0        0        0     3667 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-pastel_on_dark.js
+-rw-rw-rw-   0        0        0     3270 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_dark.js
+-rw-rw-rw-   0        0        0     3434 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_light.js
+-rw-rw-rw-   0        0        0     4196 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-sqlserver.js
+-rw-rw-rw-   0        0        0     3923 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-terminal.js
+-rw-rw-rw-   0        0        0      615 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-textmate.js
+-rw-rw-rw-   0        0        0     3641 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow.js
+-rw-rw-rw-   0        0        0     3836 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night.js
+-rw-rw-rw-   0        0        0     4064 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_blue.js
+-rw-rw-rw-   0        0        0     4593 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_bright.js
+-rw-rw-rw-   0        0        0     4282 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_eighties.js
+-rw-rw-rw-   0        0        0     3469 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-twilight.js
+-rw-rw-rw-   0        0        0     3173 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-vibrant_ink.js
+-rw-rw-rw-   0        0        0     3035 2024-02-11 16:53:43.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-wagtail.js
+-rw-rw-rw-   0        0        0     3031 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-xcode.js
+-rw-rw-rw-   0        0        0    21987 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-base.js
+-rw-rw-rw-   0        0        0   323433 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-coffee.js
+-rw-rw-rw-   0        0        0   151082 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-css.js
+-rw-rw-rw-   0        0        0   208882 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-html.js
+-rw-rw-rw-   0        0        0   514300 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-javascript.js
+-rw-rw-rw-   0        0        0    24346 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-json.js
+-rw-rw-rw-   0        0        0    48226 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-lua.js
+-rw-rw-rw-   0        0        0    78734 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-php.js
+-rw-rw-rw-   0        0        0    46914 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xml.js
+-rw-rw-rw-   0        0        0  1624915 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xquery.js
+-rw-rw-rw-   0        0        0    76731 1985-10-26 08:15:00.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-yaml.js
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.404986 wagtail_ace_editor-1.1.4/wagtail_ace_editor/templates/
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.849431 wagtail_ace_editor-1.1.4/wagtail_ace_editor/templates/wagtail_ace_editor/
+-rw-rw-rw-   0        0        0      888 2024-02-11 17:47:26.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/templates/wagtail_ace_editor/ace_editor.html
+-rw-rw-rw-   0        0        0     2203 2024-02-19 21:47:41.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/util.py
+-rw-rw-rw-   0        0        0      330 2024-02-11 17:27:32.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/wagtail_hooks.py
+-rw-rw-rw-   0        0        0     2814 2024-03-16 14:35:46.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:00:53.850438 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/
+-rw-rw-rw-   0        0        0     5371 2024-04-18 08:00:53.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    32164 2024-04-18 08:00:53.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 08:00:53.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-18 08:00:53.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-18 08:00:53.000000 wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/top_level.txt
```

### Comparing `wagtail_ace_editor-1.1.3/LICENSE` & `wagtail_ace_editor-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/PKG-INFO` & `wagtail_ace_editor-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_ace_editor
-Version: 1.1.3
+Version: 1.1.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_ace_editor
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_ace_editor-1.1.3/README.md` & `wagtail_ace_editor-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/setup.cfg` & `wagtail_ace_editor-1.1.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f61 6365 5f65   = wagtail_ace_e
 00000020: 6469 746f 720d 0a76 6572 7369 6f6e 203d  ditor..version =
-00000030: 2031 2e31 2e33 0d0a 6465 7363 7269 7074   1.1.3..descript
+00000030: 2031 2e31 2e34 0d0a 6465 7363 7269 7074   1.1.4..descript
 00000040: 696f 6e20 3d20 416e 2061 7070 6c69 6361  ion = An applica
 00000050: 7469 6f6e 206d 6164 6520 666f 7220 7468  tion made for th
 00000060: 6520 446a 616e 676f 2057 6562 2046 7261  e Django Web Fra
 00000070: 6d65 776f 726b 2e0d 0a6c 6f6e 675f 6465  mework...long_de
 00000080: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000090: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
```

### Comparing `wagtail_ace_editor-1.1.3/tests/testapp/core/tests.py` & `wagtail_ace_editor-1.1.4/tests/testapp/core/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/tests/testapp/manage.py` & `wagtail_ace_editor-1.1.4/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/tests/testapp/testapp/settings.py` & `wagtail_ace_editor-1.1.4/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/tests/testapp/testapp/urls.py` & `wagtail_ace_editor-1.1.4/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/blocks.py` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/clean.py` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/clean.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/forms.py` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-widget.css` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-controller.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-telepath.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ace.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ace.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-beautify.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-code_lens.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-code_lens.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-command_bar.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-command_bar.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-elastic_tabstops_lite.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-elastic_tabstops_lite.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-emmet.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-emmet.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-hardwrap.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-hardwrap.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-inline_autocomplete.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-inline_autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-keybinding_menu.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-keybinding_menu.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-language_tools.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-linking.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-linking.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-modelist.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-modelist.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-options.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-options.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-prompt.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-prompt.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-rtl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-rtl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-searchbox.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-searchbox.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-settings_menu.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-settings_menu.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-simple_tokenizer.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-simple_tokenizer.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-spellcheck.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-spellcheck.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-split.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-split.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-static_highlight.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-static_highlight.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-statusbar.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-statusbar.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-textarea.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-textarea.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-themelist.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-themelist.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-whitespace.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/ext-whitespace.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-emacs.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-emacs.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-sublime.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-sublime.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vim.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vscode.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/keybinding-vscode.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abap.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abap.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abc.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-abc.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-actionscript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-actionscript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ada.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ada.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-alda.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-alda.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apache_conf.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apache_conf.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apex.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-apex.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-applescript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-applescript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-aql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-aql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asciidoc.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asciidoc.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-asl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_arm32.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_arm32.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_x86.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-assembly_x86.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-astro.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-astro.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-autohotkey.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-autohotkey.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-batchfile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-batchfile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-bibtex.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-bibtex.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c9search.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c9search.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c_cpp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-c_cpp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cirru.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cirru.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-clojure.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-clojure.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cobol.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cobol.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coffee.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coffee.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coldfusion.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-coldfusion.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-crystal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-crystal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csharp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csharp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_document.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_document.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_orchestra.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_orchestra.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_score.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csound_score.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-csp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-css.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-css.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-curly.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-curly.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cuttlefish.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-cuttlefish.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-d.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-d.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dart.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dart.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-diff.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-diff.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-django.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-django.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dockerfile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dockerfile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dot.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-dot.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-drools.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-drools.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-edifact.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-edifact.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-eiffel.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-eiffel.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ejs.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ejs.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elixir.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elixir.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elm.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-elm.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-erlang.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-erlang.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-flix.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-flix.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-forth.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-forth.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fortran.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fortran.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsharp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsharp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-fsl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ftl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ftl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gcode.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gcode.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gherkin.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gitignore.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gitignore.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-glsl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-glsl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gobstones.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-gobstones.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-golang.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-golang.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-graphqlschema.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-graphqlschema.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-groovy.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-groovy.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-handlebars.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-handlebars.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell_cabal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haskell_cabal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haxe.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-haxe.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-hjson.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-hjson.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_elixir.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_elixir.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_ruby.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-html_ruby.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ini.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ini.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-io.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-io.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ion.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ion.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jack.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jack.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jade.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jade.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-java.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-java.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-javascript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jexl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jexl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json5.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-json5.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsoniq.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsoniq.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jssm.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jssm.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsx.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-jsx.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-julia.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-julia.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-kotlin.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-kotlin.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latex.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latex.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latte.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-latte.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-less.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-less.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-liquid.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-liquid.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lisp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lisp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-livescript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-livescript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logiql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logiql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logtalk.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-logtalk.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lsl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lsl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lua.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lua.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-luapage.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-luapage.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lucene.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-lucene.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-makefile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-makefile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-markdown.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-markdown.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mask.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mask.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-matlab.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-matlab.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-maze.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-maze.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mediawiki.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mediawiki.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mel.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mel.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mips.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mips.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mixal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mixal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mushcode.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mushcode.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mysql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-mysql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nasal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nasal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nginx.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nginx.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nim.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nim.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nix.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nix.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nsis.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nsis.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nunjucks.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-nunjucks.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-objectivec.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-objectivec.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ocaml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ocaml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-odin.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-odin.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-partiql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-partiql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pascal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pascal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-perl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-perl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pgsql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pgsql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php_laravel_blade.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-php_laravel_blade.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pig.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-pig.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plain_text.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plain_text.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plsql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-plsql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-powershell.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-powershell.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-praat.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-praat.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prisma.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prisma.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prolog.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prolog.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-properties.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-properties.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-protobuf.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-protobuf.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-prql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-puppet.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-puppet.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-python.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-python.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-qml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-qml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-r.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-r.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-raku.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-raku.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-razor.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-razor.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rdoc.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rdoc.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-red.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-red.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-redshift.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-redshift.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rhtml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rhtml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-robot.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-robot.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rst.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rst.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ruby.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-ruby.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rust.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-rust.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sac.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sac.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sass.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sass.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scad.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scad.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scala.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scala.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scheme.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scheme.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scrypt.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scrypt.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scss.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-scss.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sh.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sh.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sjs.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sjs.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-slim.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-slim.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smarty.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smarty.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smithy.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-smithy.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-snippets.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-snippets.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-soy_template.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-soy_template.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-space.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-space.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sparql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sparql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sqlserver.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-sqlserver.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-stylus.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-stylus.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-svg.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-svg.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-swift.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-swift.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tcl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tcl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-terraform.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-terraform.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tex.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tex.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-textile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-textile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-toml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-toml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tsx.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-tsx.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-turtle.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-turtle.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-twig.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-twig.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-typescript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-typescript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vala.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vala.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vbscript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vbscript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-velocity.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-velocity.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-verilog.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-verilog.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vhdl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vhdl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-visualforce.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-visualforce.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vue.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-vue.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-wollok.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-wollok.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xquery.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-xquery.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-yaml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-yaml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zeek.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zeek.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zig.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/mode-zig.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abc.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/abc.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/actionscript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/actionscript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c_cpp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/c_cpp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/clojure.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/clojure.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coffee.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/coffee.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_document.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_document.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_orchestra.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/csound_orchestra.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/css.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/css.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dart.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/dart.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/diff.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/diff.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/django.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/django.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/drools.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/drools.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/edifact.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/edifact.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/erlang.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/erlang.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/fsl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gobstones.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/gobstones.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/graphqlschema.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/graphqlschema.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/haskell.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/html.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/io.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/io.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/java.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/java.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/javascript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/javascript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsoniq.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsoniq.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsp.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/jsp.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/liquid.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/liquid.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lsl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lsl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lua.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/lua.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/makefile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/makefile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/markdown.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/markdown.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/maze.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/maze.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/perl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/perl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/php.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/python.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/python.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/r.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/r.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/razor.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/razor.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/robot.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/robot.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rst.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/rst.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ruby.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/ruby.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sh.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sh.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/snippets.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/snippets.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sql.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sql.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sqlserver.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/sqlserver.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tcl.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tcl.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tex.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/tex.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/textile.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/textile.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vala.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/vala.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/velocity.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/velocity.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/wollok.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/wollok.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xquery.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/snippets/xquery.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-ambiance.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-ambiance.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chaos.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chaos.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chrome.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-chrome.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_day.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_day.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night_low_color.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud9_night_low_color.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cloud_editor_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds_midnight.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-clouds_midnight.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cobalt.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-cobalt.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-crimson_editor.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-crimson_editor.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dawn.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dawn.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dracula.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dracula.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dreamweaver.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-dreamweaver.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-eclipse.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-eclipse.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-github_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gob.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gob.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_dark_hard.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_dark_hard.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_light_hard.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-gruvbox_light_hard.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-idle_fingers.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-idle_fingers.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-iplastic.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-iplastic.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-katzenmilch.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-katzenmilch.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kr_theme.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kr_theme.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kuroir.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-kuroir.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore_soft.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-merbivore_soft.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-mono_industrial.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-mono_industrial.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-monokai.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-nord_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-nord_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-one_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-one_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-pastel_on_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-pastel_on_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_dark.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_dark.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_light.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-solarized_light.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-sqlserver.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-sqlserver.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-terminal.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-terminal.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-textmate.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-textmate.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_blue.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_blue.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_bright.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_bright.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_eighties.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-tomorrow_night_eighties.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-twilight.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-twilight.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-vibrant_ink.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-vibrant_ink.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-wagtail.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-wagtail.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-xcode.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/theme-xcode.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-base.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-base.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-coffee.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-coffee.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-css.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-css.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-html.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-html.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-javascript.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-javascript.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-json.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-json.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-lua.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-lua.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-php.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-php.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xquery.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-xquery.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-yaml.js` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/static/wagtail_ace_editor/js/worker-yaml.js`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/templates/wagtail_ace_editor/ace_editor.html` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/templates/wagtail_ace_editor/ace_editor.html`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/util.py` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/util.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor/widgets.py` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/PKG-INFO` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_ace_editor
-Version: 1.1.3
+Version: 1.1.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_ace_editor
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_ace_editor-1.1.3/wagtail_ace_editor.egg-info/SOURCES.txt` & `wagtail_ace_editor-1.1.4/wagtail_ace_editor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 wagtail_ace_editor.egg-info/dependency_links.txt
 wagtail_ace_editor.egg-info/requires.txt
 wagtail_ace_editor.egg-info/top_level.txt
 wagtail_ace_editor/migrations/__init__.py
 wagtail_ace_editor/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-iframe.css
 wagtail_ace_editor/static/wagtail_ace_editor/css/ace-editor-widget.css
+wagtail_ace_editor/static/wagtail_ace_editor/js/LICENSE
 wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-controller.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor-telepath.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ace-editor.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ace.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ext-beautify.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ext-code_lens.js
 wagtail_ace_editor/static/wagtail_ace_editor/js/ext-command_bar.js
```

