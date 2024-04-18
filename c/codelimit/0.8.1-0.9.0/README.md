# Comparing `tmp/codelimit-0.8.1.tar.gz` & `tmp/codelimit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelimit-0.8.1.tar", max compression
+gzip compressed data, was "codelimit-0.9.0.tar", max compression
```

## Comparing `codelimit-0.8.1.tar` & `codelimit-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,84 @@
--rw-r--r--   0        0        0      810 2024-02-29 17:04:36.629410 codelimit-0.8.1/LICENSE
--rw-r--r--   0        0        0     2697 2024-02-29 17:04:36.629410 codelimit-0.8.1/README.md
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/__init__.py
--rwxr-xr-x   0        0        0     4812 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/__main__.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/commands/__init__.py
--rw-r--r--   0        0        0      503 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/commands/github.py
--rw-r--r--   0        0        0     2077 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/CheckResult.py
--rw-r--r--   0        0        0     2303 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Codebase.py
--rw-r--r--   0        0        0      503 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/CodebseEntry.py
--rw-r--r--   0        0        0      545 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Configuration.py
--rw-r--r--   0        0        0     1736 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Language.py
--rw-r--r--   0        0        0      923 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Location.py
--rw-r--r--   0        0        0      186 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Measurement.py
--rw-r--r--   0        0        0     3705 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Scanner.py
--rw-r--r--   0        0        0      331 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/SourceFile.py
--rw-r--r--   0        0        0      737 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/SourceFileEntry.py
--rw-r--r--   0        0        0      527 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/SourceFolder.py
--rw-r--r--   0        0        0      255 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/SourceFolderEntry.py
--rw-r--r--   0        0        0      900 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/Token.py
--rw-r--r--   0        0        0     1256 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/TokenRange.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/__init__.py
--rw-r--r--   0        0        0     2898 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/report/Report.py
--rw-r--r--   0        0        0     1115 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/report/ReportReader.py
--rw-r--r--   0        0        0      162 2024-02-29 17:04:36.629410 codelimit-0.8.1/codelimit/common/report/ReportUnit.py
--rw-r--r--   0        0        0     4690 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/report/ReportWriter.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/report/__init__.py
--rw-r--r--   0        0        0      155 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/scope/Header.py
--rw-r--r--   0        0        0      664 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/scope/Scope.py
--rw-r--r--   0        0        0      450 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/scope/ScopeExtractor.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/scope/__init__.py
--rw-r--r--   0        0        0     2965 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/scope/scope_utils.py
--rw-r--r--   0        0        0     2083 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/source_utils.py
--rw-r--r--   0        0        0      852 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/token_matching/BalancedPredicate.py
--rw-r--r--   0        0        0     2178 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/token_matching/TokenMatching.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/token_matching/__init__.py
--rw-r--r--   0        0        0      781 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/token_utils.py
--rw-r--r--   0        0        0     2593 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/common/utils.py
--rw-r--r--   0        0        0     3139 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/github_auth.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/__init__.py
--rw-r--r--   0        0        0      533 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/c/CLanguage.py
--rw-r--r--   0        0        0     1555 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/c/CScopeExtractor.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/c/__init__.py
--rw-r--r--   0        0        0      599 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/javascript/JavaScriptLanguage.py
--rw-r--r--   0        0        0     1564 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/javascript/JavaScriptScopeExtractor.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/javascript/__init__.py
--rw-r--r--   0        0        0      562 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/python/PythonLanguage.py
--rw-r--r--   0        0        0     3191 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/python/PythonScopeExtractor.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/python/__init__.py
--rw-r--r--   0        0        0      599 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/typescript/TypeScriptLanguage.py
--rw-r--r--   0        0        0     1564 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/typescript/TypeScriptScopeExtractor.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/languages/typescript/__init__.py
--rw-r--r--   0        0        0     2316 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/CodeLimitApp.py
--rw-r--r--   0        0        0     1008 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/CodeLimitAppHeader.py
--rw-r--r--   0        0        0      909 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/CodeScreen.py
--rw-r--r--   0        0        0      617 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/CodeScreenHeader.py
--rw-r--r--   0        0        0     1109 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/QualityProfile.py
--rw-r--r--   0        0        0        0 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/tui/__init__.py
--rw-r--r--   0        0        0     2293 2024-02-29 17:04:36.633410 codelimit-0.8.1/codelimit/utils.py
--rw-r--r--   0        0        0      109 2024-02-29 17:05:03.501612 codelimit-0.8.1/codelimit/version.py
--rw-r--r--   0        0        0     1043 2024-02-29 17:05:03.501612 codelimit-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 codelimit-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    32423 2024-04-18 08:41:12.145831 codelimit-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2697 2024-04-18 08:41:12.145831 codelimit-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/__init__.py
+-rwxr-xr-x   0        0        0     2253 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/app.py
+-rw-r--r--   0        0        0     1942 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/check.py
+-rw-r--r--   0        0        0     1457 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/report.py
+-rw-r--r--   0        0        0     1303 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/scan.py
+-rw-r--r--   0        0        0     1211 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/upload.py
+-rw-r--r--   0        0        0     1627 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/CheckResult.py
+-rw-r--r--   0        0        0     2303 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Codebase.py
+-rw-r--r--   0        0        0      503 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/CodebseEntry.py
+-rw-r--r--   0        0        0      566 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Configuration.py
+-rw-r--r--   0        0        0      559 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Language.py
+-rw-r--r--   0        0        0      643 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/LanguageTotals.py
+-rw-r--r--   0        0        0     1166 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Location.py
+-rw-r--r--   0        0        0      186 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Measurement.py
+-rw-r--r--   0        0        0     1581 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/ScanResultTable.py
+-rw-r--r--   0        0        0     1406 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/ScanTotals.py
+-rw-r--r--   0        0        0     7181 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/Scanner.py
+-rw-r--r--   0        0        0      331 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFile.py
+-rw-r--r--   0        0        0      873 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFileEntry.py
+-rw-r--r--   0        0        0      535 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFolder.py
+-rw-r--r--   0        0        0      255 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFolderEntry.py
+-rw-r--r--   0        0        0     1333 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/Token.py
+-rw-r--r--   0        0        0     1256 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/TokenRange.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/Expression.py
+-rw-r--r--   0        0        0      453 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/Pattern.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/Automata.py
+-rw-r--r--   0        0        0      450 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/DFA.py
+-rw-r--r--   0        0        0      444 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/NFA.py
+-rw-r--r--   0        0        0      876 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/State.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/__init__.py
+-rw-r--r--   0        0        0     3825 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/matcher.py
+-rw-r--r--   0        0        0      721 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Atom.py
+-rw-r--r--   0        0        0      389 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Concat.py
+-rw-r--r--   0        0        0      702 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/OneOrMore.py
+-rw-r--r--   0        0        0      182 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Operator.py
+-rw-r--r--   0        0        0      701 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Optional.py
+-rw-r--r--   0        0        0      854 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Union.py
+-rw-r--r--   0        0        0      714 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/ZeroOrMore.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/Identity.py
+-rw-r--r--   0        0        0      336 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/Predicate.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/__init__.py
+-rw-r--r--   0        0        0     2032 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/utils.py
+-rw-r--r--   0        0        0     1013 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/lexer_utils.py
+-rw-r--r--   0        0        0     1583 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/Report.py
+-rw-r--r--   0        0        0     1343 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportReader.py
+-rw-r--r--   0        0        0      162 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportUnit.py
+-rw-r--r--   0        0        0     5087 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportWriter.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/Header.py
+-rw-r--r--   0        0        0     1227 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/Scope.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/__init__.py
+-rw-r--r--   0        0        0     5506 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/scope_utils.py
+-rw-r--r--   0        0        0     2083 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/source_utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Balanced.py
+-rw-r--r--   0        0        0      875 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Choice.py
+-rw-r--r--   0        0        0      659 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Keyword.py
+-rw-r--r--   0        0        0      444 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Name.py
+-rw-r--r--   0        0        0      635 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Operator.py
+-rw-r--r--   0        0        0      629 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Symbol.py
+-rw-r--r--   0        0        0      364 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenPredicate.py
+-rw-r--r--   0        0        0      628 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenValue.py
+-rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_utils.py
+-rw-r--r--   0        0        0     5762 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/utils.py
+-rw-r--r--   0        0        0     3139 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/github_auth.py
+-rw-r--r--   0        0        0      926 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/C.py
+-rw-r--r--   0        0        0      858 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Cpp.py
+-rw-r--r--   0        0        0      707 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Java.py
+-rw-r--r--   0        0        0     1086 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/JavaScript.py
+-rw-r--r--   0        0        0     3018 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Python.py
+-rw-r--r--   0        0        0     1610 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/TypeScript.py
+-rw-r--r--   0        0        0      178 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/__init__.py
+-rw-r--r--   0        0        0     1911 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/utils.py
+-rw-r--r--   0        0        0       18 2024-04-18 08:41:37.982332 codelimit-0.9.0/codelimit/version.py
+-rw-r--r--   0        0        0     1124 2024-04-18 08:41:37.982332 codelimit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 codelimit-0.9.0/PKG-INFO
```

### Comparing `codelimit-0.8.1/README.md` & `codelimit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `codelimit-0.8.1/codelimit/common/CheckResult.py` & `codelimit-0.9.0/codelimit/common/CheckResult.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 from os.path import relpath
 from pathlib import Path
 
 import rich
 from rich.console import Console
-from rich.style import Style
-from rich.text import Text
 
 from codelimit.common.Measurement import Measurement
-from codelimit.common.utils import format_unit
+from codelimit.common.utils import format_measurement
 
 
 class CheckResult:
-    def __init__(self):
+    def __init__(self) -> None:
         self.file_list: list[tuple[Path, list[Measurement]]] = []
         self.hard_to_maintain = 0
         self.unmaintainable = 0
 
     def add(self, file: Path, measurements: list[Measurement]):
         self.file_list.append((file, measurements))
         self.hard_to_maintain += len([m for m in measurements if 30 < m.value <= 60])
@@ -26,27 +24,19 @@
         return len(self.file_list)
 
     def report(self):
         cwd_path = Path(os.getcwd())
         stdout = Console()
         for file, measurements in self.file_list:
             for m in measurements:
-                text = Text()
                 if cwd_path in file.parents:
-                    text.append(relpath(file, cwd_path), style=Style(bold=True))
+                    file_path = str(relpath(file, cwd_path))
                 else:
-                    text.append(str(file), style="bold")
-                text.append(":", style=Style(color="cyan"))
-                text.append(str(m.start.line))
-                text.append(":", style=Style(color="cyan"))
-                text.append(str(m.start.column))
-                text.append(":", style=Style(color="cyan"))
-                text.append(" ")
-                text.append(format_unit(m.unit_name, m.value))
-                stdout.print(text, soft_wrap=True)
+                    file_path = str(file)
+                stdout.print(format_measurement(file_path, m), soft_wrap=True)
         if self.hard_to_maintain > 0 or self.unmaintainable > 0:
             rich.print(
                 f"{len(self.file_list)} files checked, "
                 f"{self.hard_to_maintain + self.unmaintainable} functions need "
                 f"refactoring."
             )
         else:
```

### Comparing `codelimit-0.8.1/codelimit/common/Codebase.py` & `codelimit-0.9.0/codelimit/common/Codebase.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.8.1/codelimit/common/Configuration.py` & `codelimit-0.9.0/codelimit/common/Configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,7 +23,9 @@
         "build",
         "dist",
         "node_modules",
         "venv",
         "test",
         "tests",
     ]
+
+    verbose = False
```

### Comparing `codelimit-0.8.1/codelimit/common/SourceFileEntry.py` & `codelimit-0.9.0/codelimit/common/SourceFileEntry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from codelimit.common.CodebseEntry import CodebaseEntry
 from codelimit.common.Measurement import Measurement
 from codelimit.common.utils import make_profile
 
 
 class SourceFileEntry(CodebaseEntry):
-    def __init__(self, path: str, checksum: str, measurements: list[Measurement]):
+    def __init__(
+        self,
+        path: str,
+        checksum: str,
+        language: str,
+        loc: int,
+        measurements: list[Measurement],
+    ):
         super().__init__(path)
         profile = make_profile(measurements)
-        self._profile: list[int] = profile
         self._checksum = checksum
+        self.language = language
+        self.loc = loc
+        self._profile: list[int] = profile
         self._measurements = measurements
 
     def is_folder(self):
         return False
 
     def is_file(self):
         return True
```

### Comparing `codelimit-0.8.1/codelimit/common/SourceFolder.py` & `codelimit-0.9.0/codelimit/common/SourceFolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from codelimit.common.CodebseEntry import CodebaseEntry
 from codelimit.common.SourceFileEntry import SourceFileEntry
 from codelimit.common.SourceFolderEntry import SourceFolderEntry
 
 
 class SourceFolder:
-    def __init__(self):
+    def __init__(self) -> None:
         self.entries: list[CodebaseEntry] = []
         self.profile = [0, 0, 0, 0]
 
     def add_file(self, entry: SourceFileEntry):
         self.entries.append(entry)
 
     def add_folder(self, name: str):
```

### Comparing `codelimit-0.8.1/codelimit/common/Token.py` & `codelimit-0.9.0/codelimit/common/Token.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from typing import Any
 
-from pygments.token import Keyword, Text, Whitespace, Comment, Punctuation, Name
+from pygments.token import (
+    Keyword,
+    Text,
+    Whitespace,
+    Comment,
+    Punctuation,
+    Operator,
+    Name,
+)
 
 from codelimit.common.Location import Location
 
 
 class Token:
     def __init__(self, location: Location, token_type: Any, value: str):
         self.location = location
@@ -21,15 +29,28 @@
 
     def is_comment(self):
         return self.token_type in Comment
 
     def is_symbol(self, symbol: str):
         return self.token_type in Punctuation and self.value == symbol
 
+    def is_operator(self, symbol: str):
+        return self.token_type in Operator and self.value == symbol
+
     def is_name(self):
         return self.token_type in Name
 
     def __str__(self):
         return self.value
 
     def __repr__(self):
         return str(self)
+
+    def __eq__(self, other):
+        if not isinstance(other, Token):
+            return NotImplemented
+
+        return (
+            self.location == other.location
+            and str(self.token_type) == str(other.token_type)
+            and self.value == other.value
+        )
```

### Comparing `codelimit-0.8.1/codelimit/common/TokenRange.py` & `codelimit-0.9.0/codelimit/common/TokenRange.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.8.1/codelimit/common/report/ReportReader.py` & `codelimit-0.9.0/codelimit/common/report/ReportReader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from json import loads
+from typing import Optional
 
 from codelimit.common.Codebase import Codebase
-from codelimit.common.SourceFileEntry import SourceFileEntry
 from codelimit.common.Location import Location
-from codelimit.common.report.Report import Report
 from codelimit.common.Measurement import Measurement
+from codelimit.common.SourceFileEntry import SourceFileEntry
+from codelimit.common.report.Report import Report
 
 
 class ReportReader:
     @staticmethod
-    def from_json(json: str) -> Report:
+    def from_json(json: str) -> Optional[Report]:
         d = loads(json)
         codebase = Codebase(d["root"])
         report = Report(codebase)
+        report.version = d["version"] if "version" in d else None
+        if report.version != Report.VERSION:
+            return None
         report.uuid = d["uuid"]
         for k, v in d["codebase"]["files"].items():
             measurements: list[Measurement] = []
             for m in v["measurements"]:
                 start_location = Location(m["start"]["line"], m["start"]["column"])
                 end_location = Location(m["end"]["line"], m["end"]["column"])
                 measurements.append(
                     Measurement(
                         m["unit_name"], start_location, end_location, m["value"]
                     )
                 )
-            codebase.add_file(SourceFileEntry(k, v["checksum"], measurements))
+            codebase.add_file(
+                SourceFileEntry(k, v["checksum"], v["language"], v["loc"], measurements)
+            )
         codebase.aggregate()
         return report
```

### Comparing `codelimit-0.8.1/codelimit/common/report/ReportWriter.py` & `codelimit-0.9.0/codelimit/common/report/ReportWriter.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     def to_json(self) -> str:
         self.level = 0
         json = ""
         json += self._open("{")
         json += self._collection(
             [
+                self._line(f'"version": "{self.report.version}"'),
                 self._line(f'"uuid": "{self.report.uuid}"'),
                 self._line(f'"root": "{self.report.codebase.root}"'),
                 self._codebase_to_json(),
             ]
         )
         json += self._close("}")
         return json
@@ -98,24 +99,32 @@
 
     def _file_to_json(self, name: str, entry: SourceFileEntry):
         json = ""
         json += self._open(f'"{name}": {{')
         json += self._collection(
             [
                 self._file_checksum_to_json(entry),
+                self._file_language_to_json(entry),
+                self._file_loc_to_json(entry),
                 self._file_profile_to_json(entry),
                 self._file_measurements_to_json(entry),
             ]
         )
         json += self._close("}")
         return json
 
     def _file_checksum_to_json(self, entry: SourceFileEntry):
         return self._line(f'"checksum": "{entry.checksum()}"')
 
+    def _file_language_to_json(self, entry: SourceFileEntry):
+        return self._line(f'"language": "{entry.language}"')
+
+    def _file_loc_to_json(self, entry: SourceFileEntry):
+        return self._line(f'"loc": {entry.loc}')
+
     def _file_profile_to_json(self, entry: SourceFileEntry):
         return self._line(f'"profile": {entry.profile()}')
 
     def _file_measurements_to_json(self, entry: SourceFileEntry):
         json = ""
         json += self._open('"measurements": [')
         json += self._collection(
```

### Comparing `codelimit-0.8.1/codelimit/common/scope/Scope.py` & `codelimit-0.9.0/codelimit/common/gsm/predicate/Identity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from codelimit.common.Token import Token
-from codelimit.common.TokenRange import TokenRange
-from codelimit.common.scope.Header import Header
+from typing import Any
 
+from codelimit.common.gsm.predicate.Predicate import Predicate
 
-class Scope:
-    def __init__(self, header: Header, block: TokenRange):
-        self.header = header
-        self.block = block
 
-    def __str__(self):
-        return (
-            f"[{self.header.token_range[0].location}, {self.block.tokens[-1].location}]"
-        )
+class Identity(Predicate[Any]):
+
+    def __init__(self, item: Any):
+        self.item = item
 
-    def __repr__(self):
-        return self.__str__()
+    def accept(self, item: Any) -> bool:
+        return self.item == item
 
-    def __len__(self):
-        return count_lines(self.header.token_range.tokens + self.block.tokens)
+    def __str__(self):
+        return f"{self.item}"
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Identity):
+            return False
+        return self.item == other.item
 
-def count_lines(tokens: list[Token]):
-    return len(set([t.location.line for t in tokens]))
+    def __hash__(self):
+        return hash(self.item)
```

### Comparing `codelimit-0.8.1/codelimit/common/source_utils.py` & `codelimit-0.9.0/codelimit/common/source_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.8.1/codelimit/common/token_matching/BalancedPredicate.py` & `codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenValue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 from codelimit.common.Token import Token
-from codelimit.common.token_matching.TokenMatching import TokenPredicate
+from codelimit.common.token_matching.predicate.TokenPredicate import TokenPredicate
 
 
-class BalancedPredicate(TokenPredicate):
-    def __init__(self, left: TokenPredicate, right: TokenPredicate):
+class TokenValue(TokenPredicate):
+    def __init__(self, value: str):
         super().__init__()
-        self.left = left
-        self.right = right
-        self.depth = 0
-
-    def reset(self):
-        super().reset()
-        self.left.reset()
-        self.right.reset()
-        self.depth = 0
+        self.value = value
 
     def accept(self, token: Token) -> bool:
-        if self.left.accept(token):
-            self.depth += 1
-            return True
-        elif self.right.accept(token):
-            self.depth -= 1
-            if self.depth < 0:
-                return False
-            if self.depth == 0:
-                self.satisfied = True
+        if token.value == self.value:
+            self.satisfied = True
             return True
-        else:
-            return self.depth > 0
+        return False
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TokenValue):
+            return False
+        return self.value == other.value
+
+    def __hash__(self):
+        return hash(self.value)
```

### Comparing `codelimit-0.8.1/codelimit/github_auth.py` & `codelimit-0.9.0/codelimit/github_auth.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.8.1/codelimit/languages/python/PythonScopeExtractor.py` & `codelimit-0.9.0/codelimit/languages/Python.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,24 @@
+from codelimit.common.Language import Language
 from codelimit.common.Token import Token
 from codelimit.common.TokenRange import TokenRange
+from codelimit.common.gsm.operator.OneOrMore import OneOrMore
 from codelimit.common.scope.Header import Header
-from codelimit.common.scope.ScopeExtractor import ScopeExtractor
-from codelimit.common.token_matching.BalancedPredicate import BalancedPredicate
-from codelimit.common.token_matching.TokenMatching import (
-    match,
-    KeywordPredicate,
-    NamePredicate,
-    SymbolPredicate,
-)
+from codelimit.common.scope.scope_utils import get_headers
+from codelimit.common.token_matching.predicate.Balanced import Balanced
+from codelimit.common.token_matching.predicate.Keyword import Keyword
+from codelimit.common.token_matching.predicate.Name import Name
 from codelimit.common.utils import delete_indices
 
 
-class PythonScopeExtractor(ScopeExtractor):
+class Python(Language):
     def extract_headers(self, tokens: list[Token]) -> list[Header]:
-        result = []
-        matches = match(
-            tokens,
-            [
-                KeywordPredicate("def"),
-                NamePredicate(),
-                BalancedPredicate(SymbolPredicate("("), SymbolPredicate(")")),
-            ],
+        return get_headers(
+            tokens, [Keyword("def"), Name(), OneOrMore(Balanced("(", ")"))]
         )
-        for m in matches:
-            result.append(Header(m.tokens[1].value, m))
-        return result
 
     def extract_blocks(
         self, tokens: list[Token], headers: list[Header]
     ) -> list[TokenRange]:
         lines = _get_token_lines(tokens)
         result = []
         reverse_headers = headers[::-1]
```

### Comparing `codelimit-0.8.1/codelimit/languages/typescript/TypeScriptScopeExtractor.py` & `codelimit-0.9.0/codelimit/languages/TypeScript.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,40 @@
+from codelimit.common.Language import Language
 from codelimit.common.Token import Token
 from codelimit.common.TokenRange import TokenRange
+from codelimit.common.gsm.operator.OneOrMore import OneOrMore
+from codelimit.common.gsm.operator.Optional import Optional
 from codelimit.common.scope.Header import Header
-from codelimit.common.scope.ScopeExtractor import ScopeExtractor
-from codelimit.common.token_utils import get_balanced_symbol_token_indices
+from codelimit.common.scope.scope_utils import get_blocks, get_headers
+from codelimit.common.token_matching.predicate.Balanced import Balanced
+from codelimit.common.token_matching.predicate.Choice import Choice
+from codelimit.common.token_matching.predicate.Keyword import Keyword
+from codelimit.common.token_matching.predicate.Name import Name
+from codelimit.common.token_matching.predicate.Operator import Operator
+from codelimit.common.token_matching.predicate.Symbol import Symbol
 
 
-class TypeScriptScopeExtractor(ScopeExtractor):
+class TypeScript(Language):
     def extract_headers(self, tokens: list[Token]) -> list[Header]:
-        result = []
-        balanced_tokens = get_balanced_symbol_token_indices(tokens, "(", ")")
-
-        def has_name_prefix(index):
-            return index > 0 and tokens[index - 1].is_name()
-
-        def has_curly_suffix(index):
-            return index < len(tokens) - 1 and tokens[index + 1].is_symbol("{")
-
-        for bt in balanced_tokens:
-            if has_name_prefix(bt[0]) and has_curly_suffix(bt[1]):
-                result.append(
-                    Header(
-                        tokens[bt[0] - 1].value,
-                        TokenRange(tokens[bt[0] - 1 : bt[1] + 1]),
-                    )
-                )
-        return result
+        functions = get_headers(
+            tokens,
+            [Optional("function"), Name(), OneOrMore(Balanced("(", ")"))],
+            Choice("{", Operator(":")),
+        )
+        arrow_functions = get_headers(
+            tokens,
+            [
+                Optional(Keyword("const")),
+                Name(),
+                Operator("="),
+                Optional(Keyword("async")),
+                OneOrMore(Balanced("(", ")")),
+                Symbol("=>"),
+            ],
+            Symbol("{"),
+        )
+        return functions + arrow_functions
 
     def extract_blocks(
         self, tokens: list[Token], headers: list[Header]
     ) -> list[TokenRange]:
-        balanced_tokens = get_balanced_symbol_token_indices(tokens, "{", "}", False)
-        blocks = [TokenRange(tokens[bt[0] : bt[1] + 1]) for bt in balanced_tokens]
-        sorted_by_line = sorted(blocks, key=lambda tr: tr.tokens[0].location.line)
-        sorted_by_columns = sorted(
-            sorted_by_line, key=lambda tr: tr.tokens[0].location.column
-        )
-        return sorted_by_columns
+        return get_blocks(tokens, "{", "}")
```

### Comparing `codelimit-0.8.1/codelimit/utils.py` & `codelimit-0.9.0/codelimit/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,58 @@
 from pathlib import Path
 from typing import Optional
 
 import requests  # type: ignore
 import typer
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
-from codelimit.common.CheckResult import CheckResult
-from codelimit.common.Scanner import scan_file, languages
 from codelimit.common.report.Report import Report
 from codelimit.common.report.ReportReader import ReportReader
 from codelimit.common.report.ReportWriter import ReportWriter
 
 
-def check_file(path: Path, check_result: CheckResult):
-    for language in languages:
-        if language.accept_file(str(path.absolute())):
-            measurements = scan_file(language, str(path))
-            risks = sorted(
-                [m for m in measurements if m.value > 30],
-                key=lambda measurement: measurement.value,
-                reverse=True,
-            )
-            check_result.add(path, risks)
-
-
 def read_cached_report(path: Path) -> Optional[Report]:
     cache_dir = path.joinpath(".codelimit_cache").resolve()
     report_path = cache_dir.joinpath("codelimit.json").resolve()
     if report_path.exists():
         return ReportReader.from_json(report_path.read_text())
     else:
         return None
 
 
 def upload_report(
     report: Report, repository: str, branch: str, url: str, token: str
 ) -> None:
+    result = api_post_report(report, branch, repository, url, token)
+    if result.ok:
+        typer.secho("Upload successful!", fg="green")
+    else:
+        error_message = "Upload unsuccessful: "
+        if result.text:
+            error_message += result.text
+        else:
+            error_message += str(result.status_code)
+        typer.secho(error_message, fg="red")
+        raise typer.Exit(code=1)
+
+
+def api_post_report(report, branch, repository, url, token):
     data_template = (
         f'{{{{"repository": "{repository}", "branch": "{branch}", "report":{{}}}}}}'
     )
     with Progress(
-        SpinnerColumn(),
-        TextColumn("[progress.description]{task.description}"),
-        transient=True,
+            SpinnerColumn(),
+            TextColumn("[progress.description]{task.description}"),
+            transient=True,
     ) as progress:
         progress.add_task(description=f"Uploading report to {url}", total=None)
         result = requests.post(
             url,
             data=data_template.format(
                 ReportWriter(report, pretty_print=False).to_json()
             ),
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {token}",
             },
         )
-    if result.ok:
-        typer.secho("Upload successful!", fg="green")
-    else:
-        error_message = "Upload unsuccessful: "
-        if result.text:
-            error_message += result.text
-        else:
-            error_message += str(result.status_code)
-        typer.secho(error_message, fg="red")
-        raise typer.Exit(code=1)
+    return result
```

### Comparing `codelimit-0.8.1/pyproject.toml` & `codelimit-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 [tool.poetry]
 name = "codelimit"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["Rob van der Leek <robvanderleek@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 codelimit = "codelimit.__main__:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-halo = "^0.0.31"
-plotext = "^5.2.8"
 pygments = "^2.13.0"
-textual = "^0.34.0"
 requests = "^2.28.2"
 typer = "^0.9.0"
 aiohttp = "^3.9.0"
 pyyaml = "^6.0.1"
+rich = "^13.7.1"
+pathspec = "^0.12.1"
+
+[tool.pytest.ini_options]
+addopts = "--tb=short"
 
 [tool.poe.tasks.bundle]
 help = "Create a binary executable using pyinstaller"
 cmd = "pyinstaller --workpath .build --specpath dist -n codelimit codelimit/__main__.py"
 
+[tool.mypy]
+ignore_missing_imports = true
+
 [tool.semantic_release]
 branch = "main"
 version_toml = [ "pyproject.toml:tool.poetry.version" ]
 version_variables = [ "codelimit/version.py:version" ]
 upload_to_repository = false
 upload_to_release = false
 
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^5.6.1"
 pytest-cov = "^4.0.0"
 pytest = "^7.2.1"
 poethepoet = "^0.21.1"
-textual-dev = "^1.1.0"
-mkdocs-material = "^9.2.8"
+mkdocs-material = "^9.5.10"
+mkdocs-glightbox = "^0.3.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `codelimit-0.8.1/PKG-INFO` & `codelimit-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: codelimit
-Version: 0.8.1
+Version: 0.9.0
 Summary: 
 Author: Rob van der Leek
 Author-email: robvanderleek@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
-Requires-Dist: halo (>=0.0.31,<0.0.32)
-Requires-Dist: plotext (>=5.2.8,<6.0.0)
+Requires-Dist: pathspec (>=0.12.1,<0.13.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: textual (>=0.34.0,<0.35.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Code Limit
 
 Your Refactoring Alarm 🔔
```

