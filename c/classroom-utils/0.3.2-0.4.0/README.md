# Comparing `tmp/classroom_utils-0.3.2.tar.gz` & `tmp/classroom_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classroom_utils-0.3.2.tar", last modified: Thu Mar 21 23:59:01 2024, max compression
+gzip compressed data, was "classroom_utils-0.4.0.tar", last modified: Thu Apr 18 10:34:48 2024, max compression
```

## Comparing `classroom_utils-0.3.2.tar` & `classroom_utils-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/classroom_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/classroom_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/ascii_art.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/github_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/local_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.858289 classroom_utils-0.3.2/classroom_utils/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/classroom_utils/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/resources/schemas/classlist_file_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/resources/schemas/config_file_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/classroom_utils/subcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/classroom_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-21 23:59:01.000000 classroom_utils-0.3.2/classroom_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:59:01.862289 classroom_utils-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/tests/test_github_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-03-21 23:58:57.000000 classroom_utils-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/classroom_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/classroom_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/ascii_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/github_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/local_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.825436 classroom_utils-0.4.0/classroom_utils/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/classroom_utils/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/resources/schemas/classlist_file_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/resources/schemas/config_file_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/classroom_utils/subcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/classroom_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 10:34:48.000000 classroom_utils-0.4.0/classroom_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:34:48.829436 classroom_utils-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/tests/test_github_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-04-18 10:34:44.000000 classroom_utils-0.4.0/versioneer.py
```

### Comparing `classroom_utils-0.3.2/LICENSE` & `classroom_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/PKG-INFO` & `classroom_utils-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom_utils
-Version: 0.3.2
+Version: 0.4.0
 Summary: Utilities to handle stuff likes github orgs for classes.
 Home-page: https://github.com/twyleg/classroom_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: class classroom github edu education
 Description-Content-Type: text/markdown
```

### Comparing `classroom_utils-0.3.2/README.md` & `classroom_utils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/ascii_art.py` & `classroom_utils-0.4.0/classroom_utils/ascii_art.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/classes.py` & `classroom_utils-0.4.0/classroom_utils/classes.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/cli.py` & `classroom_utils-0.4.0/classroom_utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,14 @@
 
         for classlist_filepath in self.config.classlist_filepaths:
             self.classes.read_classlist_from_file(classlist_filepath)
 
     def get_class_name_from_user(self, args: argparse.Namespace) -> str:
         return args.class_name if hasattr(args, "class_name") and args.class_name else dialogs.user_input_request_class_name(self.classes.get_available_class_names())
 
-    def get_repo_prefix_from_user(self, args: argparse.Namespace) -> str | None:
-        return args.repo_prefix if hasattr(args, "repo_prefix") and args.repo_prefix else None
-
-    def get_template_from_user(self, args: argparse.Namespace) -> str | None:
-        return args.template if hasattr(args, "template") and args.template else None
-
     def get_selected_class_members_from_user(self, class_name: str) -> List[Member]:
         class_members = self.classes.get_class(class_name)
         return dialogs.user_input_request_selected_class_members(list(class_members.active_members))
 
 
 class LocalSubCommand(ClassroomUtilsBaseCommand):
 
@@ -213,14 +207,20 @@
         github_token = self.read_github_token(args)
 
         logm.debug("GITHUB_USER = '%s'", github_username)
         logm.debug("GITHUB_TOKEN = '%s'", self.get_printable_token(github_token))
 
         return GithubCredentials(github_username, github_token)
 
+    def get_repo_prefix_from_user(self, args: argparse.Namespace) -> str | None:
+        return args.repo_prefix if hasattr(args, "repo_prefix") and args.repo_prefix else dialogs.user_input_request_optional_repo_prefix()
+
+    def get_template_from_user(self, args: argparse.Namespace) -> str | None:
+        return args.template if hasattr(args, "template") and args.template else dialogs.user_input_request_optional_template_repo_name(self.github_ops)
+
     def get_org_name_from_user(self, args: argparse.Namespace) -> str:
         return args.org_name if hasattr(args, "org_name") and args.org_name else dialogs.user_input_request_org_name(self.github_ops)
 
     def get_repo_name_from_user(self, args: argparse.Namespace) -> str:
         return args.repo if hasattr(args, "repo") and args.repo else dialogs.user_input_request_repo_name(self.github_ops)
 
     def get_permission_from_user(self, args: argparse.Namespace) -> str:
@@ -292,15 +292,15 @@
 
         logm.debug(f"github org init:")
         logm.debug("\t-org_name=%s", org_name)
         logm.debug("\t-class_name=%s", class_name)
         logm.debug("\t-repo_prefix=%s", repo_prefix)
         logm.debug("\t-template=%s", template)
 
-        self.github_ops.create_personal_class_repos_in_org(org_name, class_name, repo_prefix, template)
+        self.github_ops.org_create_personal_repos(org_name, class_name, repo_prefix, template)
 
 
 class GithubOrgCloneSubCommand(GithubOrgSubCommand):
     def __init__(self, parser):
         super().__init__(parser)
         self.parser.add_argument('--class-name', type=str, default=None, help="Class name")
         self.parser.add_argument(
@@ -356,15 +356,15 @@
 
         logm.debug(f"github org access grant:")
         logm.debug("\t-org_name=%s", org_name)
         logm.debug("\t-class_name=%s", class_name)
         logm.debug("\t-selected_class_members%s", selected_class_members)
         logm.debug("\t-permission=%s", permission)
 
-        self.github_ops.grant_access_to_personal_class_repos_in_org(org_name, selected_class_members, permission)
+        self.github_ops.org_access_grant_personal_repos(org_name, selected_class_members, permission)
 
 
 class GithubOrgAccessRevokeSubCommand(GithubOrgInitSubCommand):
     def __init__(self, parser):
         super().__init__(parser)
 
     def handle(self, args: argparse.Namespace) -> None:
@@ -374,15 +374,15 @@
         selected_class_members = self.get_selected_class_members_from_user(class_name)
 
         logm.debug(f"github org access grant:")
         logm.debug("\t-org_name=%s", org_name)
         logm.debug("\t-class_name=%s", class_name)
         logm.debug("\t-selected_class_members%s", selected_class_members)
 
-        self.github_ops.revoke_access_from_personal_class_repos_in_org(org_name, selected_class_members)
+        self.github_ops.org_access_revoke_personal_repos(org_name, selected_class_members)
 
 
 class GithubOrgReviewCreateSubCommand(GithubOrgInitSubCommand):
     def __init__(self, parser):
         super().__init__(parser)
 
         self.parser.add_argument(
@@ -407,15 +407,15 @@
 
         logm.debug(f"github org review create:")
         logm.debug("\torg_name=%s", org_name)
         logm.debug("\tclass_name=%s", class_name)
         logm.debug("\thead_branch=%s", head_branch_name)
         logm.debug("\treview_branch=%s", review_branch_name)
 
-        self.github_ops.create_reviews_for_repos_in_org(org_name, class_name, head_branch_name, review_branch_name)
+        self.github_ops.org_reviews_create(org_name, class_name, head_branch_name, review_branch_name)
 
 
 class GithubOrgReviewStatusSubCommand(GithubOrgSubCommand):
     def __init__(self, parser):
         super().__init__(parser)
 
     def handle(self, args: argparse.Namespace) -> None:
@@ -471,15 +471,15 @@
 
         logm.debug(f"github repo access grant")
         logm.debug("\t-repo_name=%s", repo_name)
         logm.debug("\t-class_name=%s", class_name)
         logm.debug("\t-selected_class_members=%s", selected_class_members)
         logm.debug("\t-permission=%s", permission)
 
-        self.github_ops.grant_class_access_to_repo(repo_name, selected_class_members, permission)
+        self.github_ops.repo_access_grant_for_class(repo_name, selected_class_members, permission)
 
 
 class GithubRepoAccessRevokeSubCommand(GithubRepoSubCommand):
     def __init__(self, parser):
         super().__init__(parser)
 
     def handle(self, args: argparse.Namespace) -> None:
@@ -489,9 +489,9 @@
         selected_class_members = self.get_selected_class_members_from_user(class_name)
 
         logm.debug(f"github repo access revoke:")
         logm.debug("\t-repo_name=%s", repo_name)
         logm.debug("\t-class_name=%s", class_name)
         logm.debug("\t-selected_class_members=%s", selected_class_members)
 
-        self.github_ops.revoke_class_access_from_repo(repo_name, selected_class_members)
+        self.github_ops.repo_access_revoke_for_class(repo_name, selected_class_members)
```

### Comparing `classroom_utils-0.3.2/classroom_utils/config.py` & `classroom_utils-0.4.0/classroom_utils/config.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/dialogs.py` & `classroom_utils-0.4.0/classroom_utils/dialogs.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,7 +61,44 @@
 
     selected_class_members: List[Member] = []
     for class_member in class_members:
         if class_member.fullname in result:
             selected_class_members.append(class_member)
 
     return selected_class_members
+
+
+def user_input_request_optional_repo_prefix() -> str | None:
+    yes = inquirer.confirm(message="Specify repo prefix?", default=False).execute()
+
+    if not yes:
+        return None
+
+    prefix = inquirer.text(
+        message="Repo prefix to use:",
+        multicolumn_complete=True,
+    ).execute()
+
+    return prefix.rstrip("_")
+
+
+def user_input_request_optional_template_repo_name(github_ops: github_operations.GithubOperations) -> str | None:
+    yes = inquirer.confirm(message="Specify repo template?", default=False).execute()
+
+    if not yes:
+        return None
+
+    available_orgs = github_ops.get_org_names()
+    logm.debug("Available orgs: %s",available_orgs)
+    org_name = inquirer.fuzzy(
+        message="Select org of template:",
+        choices=available_orgs,
+        border=True
+    ).execute()
+
+    full_repo_names_of_org = github_ops.get_full_repo_names_by_org(org_name)
+    logm.debug("Choose repos in org '%s': %s",org_name, full_repo_names_of_org)
+    return inquirer.fuzzy(
+        message="Select a template repo:",
+        choices=full_repo_names_of_org,
+        border=True
+    ).execute()
```

### Comparing `classroom_utils-0.3.2/classroom_utils/github_operations.py` & `classroom_utils-0.4.0/classroom_utils/github_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,35 +43,119 @@
     def _validate_user(self, github_username: str) -> bool:
         try:
             self.github_connection.get_user(github_username)
             return True
         except github.UnknownObjectException as e:
             return False
 
-    def validate_users(self, users: List[User]) -> None:
+    def _validate_users(self, users: List[User]) -> None:
         with alive_bar(len(users), title="Validating users:", enrich_print=False) as bar:
             for user in users:
                 if self._validate_user(user.github_username):
                     logm.info("  Valid: %s", user)
                 else:
                     logm.warning("  Invalid: %s", user)
                 bar()
 
-    def get_user(self) -> github.NamedUser.NamedUser:
-        return self.github_connection.get_user()
-
-    def get_named_user(self, github_username: str) -> github.NamedUser.NamedUser:
+    def _get_named_user(self, github_username: str) -> github.NamedUser.NamedUser:
         return self.github_connection.get_user(github_username)
 
-    def get_org(self, org_name: str) -> github.Organization.Organization:
+    def _get_org(self, org_name: str) -> github.Organization.Organization:
         return self.github_connection.get_organization(org_name)
 
-    def get_orgs(self) -> PaginatedList[Organization]:
+    def _get_orgs(self) -> PaginatedList[Organization]:
         return self.get_user().get_orgs()
 
+    def _get_repo(self, full_repo_name: str) -> github.Repository.Repository:
+        return self.github_connection.get_repo(full_repo_name)
+
+    def _get_template_repo(self, template_repo_full_name: str) -> github.Repository.Repository:
+        template_repo = self._get_repo(template_repo_full_name)
+        if template_repo.is_template:
+            return template_repo
+        else:
+            logm.error("Repo '%s' is not a template! Unable to create personal class repos!", template_repo.name)
+            sys.exit(-1)
+
+    def _is_repo_existing(self, full_repo_name: str) -> bool:
+        try:
+            self.github_connection.get_repo(full_repo_name)
+            return True
+        except github.GithubException:
+            return False
+
+    @staticmethod
+    def _get_branch_by_name(repo: github.Repository.Repository, name: str) -> github.Branch.Branch | None:
+        for branch in repo.get_branches():
+            if branch.name == name:
+                return branch
+        return None
+
+    @staticmethod
+    def _get_pull_request_by_title(repo: github.Repository.Repository, title: str) -> github.PullRequest.PullRequest | None:
+        for pull in repo.get_pulls():
+            if pull.title == title:
+                return pull
+        return None
+
+    @staticmethod
+    def _repo_remove_invitation(repo: github.Repository.Repository, invitee: github.NamedUser.NamedUser) -> None:
+        logm.debug("Removing invitations in repo '%s' for user '%s'", repo.full_name, invitee.login)
+
+        pending_invitations = repo.get_pending_invitations()
+
+        for invitation in pending_invitations:
+            if invitation.invitee.login == invitee.login:
+                logm.debug("Found invitation: '%s'", invitation.invitee.login)
+                repo.remove_invitation(invitation.id)
+                return
+        logm.warning("Unable to find and remove invitation for '%s'", invitation.invitee.login)
+
+
+    @staticmethod
+    def _repo_is_invitation_for_user_pending(repo: github.Repository, user: github.NamedUser) -> bool:
+        pending_invitations = repo.get_pending_invitations()
+        for pending_invitation in pending_invitations:
+            if pending_invitation.invitee == user:
+                return True
+        return False
+
+    def _repo_create(self, org: Organization, member: Member, repo_prefix: str | None,
+                     template_repo: github.Repository.Repository | None) -> None:
+
+        repo_name = member.generate_personal_repo_name(repo_prefix)
+        full_repo_name = f"{org.login}/{repo_name}"
+        if self._is_repo_existing(full_repo_name):
+            logm.warning("Repo already existing: '%s'. Nothing todo!", full_repo_name)
+        elif template_repo:
+            org.create_repo_from_template(repo_name, template_repo, private=True)
+            logm.info("Created repo '%s' from template '%s'", full_repo_name, template_repo.full_name)
+        else:
+            org.create_repo(repo_name, private=True, auto_init=True)
+            logm.info("Created repo '%s'", full_repo_name)
+
+    def _repo_access_grant(self, repo: github.Repository.Repository, member: Member, permission: str = "pull"):
+        member_named_user = self._get_named_user(member.github_username)
+        if repo.has_in_collaborators(member_named_user):
+            logm.warning("User already a collaborator of repo '%s' -> '%s' already pending. Nothing todo!", member, repo.full_name)
+        else:
+            if self._repo_is_invitation_for_user_pending(repo, member_named_user):
+                logm.warning("Invitation already pending: '%s' -> '%s'. Inviting again!", member, repo.full_name)
+                self._repo_remove_invitation(repo, member_named_user)
+            repo.add_to_collaborators(member_named_user, permission=permission)
+            logm.info("Granted access to repo '%s' -> '%s', permission: '%s'", member, repo.full_name, permission)
+
+    def _repo_clone(self, clone_url: str, target_dir) -> None:
+
+        logm.debug("Clone URL: '%s'", clone_url)
+
+        os.environ["GIT_USERNAME"] = self.github_credentials.username
+        os.environ["GIT_PASSWORD"] = self.github_credentials.token
+        git.Repo.clone_from(clone_url, target_dir)
+
     def get_org_names(self) -> List[str]:
 
         org_names: List[str] = []
 
         params = {
             "per_page": "100",
             "sort": "full_name",
@@ -97,241 +181,177 @@
 
                 for org in data_dict:
                     org_names.append(org["login"])
             if len(data_dict) == 0:
                 return org_names
 
     def get_repo_names_by_org(self, org_name: str) -> List[str]:
-        org = self.get_org(org_name)
+        org = self._get_org(org_name)
         repos = org.get_repos(sort="name")
         return [repo.name for repo in repos]
 
     def get_full_repo_names_by_org(self, org_name: str) -> List[str]:
-        org = self.get_org(org_name)
+        org = self._get_org(org_name)
         repos = org.get_repos(sort="full_name")
         return [repo.full_name for repo in repos]
 
-    def get_repo(self, full_repo_name: str) -> github.Repository.Repository:
-        return self.github_connection.get_repo(full_repo_name)
-
-    @staticmethod
-    def get_branch_by_name(repo: github.Repository.Repository, name: str) -> github.Branch.Branch | None:
-        for branch in repo.get_branches():
-            if branch.name == name:
-                return branch
-        return None
-
-    @staticmethod
-    def get_pull_request_by_title(repo: github.Repository.Repository, title: str) -> github.PullRequest.PullRequest | None:
-        for pull in repo.get_pulls():
-            if pull.title == title:
-                return pull
-        return None
-
-    @staticmethod
-    def remove_invitation(repo: github.Repository.Repository, invitee: github.NamedUser.NamedUser) -> None:
-        logm.debug("Removing invitations in repo '%s' for user '%s'", repo.full_name, invitee.login)
-        for invitation in repo.get_pending_invitations():
-            logm.debug("  - Found invitation: '%s'", invitation.invitee.login)
-            if invitation.invitee.login == invitee.login:
-                logm.debug("  - Remove invitation!")
-                repo.remove_invitation(invitation.id)
-
-    def clone_repo(self, clone_url: str, target_dir) -> None:
-
-        logm.debug("Clone URL: '%s'", clone_url)
-
-        os.environ["GIT_USERNAME"] = self.github_credentials.username
-        os.environ["GIT_PASSWORD"] = self.github_credentials.token
-        git.Repo.clone_from(clone_url, target_dir)
+    def get_user(self) -> github.NamedUser.NamedUser:
+        return self.github_connection.get_user()
 
     def get_user_info(self, github_username: str) -> None:
-        github_user = self.get_named_user(github_username)
+        github_user = self._get_named_user(github_username)
         logm.info("Name: %s", github_user.name)
         logm.info("GitHub username: %s", github_user.login)
         logm.info("Orgs:")
         for org_name in self.get_org_names():
             logm.info("  %s", org_name)
 
     def class_check(self, class_name: str) -> None:
         logm.info("Validating class '%s'", class_name)
 
         class_to_validate = self.classes.get_class(class_name)
         logm.info("Moderators:")
-        self.validate_users(class_to_validate.moderators)
+        self._validate_users(class_to_validate.moderators)
         logm.info("Members:")
-        self.validate_users(class_to_validate.members)
+        self._validate_users(class_to_validate.members)
 
-    def create_personal_class_repos_in_org(self, org_name: str, class_name: str, repo_prefix: str | None, template_repo_full_name: str | None) -> None:
+    def org_create_personal_repos(self, org_name: str, class_name: str, repo_prefix: str | None, template_repo_full_name: str | None) -> None:
         logm.info("Create class repos in org '%s' for class '%s'", org_name, class_name)
 
         selected_class = self.classes.get_class(class_name)
-        org = self.get_org(org_name)
+        org = self._get_org(org_name)
+        template_repo = self._get_template_repo(template_repo_full_name) if template_repo_full_name else None
 
-        template_repo: github.Repository.Repository | None = None
-        if template_repo_full_name:
-            template_repo = self.get_repo(template_repo_full_name)
-            if not template_repo.is_template:
-                logm.error("Repo '%s' is not a template! Unable to create personal class repos!", template_repo.name)
-                sys.exit(-1)
-
-        for class_member in selected_class.active_members:
-            repo_name = class_member.generate_personal_repo_name(repo_prefix)
-            if template_repo:
-                org.create_repo_from_template(repo_name, template_repo, private=True)
-                logm.info("Created personal class repo '%s' from template '%s'", repo_name, template_repo.full_name)
-            else:
-                org.create_repo(repo_name, private=True, auto_init=True)
-                logm.info("Created personal class repo '%s'", repo_name)
+        with alive_bar(len(selected_class.members), title="Creating personal repo:", enrich_print=False) as bar:
+            for class_member in selected_class.active_members:
+                self._repo_create(org, class_member, repo_prefix, template_repo)
+                bar()
 
-        for class_member in selected_class.inactive_members:
-            logm.info("Skipping repo creation of '%s' due to inactivity of class member", class_member.fullname)
+            for class_member in selected_class.inactive_members:
+                logm.info("Skipping repo creation of '%s' due to inactivity of class member", class_member.fullname)
+                bar()
 
-    def create_reviews_for_repos_in_org(self, org_name: str, class_name: str, head_branch_name: str, review_branch_name: str) -> None:
+    def org_reviews_create(self, org_name: str, class_name: str, head_branch_name: str, review_branch_name: str) -> None:
 
         logm.info("Create reviews in '%s' for class '%s'", org_name, class_name)
 
         selected_class = self.classes.get_class(class_name)
 
-        org = self.get_org(org_name)
+        org = self._get_org(org_name)
         repos = org.get_repos()
 
         pr_title = "Review"
 
-        for class_member in selected_class.active_members:
+        active_members = list(selected_class.active_members)
 
-            logm.info("Class member: '%s'", class_member)
+        with alive_bar(len(active_members), title="Cloning repos:", enrich_print=False) as bar:
+            for class_member in active_members:
 
-            repo = class_member.find_personal_repo(repos)
+                logm.info("Class member: '%s'", class_member)
 
-            if repo is None:
-                logm.warning("Failed to create review for '%s' ('%s')! Unable to find repo in org '%s'",
-                                class_member.fullname, class_member.github_username, org_name)
-                continue
+                repo = class_member.find_personal_repo(repos)
 
-            logm.info("Repo: '%s'", repo.full_name)
+                if repo is None:
+                    logm.warning("Failed to create review for '%s' ('%s')! Unable to find repo in org '%s'",
+                                 class_member.fullname, class_member.github_username, org_name)
+                    continue
 
-            if self.get_branch_by_name(repo, review_branch_name) is None:
-                commit_history = repo.get_commits().reversed
-                first_commit = commit_history[0]
+                logm.info("Repo: '%s'", repo.full_name)
 
-                repo.create_git_ref(f'refs/heads/{review_branch_name}', first_commit.sha)
-                logm.info("Created '%s' branch from first commit ('%s')", review_branch_name, first_commit)
-            else:
-                logm.warning("Branch '%s' already existing in repo '%s'!", review_branch_name, repo.name)
+                if self._get_branch_by_name(repo, review_branch_name) is None:
+                    commit_history = repo.get_commits().reversed
+                    first_commit = commit_history[0]
 
-            if self.get_pull_request_by_title(repo, pr_title) is not None:
-                logm.warning("Pull-Request with '%s' already existing in repo '%s'!", review_branch_name, repo.name)
-                continue
-
-            base_branch = self.get_branch_by_name(repo, review_branch_name)
-            head_branch = self.get_branch_by_name(repo, head_branch_name)
-
-            if base_branch.commit.sha == head_branch.commit.sha:
-                logm.warning("Unable to create PR! Base branch '%s' and head branch '%s' are equal.",
-                                base_branch.name, head_branch.name)
-                continue
+                    repo.create_git_ref(f'refs/heads/{review_branch_name}', first_commit.sha)
+                    logm.info("Created '%s' branch from first commit ('%s')", review_branch_name, first_commit)
+                else:
+                    logm.warning("Branch '%s' already existing in repo '%s'!", review_branch_name, repo.name)
 
-            try:
-                repo.create_pull(review_branch_name, head_branch_name, title=pr_title)
-                logm.info("Created pullrequest '%s' <- '%s' in repository '%s'", review_branch_name,
-                             head_branch_name, repo.name)
-            except github.GithubException as e:
-                logm.error("Create pullrequest failed with message: '$s'", e.message)
+                if self._get_pull_request_by_title(repo, pr_title) is not None:
+                    logm.warning("Pull-Request with '%s' already existing in repo '%s'!", review_branch_name, repo.name)
+                    continue
+
+                base_branch = self._get_branch_by_name(repo, review_branch_name)
+                head_branch = self._get_branch_by_name(repo, head_branch_name)
+
+                if base_branch.commit.sha == head_branch.commit.sha:
+                    logm.warning("Unable to create PR! Base branch '%s' and head branch '%s' are equal.",
+                                    base_branch.name, head_branch.name)
+                    continue
+                try:
+                    repo.create_pull(review_branch_name, head_branch_name, title=pr_title)
+                    logm.info("Created pullrequest '%s' <- '%s' in repository '%s'", review_branch_name,
+                              head_branch_name, repo.name)
+                except github.GithubException as e:
+                    logm.error("Create pullrequest failed with message: '$s'", e.message)
+            bar()
 
-    def grant_access_to_personal_class_repos_in_org(self, org_name: str, selected_class_members: List[Member],
-                                                    permission: str) -> None:
+    def org_access_grant_personal_repos(self, org_name: str, selected_class_members: List[Member],
+                                        permission: str) -> None:
         logm.info("Grant access to personal class repos in org '%s' for the following class members:", org_name)
+        org = self._get_org(org_name)
 
-        org = self.get_org(org_name)
-
-        with alive_bar(len(selected_class_members), title="Granting access:") as bar:
+        with alive_bar(len(selected_class_members), title="Granting access:", enrich_print=False) as bar:
             for class_member in selected_class_members:
                 repo_name = class_member.generate_personal_repo_name()
-
-                class_member_named_user = self.get_named_user(class_member.github_username)
-
                 repo = org.get_repo(repo_name)
-                repo.add_to_collaborators(class_member_named_user, permission=permission)
-                logm.info("Granted access to personal class repo for '%s' -> '%s, permission: '%s'", class_member, repo_name,
-                             permission)
+                self._repo_access_grant(repo, class_member, permission)
                 bar()
 
-    def revoke_access_from_personal_class_repos_in_org(self, org_name: str, selected_class_members: List[Member],) -> None:
+    def org_access_revoke_personal_repos(self, org_name: str, selected_class_members: List[Member], ) -> None:
         logm.info("Revoke access from personal class repos in org '%s' for the following class members:'", org_name)
 
-        org = self.get_org(org_name)
+        org = self._get_org(org_name)
 
-        with alive_bar(len(selected_class_members), title="Revoking access:") as bar:
-            for class_member in selected_class_members:
-                repo_name = class_member.generate_personal_repo_name()
-                class_member_named_user = self.get_named_user(class_member.github_username)
-                try:
-                    repo = org.get_repo(repo_name)
-                    repo.remove_from_collaborators(class_member_named_user)
+        for class_member in selected_class_members:
+            repo_name = class_member.generate_personal_repo_name()
+            class_member_named_user = self._get_named_user(class_member.github_username)
+            try:
+                repo = org.get_repo(repo_name)
+                repo.remove_from_collaborators(class_member_named_user)
 
-                    self.remove_invitation(repo, class_member_named_user)
+                self._repo_remove_invitation(repo, class_member_named_user)
 
-                    logm.info("Revoked access from personal class repo '%s' for '%s'", repo.full_name, class_member)
-                except github.UnknownObjectException as e:
-                    logm.error("%s", e)
-                    logm.error("Unable to revoke access for '%s'", repo_name)
-                bar()
+                logm.info("Revoked access from personal class repo '%s' for '%s'", repo.full_name, class_member)
+            except github.UnknownObjectException as e:
+                logm.error("%s", e)
+                logm.error("Unable to revoke access for '%s'", repo_name)
 
-    def grant_class_access_to_repo(self, full_repo_name: str, selected_class_members: List[Member], permission: str) -> None:
+    def repo_access_grant_for_class(self, full_repo_name: str, selected_class_members: List[Member], permission: str) -> None:
         logm.info("Grant class access to repo '%s' with permission '%s' for the following class members:",
                   full_repo_name, permission)
 
-        repo = self.get_repo(full_repo_name)
+        repo = self._get_repo(full_repo_name)
 
-        with alive_bar(len(selected_class_members), title="Granting access:") as bar:
+        with alive_bar(len(selected_class_members), title="Granting access:", enrich_print=False) as bar:
             for class_member in selected_class_members:
-                class_member_named_user = self.get_named_user(class_member.github_username)
-                logm.info("Inviting class member '%s' to repo '%s' with permission: '%s'", class_member, repo.full_name, permission)
-                repo.add_to_collaborators(class_member_named_user, permission=permission)
-                logm.info("Invited successfully!")
+                logm.info("Granting access for '%s' to repo '%s' with permission: '%s'", class_member, repo.full_name, permission)
+                self._repo_access_grant(repo, class_member, permission)
                 bar()
 
-    def revoke_class_access_from_repo(self, full_repo_name: str, selected_class_members: List[Member],) -> None:
+    def repo_access_revoke_for_class(self, full_repo_name: str, selected_class_members: List[Member], ) -> None:
         logm.info("Revoke class access from repo '%s' for the following class members.", full_repo_name)
 
-        repo = self.get_repo(full_repo_name)
+        repo = self._get_repo(full_repo_name)
 
-        with alive_bar(len(selected_class_members), title="Revoke access:") as bar:
+        with alive_bar(len(selected_class_members), title="Revoke access:", enrich_print=False) as bar:
             for class_member in selected_class_members:
-                class_member_named_user = self.get_named_user(class_member.github_username)
+                class_member_named_user = self._get_named_user(class_member.github_username)
                 try:
                     repo.remove_from_collaborators(class_member_named_user)
-                    self.remove_invitation(repo, class_member_named_user)
+                    self._repo_remove_invitation(repo, class_member_named_user)
 
                     logm.info("Revoked access from repo '%s' for user '%s'", repo.full_name, class_member)
                 except github.UnknownObjectException as e:
                     logm.error("%s", e)
                     logm.error("Unable to revoke access from repo '%s' for user '%s'", repo.full_name, class_member)
                 bar()
 
-    def clone_org(self, org_name: str, working_dir: Path) -> None:
-        logm.info("Cloning all repos of org '%s'", org_name)
-
-        backup_dir = working_dir / org_name
-        backup_dir.mkdir(exist_ok=False)
-
-        org = self.get_org(org_name)
-        repos = org.get_repos()
-
-        with alive_bar(repos.totalCount, title="Cloning repos:") as bar:
-            for repo in repos:
-                backup_repo_dir = backup_dir / repo.name
-                logm.info("Cloning repo '%s' -> '%s'", repo.clone_url, backup_repo_dir)
-                backup_repo_dir.mkdir()
-                self.clone_repo(repo.clone_url, backup_repo_dir)
-                bar()
-
     def repo_print_details(self, full_repo_name: str) -> None:
-        repo = self.get_repo(full_repo_name)
+        repo = self._get_repo(full_repo_name)
 
         logm.info("Repository details '%s':", full_repo_name)
         logm.info("  - Created: %s", repo.created_at)
         logm.info("  - Modified: %s", repo.last_modified)
 
         logm.info("  - Pending invitations:")
         invitations = repo.get_pending_invitations()
@@ -339,7 +359,24 @@
             logm.info("    - %s: %s", invitation.invitee.login, invitation.permissions)
 
         logm.info("  - Collaborators:")
         collaborators = repo.get_collaborators()
         for collaborator in collaborators:
             collaborator_permission = repo.get_collaborator_permission(collaborator)
             logm.info("    - %s: %s", collaborator.login, collaborator_permission)
+
+    def clone_org(self, org_name: str, working_dir: Path) -> None:
+        logm.info("Cloning all repos of org '%s'", org_name)
+
+        backup_dir = working_dir / org_name
+        backup_dir.mkdir(exist_ok=False)
+
+        org = self._get_org(org_name)
+        repos = org.get_repos()
+
+        with alive_bar(repos.totalCount, title="Cloning repos:", enrich_print=False) as bar:
+            for repo in repos:
+                backup_repo_dir = backup_dir / repo.name
+                logm.info("Cloning repo '%s' -> '%s'", repo.clone_url, backup_repo_dir)
+                backup_repo_dir.mkdir()
+                self._repo_clone(repo.clone_url, backup_repo_dir)
+                bar()
```

### Comparing `classroom_utils-0.3.2/classroom_utils/local_operations.py` & `classroom_utils-0.4.0/classroom_utils/local_operations.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/main.py` & `classroom_utils-0.4.0/classroom_utils/main.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/resources/schemas/classlist_file_schema.json` & `classroom_utils-0.4.0/classroom_utils/resources/schemas/classlist_file_schema.json`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils/subcommands.py` & `classroom_utils-0.4.0/classroom_utils/subcommands.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/classroom_utils.egg-info/PKG-INFO` & `classroom_utils-0.4.0/classroom_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom_utils
-Version: 0.3.2
+Version: 0.4.0
 Summary: Utilities to handle stuff likes github orgs for classes.
 Home-page: https://github.com/twyleg/classroom_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: class classroom github edu education
 Description-Content-Type: text/markdown
```

### Comparing `classroom_utils-0.3.2/classroom_utils.egg-info/SOURCES.txt` & `classroom_utils-0.4.0/classroom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/setup.py` & `classroom_utils-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/tests/test_config.py` & `classroom_utils-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/tests/test_example.py` & `classroom_utils-0.4.0/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/tests/test_github_operations.py` & `classroom_utils-0.4.0/tests/test_github_operations.py`

 * *Files identical despite different names*

### Comparing `classroom_utils-0.3.2/versioneer.py` & `classroom_utils-0.4.0/versioneer.py`

 * *Files identical despite different names*

