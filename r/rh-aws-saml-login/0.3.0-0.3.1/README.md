# Comparing `tmp/rh_aws_saml_login-0.3.0.tar.gz` & `tmp/rh_aws_saml_login-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rh_aws_saml_login-0.3.0.tar", max compression
+gzip compressed data, was "rh_aws_saml_login-0.3.1.tar", max compression
```

## Comparing `rh_aws_saml_login-0.3.0.tar` & `rh_aws_saml_login-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3292 2024-03-12 12:22:04.976163 rh_aws_saml_login-0.3.0/README.md
--rw-r--r--   0        0        0     1867 2024-03-12 12:22:04.984162 rh_aws_saml_login-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 12:22:04.984162 rh_aws_saml_login-0.3.0/rh_aws_saml_login/__init__.py
--rw-r--r--   0        0        0     2790 2024-03-12 12:22:04.984162 rh_aws_saml_login-0.3.0/rh_aws_saml_login/__main__.py
--rw-r--r--   0        0        0     8085 2024-03-12 12:22:04.985162 rh_aws_saml_login-0.3.0/rh_aws_saml_login/core.py
--rw-r--r--   0        0        0     1448 2024-03-12 12:22:04.985162 rh_aws_saml_login-0.3.0/rh_aws_saml_login/utils.py
--rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.0/setup.py
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3292 2024-04-18 07:57:45.743430 rh_aws_saml_login-0.3.1/README.md
+-rw-r--r--   0        0        0     2131 2024-04-18 07:57:45.751430 rh_aws_saml_login-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 07:57:45.751430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/__init__.py
+-rw-r--r--   0        0        0     2795 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/__main__.py
+-rw-r--r--   0        0        0     8107 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/core.py
+-rw-r--r--   0        0        0     1464 2024-04-18 07:57:45.752430 rh_aws_saml_login-0.3.1/rh_aws_saml_login/utils.py
+-rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.1/setup.py
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 rh_aws_saml_login-0.3.1/PKG-INFO
```

### Comparing `rh_aws_saml_login-0.3.0/README.md` & `rh_aws_saml_login-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rh_aws_saml_login-0.3.0/pyproject.toml` & `rh_aws_saml_login-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rh-aws-saml-login"
-version = "0.3.0"
+version = "0.3.1"
 description = "A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "rh_aws_saml_login" }]
 homepage = "https://github.com/app-sre/rh-aws-saml-login"
 repository = "https://github.com/app-sre/rh-aws-saml-login"
@@ -18,15 +18,15 @@
 rich = "^13.7.0"
 pyquery = "^2.0.0"
 boto3 = "^1.34.37"
 tzlocal = "^5.2"
 humanize = "^4.9.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.1"
+ruff = "^0.3.7"
 types-requests = "^2.31.0.20240125"
 pytest = "^8.0.0"
 mypy = "^1.8.0"
 requests-mock = "^1.11.0"
 
 [build-system]
 requires = ["poetry-core"]
@@ -34,15 +34,15 @@
 
 [tool.poetry.scripts]
 rh-aws-saml-login = 'rh_aws_saml_login.__main__:app'
 
 [tool.ruff]
 line-length = 88
 target-version = 'py311'
-required-version = "0.2.1"
+required-version = "0.3.7"
 src = ["rh_aws_saml_login"]
 extend-exclude = [".local", ".cache"]
 fix = true
 
 [tool.ruff.lint]
 preview = true
 # defaults are ["E4", "E7", "E9", "F"]
@@ -59,14 +59,25 @@
 
 [tool.ruff.format]
 preview = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["rh_aws_saml_login"]
 
+[tool.mypy]
+files = ["rh_aws_saml_login"]
+enable_error_code = ["truthy-bool", "redundant-expr"]
+no_implicit_optional = true
+check_untyped_defs = true
+warn_unused_ignores = true
+show_error_codes = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+
+
 [[tool.mypy.overrides]]
 # Below are all of the packages that don't implement stub packages. Mypy will throw an error if we don't ignore the
 # missing imports. See: https://mypy.readthedocs.io/en/stable/running_mypy.html#missing-imports
 module = [
     "requests_kerberos.*",
     "iterfzf.*",
     "botocore.*",
```

### Comparing `rh_aws_saml_login-0.3.0/rh_aws_saml_login/__main__.py` & `rh_aws_saml_login-0.3.1/rh_aws_saml_login/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+from collections.abc import Generator
 from pathlib import Path
 
 import typer
 from rich import print
 
 from rh_aws_saml_login import core
 from rh_aws_saml_login.utils import blend_text, enable_requests_logging
@@ -31,18 +32,17 @@
 def read_accounts_cache() -> list[str]:
     """Read accounts cache from disk."""
     if ACCOUNT_CACHE.exists():
         return json.load(ACCOUNT_CACHE.open())
     return []
 
 
-def complete_account(ctx: typer.Context, incomplete: str):
-    names = ctx.params.get("account_name") or []
+def complete_account(ctx: typer.Context, incomplete: str) -> Generator[str, None, None]:
     for name in read_accounts_cache():
-        if name.startswith(incomplete) and name not in names:
+        if name.startswith(incomplete):
             yield name
 
 
 @app.command(epilog="Made with [red]:heart:[/] by [blue]https://github.com/app-sre[/]")
 def cli(  # noqa: PLR0913, PLR0917
     account_name: str = typer.Argument(
         None,
@@ -55,15 +55,15 @@
         False, help="Open the AWS console in browser instead of a local shell"
     ),
     display_banner: bool = typer.Option(True, help="Display a shiny banner"),
     saml_url: str = typer.Option(
         "https://auth.redhat.com/auth/realms/EmployeeIDP/protocol/saml/clients/itaws",
         help="SAML URL",
     ),
-):
+) -> None:
     """Login to AWS using SAML."""
     logging.basicConfig(
         level=logging.INFO if not debug else logging.DEBUG, format="%(message)s"
     )
     if display_banner:
         print(blend_text(BANNER, (32, 32, 255), (255, 32, 255)))
     if debug:
```

### Comparing `rh_aws_saml_login-0.3.0/rh_aws_saml_login/core.py` & `rh_aws_saml_login-0.3.1/rh_aws_saml_login/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     try:
         run(["klist", "--test"], check=True)
         return True
     except subprocess.CalledProcessError:
         return False
 
 
-def kinit():
+def kinit() -> None:
     """Acquire a kerberos ticket."""
     run(["kinit"], check=True, capture_output=False)
 
 
 def get_saml_auth(url: str) -> tuple[str, str]:
     with requests.Session() as session:
         session.auth = HTTPKerberosAuth(mutual_authentication=OPTIONAL)
@@ -141,15 +141,17 @@
         access_key=response["Credentials"]["AccessKeyId"],
         secret_key=response["Credentials"]["SecretAccessKey"],
         session_token=response["Credentials"]["SessionToken"],
         expiration=response["Credentials"]["Expiration"],
     )
 
 
-def open_aws_shell(account: AwsAccount, credentials: AwsCredentials, region: str):
+def open_aws_shell(
+    account: AwsAccount, credentials: AwsCredentials, region: str
+) -> None:
     print(
         dedent(f"""
             Spawning a new shell. Use exit or CTRL+d to leave it!
 
             :nerd_face: {account.name}
             :rocket: {account.role_name}
             :hourglass: {humanize.naturaltime(credentials.expiration)} ({credentials.expiration.astimezone(tz=get_localzone())})
```

### Comparing `rh_aws_saml_login-0.3.0/rh_aws_saml_login/utils.py` & `rh_aws_saml_login-0.3.1/rh_aws_saml_login/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     for index in range(size):
         blend = index / size
         color = f"#{int(r1 + dr * blend):2X}{int(g1 + dg * blend):2X}{int(b1 + db * blend):2X}"
         text.stylize(color, index, index + 1)
     return text
 
 
-def bye():
+def bye() -> None:
     print(
         "Thank you for using rh-aws-saml-login. :man_bowing: Have a great day ahead! :red_heart-emoji:"
     )
 
 
-def enable_requests_logging():
+def enable_requests_logging() -> None:
     from http.client import HTTPConnection  # noqa: PLC0415
 
     HTTPConnection.debuglevel = 1
     logging.getLogger().setLevel(logging.DEBUG)
     requests_log = logging.getLogger("urllib3")
     requests_log.setLevel(logging.DEBUG)
     requests_log.propagate = True
```

### Comparing `rh_aws_saml_login-0.3.0/setup.py` & `rh_aws_saml_login-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tzlocal>=5.2,<6.0']
 
 entry_points = \
 {'console_scripts': ['rh-aws-saml-login = rh_aws_saml_login.__main__:app']}
 
 setup_kwargs = {
     'name': 'rh-aws-saml-login',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP',
     'long_description': '# rh-aws-saml-login\n\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n[![PyPI](https://img.shields.io/pypi/v/rh-aws-saml-login)][pypi-link]\n[![PyPI platforms][pypi-platforms]][pypi-link]\n![PyPI - License](https://img.shields.io/pypi/l/rh-aws-saml-login)\n\nA CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP.\n\n![demo](/demo/quickstart.gif)\n\n## Pre-requisites\n\n- Python 3.11 or later\n- Connected to Red Hat VPN\n- A Red Hat managed computer (Kerberos must be installed and configured) and you are logged in with your Red Hat account\n\n## How it works\n\nThe `rh-aws-saml-login` CLI is a tool that simplifies the process of logging into an AWS account via Red Hat SSO. It retrieves a SAML token from the Red Hat SSO server, then fetches and parses the AWS SSO login page to present you with a list of all available accounts and their respective roles. You can then choose your desired account and role, and `rh-aws-saml-login` uses the SAML token to generate temporary AWS role credentials. Finally, it spawns a new shell with the necessary `AWS_` environment variables already set up, so you can immediately use the `aws` CLI without any further configuration.\n\n## Installation\n\nOn CSB Fedora, you need to install the Kerberos development package:\n\n```shell\nsudo dnf install krb5-devel\n```\n\nYou can install this library from [PyPI][pypi-link] with `pip`:\n\n```shell\npython3 -m pip install rh-aws-saml-login\n```\n\nor install it with `pipx`:\n\n```shell\npipx install rh-aws-saml-login\n```\n\nYou can also use `pipx` to run the library without installing it:\n\n```shell\npipx run rh-aws-saml-login\n```\n\n## Usage\n\n```shell\nrh-aws-saml-login\n```\n\nThis spawns a new shell with the following environment variables are set:\n\n- `AWS_ACCOUNT_NAME`: The name/alias of the AWS account\n- `AWS_ROLE_NAME`:  The name of the role\n- `AWS_ROLE_ARN`: The ARN of the role\n- `AWS_ACCESS_KEY_ID`: The access key used by the AWS CLI\n- `AWS_SECRET_ACCESS_KEY`: The secret access key used by the AWS CLI\n- `AWS_SESSION_TOKEN`: The session token used by the AWS CLI\n- `AWS_REGION`: The default region used by the AWS CLI\n\n## Features\n\nrh-aws-saml-login currently provides the following features (get help with `-h` or `--help`):\n\n- No configuration needed\n- Uses Kerberos authentication\n- Open the AWS web console for an account with the `--console` option\n- Shell auto-completion (bash, zsh, and fish) including AWS account names\n- Integrates nicely with the [starship](https://starship.rs)\n\n  ```toml\n   [env_var.AWS_ACCOUNT_NAME]\n   format = "$symbol$style [$env_value]($style) "\n   style = "cyan"\n   symbol = "🚀"\n  ```\n\n## Development\n\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n\n- Update CHANGELOG.md with the new version number and date\n- Bump the version number in [pyproject.toml](/pyproject.toml)\n\n[pypi-link]:                https://pypi.org/project/rh-aws-saml-login/\n[pypi-platforms]:           https://img.shields.io/pypi/pyversions/rh-aws-saml-login\n',
     'author': 'Christian Assing',
     'author_email': 'cassing@redhat.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/app-sre/rh-aws-saml-login',
```

### Comparing `rh_aws_saml_login-0.3.0/PKG-INFO` & `rh_aws_saml_login-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rh-aws-saml-login
-Version: 0.3.0
+Version: 0.3.1
 Summary: A CLI tool that allows you to log in and retrieve AWS temporary credentials using Red Hat SAML IDP
 Home-page: https://github.com/app-sre/rh-aws-saml-login
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

