# Comparing `tmp/ghit_smartptr-0.1.4.tar.gz` & `tmp/ghit_smartptr-0.1.5.tar.gz`

## Comparing `ghit_smartptr-0.1.4.tar` & `ghit_smartptr-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/requirements.txt
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/__main__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/args.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/branch_commands.py
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/common.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/error.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh_formatting.py
--rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh_graphql.py
--rwxr-xr-x   0        0        0     3563 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/ghit.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gitools.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/graphql.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/stack.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/stack_commands.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/styling.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/terminal.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/top_commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_gh_graphql.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_graphql.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_stack.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/LICENSE
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/README.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/__main__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/args.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/branch_commands.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/common.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/error.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/gh.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/gh_formatting.py
+-rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/gh_graphql.py
+-rwxr-xr-x   0        0        0     3850 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/ghit.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/gitools.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/graphql.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/stack.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/stack_commands.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/styling.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/terminal.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/ghit/top_commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/tests/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/tests/test_gh_graphql.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/tests/test_graphql.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/src/tests/test_stack.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.5/PKG-INFO
```

### Comparing `ghit_smartptr-0.1.4/.github/workflows/python-app.yml` & `ghit_smartptr-0.1.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/.github/workflows/python-publish.yml` & `ghit_smartptr-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/branch_commands.py` & `ghit_smartptr-0.1.5/src/ghit/branch_commands.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/common.py` & `ghit_smartptr-0.1.5/src/ghit/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 from pathlib import Path
 
 import pygit2 as git
 
 from . import gh_formatting as ghf
+from . import gh_graphql as ghgql
 from . import styling as s
 from . import terminal
 from .args import Args
 from .error import GhitError
 from .gh import GH, init_gh
 from .gh_formatting import pr_number_with_style
 from .gitools import MyRemoteCallback, get_current_branch, last_commits
@@ -79,15 +80,15 @@
 def push_and_pr(
     repo: git.Repository,
     gh: GH,
     origin: git.Remote,
     record: Stack,
     title: str = '',
     draft: bool = False,
-) -> None:
+) -> tuple[list[ghgql.PR], bool]:
     branch = repo.branches[record.branch_name]
     if not branch.upstream:
         push_branch(origin, branch)
         update_upstream(repo, origin, branch)
 
     prs = gh.get_prs(record.branch_name)
     for pr in prs:
@@ -109,14 +110,17 @@
         pr = gh.create_pr(record.get_parent().branch_name, record.branch_name, title, draft)
         terminal.stdout(
             'Created draft PR ' if draft else 'Created PR ',
             pr_number_with_style(pr),
             '.',
             sep='',
         )
+        prs.append(pr)
+        return prs, True
+    return prs, False
 
 
 def rewrite_stack(args_stack: str, repo: git.Repository, stack: Stack):
     with (Path(args_stack) if args_stack else stack_filename(repo)).open('w') as ghit_stack:
         ghit_stack.write('\n'.join(stack.dumps()) + '\n')
```

### Comparing `ghit_smartptr-0.1.4/src/ghit/gh.py` & `ghit_smartptr-0.1.5/src/ghit/gh.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/gh_formatting.py` & `ghit_smartptr-0.1.5/src/ghit/gh_formatting.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/gh_graphql.py` & `ghit_smartptr-0.1.5/src/ghit/gh_graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/ghit.py` & `ghit_smartptr-0.1.5/src/ghit/ghit.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,25 +64,29 @@
     parser_branch_sub.add_parser('check', help='check the state of the branch and possible PRs').set_defaults(
         func=bcom.check
     )
 
 
 def ghit(argv: list[str]) -> int:
     parser = argparse.ArgumentParser()
-    parser.add_argument('-r', '--repository', default='.')
-    parser.add_argument('-s', '--stack')
-    parser.add_argument('-o', '--offline', action='store_true')
+    parser.add_argument('-r', '--repository', default='.', help='the git repository path (default .)')
+    parser.add_argument('-s', '--stack', help='the stack filename (default .ghit/stack)')
+    parser.add_argument('-o', '--offline', action='store_true', help='do not call GitHub')
     parser.add_argument('-g', '--debug', action='store_true')
     parser.add_argument('-v', '--verbose', action='store_true')
 
     commands = add_top_commands(parser)
     add_stack_commands(commands.add_parser('stack', aliases=['s', 'st']))
     add_branch_commands(commands.add_parser('branch', aliases=['b', 'br']))
 
     args = parser.parse_args(args=argv)
+    if 'func' not in args:
+        parser.print_usage()
+        terminal.stderr('Please provide the full command, with necessary subcommands.', args)
+        return 1
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
         try:
             args.func(args)
         except GhitError as br:
             msg = str(br)
             if msg:
```

### Comparing `ghit_smartptr-0.1.4/src/ghit/gitools.py` & `ghit_smartptr-0.1.5/src/ghit/gitools.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/graphql.py` & `ghit_smartptr-0.1.5/src/ghit/graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/stack.py` & `ghit_smartptr-0.1.5/src/ghit/stack.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/stack_commands.py` & `ghit_smartptr-0.1.5/src/ghit/stack_commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,17 +22,26 @@
     repo, stack, gh = connect(args)
     if repo.is_empty or args.offline or not gh:
         return
     origin = repo.remotes['origin']
     if not origin:
         raise GhitError(s.warning('No origin found for the repository.'))
 
+    prs = []
+    needs_update = False
     for record in stack.traverse(False):
-        push_and_pr(repo, gh, origin, record)
+        branch_prs, pr_created = push_and_pr(repo, gh, origin, record)
+        prs.extend(branch_prs)
+        needs_update = needs_update or pr_created
 
+    if needs_update and len(prs) > 1:
+        # Update the ghit comments in all PRs except the last one, which doesn't
+        # need to be updated, if a new PR has been created.
+        for pr in prs[:-1]:
+            gh.comment(pr)
 
 def cleanup(args: Args) -> None:
     repo, stack, gh = connect(args)
     if repo.is_empty:
         return
 
     for record in stack.traverse(False):
```

### Comparing `ghit_smartptr-0.1.4/src/ghit/styling.py` & `ghit_smartptr-0.1.5/src/ghit/styling.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/ghit/top_commands.py` & `ghit_smartptr-0.1.5/src/ghit/top_commands.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/tests/test_gh_graphql.py` & `ghit_smartptr-0.1.5/src/tests/test_gh_graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/tests/test_graphql.py` & `ghit_smartptr-0.1.5/src/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/src/tests/test_stack.py` & `ghit_smartptr-0.1.5/src/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/LICENSE` & `ghit_smartptr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/README.md` & `ghit_smartptr-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/pyproject.toml` & `ghit_smartptr-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.4/PKG-INFO` & `ghit_smartptr-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ghit-smartptr
-Version: 0.1.4
+Version: 0.1.5
 Summary: ghit
 Project-URL: Homepage, https://github.com/0x656b694d/ghit
 Project-URL: Issues, https://github.com/0x656b694d/ghit/issues
 Author-email: Michaël Petrov <smartptr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Michaël
```

