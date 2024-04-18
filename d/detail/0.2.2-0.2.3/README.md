# Comparing `tmp/detail-0.2.2.tar.gz` & `tmp/detail-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detail-0.2.2.tar", max compression
+gzip compressed data, was "detail-0.2.3.tar", max compression
```

## Comparing `detail-0.2.2.tar` & `detail-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1456 2022-08-20 21:26:28.640066 detail-0.2.2/LICENSE
--rw-r--r--   0        0        0     1898 2022-08-20 21:26:28.640066 detail-0.2.2/README.rst
--rw-r--r--   0        0        0      418 2022-08-20 21:26:28.640066 detail-0.2.2/detail/__init__.py
--rw-r--r--   0        0        0     3455 2022-08-20 21:26:28.640066 detail-0.2.2/detail/cli.py
--rw-r--r--   0        0        0    19675 2022-08-20 21:26:28.640066 detail-0.2.2/detail/core.py
--rw-r--r--   0        0        0      678 2022-08-20 21:26:28.640066 detail-0.2.2/detail/exceptions.py
--rw-r--r--   0        0        0     4609 2022-08-20 21:26:28.640066 detail-0.2.2/detail/github.py
--rw-r--r--   0        0        0        0 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/__init__.py
--rw-r--r--   0        0        0     3833 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_cli.py
--rw-r--r--   0        0        0     3134 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_core.py
--rw-r--r--   0        0        0     7159 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_github.py
--rw-r--r--   0        0        0    12869 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_integration.py
--rw-r--r--   0        0        0     1163 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_utils.py
--rw-r--r--   0        0        0       66 2022-08-20 21:26:28.640066 detail-0.2.2/detail/tests/test_version.py
--rw-r--r--   0        0        0     1106 2022-08-20 21:26:28.640066 detail-0.2.2/detail/utils.py
--rw-r--r--   0        0        0      144 2022-08-20 21:26:28.640066 detail-0.2.2/detail/version.py
--rw-r--r--   0        0        0     1998 2022-08-20 21:26:44.400432 detail-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2997 2022-08-20 21:26:48.879004 detail-0.2.2/setup.py
--rw-r--r--   0        0        0     3125 2022-08-20 21:26:48.879431 detail-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-18 12:09:29.055768 detail-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1786 2024-04-18 12:09:29.055768 detail-0.2.3/README.md
+-rw-r--r--   0        0        0      256 2024-04-18 12:09:29.055768 detail-0.2.3/detail/__init__.py
+-rw-r--r--   0        0        0     3456 2024-04-18 12:09:29.055768 detail-0.2.3/detail/cli.py
+-rw-r--r--   0        0        0    19842 2024-04-18 12:09:29.055768 detail-0.2.3/detail/core.py
+-rw-r--r--   0        0        0      678 2024-04-18 12:09:29.055768 detail-0.2.3/detail/exceptions.py
+-rw-r--r--   0        0        0     4590 2024-04-18 12:09:29.055768 detail-0.2.3/detail/github.py
+-rw-r--r--   0        0        0        0 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/__init__.py
+-rw-r--r--   0        0        0     3833 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_cli.py
+-rw-r--r--   0        0        0     3116 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_core.py
+-rw-r--r--   0        0        0     7142 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_github.py
+-rw-r--r--   0        0        0    12860 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_integration.py
+-rw-r--r--   0        0        0     1164 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_utils.py
+-rw-r--r--   0        0        0       66 2024-04-18 12:09:29.055768 detail-0.2.3/detail/tests/test_version.py
+-rw-r--r--   0        0        0     1106 2024-04-18 12:09:29.055768 detail-0.2.3/detail/utils.py
+-rw-r--r--   0        0        0       73 2024-04-18 12:09:29.055768 detail-0.2.3/detail/version.py
+-rw-r--r--   0        0        0     2194 2024-04-18 12:09:50.400089 detail-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 detail-0.2.3/PKG-INFO
```

### Comparing `detail-0.2.2/LICENSE` & `detail-0.2.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `detail-0.2.2/README.rst` & `detail-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,37 @@
-detail
-#######
+# detail
 
-``detail`` allows contributors to create structured and configurable notes in a project,
-providing the ability to do automations such as:
+`detail` allows contributors to create structured and configurable notes in a project, providing the ability to do automations such as:
 
-1. Ensuring that contributors add information to pull requests that provide
-   QA instructions, release notes, and associated tickets. The ``detail lint`` command
-   ensures that notes are present in a pull request and adhere to the schema.
+1. Ensuring that contributors add information to pull requests that provide QA instructions, release notes, and associated tickets. The `detail lint` command ensures that notes are present in a pull request and adhere to the schema.
 
-2. Rendering dynamic logs from the notes. ``detail log`` provides the ability
-   to slice and dice the commit log however you need, pulling in a ``notes``
-   variable in a Jinja template with all notes that can be grouped and filtered.
+2. Rendering dynamic logs from the notes. `detail log` provides the ability to slice and dice the commit log however you need, pulling in a `notes` variable in a Jinja template with all notes that can be grouped and filtered.
 
-3. Other automations, such as version bumping, Slack posting, ticket comments,
-   etc can be instrumented in continuous integration from the structured notes.
+3. Other automations, such as version bumping, Slack posting, ticket comments, etc can be instrumented in continuous integration from the structured notes.
 
-When contributing a change, call ``detail`` to be prompted for all information
-defined in the project's detail schema. Information can be collected conditionally
-based on previous steps all thanks to the `formaldict <https://github.com/Opus10/formaldict>`__ library.
+When contributing a change, call `detail` to be prompted for all information defined in the project's detail schema. Information can be collected conditionally based on previous steps all thanks to the [formaldict](https://github.com/Opus10/formaldict) library.
 
-Below is an example of a contributor creating a structured note with the type
-of change they are making, a summary, a description, and an associated Jira
-ticket:
+Below is an example of a contributor creating a structured note with the type of change they are making, a summary, a description, and an associated Jira ticket:
 
-.. image:: https://raw.githubusercontent.com/opus10/detail/master/docs/_static/detail-intro.gif
-    :width: 600
+![intro.gif](https://raw.githubusercontent.com/opus10/detail/main/docs/static/detail-intro.gif)
 
-Notes are commited to projects, allowing review of them before they are used to
-perform automations in continuous integration.
+Notes are commited to projects, allowing review of them before they are used to perform automations in continuous integration.
 
-Documentation
-=============
+## Documentation
 
-`View the detail docs here
-<https://detail.readthedocs.io/>`_.
+[View the detail docs here](https://detail.readthedocs.io/).
 
-Installation
-============
+## Installation
 
-Install detail with::
+Install detail with:
 
     pip3 install detail
 
 
-Contributing Guide
-==================
+## Contributing Guide
 
-For information on setting up detail for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+For information on setting up detail for development and contributing changes, view [CONTRIBUTING.rst](CONTRIBUTING.rst).
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
 - @tomage (Tómas Árni Jónasson)
```

### Comparing `detail-0.2.2/detail/cli.py` & `detail-0.2.3/detail/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Commands
 ~~~~~~~~
 
 * ``detail`` - Creates a note
 * ``detail log`` - Renders templated notes
 * ``detail lint`` - Validates structure of notes
 """
+
 import sys
 
 import click
 from click_default_group import DefaultGroup
 
 import detail as detail_module
 from detail import core
```

### Comparing `detail-0.2.2/detail/core.py` & `detail-0.2.3/detail/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 The core detail API
 """
 
+from __future__ import annotations
+
 import collections.abc
 import datetime as dt
 import io
 import re
 import subprocess
 import uuid
+from typing import Optional, Tuple
 
 import dateutil.parser
 import formaldict
 import jinja2
 import yaml
 
-from detail import exceptions
-from detail import github
-from detail import utils
-
+from detail import exceptions, github, utils
 
 # The default log Jinja template
 DEFAULT_LOG_TEMPLATE = """
 {% for tag, notes_by_tag in notes.group('commit_tag').items() %}
 ## {{ tag|default('Unreleased', True) }} {% if tag.date %}({{ tag.date.date() }}){% endif %}
 {% for note in notes_by_tag %}
 - {{ note.commit_author_name }} [{{ note.commit_sha[:7] }}]
@@ -113,18 +113,18 @@
 def _load_note_schema(path=None):
     """Loads the detail schema"""
     path = path or utils.get_detail_schema_path()
 
     try:
         with open(path, "r") as schema_f:
             schema = yaml.safe_load(schema_f)
-    except IOError:
+    except IOError as exc:
         raise exceptions.SchemaError(
             'Must create a schema.yaml in the ".detail" directory of your project'
-        )
+        ) from exc
 
     for entry in schema:
         if "label" not in entry:
             raise exceptions.SchemaError(f"Entry in schema does not have label - {entry}")
 
     return formaldict.Schema(schema)
 
@@ -132,40 +132,40 @@
 class Tag(collections.UserString):
     """A git tag."""
 
     def __init__(self, tag):
         self.data = tag
 
     @classmethod
-    def from_sha(cls, sha, tag_match=None):
+    def from_sha(cls, sha, tag_match=None) -> Optional[Tag]:
         """
         Create a Tag object from a sha or return None if there is no
         associated tag
 
         Returns:
-            Tag: A constructed tag or ``None`` if no tags contain the commit.
+            A constructed tag or ``None`` if no tags contain the commit.
         """
         describe_cmd = f"git describe {sha} --contains"
         if tag_match:
             describe_cmd += f" --match={tag_match}"
 
         rev = (
             utils.shell_stdout(describe_cmd, check=False, stderr=subprocess.PIPE)
             .replace("~", ":")
             .replace("^", ":")
         )
         return cls(rev.split(":")[0]) if rev else None
 
     @property
-    def date(self):
+    def date(self) -> Optional[dt.datetime]:
         """
         Parse the date of the tag
 
         Returns:
-            datetime: The tag parsed as a datetime object.
+            The tag parsed as a datetime object.
         """
         if not hasattr(self, "_date"):
             try:
                 self._date = dateutil.parser.parse(
                     utils.shell_stdout(f"git log -1 --format=%ad {self}")
                 )
             except dateutil.parser.ParserError:
@@ -270,66 +270,65 @@
 
     def __getitem__(self, i):
         return self._notes[i]
 
     def __len__(self):
         return len(self._notes)
 
-    def filter(self, attr, value, match=False):
+    def filter(self, attr, value, match=False) -> Notes:
         """Filter notes by an attribute
 
         Args:
             attr (str): The name of the attribute on the `Note` object.
             value (str|bool): The value to filter by.
             match (bool, default=False): Treat ``value`` as a regex pattern and
                 match against it.
 
         Returns:
-            `Notes`: The filtered notes.
+            The filtered notes.
         """
         return Notes([note for note in self if _equals(getattr(note, attr), value, match=match)])
 
-    def exclude(self, attr, value, match=False):
+    def exclude(self, attr, value, match=False) -> Notes:
         """Exclude notes by an attribute
 
         Args:
             attr (str): The name of the attribute on the `Note` object.
             value (str|bool): The value to exclude by.
             match (bool, default=False): Treat ``value`` as a regex pattern and
                 match against it.
 
         Returns:
-            `Notes`: The excluded commits.
+            The excluded commits.
         """
         return Notes(
             [note for note in self if not _equals(getattr(note, attr), value, match=match)]
         )
 
     def group(
         self,
         attr,
         ascending_keys=False,
         descending_keys=False,
         none_key_first=False,
         none_key_last=False,
-    ):
+    ) -> collections.OrderedDict[str, Notes]:
         """Group notes by an attribute
 
         Args:
             attr (str): The attribute to group by.
             ascending_keys (bool, default=False): Sort the keys in ascending
                 order.
             descending_keys (bool, default=False): Sort the keys in descending
                 order.
             none_key_first (bool, default=False): Make the "None" key be first.
             none_key_last (bool, default=False): Make the "None" key be last.
 
         Returns:
-            `collections.OrderedDict`: A dictionary of `Notes` keyed on
-            groups.
+            A dictionary of `Notes` keyed on groups.
         """
         if any([ascending_keys, descending_keys]) and not any([none_key_first, none_key_last]):
             # If keys are sorted, default to making the "None" key last
             none_key_last = True
 
         # Get the natural ordering of the keys
         keys = list(collections.OrderedDict((getattr(note, attr), True) for note in self).keys())
@@ -485,50 +484,50 @@
                 )
                 for path, data, sha in note_log
                 if data
             ]
         )
 
 
-def detail(path=None):
+def detail(path: Optional[str] = None) -> Tuple[str, formaldict.FormalDict]:
     """
     Creates or updates a note
 
     Arguments:
         path (str, default=None): A path to an existing note.
             If provided, the note will be updated.
 
     Returns:
-        subprocess.CompletedProcess: The result from running
-        git commit. Returns the git pre-commit hook results if
-        failing during hook execution.
+        The result from running git commit. Returns the git pre-commit
+        hook results if failing during hook execution.
     """
     defaults = {}
     if path:
         with open(path) as f:
             defaults = yaml.safe_load(f.read())
     else:
-        now = dt.datetime.utcnow()
-        path = (
+        now = dt.datetime.now(dt.timezone.utc)
+        autopath = (
             utils.get_detail_note_root()
             / f'{now.strftime("%Y-%m-%d")}-{str(uuid.uuid4())[:6]}.yaml'
         )
-        path.parent.mkdir(exist_ok=True, parents=True)
+        autopath.parent.mkdir(exist_ok=True, parents=True)
+        path = str(autopath)
 
     schema = _load_note_schema()
     entry = schema.prompt(defaults=defaults)
     serialized = yaml.dump(entry.data, default_style="|")
 
     with open(path, "w") as f:
         f.write(serialized)
 
     return path, entry
 
 
-def lint(range=""):
+def lint(range="") -> Tuple[bool, Notes]:
     """
     Lint notes against a range (branch, sha, etc).
 
     Linting passes when either succeed:
 
     - No commits are in the range.
     - Commits are found, and all notes pass linting. At least one
@@ -565,15 +564,15 @@
     style="default",
     template=None,
     tag_match=None,
     before=None,
     after=None,
     reverse=False,
     output=None,
-):
+) -> str:
     """
     Renders notes.
 
     Args:
         range (str, default=''): The git revision range over which logs are
             output. Using ":github/pr" as the range will use the base branch
             of an open github pull request as the range. No range will result
@@ -600,15 +599,15 @@
     Raises:
         `NoGithubPullRequestFoundError`: When using ``:github/pr`` as
             the range and no pull requests are found.
         `MultipleGithubPullRequestsFoundError`: When using ``:github/pr`` as
             the range and multiple pull requests are found.
 
     Returns:
-        str: The rendered log.
+        The rendered log.
     """
     notes = NoteRange(
         range=range,
         tag_match=tag_match,
         before=before,
         after=after,
         reverse=reverse,
```

### Comparing `detail-0.2.2/detail/exceptions.py` & `detail-0.2.3/detail/exceptions.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.2/detail/github.py` & `detail-0.2.3/detail/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 Utilities for accessing Github
 """
 
 import os
 
 import requests
 
-from detail import exceptions
-from detail import utils
-
+from detail import exceptions, utils
 
 GITHUB_API_TOKEN_ENV_VAR = "GITHUB_API_TOKEN"
 GITHUB_USERNAME_ENV_VAR = "GITHUB_USERNAME"
 
 
 def get_org_and_repo_name():
     remote_url = utils.shell_stdout("git remote get-url origin")
```

### Comparing `detail-0.2.2/detail/tests/test_cli.py` & `detail-0.2.3/detail/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.2/detail/tests/test_core.py` & `detail-0.2.3/detail/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Tests the detail.core module
 
 Most of the test coverage of the core module is from the integration
 tests in detail/tests/test_integration.py.
 """
+
 from contextlib import ExitStack as does_not_raise
 from unittest import mock
 
 import pytest
 
-from detail import core
-from detail import exceptions
-
+from detail import core, exceptions
 
 # A valid user schema
 valid_schema = """
 - label: type
 - label: summary
 - label: description
   condition: ['!=', 'type', 'trivial']
```

### Comparing `detail-0.2.2/detail/tests/test_github.py` & `detail-0.2.3/detail/tests/test_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests for the detail.github module"""
-from contextlib import ExitStack as does_not_raise
+
 import json
+from contextlib import ExitStack as does_not_raise
 from unittest import mock
 
 import pytest
 import requests
 
-from detail import exceptions
-from detail import github
+from detail import exceptions, github
 
 
 @pytest.fixture(autouse=True)
 def setup_github_env_vars(monkeypatch):
     monkeypatch.setenv("GITHUB_API_TOKEN", "github_token")
```

### Comparing `detail-0.2.2/detail/tests/test_integration.py` & `detail-0.2.3/detail/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Integration tests for detail"""
-from contextlib import ExitStack as does_not_raise
+
 import io
 import os
 import pathlib
 import shutil
+from contextlib import ExitStack as does_not_raise
 
 import formaldict
 import jinja2.exceptions
 import pytest
 import yaml
 
-from detail import core
-from detail import utils
+from detail import core, utils
 
 
 @pytest.fixture()
 def detail_config(tmp_path, mocker):
     """Creates an example detail config for integration tests"""
     detail_root = tmp_path / ".detail"
     detail_root.mkdir()
@@ -184,15 +184,15 @@
     assert (
         str(invalid_note.validation_errors)
         == 'jira: Value "INVALID" does not match pattern "WEB-[\\d]+".'
     )
     assert invalid_note.type == "feature"
     assert not invalid_note.is_valid
     with pytest.raises(AttributeError):
-        invalid_note.invalid_attribute
+        invalid_note.invalid_attribute  # noqa
     assert invalid_note.jira is None
     assert invalid_note.commit_tag is None
 
     api_break_note = list(nr.filter("type", "api-break"))[0]
     assert str(api_break_note.commit.tag) == "v1.1"
 
     # Check various filterings on the range
```

### Comparing `detail-0.2.2/detail/tests/test_utils.py` & `detail-0.2.3/detail/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests the detail.utils() module"""
+
 from detail import utils
 
 
 def test_shell_stdout():
     """Tests utils.shell_stdout()"""
     assert utils.shell_stdout('echo "hello world"') == "hello world"
```

### Comparing `detail-0.2.2/detail/utils.py` & `detail-0.2.3/detail/utils.py`

 * *Files identical despite different names*

### Comparing `detail-0.2.2/pyproject.toml` & `detail-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,97 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py37']
-
 [tool.coverage.run]
 branch = true
 source = ["detail"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "detail"
 packages = [
   { include = "detail" },
 ]
-version = "0.2.2"
+version = "0.2.3"
 description = "Build automations off of structured notes in your project"
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 license = "BSD-3-Clause"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/Opus10/detail"
 repository = "https://github.com/Opus10/detail"
 documentation = "https://detail.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
-importlib_metadata = { version = ">=4", python = "~3.7" }
+python = ">=3.8.0,<4"
 click = ">=7.0"
 click-default-group = ">=1.2.2"
 formaldict = ">=0.2.0"
 jinja2 = ">=2.10.3"
 python-dateutil = ">=2.8.1"
-pyyaml = ">=5.1.2"
+pyyaml = ">=5.1.2,<=5.3.1"
 requests = ">=2.22.0"
 
 [tool.poetry.dev-dependencies]
-black = "22.1.0"
-flake8 = "3.9.2"
-flake8-bugbear = "22.1.11"
-flake8-comprehensions = "3.8.0"
-flake8-import-order = "0.18.1"
-flake8-logging-format = "0.6.0"
-flake8-mutable = "1.2.0"
-footing = "*"
-git-tidy = "1.1.1"
-myst-parser = "0.18.0"
-pytest = "6.2.5"
-pytest-cov = "3.0.0"
+git-tidy = "1.2.0"
+pytest = "7.4.2"
+pytest-cov = "4.1.0"
+pytest-dotenv = "0.5.2"
 pytest-mock = "3.7.0"
-pytest-responses = "0.5.0"
-Sphinx = "4.4.0"
-sphinx-click = "3.0.0"
-sphinx-rtd-theme = "1.0.0"
-tox = "3.24.5"
+pytest-responses = "0.5.1"
+tox = "4.11.3"
+ruff = "0.3.7"
+pyright = "1.1.358"
+mkdocs = "1.5.3"
+black = "24.4.0"
+mkdocs-material = "9.5.18"
+mkdocstrings-python = "1.9.2"
+footing = "*"
+setuptools = "*"
+poetry-core = "*"
 
 [tool.poetry.scripts]
 detail = 'detail.cli:main'
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "detail/tests"
 norecursedirs = ".venv"
+
+[tool.ruff]
+lint.select = ["E", "F", "B", "I", "G", "C4"]
+line-length = 99
+target-version = "py38"
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/migrations/**",
+    "**/tests/**",
+]
+pythonVersion = "3.8"
+typeCheckingMode = "standard"
```

### Comparing `detail-0.2.2/PKG-INFO` & `detail-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,68 @@
 Metadata-Version: 2.1
 Name: detail
-Version: 0.2.2
+Version: 0.2.3
 Summary: Build automations off of structured notes in your project
 Home-page: https://github.com/Opus10/detail
 License: BSD-3-Clause
 Author: Opus 10 Engineering
-Requires-Python: >=3.7.0,<4
+Requires-Python: >=3.8.0,<4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: click (>=7.0)
 Requires-Dist: click-default-group (>=1.2.2)
 Requires-Dist: formaldict (>=0.2.0)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: python-dateutil (>=2.8.1)
-Requires-Dist: pyyaml (>=5.1.2)
+Requires-Dist: pyyaml (>=5.1.2,<=5.3.1)
 Requires-Dist: requests (>=2.22.0)
 Project-URL: Documentation, https://detail.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/detail
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-detail
-#######
+# detail
 
-``detail`` allows contributors to create structured and configurable notes in a project,
-providing the ability to do automations such as:
+`detail` allows contributors to create structured and configurable notes in a project, providing the ability to do automations such as:
 
-1. Ensuring that contributors add information to pull requests that provide
-   QA instructions, release notes, and associated tickets. The ``detail lint`` command
-   ensures that notes are present in a pull request and adhere to the schema.
+1. Ensuring that contributors add information to pull requests that provide QA instructions, release notes, and associated tickets. The `detail lint` command ensures that notes are present in a pull request and adhere to the schema.
 
-2. Rendering dynamic logs from the notes. ``detail log`` provides the ability
-   to slice and dice the commit log however you need, pulling in a ``notes``
-   variable in a Jinja template with all notes that can be grouped and filtered.
+2. Rendering dynamic logs from the notes. `detail log` provides the ability to slice and dice the commit log however you need, pulling in a `notes` variable in a Jinja template with all notes that can be grouped and filtered.
 
-3. Other automations, such as version bumping, Slack posting, ticket comments,
-   etc can be instrumented in continuous integration from the structured notes.
+3. Other automations, such as version bumping, Slack posting, ticket comments, etc can be instrumented in continuous integration from the structured notes.
 
-When contributing a change, call ``detail`` to be prompted for all information
-defined in the project's detail schema. Information can be collected conditionally
-based on previous steps all thanks to the `formaldict <https://github.com/Opus10/formaldict>`__ library.
+When contributing a change, call `detail` to be prompted for all information defined in the project's detail schema. Information can be collected conditionally based on previous steps all thanks to the [formaldict](https://github.com/Opus10/formaldict) library.
 
-Below is an example of a contributor creating a structured note with the type
-of change they are making, a summary, a description, and an associated Jira
-ticket:
+Below is an example of a contributor creating a structured note with the type of change they are making, a summary, a description, and an associated Jira ticket:
 
-.. image:: https://raw.githubusercontent.com/opus10/detail/master/docs/_static/detail-intro.gif
-    :width: 600
+![intro.gif](https://raw.githubusercontent.com/opus10/detail/main/docs/static/detail-intro.gif)
 
-Notes are commited to projects, allowing review of them before they are used to
-perform automations in continuous integration.
+Notes are commited to projects, allowing review of them before they are used to perform automations in continuous integration.
 
-Documentation
-=============
+## Documentation
 
-`View the detail docs here
-<https://detail.readthedocs.io/>`_.
+[View the detail docs here](https://detail.readthedocs.io/).
 
-Installation
-============
+## Installation
 
-Install detail with::
+Install detail with:
 
     pip3 install detail
 
 
-Contributing Guide
-==================
+## Contributing Guide
 
-For information on setting up detail for development and
-contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+For information on setting up detail for development and contributing changes, view [CONTRIBUTING.rst](CONTRIBUTING.rst).
 
-Primary Authors
-===============
+## Creators
 
 - @wesleykendall (Wes Kendall)
 - @tomage (Tómas Árni Jónasson)
```

