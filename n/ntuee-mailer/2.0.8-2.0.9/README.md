# Comparing `tmp/ntuee-mailer-2.0.8.tar.gz` & `tmp/ntuee-mailer-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntuee-mailer-2.0.8.tar", max compression
+gzip compressed data, was "ntuee-mailer-2.0.9.tar", max compression
```

## Comparing `ntuee-mailer-2.0.8.tar` & `ntuee-mailer-2.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2022-11-08 19:06:12.331973 ntuee-mailer-2.0.8/LICENSE
--rw-r--r--   0        0        0     2609 2022-11-08 19:06:12.332128 ntuee-mailer-2.0.8/README.md
--rw-r--r--   0        0        0    14920 2022-11-08 19:06:12.332395 ntuee-mailer-2.0.8/ntuee_mailer/AutoMailer.py
--rw-r--r--   0        0        0    15336 2022-11-08 19:06:12.332590 ntuee-mailer-2.0.8/ntuee_mailer/Letter.py
--rw-r--r--   0        0        0        0 2022-11-08 19:06:12.332642 ntuee-mailer-2.0.8/ntuee_mailer/__init__.py
--rw-r--r--   0        0        0       76 2022-11-08 19:06:12.332768 ntuee-mailer-2.0.8/ntuee_mailer/__main__.py
--rw-r--r--   0        0        0      109 2022-11-08 19:06:12.332971 ntuee-mailer-2.0.8/ntuee_mailer/config-default.ini
--rw-r--r--   0        0        0      434 2022-12-03 06:35:40.085736 ntuee-mailer-2.0.8/ntuee_mailer/globals.py
--rw-r--r--   0        0        0     6414 2022-11-08 19:06:12.333302 ntuee-mailer-2.0.8/ntuee_mailer/main.py
--rw-r--r--   0        0        0        0 2022-11-08 19:06:12.333505 ntuee-mailer-2.0.8/ntuee_mailer/template_letter/attachments/.placeholder
--rw-r--r--   0        0        0      177 2022-11-08 19:06:12.333629 ntuee-mailer-2.0.8/ntuee_mailer/template_letter/config.yml
--rw-r--r--   0        0        0      214 2022-11-08 19:06:12.333740 ntuee-mailer-2.0.8/ntuee_mailer/template_letter/content.html
--rw-r--r--   0        0        0       80 2022-11-08 19:06:12.333835 ntuee-mailer-2.0.8/ntuee_mailer/template_letter/recipients.csv
--rw-r--r--   0        0        0     5279 2022-11-08 19:06:12.333937 ntuee-mailer-2.0.8/ntuee_mailer/utils.py
--rw-r--r--   0        0        0      739 2022-12-03 06:45:13.768332 ntuee-mailer-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3733 2022-12-03 06:45:20.889388 ntuee-mailer-2.0.8/setup.py
--rw-r--r--   0        0        0     3483 2022-12-03 06:45:20.889636 ntuee-mailer-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-08 19:06:12.331973 ntuee-mailer-2.0.9/LICENSE
+-rw-r--r--   0        0        0     2609 2022-11-08 19:06:12.332128 ntuee-mailer-2.0.9/README.md
+-rw-r--r--   0        0        0    14920 2022-11-08 19:06:12.332395 ntuee-mailer-2.0.9/ntuee_mailer/AutoMailer.py
+-rw-r--r--   0        0        0    15336 2022-11-08 19:06:12.332590 ntuee-mailer-2.0.9/ntuee_mailer/Letter.py
+-rw-r--r--   0        0        0        0 2022-11-08 19:06:12.332642 ntuee-mailer-2.0.9/ntuee_mailer/__init__.py
+-rw-r--r--   0        0        0       76 2022-11-08 19:06:12.332768 ntuee-mailer-2.0.9/ntuee_mailer/__main__.py
+-rw-r--r--   0        0        0      109 2022-11-08 19:06:12.332971 ntuee-mailer-2.0.9/ntuee_mailer/config-default.ini
+-rw-r--r--   0        0        0      434 2022-12-03 06:35:40.085736 ntuee-mailer-2.0.9/ntuee_mailer/globals.py
+-rw-r--r--   0        0        0     6414 2022-11-08 19:06:12.333302 ntuee-mailer-2.0.9/ntuee_mailer/main.py
+-rw-r--r--   0        0        0        0 2022-11-08 19:06:12.333505 ntuee-mailer-2.0.9/ntuee_mailer/template_letter/attachments/.placeholder
+-rw-r--r--   0        0        0      177 2022-11-08 19:06:12.333629 ntuee-mailer-2.0.9/ntuee_mailer/template_letter/config.yml
+-rw-r--r--   0        0        0      214 2022-11-08 19:06:12.333740 ntuee-mailer-2.0.9/ntuee_mailer/template_letter/content.html
+-rw-r--r--   0        0        0       80 2022-11-08 19:06:12.333835 ntuee-mailer-2.0.9/ntuee_mailer/template_letter/recipients.csv
+-rw-r--r--   0        0        0     5279 2022-11-08 19:06:12.333937 ntuee-mailer-2.0.9/ntuee_mailer/utils.py
+-rw-r--r--   0        0        0      739 2022-12-03 06:57:54.475354 ntuee-mailer-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3733 2022-12-03 07:05:41.323671 ntuee-mailer-2.0.9/setup.py
+-rw-r--r--   0        0        0     3533 2022-12-03 07:05:41.323876 ntuee-mailer-2.0.9/PKG-INFO
```

### Comparing `ntuee-mailer-2.0.8/LICENSE` & `ntuee-mailer-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/README.md` & `ntuee-mailer-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/ntuee_mailer/AutoMailer.py` & `ntuee-mailer-2.0.9/ntuee_mailer/AutoMailer.py`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/ntuee_mailer/Letter.py` & `ntuee-mailer-2.0.9/ntuee_mailer/Letter.py`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/ntuee_mailer/main.py` & `ntuee-mailer-2.0.9/ntuee_mailer/main.py`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/ntuee_mailer/utils.py` & `ntuee-mailer-2.0.9/ntuee_mailer/utils.py`

 * *Files identical despite different names*

### Comparing `ntuee-mailer-2.0.8/pyproject.toml` & `ntuee-mailer-2.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "ntuee-mailer"
-version = "2.0.8"
+version = "2.0.9"
 description = "an auto mailer to send emails in batch for you"
 authors = ["madmaxieee <76544194+madmaxieee@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/madmaxieee/ntuee-mailer"
 packages = [{ include = "ntuee_mailer" }]
 
 [tool.poetry.scripts]
 ntuee-mailer = "ntuee_mailer.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.6"
 Cerberus = "1.3.4"
 email-validator = "1.2.1"
 PyYAML = "6.0"
 rich = "12.5.1"
 typer = { extras = ["all"], version = "^0.6.1" }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `ntuee-mailer-2.0.8/setup.py` & `ntuee-mailer-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['ntuee-mailer = ntuee_mailer.main:app']}
 
 setup_kwargs = {
     'name': 'ntuee-mailer',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': 'an auto mailer to send emails in batch for you',
     'long_description': '# `ntuee-mailer`\n\nThis is a simple mailer for NTU students to send letters in batches.\n\n**Installation**\n\n```bash\n$ pip install ntuee-mailer\n```\n\n**Usage**:\n\n```bash\n$ ntuee-mailer [OPTIONS] COMMAND [ARGS]...\n```\n\n**Options**:\n\n- `--install-completion`: Install completion for the current shell.\n- `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n- `--help`: Show this message and exit.\n\n**Commands**:\n\n- `check`: check wether a directory is a valid letter a...\n- `config`: configure the auto mailer a valid config file...\n- `new`: create a new letter from template\n- `send`: send emails to a list of recipients as...\n\n## `ntuee-mailer check`\n\ncheck wether a directory is a valid letter\n\na letter folder should be structured as follows:\n\nletter\n\n├── attachments\n\n│ ├── ...\n\n│ └── ...\n\n├── config.yml\n\n├── content.html\n\n└── recipients.csv\n\n**Usage**:\n\n```console\n$ ntuee-mailer check [OPTIONS] LETTER_PATH\n```\n\n**Arguments**:\n\n- `LETTER_PATH`: Path to letter directory [required]\n\n**Options**:\n\n- `--help`: Show this message and exit.\n\n## `ntuee-mailer config`\n\nconfigure the auto mailer\n\na valid config file should have the following structure:\n\n[smtp]\n\nhost=smtps.ntu.edu.tw\n\nport=465\n\ntimeout=5\n\n[pop3]\n\nhost=msa.ntu.edu.tw\n\nport=995\n\ntimeout=5\n\n[account]\n\nname=John Doe\n\n**Usage**:\n\n```console\n$ ntuee-mailer config [OPTIONS]\n```\n\n**Options**:\n\n- `-f, --file TEXT`: Path to new config file whose content will be copied to config.ini\n- `-r, --reset`: Reset config.ini to default [default: False]\n- `-l, --list`: list current config [default: False]\n- `--help`: Show this message and exit.\n\n## `ntuee-mailer new`\n\ncreate a new letter from template\n\n**Usage**:\n\n```console\n$ ntuee-mailer new [OPTIONS] LETTER_NAME\n```\n\n**Arguments**:\n\n- `LETTER_NAME`: Name of letter [required]\n\n**Options**:\n\n- `--help`: Show this message and exit.\n\n## `ntuee-mailer send`\n\nsend emails to a list of recipients as configured in your letter\n\n**Usage**:\n\n```console\n$ ntuee-mailer send [OPTIONS] [LETTER_PATH]\n```\n\n**Arguments**:\n\n- `[LETTER_PATH]`: Path to letter\n\n**Options**:\n\n- `-t, --test`: Test mode: send mail to yourself [default: False]\n- `-c, --config FILE`: Path to config.ini [default: /home/madmax/.config/ntuee-mailer/config.ini]\n- `-q, --quiet`: Quiet mode: less output [default: False]\n- `-d, --debug INTEGER RANGE`: Debug level [default: 0]\n- `--help`: Show this message and exit.\n\n## `ntuee-mailer test`\n\n**Usage**:\n\n```console\n$ ntuee-mailer test [OPTIONS]\n```\n\n**Options**:\n\n- `--help`: Show this message and exit.\n',
     'author': 'madmaxieee',
     'author_email': '76544194+madmaxieee@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/madmaxieee/ntuee-mailer',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.6,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ntuee-mailer-2.0.8/PKG-INFO` & `ntuee-mailer-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ntuee-mailer
-Version: 2.0.8
+Version: 2.0.9
 Summary: an auto mailer to send emails in batch for you
 Home-page: https://github.com/madmaxieee/ntuee-mailer
 License: MIT
 Author: madmaxieee
 Author-email: 76544194+madmaxieee@users.noreply.github.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Cerberus (==1.3.4)
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: email-validator (==1.2.1)
 Requires-Dist: rich (==12.5.1)
```

