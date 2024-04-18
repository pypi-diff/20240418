# Comparing `tmp/iam_builder-4.2.2.tar.gz` & `tmp/iam_builder-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_builder-4.2.2.tar", max compression
+gzip compressed data, was "iam_builder-4.3.0.tar", max compression
```

## Comparing `iam_builder-4.2.2.tar` & `iam_builder-4.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5141 2024-02-27 14:07:35.831352 iam_builder-4.2.2/README.md
--rw-r--r--   0        0        0        0 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/__init__.py
--rw-r--r--   0        0        0      803 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/command_line.py
--rw-r--r--   0        0        0       93 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/exceptions.py
--rw-r--r--   0        0        0     3227 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/iam_builder.py
--rw-r--r--   0        0        0      430 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/iam_schema.py
--rw-r--r--   0        0        0     2993 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/schemas/iam_schema.json
--rwxr-xr-x   0        0        0    11274 2024-02-27 14:07:35.831352 iam_builder-4.2.2/iam_builder/templates.py
--rw-r--r--   0        0        0      476 2024-02-27 14:07:35.831352 iam_builder-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 iam_builder-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5365 2024-04-18 13:42:16.185654 iam_builder-4.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/command_line.py
+-rw-r--r--   0        0        0       93 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/exceptions.py
+-rw-r--r--   0        0        0     3414 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/iam_builder.py
+-rw-r--r--   0        0        0      430 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/iam_schema.py
+-rw-r--r--   0        0        0     3216 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/schemas/iam_schema.json
+-rwxr-xr-x   0        0        0    11633 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/templates.py
+-rw-r--r--   0        0        0      476 2024-04-18 13:42:16.185654 iam_builder-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 iam_builder-4.3.0/PKG-INFO
```

### Comparing `iam_builder-4.2.2/README.md` & `iam_builder-4.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 
   read_write:
     - test_bucket_read_write/*
     - test_bucket_read_only/write_folder/*
 
   deny:
     - test_bucket_read_write/sensitive_table/*
+
+kms:
+  - test_kms_key_arn
 ```
 
 Whilst the example json (`iam_config.json`) looks like this:
 
 ```json
 {
   "iam_role_name": "iam_role_name",
@@ -89,15 +92,16 @@
       "test_bucket_write_only/*",
       "test_bucket_read_only/write_only_folder/*"
     ],
     "read_write": [
       "test_bucket_read_write/*",
       "test_bucket_read_only/write_folder/*"
     ]
-  }
+  },
+  "kms": ["test_kms_key_arn"]
 }
 ```
 - **iam_role_name:** The role name of your airflow job; required if you want to run glue jobs or access secrets.
 
 - **athena:** Can have two keys. 
   - **write**: Either `true` or `false`. If `false` then only read access to Athena (cannot create, delete or alter tables, databases and partitions). If `true` then the role will also have the ability to do stuff like CTAS queries, `DROP TABLE`, `CREATE DATABASE`, etc.
   - **dump_bucket**: The location in S3 (either an S3 path or a list of S3 paths) for temporarily storing the results of queries. This defaults to `mojap-athena-query-dump` and should not normally need changing.
@@ -111,14 +115,18 @@
   - **read_only:** A list of s3 paths that the iam_role should be able to access (read only). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **write_only:** A list of s3 paths that the iam_role should be able to access (write only). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **read_write:** A list of s3 paths that the iam_role should be able to access (read and write). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **deny:** A list of s3 paths that the iam_role should _not_ be able to access. This should be used to add exceptions to wildcarded access to folders, for example excluding sensitive tables in order to provide basic access to a database. Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
+
+- **kms:**: A list of kms arns that the iam_role should be able to access. Can call the DescribeKey, GenerateDataKey, Decrypt, Encrypt and ReEncrypt 
+  operations.
+
 ## How to update
 
 When updating IAM builder, make sure to change the version number in `pyproject.toml` and describe the change in `CHANGELOG.md`.
 
 If you have changed any dependencies in `pyproject.yaml`, run `poetry update` to update `poetry.lock`.
 
 Once you have created a release in GitHub, a Github Action will run to publish the release on PyPI automatically.
```

### Comparing `iam_builder-4.2.2/iam_builder/command_line.py` & `iam_builder-4.3.0/iam_builder/command_line.py`

 * *Files identical despite different names*

### Comparing `iam_builder-4.2.2/iam_builder/iam_builder.py` & `iam_builder-4.3.0/iam_builder/iam_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     get_pass_role_to_glue_policy,
     get_read_only_policy,
     get_write_only_policy,
     get_read_write_policy,
     get_deny_policy,
     get_s3_list_bucket_policy,
     get_secrets,
+    get_kms_permissions
 )
 from iam_builder.iam_schema import validate_iam
 
 
 def build_iam_policy(config: dict) -> dict:  # noqa: C901
     """
     Takes a configuration for an IAM policy and returns the policy as a dict.
@@ -86,8 +87,13 @@
         secrets = config["secrets"]
         if isinstance(secrets, str) or secrets:
             readwrite = secrets == "readwrite"
             secrets_statement = get_secrets(config["iam_role_name"], readwrite)
             iam["Statement"].append(secrets_statement)
             iam["Statement"].extend(iam_lookup["decrypt_statement"])
 
+    if "kms" in config:
+        kms_arns = config["kms"]
+        kms_permissions = get_kms_permissions(kms_arns)
+        iam["Statement"].append(kms_permissions)
+
     return iam
```

### Comparing `iam_builder-4.2.2/iam_builder/schemas/iam_schema.json` & `iam_builder-4.3.0/iam_builder/schemas/iam_schema.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'properties'": "{'kms': OrderedDict([('description', 'A list of kms key arns that the iam_role "*

 * *                 "should be able to acces.'), ('type', 'array'), ('items', OrderedDict([('type', "*

 * *                 "'string')]))])}"}*

```diff
@@ -30,14 +30,21 @@
             "description": "glue_job must be set to true to allow role to run glue jobs",
             "type": "boolean"
         },
         "iam_role_name": {
             "description": "The role name of the airflow job",
             "type": "string"
         },
+        "kms": {
+            "description": "A list of kms key arns that the iam_role should be able to acces.",
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
         "role_duration_seconds": {
             "description": "Max duration role can be assumed for in seconds",
             "type": "integer"
         },
         "s3": {
             "additionalProperties": false,
             "description": "S3 access configuration",
```

### Comparing `iam_builder-4.2.2/iam_builder/templates.py` & `iam_builder-4.3.0/iam_builder/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -368,7 +368,22 @@
                 "ssm:GetParametersByPath"
             ],
             "Resource": [
                 f"arn:aws:ssm:*:*:parameter/alpha/airflow/{iam_role}/*"
             ]
         }
     return statement
+
+def get_kms_permissions(kms_arns: list) -> dict:
+    policy = {
+        "Sid": "kmsPermissions",
+        "Action": [
+            "kms:ReEncrypt*",
+            "kms:GenerateDataKey*",
+            "kms:Encrypt",
+            "kms:DescribeKey",
+            "kms:Decrypt"
+        ],
+        "Effect": "Allow",
+        "Resource": kms_arns,
+    }
+    return policy
```

### Comparing `iam_builder-4.2.2/PKG-INFO` & `iam_builder-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam_builder
-Version: 4.2.2
+Version: 4.3.0
 Summary: A lil python package to generate iam policies
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -86,14 +86,17 @@
 
   read_write:
     - test_bucket_read_write/*
     - test_bucket_read_only/write_folder/*
 
   deny:
     - test_bucket_read_write/sensitive_table/*
+
+kms:
+  - test_kms_key_arn
 ```
 
 Whilst the example json (`iam_config.json`) looks like this:
 
 ```json
 {
   "iam_role_name": "iam_role_name",
@@ -110,15 +113,16 @@
       "test_bucket_write_only/*",
       "test_bucket_read_only/write_only_folder/*"
     ],
     "read_write": [
       "test_bucket_read_write/*",
       "test_bucket_read_only/write_folder/*"
     ]
-  }
+  },
+  "kms": ["test_kms_key_arn"]
 }
 ```
 - **iam_role_name:** The role name of your airflow job; required if you want to run glue jobs or access secrets.
 
 - **athena:** Can have two keys. 
   - **write**: Either `true` or `false`. If `false` then only read access to Athena (cannot create, delete or alter tables, databases and partitions). If `true` then the role will also have the ability to do stuff like CTAS queries, `DROP TABLE`, `CREATE DATABASE`, etc.
   - **dump_bucket**: The location in S3 (either an S3 path or a list of S3 paths) for temporarily storing the results of queries. This defaults to `mojap-athena-query-dump` and should not normally need changing.
@@ -132,14 +136,18 @@
   - **read_only:** A list of s3 paths that the iam_role should be able to access (read only). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **write_only:** A list of s3 paths that the iam_role should be able to access (write only). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **read_write:** A list of s3 paths that the iam_role should be able to access (read and write). Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
 
   - **deny:** A list of s3 paths that the iam_role should _not_ be able to access. This should be used to add exceptions to wildcarded access to folders, for example excluding sensitive tables in order to provide basic access to a database. Each item in the list should either be a path to a object or finish with `/*` to denote that it can access everything within that directory. _Note the S3 paths don't start with `s3://` in the config._
+
+- **kms:**: A list of kms arns that the iam_role should be able to access. Can call the DescribeKey, GenerateDataKey, Decrypt, Encrypt and ReEncrypt 
+  operations.
+
 ## How to update
 
 When updating IAM builder, make sure to change the version number in `pyproject.toml` and describe the change in `CHANGELOG.md`.
 
 If you have changed any dependencies in `pyproject.yaml`, run `poetry update` to update `poetry.lock`.
 
 Once you have created a release in GitHub, a Github Action will run to publish the release on PyPI automatically.
```

