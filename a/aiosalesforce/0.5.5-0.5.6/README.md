# Comparing `tmp/aiosalesforce-0.5.5.tar.gz` & `tmp/aiosalesforce-0.5.6.tar.gz`

## Comparing `aiosalesforce-0.5.5.tar` & `aiosalesforce-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/__init__.py
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/client.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/py.typed
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/sobject.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/utils.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/__init__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/base.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/client_credentials_flow.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/jwt_bearer_flow.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/auth/soap.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/__init__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/_csv.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/client.py
--rw-r--r--   0        0        0    13354 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/ingest.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/event_bus.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/events/events.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/__init__.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/policy.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/src/aiosalesforce/retries/rules.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/LICENSE
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/README.md
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/__init__.py
+-rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/client.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/py.typed
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/sobject.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/auth/__init__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/auth/base.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/auth/client_credentials_flow.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/auth/jwt_bearer_flow.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/auth/soap.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/bulk/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/__init__.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/_csv.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/client.py
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/ingest.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/events/__init__.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/events/event_bus.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/events/events.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/retries/__init__.py
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/retries/policy.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/src/aiosalesforce/retries/rules.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/README.md
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 aiosalesforce-0.5.6/PKG-INFO
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/__init__.py` & `aiosalesforce-0.5.6/src/aiosalesforce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 __all__ = [
     "ClientCredentialsFlow",
     "JwtBearerFlow",
     "SoapLogin",
     "Salesforce",
     "BulkApiBatchConsumptionEvent",
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/client.py` & `aiosalesforce-0.5.6/src/aiosalesforce/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,18 +60,15 @@
     concurrency_limit : int, optional
         Maximum number of simultaneous requests to Salesforce.
         The default is 100.
 
     """
 
     httpx_client: httpx.AsyncClient
-    base_url: str
-    """Base URL in the format https://[subdomain(s)].my.salesforce.com"""
     auth: Auth
-    version: str
     event_bus: EventBus
     retry_policy: RetryPolicy
     _semaphore: asyncio.Semaphore
 
     def __init__(
         self,
         httpx_client: httpx.AsyncClient,
@@ -79,46 +76,60 @@
         auth: Auth,
         version: str = "60.0",
         event_hooks: Iterable[Callable[[Event], Awaitable[None] | None]] | None = None,
         retry_policy: RetryPolicy | None = POLICY_DEFAULT,
         concurrency_limit: int = 100,
     ) -> None:
         self.httpx_client = httpx_client
+        self.base_url = base_url
         self.auth = auth
+        self.version = version
 
-        # Validate version
-        if not (match_ := re.fullmatch(r"^(v)?(\d+)(\.(0)?)?$", version)):
+        self.event_bus = EventBus(event_hooks)
+        self.retry_policy = retry_policy or RetryPolicy()
+        self._semaphore = asyncio.Semaphore(concurrency_limit)
+
+    @property
+    def version(self) -> str:
+        return self.__version
+
+    @version.setter
+    def version(self, value: str) -> None:
+        """API version in the format '60.0'."""
+        if not (match_ := re.fullmatch(r"^(v)?(\d+)(\.(0)?)?$", value)):
             raise ValueError(
-                f"Invalid Salesforce API version: '{version}'. "
+                f"Invalid Salesforce API version: '{value}'. "
                 f"A valid version should look like '60.0'."
             )
-        self.version = f"{match_.groups()[1]}.0"
+        self.__version = f"{match_.groups()[1]}.0"
+
+    @property
+    def base_url(self) -> str:
+        """Base URL in the format https://[subdomain(s)].my.salesforce.com"""
+        return self.__base_url
 
-        # Validate url
+    @base_url.setter
+    def base_url(self, value: str) -> None:
         match_ = re.fullmatch(
             r"(https://[a-zA-Z0-9-]+(\.(sandbox|develop))?\.my\.salesforce\.com).*",
-            base_url.strip(" ").lower(),
+            value.strip(" ").lower(),
         )
         if not match_:
             raise ValueError(
                 "\n".join(
                     [
-                        f"Invalid Salesforce URL: {base_url}",
+                        f"Invalid Salesforce URL: {value}",
                         "Supported formats:",
                         "  Production    : https://[MyDomainName].my.salesforce.com",
                         "  Sandbox       : https://[MyDomainName]-[SandboxName].sandbox.my.salesforce.com",
                         "  Developer org : https://[MyDomainName].develop.my.salesforce.com",
                     ]
                 )
             )
-        self.base_url = str(match_.groups()[0])
-
-        self.event_bus = EventBus(event_hooks)
-        self.retry_policy = retry_policy or RetryPolicy()
-        self._semaphore = asyncio.Semaphore(concurrency_limit)
+        self.__base_url = str(match_.groups()[0])
 
     @wraps(httpx.AsyncClient.request)
     async def request(self, *args, **kwargs) -> httpx.Response:
         """
         Make an HTTP request to Salesforce.
 
         """
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/exceptions.py` & `aiosalesforce-0.5.6/src/aiosalesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/sobject.py` & `aiosalesforce-0.5.6/src/aiosalesforce/sobject.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/utils.py` & `aiosalesforce-0.5.6/src/aiosalesforce/utils.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/auth/base.py` & `aiosalesforce-0.5.6/src/aiosalesforce/auth/base.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/auth/client_credentials_flow.py` & `aiosalesforce-0.5.6/src/aiosalesforce/auth/client_credentials_flow.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/auth/jwt_bearer_flow.py` & `aiosalesforce-0.5.6/src/aiosalesforce/auth/jwt_bearer_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 
         if jwt is None or serialization is None:  # pragma: no cover
             raise ImportError("Install aiosalesforce[jwt] to use the JwtBearerFlow.")
 
     async def _acquire_new_access_token(self, client: "Salesforce") -> str:
         payload = {
             "iss": self.client_id,
-            "aud": "https://sandbox.salesforce.com"
-            if "sandbox" in client.base_url.lower()
+            "aud": "https://test.salesforce.com"
+            if client.base_url.endswith(".sandbox.my.salesforce.com")
             else "https://login.salesforce.com",
             "sub": self.username,
             "exp": int(time.time()) + 300,
         }
         with open(self.private_key_file, "rb") as file:
             private_key = serialization.load_pem_private_key(
                 data=file.read(),
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/auth/soap.py` & `aiosalesforce-0.5.6/src/aiosalesforce/auth/soap.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/_csv.py` & `aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,24 +178,24 @@
             yield buffer.content
             buffer.flush()
 
     if buffer.size > 0:
         yield buffer.content
 
 
-def deserialize_ingest_results(data: bytes) -> list[dict[str, Any]]:
+def deserialize_ingest_results(data: bytes) -> list[dict[str, str]]:
     """
     Deserialize Salesforce Bulk API 2.0 ingest results from CSV.
 
     Parameters
     ----------
     data : bytes
         CSV file as a byte string.
 
     Returns
     -------
-    list[dict[str, Any]]
+    list[dict[str, str]]
         List of records as dictionaries.
 
     """
     reader = csv.DictReader(data.decode("utf-8").splitlines())
     return list(reader)
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/client.py` & `aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from .ingest import BulkIngestClient, JobInfo, OperationType
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class IngestResult:
-    """Bulk API 2.0 ingest job result."""
+    """Bulk API 2.0 ingest operation result."""
 
     jobs: list[JobInfo]
-    successful_results: list[dict[str, Any]]
-    failed_results: list[dict[str, Any]]
-    unprocessed_records: list[dict[str, Any]]
+    successful_results: list[dict[str, str]]
+    failed_results: list[dict[str, str]]
+    unprocessed_records: list[dict[str, str]]
 
 
 class BulkClientV2:
     """
     Salesforce Bulk API 2.0 client.
 
     Use this client to execute bulk ingest and query operations.
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/bulk/v2/ingest.py` & `aiosalesforce-0.5.6/src/aiosalesforce/bulk/v2/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,38 +65,45 @@
         "PIPE",
         "SEMICOLON",
         "TAB",
     ]
 
     @classmethod
     def from_json(cls, data: bytes) -> Self:
-        return cls(
+        job_info = cls(
             **{
                 field.name: (_ := json_loads(data)).get(
                     "".join(
                         [
                             component.capitalize() if i > 0 else component
                             for i, component in enumerate(field.name.split("_"))
                         ]
                     ),
                     None,
                 )
                 for field in dataclasses.fields(cls)
             }
         )
+        for attr in ["created_date", "system_modstamp"]:
+            setattr(
+                job_info,
+                attr,
+                datetime.datetime.fromisoformat(getattr(job_info, attr)),
+            )
+        return job_info
 
 
 @dataclasses.dataclass
 class JobResult:
     """Bulk API 2.0 ingest job result."""
 
     job_info: JobInfo
-    successful_results: list[dict[str, Any]]
-    failed_results: list[dict[str, Any]]
-    unprocessed_records: list[dict[str, Any]]
+    successful_results: list[dict[str, str]]
+    failed_results: list[dict[str, str]]
+    unprocessed_records: list[dict[str, str]]
 
 
 class BulkIngestClient:
     """
     Salesforce Bulk API 2.0 ingest client.
 
     This is a low-level client used to manage ingest jobs.
```

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/events/event_bus.py` & `aiosalesforce-0.5.6/src/aiosalesforce/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/events/events.py` & `aiosalesforce-0.5.6/src/aiosalesforce/events/events.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/retries/__init__.py` & `aiosalesforce-0.5.6/src/aiosalesforce/retries/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/retries/policy.py` & `aiosalesforce-0.5.6/src/aiosalesforce/retries/policy.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/src/aiosalesforce/retries/rules.py` & `aiosalesforce-0.5.6/src/aiosalesforce/retries/rules.py`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/LICENSE` & `aiosalesforce-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/README.md` & `aiosalesforce-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/pyproject.toml` & `aiosalesforce-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiosalesforce-0.5.5/PKG-INFO` & `aiosalesforce-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aiosalesforce
-Version: 0.5.5
+Version: 0.5.6
 Summary: Salesforce REST API client
 Project-URL: Homepage, https://github.com/georgebv/aiosalesforce
 Project-URL: Documentation, https://github.com/georgebv/aiosalesforce
 Project-URL: Repository, https://github.com/georgebv/aiosalesforce
 Author-email: Georgii Bocharov <bocharovgeorgii@gmail.com>
 License: Copyright 2024 Georgii Bocharov
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: aiosalesforce Version: 0.5.5 Summary: Salesforce
+Metadata-Version: 2.3 Name: aiosalesforce Version: 0.5.6 Summary: Salesforce
 REST API client Project-URL: Homepage, https://github.com/georgebv/
 aiosalesforce Project-URL: Documentation, https://github.com/georgebv/
 aiosalesforce Project-URL: Repository, https://github.com/georgebv/
 aiosalesforce Author-email: Georgii Bocharov
 gmail.com> License: Copyright 2024 Georgii Bocharov Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
```

