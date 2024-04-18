# Comparing `tmp/fast_dev_cli-0.6.6.tar.gz` & `tmp/fast_dev_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.6.6.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.7.0.tar", max compression
```

## Comparing `fast_dev_cli-0.6.6.tar` & `fast_dev_cli-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.6.6/LICENSE
--rw-r--r--   0        0        0     1755 2024-04-07 08:42:22.439293 fast_dev_cli-0.6.6/README.md
--rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.6.6/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.6.6/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    20963 2024-04-12 08:59:28.048538 fast_dev_cli-0.6.6/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.6.6/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1357 2024-04-12 08:59:28.049030 fast_dev_cli-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 fast_dev_cli-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1755 2024-04-07 08:42:22.439293 fast_dev_cli-0.7.0/README.md
+-rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.7.0/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.0/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    20260 2024-04-18 04:13:37.056185 fast_dev_cli-0.7.0/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.0/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1225 2024-04-18 04:09:13.720129 fast_dev_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.0/PKG-INFO
```

### Comparing `fast_dev_cli-0.6.6/LICENSE` & `fast_dev_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.6/README.md` & `fast_dev_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.6/fast_dev_cli/cli.py` & `fast_dev_cli-0.7.0/fast_dev_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,15 +242,16 @@
             parent = parent.parent
         return None
 
     @classmethod
     def get_work_dir(
         cls: Type[Self], name=TOML_FILE, cwd: Path | None = None, allow_cwd=False
     ) -> Path:
-        if d := cls.work_dir(name, cwd or Path.cwd(), cls.path_depth):
+        cwd = cwd or Path.cwd()
+        if d := cls.work_dir(name, cwd, cls.path_depth):
             return d
         if allow_cwd:
             return cls.get_root_dir(cwd)
         raise EnvError(f"{name} not found! Make sure this is a poetry project.")
 
     @classmethod
     def load_toml_text(cls: Type[Self]) -> str:
@@ -418,15 +419,15 @@
                 _upgrade += " && "
             _upgrade += command + dev_flags + " " + " ".join(dev_args)
         for single in others:
             _upgrade += f" && poetry add {' '.join(single)}"
         return _upgrade
 
     def gen(self: Self) -> str:
-        return self.gen_cmd() + " && poetry update"
+        return self.gen_cmd() + " && poetry lock && poetry update"
 
 
 @cli.command()
 def upgrade(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Upgrade dependencies in pyproject.toml to latest versions"""
@@ -483,44 +484,28 @@
     def __init__(self: Self, args, check_only=False, _exit=False, dry=False) -> None:
         self.args = args
         self.check_only = check_only
         super().__init__(_exit, dry)
 
     @staticmethod
     def check_lint_tool_installed() -> bool:
-        return check_call("black --version")
+        return check_call("ruff --version")
 
     @classmethod
     def to_cmd(cls: Type[Self], paths=".", check_only=False) -> str:
         cmd = ""
-        tools = ["isort --profile=black", "black", "ruff check --fix", "mypy"]
+        tools = ["ruff check --extend-select=I --fix", "ruff format", "mypy"]
         if check_only:
-            tools[0] += " --check-only"
-            tools[1] += " --check --fast"
+            tools[1] += " --check"
         if check_only or load_bool("NO_FIX"):
-            tools[2] = tools[2].replace(" --fix", "")
+            tools[0] = tools[0].replace(" --fix", "")
         if load_bool("SKIP_MYPY"):
             # Sometimes mypy is too slow
             tools = tools[:-1]
         lint_them = " && ".join("{0}{%d} {1}" % i for i in range(2, len(tools) + 2))
-        current_path = Path.cwd()
-        root = Project.get_work_dir(cwd=current_path, allow_cwd=True)
-        app_name = root.name.replace("-", "_")
-        if (app_dir := root / app_name).exists() or (app_dir := root / "app").exists():
-            if current_path == app_dir:
-                tools[0] += " --src=."
-            elif current_path == root:
-                tools[0] += f" --src={app_dir.name}"
-            else:
-                parents = "../"
-                for i, p in enumerate(current_path.parents):
-                    if p == root:
-                        parents *= i + 1
-                        break
-                tools[0] += f" --src={parents}{app_dir.name}"
         prefix = "poetry run "
         if is_venv():
             if cls.check_lint_tool_installed():
                 prefix = ""
             else:
                 if check_call("python -c 'import fast_dev_cli'"):
                     command = 'python -m pip install -U "fast_dev_cli[all]"'
@@ -546,15 +531,15 @@
 
 @cli.command(name="lint")
 def make_style(
     files: list[str],
     check_only: bool = Option(False, "--check-only", "-c"),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
-    """Run: isort+black+ruff to reformat code and then mypy to check"""
+    """Run: ruff check/format to reformat code and then mypy to check"""
     if isinstance(files, str):
         files = [files]
     if check_only:
         check(files, dry=dry)
     else:
         lint(files, dry=dry)
```

### Comparing `fast_dev_cli-0.6.6/pyproject.toml` & `fast_dev_cli-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.6.6"
+version = "0.7.0"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 click = ">=7.1.1"
-isort = {version = ">=5.12.0", optional = true}
-black = {version = ">=23.9.1", optional = true}
 ruff = {version = ">=0.3", optional = true}
 mypy = {version = ">=1.5.0", optional = true}
 coverage = {version = ">=6.5.0", optional = true}
 bumpversion = {version = "^0.6.0", optional = true}
 pytest = {version = "^8.1.1", optional = true}
 typer = {version = ">=0.12.0", optional = true}
 
 [tool.poetry.extras]
-all = ["isort", "black", "ruff", "typer", "mypy", "bumpversion", "pytest", "coverage"]
+all = ["ruff", "typer", "mypy", "bumpversion", "pytest", "coverage"]
 
 [tool.poetry.group.dev.dependencies]
-isort = "*"
-black = "*"
 ruff = ">=0.3"
 mypy = "*"
 pytest = "*"
 coverage = "*"
 bumpversion = "*"
 typer = {extras = ["all"], version = "*"}
 ipython = "^8.23.0"
@@ -37,16 +33,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fast = "fast_dev_cli:cli"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+target-version = "py311"
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
```

### Comparing `fast_dev_cli-0.6.6/PKG-INFO` & `fast_dev_cli-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.6.6
+Version: 0.7.0
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
-Requires-Dist: black (>=23.9.1) ; extra == "all"
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all"
 Requires-Dist: click (>=7.1.1)
 Requires-Dist: coverage (>=6.5.0) ; extra == "all"
-Requires-Dist: isort (>=5.12.0) ; extra == "all"
 Requires-Dist: mypy (>=1.5.0) ; extra == "all"
 Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "all"
 Requires-Dist: ruff (>=0.3) ; extra == "all"
 Requires-Dist: typer (>=0.12.0) ; extra == "all"
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.6.6 Summary: Author: Waket
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.0 Summary: Author: Waket
 Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: all Requires-Dist: black (>=23.9.1) ; extra == "all" Requires-
-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist: click
-(>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-Dist:
-isort (>=5.12.0) ; extra == "all" Requires-Dist: mypy (>=1.5.0) ; extra ==
-"all" Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "all" Requires-Dist:
-ruff (>=0.3) ; extra == "all" Requires-Dist: typer (>=0.12.0) ; extra == "all"
-Description-Content-Type: text/markdown
+Provides-Extra: all Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra ==
+"all" Requires-Dist: click (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra
+== "all" Requires-Dist: mypy (>=1.5.0) ; extra == "all" Requires-Dist: pytest
+(>=8.1.1,<9.0.0) ; extra == "all" Requires-Dist: ruff (>=0.3) ; extra == "all"
+Requires-Dist: typer (>=0.12.0) ; extra == "all" Description-Content-Type:
+text/markdown
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                                     _S_t_a_t_u_s_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
```

