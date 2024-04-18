# Comparing `tmp/polymatch-0.4.0.tar.gz` & `tmp/polymatch-0.4.1.tar.gz`

## Comparing `polymatch-0.4.0.tar` & `polymatch-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 polymatch-0.4.0/.editorconfig
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 polymatch-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 polymatch-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 polymatch-0.4.0/codecov.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 polymatch-0.4.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 polymatch-0.4.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polymatch-0.4.0/.vscode/extensions.json
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 polymatch-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/_version.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/base.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/py.typed
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/glob.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/regex.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/base_test.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_glob.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_pickling.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_regex.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_registry.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_standard.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 polymatch-0.4.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 polymatch-0.4.0/LICENSE
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 polymatch-0.4.0/README.md
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 polymatch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 polymatch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 polymatch-0.4.1/.editorconfig
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 polymatch-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 polymatch-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 polymatch-0.4.1/codecov.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 polymatch-0.4.1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 polymatch-0.4.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 polymatch-0.4.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 polymatch-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/_version.py
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/base.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/py.typed
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/registry.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/matchers/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/matchers/glob.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/matchers/regex.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 polymatch-0.4.1/polymatch/matchers/standard.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/base_test.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/test_glob.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/test_pickling.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/test_regex.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/test_registry.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 polymatch-0.4.1/tests/test_standard.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 polymatch-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 polymatch-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 polymatch-0.4.1/README.md
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 polymatch-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 polymatch-0.4.1/PKG-INFO
```

### Comparing `polymatch-0.4.0/.pre-commit-config.yaml` & `polymatch-0.4.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     - --autofix
     - --no-sort-keys
     exclude: ^\.(vscode|devcontainer)/
     id: pretty-format-json
   - id: check-toml
   repo: https://github.com/pre-commit/pre-commit-hooks
   rev: 2c9f875913ee60ca25ce70243dc24d5b6415598c
+- repo: https://github.com/bwhmather/ssort
+  rev: dcb59fdb9b46ed1bb8e6ca2107e35f76cdc9c97e  # frozen: 0.12.4
+  hooks:
+  - id: ssort
 - hooks:
   - id: black
   repo: https://github.com/psf/black
   rev: 8fe627072f15ff2e3d380887b92f7868efaf6d05
 - hooks:
   - id: isort
   repo: https://github.com/pycqa/isort
```

### Comparing `polymatch-0.4.0/.devcontainer/devcontainer.json` & `polymatch-0.4.1/.devcontainer/devcontainer.json`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,16 @@
                 "EditorConfig.EditorConfig",
                 "GitHub.vscode-pull-request-github",
                 "github.vscode-github-actions",
                 "redhat.vscode-yaml",
                 "ms-python.black-formatter",
                 "ms-python.isort",
                 "ms-azuretools.vscode-docker",
-                "ms-python.mypy-type-checker"
+                "ms-python.mypy-type-checker",
+                "sunipkm.autodocstringpy"
             ],
             "settings": {
                 "python.defaultInterpreterPath": "~/.virtualenvs/polymatch/bin/python",
                 "python.testing.pytestArgs": ["--no-cov"],
                 "terminal.integrated.profiles.linux": {
                     "zsh": {
                         "path": "/usr/bin/zsh"
```

### Comparing `polymatch-0.4.0/polymatch/__init__.py` & `polymatch-0.4.1/polymatch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+"""Polymorphic pattern matchers."""
+
+from polymatch._version import (
+    __version__,
+    __version_tuple__,
+    version,
+    version_tuple,
+)
 from polymatch.base import CaseAction, PolymorphicMatcher
 from polymatch.error import (
     DuplicateMatcherRegistrationError,
     NoMatchersAvailableError,
     NoSuchMatcherError,
     PatternCompileError,
     PatternNotCompiledError,
     PatternTextTypeMismatchError,
 )
 from polymatch.registry import pattern_registry
 
-__version__ = "0.3.0"
-
 __all__ = [
+    "__version__",
+    "__version_tuple__",
+    "version",
+    "version_tuple",
     "PolymorphicMatcher",
     "CaseAction",
     "pattern_registry",
     "NoSuchMatcherError",
     "NoMatchersAvailableError",
     "PatternNotCompiledError",
     "PatternCompileError",
```

### Comparing `polymatch-0.4.0/polymatch/matchers/glob.py` & `polymatch-0.4.1/polymatch/matchers/glob.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,35 @@
+"""Glob pattern matcher."""
+
 from fnmatch import translate
 from typing import TYPE_CHECKING, AnyStr
 
 from polymatch.matchers.regex import RegexMatcher
 
 if TYPE_CHECKING:
     import regex
 
 
 class GlobMatcher(RegexMatcher[AnyStr]):
+    """Match glob patterns.
+
+    Implemented as a subclass of RegexMatcher, glob patterns are translated to regex on compilation.
+    """
+
     def compile_pattern(
         self, raw_pattern: AnyStr, *, flags: int = 0
     ) -> "regex.Pattern[AnyStr]":
+        """Override RegexMatcher compile to transform glob-syntax."""
         if isinstance(raw_pattern, str):
             res = translate(raw_pattern)
         else:
             # Mimic how fnmatch handles bytes patterns
             pat_str = str(raw_pattern, "ISO-8859-1")
             res_str = translate(pat_str)
             res = bytes(res_str, "ISO-8859-1")
 
         return RegexMatcher.compile_pattern(self, res, flags=flags)
 
     @classmethod
     def get_type(cls) -> str:
+        """Pattern type."""
         return "glob"
```

### Comparing `polymatch-0.4.0/tests/base_test.py` & `polymatch-0.4.1/tests/base_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+"""Test base patterns."""
+
 import pytest
 
 from polymatch import pattern_registry
 from polymatch.base import CaseAction
 from polymatch.error import (
     PatternNotCompiledError,
     PatternTextTypeMismatchError,
 )
 from polymatch.matchers.standard import ExactMatcher
 
 
 def test_case_action_validate() -> None:
+    """Ensure an informative error is raised when a bytes pattern is configured with casefolding."""
     with pytest.raises(
         TypeError, match="Case-folding is not supported with bytes patterns"
     ):
         _ = ExactMatcher(b"foo", CaseAction.CASEFOLD)
 
 
 def test_type_mismatch() -> None:
+    """Test comparing a bytes pattern against a string."""
     matcher = ExactMatcher(b"foo", CaseAction.CASEINSENSITIVE)
     with pytest.raises(PatternTextTypeMismatchError):
         matcher.match("foo")  # type: ignore[arg-type]
 
 
 def test_compare() -> None:
+    """Test basic comparison."""
     matcher = pattern_registry.pattern_from_string("exact:ci:foo")
     matcher.compile()
     res = matcher == 123
     assert not res
     res = matcher != "aaaaa"
     assert res
     res = matcher != "foo"
     assert not res
     res = matcher != 123
     assert res
 
 
 def test_compare_invert() -> None:
+    """Test inverted compare."""
     matcher = pattern_registry.pattern_from_string("~exact:ci:foo")
     matcher.compile()
     assert matcher == "lekndlwkn"
     assert matcher != "FOO"
 
 
 def test_compare_no_compile() -> None:
+    """Test comparing against an uncompiled pattern."""
     matcher = pattern_registry.pattern_from_string("~exact:ci:foo")
     with pytest.raises(PatternNotCompiledError):
         matcher.match("foo")
```

### Comparing `polymatch-0.4.0/tests/test_glob.py` & `polymatch-0.4.1/tests/test_glob.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test glob matcher."""
+
 import pytest
 
 from polymatch import pattern_registry
 
 data = (
     ("glob::*", "", True),
     ("glob::*?", "", False),
@@ -11,16 +13,18 @@
     (b"glob:*!*@thing", b"itd!a@thing", True),
     (b"glob:*!*@thing", b"itd!a@THING", False),
 )
 
 
 @pytest.mark.parametrize(("pattern", "text", "result"), data)
 def test_patterns(pattern: str, text: str, result: bool) -> None:
+    """Ensure various patterns match their expected text."""
     matcher = pattern_registry.pattern_from_string(pattern)
     matcher.compile()
     assert bool(matcher == text) is result
 
 
 def test_invert() -> None:
+    """Ensure parsing inverted pattern works."""
     pattern = pattern_registry.pattern_from_string("~glob::beep")
     pattern.compile()
     assert pattern.inverted
```

### Comparing `polymatch-0.4.0/tests/test_pickling.py` & `polymatch-0.4.1/tests/test_pickling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+"""Test pickling the pattern objects."""
+
 import itertools
 import pickle
 from typing import Any, TypeVar, cast
 
 import pytest
 
 import polymatch
 from polymatch import pattern_registry
 from polymatch.base import PolymorphicMatcher
 
 patterns = ("regex::test", "exact::test", "contains:cf:test", "glob::beep")
 
 
 class C:
+    """Test object for pickling list of patterns."""
+
     def __init__(self, pat: PolymorphicMatcher[Any, Any]) -> None:
+        """Construct testing object."""
         self.patterns = [pat]
 
 
 T = TypeVar("T")
 
 
 def cycle_pickle(obj: T, proto: int) -> T:
+    """Pickle and unpickle an item, and return the result."""
     return cast(T, pickle.loads(pickle.dumps(obj, proto)))
 
 
 @pytest.mark.parametrize(
     ("pattern", "pickle_proto"),
     itertools.product(patterns, range(pickle.HIGHEST_PROTOCOL + 1)),
 )
 def test_compile_state(pattern: str, pickle_proto: int) -> None:
+    """Ensure the compile state is preserved."""
     compiled_pattern = pattern_registry.pattern_from_string(pattern)
     compiled_pattern.compile()
 
     assert compiled_pattern.is_compiled()
 
     uncompiled_pattern = pattern_registry.pattern_from_string(pattern)
 
@@ -47,14 +54,15 @@
 
 
 @pytest.mark.parametrize(
     ("pattern", "pickle_proto"),
     itertools.product(patterns, range(pickle.HIGHEST_PROTOCOL + 1)),
 )
 def test_properties(pattern: str, pickle_proto: int) -> None:
+    """Ensure pattern properties are preserved (e.g. inverted state)."""
     pat = pattern_registry.pattern_from_string(pattern)
     pat.compile()
 
     inv_pat = pattern_registry.pattern_from_string(f"~{pattern}")
     inv_pat.compile()
 
     assert not pat.inverted
@@ -74,22 +82,23 @@
 
 
 @pytest.mark.parametrize(
     ("pattern", "pickle_proto"),
     itertools.product(patterns, range(pickle.HIGHEST_PROTOCOL + 1)),
 )
 def test_version_checks(pattern: str, pickle_proto: int) -> None:
+    """Ensure pattern is recompiled when pickled compiled and library version changes."""
     pat = pattern_registry.pattern_from_string(pattern)
     pat.compile()
 
     assert pat.is_compiled()
 
     data = pickle.dumps(pat, pickle_proto)
 
     # Change version
     v = polymatch.__version__.split(".")
-    v[-1] = str(int(v[-1]) + 1)
+    v[0] = str(int(v[0]) + 1)
     polymatch.__version__ = ".".join(v)
 
     new_pat = pickle.loads(data)
 
     assert new_pat.is_compiled()
```

### Comparing `polymatch-0.4.0/tests/test_regex.py` & `polymatch-0.4.1/tests/test_regex.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test regex matcher."""
+
 import pytest
 
 from polymatch import pattern_registry
 
 data = (
     (r"regex::\btest\b", "test", True),
     (r"regex::\btest\b", "test1", False),
@@ -12,16 +14,18 @@
     (r"regex:ci:foo", "FOO", True),
     (r"regex:ci:foo", "foo", True),
 )
 
 
 @pytest.mark.parametrize(("pattern", "text", "result"), data)
 def test_patterns(pattern: str, text: str, result: bool) -> None:
+    """Test various patterns against different inputs."""
     matcher = pattern_registry.pattern_from_string(pattern)
     matcher.compile()
     assert bool(matcher == text) is result
 
 
 def test_invert() -> None:
+    """Test pattern invert."""
     pattern = pattern_registry.pattern_from_string("~regex::beep")
     pattern.compile()
     assert pattern.inverted
```

### Comparing `polymatch-0.4.0/tests/test_registry.py` & `polymatch-0.4.1/tests/test_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test the pattern registry."""
+
 import pytest
 
 from polymatch import pattern_registry
 from polymatch.base import CaseAction
 from polymatch.error import (
     DuplicateMatcherRegistrationError,
     NoMatchersAvailableError,
@@ -9,67 +11,76 @@
 )
 from polymatch.matchers.glob import GlobMatcher
 from polymatch.matchers.standard import ExactMatcher
 from polymatch.registry import PatternMatcherRegistry
 
 
 def test_register_duplicate() -> None:
+    """Test registering duplicate matchers."""
     registry = PatternMatcherRegistry()
     registry.register(GlobMatcher)
     with pytest.raises(DuplicateMatcherRegistrationError):
         registry.register(GlobMatcher)
 
 
 def test_register_non_pattern() -> None:
+    """Test registering something that isn't a PolymorphicMatcher."""
     registry = PatternMatcherRegistry()
     with pytest.raises(TypeError):
         registry.register(object)
 
 
 def test_parse() -> None:
+    """Test parsing a basic pattern."""
     matcher = pattern_registry.pattern_from_string("foo")
     matcher.compile()
     assert matcher.match("foo")
     assert not matcher.match("Foo")
     assert isinstance(matcher, ExactMatcher)
     assert not matcher.inverted
     assert matcher.case_action == CaseAction.NONE
 
 
 def test_parse_error_bad_type() -> None:
+    """Ensure an error is raised when an incorrect type is given to pattern_from_string()."""
     with pytest.raises(
         TypeError, match="Unable to parse pattern string of type 'int'"
     ):
         pattern_registry.pattern_from_string(27)  # type: ignore[type-var]
 
 
 def test_parse_error_no_matcher() -> None:
+    """Ensure an error is raised when no matching pattern handler exists."""
     with pytest.raises(LookupError, match="av"):
         pattern_registry.pattern_from_string("av:cs:foo")
 
 
 def test_parse_error_no_case_action() -> None:
+    """Ensure an error is raised when an invalid CaseAction is given."""
     with pytest.raises(LookupError, match="av"):
         pattern_registry.pattern_from_string("regex:av:foo")
 
 
 def test_parse_error_no_default_matcher() -> None:
+    """Test that the correct error is thrown when no default matcher exists."""
     registry = PatternMatcherRegistry()
     with pytest.raises(NoMatchersAvailableError):
         registry.pattern_from_string("foo")
 
 
 @pytest.mark.parametrize(
     ("pattern", "success"), [("regex:foo\\\\a[-{", False), ("foo", True)]
 )
 def test_parse_error_bad_regex(pattern: str, success: bool) -> None:
+    """Ensure parse errors cause try_compile() to return False."""
     matcher = pattern_registry.pattern_from_string(pattern)
     assert matcher.try_compile() is success
 
 
 def test_remove() -> None:
+    """Ensure removing a pattern class from the registry works."""
     registry = PatternMatcherRegistry()
     registry.register(GlobMatcher)
     assert registry["glob"] is GlobMatcher
     registry.remove("glob")
     with pytest.raises(NoSuchMatcherError):
         registry["glob"]
```

### Comparing `polymatch-0.4.0/tests/test_standard.py` & `polymatch-0.4.1/tests/test_standard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Test standard matchers."""
+
 import pytest
 
 from polymatch import pattern_registry
 
 data = (
     ("exact::a", "a", True),
     ("exact::b", "n", False),
@@ -20,86 +22,104 @@
     ("contains:ci:i", "AIR", True),
     ("contains:cf:i", "AIR", True),
 )
 
 
 @pytest.mark.parametrize(("pattern", "text", "result"), data)
 def test_patterns(pattern: str, text: str, result: bool) -> None:
+    """Test expected pattern matches.
+
+    Args:
+        pattern: Pattern string to test.
+        text: Text to match against.
+        result: Whether the text is expected to match.
+    """
     matcher = pattern_registry.pattern_from_string(pattern)
     matcher.compile()
     assert bool(matcher == text) is result
 
 
 def test_invert() -> None:
+    """Ensure inverted patterns are parsed correctly."""
     pattern = pattern_registry.pattern_from_string("~exact::beep")
     pattern.compile()
     assert pattern.inverted
 
 
 def test_repr() -> None:
+    """Ensure __repr__() for strings patterns represents the pattern text."""
     pattern = pattern_registry.pattern_from_string("~exact:ci:beep")
     pattern.compile()
     assert (
         repr(pattern)
         == "ExactMatcher(pattern='beep', case_action=CaseAction.CASEINSENSITIVE, invert=True)"
     )
 
 
 def test_repr_bytes() -> None:
+    """Ensure __repr__() for bytes patterns represents the pattern text."""
     pattern = pattern_registry.pattern_from_string(b"~exact:ci:beep")
     pattern.compile()
     assert (
         repr(pattern)
         == "ExactMatcher(pattern=b'beep', case_action=CaseAction.CASEINSENSITIVE, invert=True)"
     )
 
 
 def test_str() -> None:
+    """Ensure that __str__() on string patterns always returns strings."""
     pattern = pattern_registry.pattern_from_string("~exact:ci:beep")
     pattern.compile()
     assert str(pattern) == "~exact:ci:beep"
 
 
 def test_str_bytes() -> None:
+    """Ensure that __str__() on bytes patterns always returns strings."""
     pattern = pattern_registry.pattern_from_string(b"~exact:ci:beep")
     pattern.compile()
     assert str(pattern) == "~exact:ci:beep"
 
 
 def test_to_string() -> None:
+    """Ensure string patterns serialize to strings."""
     pattern = pattern_registry.pattern_from_string("~exact:ci:beep")
     pattern.compile()
     assert pattern.to_string() == "~exact:ci:beep"
 
 
 def test_to_string_bytes() -> None:
+    """Ensure bytes patterns serialize to bytes."""
     pattern = pattern_registry.pattern_from_string(b"~exact:ci:beep")
     pattern.compile()
     assert pattern.to_string() == b"~exact:ci:beep"
 
 
 def test_cf_match_bytes() -> None:
+    """Test exact matcher match_text_cf() handling of bytes objects."""
     matcher = pattern_registry.pattern_from_string("~exact:ci:foo")
     matcher.compile()
     with pytest.raises(TypeError):
         matcher.match_text_cf(b"cc", b"foo")
 
 
 def test_cf_compile_bytes_bypass() -> None:
+    """Test exact matcher compile_pattern_cf() handling of bytes objects."""
     matcher = pattern_registry.pattern_from_string("~exact:cf:foo")
     matcher.compile()
     with pytest.raises(TypeError):
         matcher.compile_pattern_cf(b"foo")
 
 
 def test_contains_cf_match_bytes() -> None:
+    """Test what happens if a bytes object somehow hits match_text_cf()."""
     matcher = pattern_registry.pattern_from_string("contains:cf:foo")
     matcher.compile()
     with pytest.raises(TypeError):
         matcher.match_text_cf(b"cc", b"foo")
 
 
 def test_contains_cf_compile_bytes_bypass() -> None:
+    """Test what happens if a bytes object somehow hits compile_pattern_cf()."""
     matcher = pattern_registry.pattern_from_string("contains:cf:foo")
     matcher.compile()
     with pytest.raises(TypeError):
         matcher.compile_pattern_cf(b"foo")
```

### Comparing `polymatch-0.4.0/.gitignore` & `polymatch-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.0/LICENSE` & `polymatch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.0/README.md` & `polymatch-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # poly-match
 Python Polymorphic Pattern Matching library
 
 [![CI - Test](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-tests.yml/badge.svg)](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-tests.yml)
 [![CD - Build](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-publish.yml/badge.svg)](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/gh/TotallyNotRobots/poly-match/graph/badge.svg?token=nJqN3RacOa)](https://codecov.io/gh/TotallyNotRobots/poly-match)
 
-[![PyPI - Version](https://img.shields.io/pypi/v/polymatch.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/polymatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/polymatch.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/polymatch/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polymatch.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/polymatch/)
+[![PyPI - Version](https://img.shields.io/pypi/v/polymatch.svg)](https://pypi.org/project/polymatch/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/polymatch.svg)](https://pypi.org/project/polymatch/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polymatch.svg)](https://pypi.org/project/polymatch/)
 
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
```

### Comparing `polymatch-0.4.0/pyproject.toml` & `polymatch-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,18 @@
     "FLY002",
     "TCH001",
     "TCH002",
     "TRY400",
     "SIM117",
     "SIM108",
     "ANN201",
+    "D415",
+    "D200",
 ]
 ignore = [
-    "D",
     "TRY003", # TODO(aspen): Switch to custom exceptions
     "ANN101", # Due to be deprecated in ruff
     "ANN102", # Due to be deprecated in ruff
     "COM812", # Conflicts with formatter
     "ISC001", # Conflicts with formatter
     "EXE002", # pre-commit does it better, works with SMB shares
     "FA100",
@@ -135,15 +136,15 @@
 [tool.ruff.lint.pycodestyle]
 max-line-length = 100
 
 [tool.ruff.lint.isort]
 split-on-trailing-comma = false
 
 [tool.ruff.lint.pydocstyle]
-convention = "pep257"
+convention = "google"
 
 [tool.flynt]
 aggressive = true
 transform-joins = true
 transform-concats = true
 
 [tool.mypy]
```

### Comparing `polymatch-0.4.0/PKG-INFO` & `polymatch-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polymatch
-Version: 0.4.0
+Version: 0.4.1
 Summary: A polymorphic pattern matching library for Python
 Project-URL: Homepage, https://github.com/TotallyNotRobots/polymatch
 Author-email: linuxdaemon <linuxdaemon.irc@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: library,pattern-matching,regex,utility
 Classifier: Development Status :: 3 - Alpha
@@ -21,16 +21,17 @@
 Description-Content-Type: text/markdown
 
 # poly-match
 Python Polymorphic Pattern Matching library
 
 [![CI - Test](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-tests.yml/badge.svg)](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-tests.yml)
 [![CD - Build](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-publish.yml/badge.svg)](https://github.com/TotallyNotRobots/poly-match/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/gh/TotallyNotRobots/poly-match/graph/badge.svg?token=nJqN3RacOa)](https://codecov.io/gh/TotallyNotRobots/poly-match)
 
-[![PyPI - Version](https://img.shields.io/pypi/v/polymatch.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/polymatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/polymatch.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/polymatch/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polymatch.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/polymatch/)
+[![PyPI - Version](https://img.shields.io/pypi/v/polymatch.svg)](https://pypi.org/project/polymatch/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/polymatch.svg)](https://pypi.org/project/polymatch/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/polymatch.svg)](https://pypi.org/project/polymatch/)
 
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
```

