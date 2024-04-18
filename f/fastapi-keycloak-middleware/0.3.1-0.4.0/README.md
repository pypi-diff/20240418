# Comparing `tmp/fastapi_keycloak_middleware-0.3.1.tar.gz` & `tmp/fastapi_keycloak_middleware-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_keycloak_middleware-0.3.1.tar", max compression
+gzip compressed data, was "fastapi_keycloak_middleware-0.4.0.tar", max compression
```

## Comparing `fastapi_keycloak_middleware-0.3.1.tar` & `fastapi_keycloak_middleware-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/LICENSE
--rw-r--r--   0        0        0     4016 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/README.md
--rw-r--r--   0        0        0     1369 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/decorators/__init__.py
--rw-r--r--   0        0        0     5182 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/decorators/require_permission.py
--rw-r--r--   0        0        0      856 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/decorators/strip_request.py
--rw-r--r--   0        0        0      352 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/dependencies/__init__.py
--rw-r--r--   0        0        0      467 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
--rw-r--r--   0        0        0      420 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/dependencies/get_user.py
--rw-r--r--   0        0        0      703 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/exceptions.py
--rw-r--r--   0        0        0     1042 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/fast_api_user.py
--rw-r--r--   0        0        0     7773 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/keycloak_backend.py
--rw-r--r--   0        0        0     7954 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/middleware.py
--rw-r--r--   0        0        0        0 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/__init__.py
--rw-r--r--   0        0        0      523 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/authorization_methods.py
--rw-r--r--   0        0        0     1233 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/authorization_result.py
--rw-r--r--   0        0        0     6112 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
--rw-r--r--   0        0        0      581 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/match_strategy.py
--rw-r--r--   0        0        0      739 2024-03-03 18:12:05.487428 fastapi_keycloak_middleware-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.3.1/setup.py
--rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4016 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/README.md
+-rw-r--r--   0        0        0     1481 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/__init__.py
+-rw-r--r--   0        0        0     5169 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/require_permission.py
+-rw-r--r--   0        0        0      856 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/strip_request.py
+-rw-r--r--   0        0        0      352 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/__init__.py
+-rw-r--r--   0        0        0      467 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
+-rw-r--r--   0        0        0      420 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/dependencies/get_user.py
+-rw-r--r--   0        0        0      703 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/exceptions.py
+-rw-r--r--   0        0        0     1042 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/fast_api_user.py
+-rw-r--r--   0        0        0     7773 2024-04-18 18:10:41.863168 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/keycloak_backend.py
+-rw-r--r--   0        0        0     7995 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_methods.py
+-rw-r--r--   0        0        0     1257 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_result.py
+-rw-r--r--   0        0        0      232 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/exception_response.py
+-rw-r--r--   0        0        0     6452 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
+-rw-r--r--   0        0        0      581 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/match_strategy.py
+-rw-r--r--   0        0        0     5775 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/setup.py
+-rw-r--r--   0        0        0      739 2024-04-18 18:10:41.867169 fastapi_keycloak_middleware-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.0/setup.py
+-rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.0/PKG-INFO
```

### Comparing `fastapi_keycloak_middleware-0.3.1/LICENSE` & `fastapi_keycloak_middleware-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/README.md` & `fastapi_keycloak_middleware-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/__init__.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Middleware for FastAPI that supports authenticating users against Keycloak
 """
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 import logging
 
 from fastapi_keycloak_middleware.decorators.require_permission import require_permission
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.dependencies.get_authorization_result import (
     get_authorization_result,
@@ -18,22 +18,24 @@
     AuthorizationMethod,
 )
 from fastapi_keycloak_middleware.schemas.authorization_result import AuthorizationResult
 from fastapi_keycloak_middleware.schemas.keycloak_configuration import (
     KeycloakConfiguration,
 )
 from fastapi_keycloak_middleware.schemas.match_strategy import MatchStrategy
+from fastapi_keycloak_middleware.setup import setup_keycloak_middleware
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __all__ = [
     AuthorizationResult.__name__,
     KeycloakMiddleware.__name__,
     KeycloakConfiguration.__name__,
     AuthorizationMethod.__name__,
     MatchStrategy.__name__,
     FastApiUser.__name__,
     get_user.__name__,
     get_authorization_result.__name__,
     require_permission.__name__,
+    setup_keycloak_middleware.__name__,
     strip_request.__name__,
 ]
```

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/decorators/require_permission.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/require_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import typing
 from collections import OrderedDict
 from functools import wraps
 from inspect import Parameter, signature
 from typing import Callable
 
 import starlette
-from starlette.exceptions import HTTPException
+from fastapi import HTTPException
 from starlette.requests import Request
 
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.schemas.authorization_methods import (
     AuthorizationMethod,
 )
 from fastapi_keycloak_middleware.schemas.authorization_result import AuthorizationResult
```

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/decorators/strip_request.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/decorators/strip_request.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/exceptions.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/fast_api_user.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/fast_api_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/keycloak_backend.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/keycloak_backend.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/middleware.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 here: https://github.com/code-specialist/fastapi-auth-middleware
 """
 
 import logging
 import re
 import typing
 
-from fastapi import FastAPI
 from starlette.requests import HTTPConnection
-from starlette.responses import PlainTextResponse
-from starlette.types import Receive, Scope, Send
+from starlette.responses import JSONResponse
+from starlette.types import ASGIApp, Receive, Scope, Send
 
 from fastapi_keycloak_middleware.exceptions import (
     AuthHeaderMissing,
     AuthInvalidToken,
     AuthTokenExpired,
     AuthUserError,
 )
@@ -58,15 +57,15 @@
         extracted from the token to permissions meaningful for your application,
         defaults to None
     :type scope_mapper: typing.Callable[[typing.List[str]], typing.List[str]], optional
     """
 
     def __init__(
         self,
-        app: FastAPI,
+        app: ASGIApp,
         keycloak_configuration: KeycloakConfiguration,
         exclude_patterns: typing.List[str] = None,
         user_mapper: typing.Callable[
             [typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]
         ] = None,
         scope_mapper: typing.Callable[[typing.List[str]], typing.List[str]] = None,
     ):
@@ -160,53 +159,55 @@
         except AuthInvalidToken:
             response = self._invalid_token()
             log.warning("Provided access token could not be validated")
             await response(scope, receive, send)
             return
 
         except Exception as exc:  # pylint: disable=broad-except
-            response = PlainTextResponse(
-                f"An error occurred: {exc.__class__.__name__}", status_code=401
+            response = JSONResponse(
+                {"detail": f"An error occurred: {exc.__class__.__name__}"},
+                status_code=401,
             )
             log.error("An error occurred while authenticating the user")
             await response(scope, receive, send)
             return
 
         log.debug("Sending request to next middleware")
         await self.app(scope, receive, send)  # Token is valid
 
     @staticmethod
     def _auth_header_missing(*args, **kwargs):  # pylint: disable=unused-argument
         """
         Returns a response notifying the user that the request
         is missing an 'Authorization' HTTP header.
         """
-        return PlainTextResponse(
-            "Your request is missing an 'Authorization' HTTP header", status_code=401
+        return JSONResponse(
+            {"detail": "Your request is missing an 'Authorization' HTTP header"},
+            status_code=401,
         )
 
     @staticmethod
     def _token_has_expired(*args, **kwargs):  # pylint: disable=unused-argument
         """
         Returns a response notifying the user that the token has expired.
         """
-        return PlainTextResponse(
-            "Your 'Authorization' HTTP header is invalid", status_code=401
+        return JSONResponse(
+            {"detail": "Your 'Authorization' HTTP header is invalid"}, status_code=401
         )
 
     @staticmethod
     def _user_not_found(*args, **kwargs):  # pylint: disable=unused-argument
         """
         Returns a response notifying the user that the user was not found.
         """
-        return PlainTextResponse(
-            "Could not find a user based on this token", status_code=401
+        return JSONResponse(
+            {"detail": "Could not find a user based on this token"}, status_code=401
         )
 
     @staticmethod
     def _invalid_token(*args, **kwargs):  # pylint: disable=unused-argument
         """
         Returns a response notifying the user that the acess token is invalid.
         """
-        return PlainTextResponse(
-            "Unable to verify provided access token", status_code=401
+        return JSONResponse(
+            {"detail": "Unable to verify provided access token"}, status_code=401
         )
```

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/authorization_methods.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/authorization_result.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/authorization_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
     The following attributes will be set when returning the class in your
     path function:
     """
 
     #: The method that was used to authorize the user
     method: typing.Union[None, AuthorizationMethod] = Field(
-        None,
+        default=None,
         title="Method",
         description="The method used to authorize the user.",
     )
     #: Whether the user is authorized or not
     authorized: bool = Field(
-        False,
+        default=False,
         title="Authorized",
         description="Whether the user is authorized or not.",
     )
     #: The scopes that matched the user's scopes
     matched_scopes: typing.List[str] = Field(
-        [],
+        default=[],
         title="Matched Scopes",
         description="The scopes that matched the user's scopes.",
     )
```

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/keycloak_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     :param realm: Keycloak realm that should be used for token authentication.
     :type realm: str
     :param url: URL of the Keycloak server. If you use legacy Keycloak versions
         or still have the auth context, you need to add the auth context to the URL.
     :type url: str
     :param client_id: Client ID of the client used to validate the token.
     :type client_id: str
+    :param swagger_client_id: Client ID for swagger UI authentication. Defaults to None.
+    :type swagger_client_id: str, optional
     :param client_secret: Client secret of the client used to validate the token.
         The client secret is only needed if you use the introspection endpoint.
     :type client_secret: str, optional
     :param claims: List of claims that should be extracted from the access token.
         Defaults to
         ``["sub", "name", "family_name", "given_name", "preferred_username", "email"]``.
     :type claims: list[str], optional
@@ -60,78 +62,81 @@
         function. Defaults to ``{"verify_signature": True, "verify_aud": True,
         "verify_exp": True}``. See the following project for an overview of
         acceptable options:
         https://github.com/mpdavis/python-jose/blob/4b0701b46a8d00988afcc5168c2b3a1fd60d15d8/jose/jwt.py#L81
     :type decode_options: Dict[str, Union[bool,int]], optional
     """
 
-    realm: str = Field(..., title="Realm", description="The realm to use.")
-    url: str = Field(..., title="URL", description="The URL of the Keycloak server.")
-    client_id: str = Field(..., title="Client ID", description="The client ID.")
+    realm: str = Field(title="Realm", description="The realm to use.")
+    url: str = Field(title="URL", description="The URL of the Keycloak server.")
+    client_id: str = Field(title="Client ID", description="The client ID.")
+    swagger_client_id: Optional[str] = Field(
+        title="Swagger Client ID", description="The client ID for the swagger UI."
+    )
     client_secret: Optional[str] = Field(
-        None, title="Client Secret", description="The client secret."
+        default=None, title="Client Secret", description="The client secret."
     )
     claims: list[str] = Field(
-        [
+        default=[
             "sub",
             "name",
             "family_name",
             "given_name",
             "preferred_username",
             "email",
         ],
         title="Claims",
         description="The claims to add to the user object.",
     )
     reject_on_missing_claim: bool = Field(
-        True,
+        default=True,
         title="Reject on Missing Claim",
         description="Whether to reject the request if a claim is missing.",
     )
     authentication_scheme: str = Field(
-        "Bearer",
+        default="Bearer",
         title="Authentication Scheme",
         description="The authentication scheme to use.",
     )
     authorization_method: AuthorizationMethod = Field(
-        AuthorizationMethod.NONE,
+        default=AuthorizationMethod.NONE,
         title="Authorization Method",
         description="The authorization method to use.",
     )
     authorization_claim: str = Field(
-        "roles",
+        default="roles",
         title="Authorization Claim",
         description="The claim to use for authorization.",
     )
     use_introspection_endpoint: bool = Field(
-        False,
+        default=False,
         title="Use Introspection Endpoint",
         description="Whether to use the introspection endpoint.",
     )
     enable_device_authentication: bool = Field(
-        False,
+        default=False,
         title="Enable Device Authentication",
         description="Whether to enable device authentication. If device authentication"
         " is enabled, the middleware will ignore required user claims and not attempt"
         " to map the user. The token will be validated and then the request"
         " forwarded unmodified.",
     )
     device_authentication_claim: str = Field(
-        "is_device",
+        default="is_device",
         title="Device Authentication Claim",
         description="The claim that will be checked. If present and if it evaluates to"
         " true, the device authentication will be applied for the request.",
     )
     verify: Union[bool, str] = Field(
-        True,
+        default=True,
         title="Verify",
         description="Whether to verify the SSL connection",
     )
     decode_options: Dict[str, Union[bool, int]] = Field(
-        {
+        default={
             "verify_signature": True,
             "verify_aud": True,
             "verify_exp": True,
         },
         title="JWT Decode Options",
         description="Decode options that are passed to python-jose decode function.",
     )
```

### Comparing `fastapi_keycloak_middleware-0.3.1/fastapi_keycloak_middleware/schemas/match_strategy.py` & `fastapi_keycloak_middleware-0.4.0/fastapi_keycloak_middleware/schemas/match_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.3.1/pyproject.toml` & `fastapi_keycloak_middleware-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-keycloak-middleware"
-version = "0.3.1"
+version = "0.4.0"
 description = "Middleware for FastAPI to authenticate a user against keycloak"
 authors = ["Daniel Herrmann <daniel.herrmann1@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "fastapi_keycloak_middleware" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fastapi_keycloak_middleware-0.3.1/setup.py` & `fastapi_keycloak_middleware-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.73.0', 'install>=1.3.5,<2.0.0', 'python-keycloak>2.14.0,<3.9.1']
 
 setup_kwargs = {
     'name': 'fastapi-keycloak-middleware',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Middleware for FastAPI to authenticate a user against keycloak',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)\n[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)\n![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)\n![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/waza-ari/fastapi-keycloak-middleware/development.svg)](https://results.pre-commit.ci/latest/github/waza-ari/fastapi-keycloak-middleware/development)\n\n\n# FastAPI Keycloak Middleware\n\n**Full documentation** is [available at Read The Docs](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/)\n\nThis package provides a middleware for [FastAPI](http://fastapi.tiangolo.com)  that\nsimplifies integrating with [Keycloak](http://keycloak.org) for\nauthentication and authorization. It supports OIDC and supports validating access\ntokens, reading roles and basic authentication. In addition it provides several\ndecorators and dependencies to easily integrate into your FastAPI application.\n\nIt relies on the [python-keycloak](http://python-keycloak.readthedocs.io) package,\nwhich is the only dependency outside of the FastAPI ecosystem which would be installed\nanyway. Shoutout to the author of [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich served as inspiration for this package and some of its code.\n\nIn the future, I plan to add support for fine grained authorization using Keycloak\nAuthorization services.\n\n## Motivation\n\nUsing FastAPI and Keycloak quite a lot, and keeping to repeat myself quite a lot when\nit comes to authentiating users, I decided to create this library to help with this.\n\nThere is a clear separation between the authentication and authorization:\n\n- **Authentication** is about verifying the identity of the user\n  (who they are). This is done by an authentication backend\n  that verifies the users access token obtained from the\n  identity provider (Keycloak in this case).\n- **Authorization** is about deciding which resources can be\n  accessed. This package providers convenience decoraters to\n  enforce certain roles or permissions on FastAPI endpoints.\n\n## Installation\n\nInstall the package using poetry:\n\n```bash\npoetry add fastapi-keycloak-middleware\n```\n\nor `pip`:\n\n```bash\npip install fastapi-keycloak-middleware\n```\n\n## Features\n\nThe package helps with:\n\n* An easy to use middleware that validates the request for an access token\n* Validation can done in one of two ways:\n   * Validate locally using the public key obtained from Keycloak\n   * Validate using the Keycloak token introspection endpoint\n* Using Starlette authentication mechanisms to store both the user object as well as the authorization scopes in the Request object\n* Ability to provide custom callback functions to retrieve the user object (e.g. from your database) and to provide an arbitrary mapping to authentication scopes (e.g. roles to permissions)\n* A decorator to use previously stored information to enforce certain roles or permissions on FastAPI endpoints\n* Convenience dependencies to retrieve the user object or the authorization result after evaluation within the FastAPI endpoint\n\n## Acknowledgements\n\nThis package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich provides some of the same functionality but without the direct integration\ninto Keycloak. Thanks for writing and providing this great piece of software!\n\n## Development\n\nThis project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used\nto work locally and also to test Github actions before deploying them.\n',
     'author': 'Daniel Herrmann',
     'author_email': 'daniel.herrmann1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_keycloak_middleware-0.3.1/PKG-INFO` & `fastapi_keycloak_middleware-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-keycloak-middleware
-Version: 0.3.1
+Version: 0.4.0
 Summary: Middleware for FastAPI to authenticate a user against keycloak
 Author: Daniel Herrmann
 Author-email: daniel.herrmann1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

