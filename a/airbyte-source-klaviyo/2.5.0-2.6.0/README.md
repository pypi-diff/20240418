# Comparing `tmp/airbyte_source_klaviyo-2.5.0.tar.gz` & `tmp/airbyte_source_klaviyo-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_klaviyo-2.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_klaviyo-2.6.0.tar", max compression
```

## Comparing `airbyte_source_klaviyo-2.5.0.tar` & `airbyte_source_klaviyo-2.6.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     4519 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/README.md
--rw-r--r--   0        0        0      746 2024-04-15 16:12:34.687305 airbyte_source_klaviyo-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/__init__.py
--rw-r--r--   0        0        0      975 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/availability_strategy.py
--rw-r--r--   0        0        0      865 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/components/datetime_based_cursor.py
--rw-r--r--   0        0        0      196 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/exceptions.py
--rw-r--r--   0        0        0     5924 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/manifest.yaml
--rw-r--r--   0        0        0      233 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/run.py
--rw-r--r--   0        0        0     4491 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/campaigns.json
--rw-r--r--   0        0        0      935 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/email_templates.json
--rw-r--r--   0        0        0     2136 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/events.json
--rw-r--r--   0        0        0     2262 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/flows.json
--rw-r--r--   0        0        0     3931 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/global_exclusions.json
--rw-r--r--   0        0        0     1839 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/lists.json
--rw-r--r--   0        0        0      787 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/metrics.json
--rw-r--r--   0        0        0     3931 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/profiles.json
--rw-r--r--   0        0        0     2892 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/shared/subscriptions.json
--rw-r--r--   0        0        0     1020 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/source.py
--rw-r--r--   0        0        0     1114 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/spec.json
--rw-r--r--   0        0        0    10876 2024-04-15 07:04:29.000000 airbyte_source_klaviyo-2.5.0/source_klaviyo/streams.py
--rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/README.md
+-rw-r--r--   0        0        0      746 2024-04-18 16:17:22.539022 airbyte_source_klaviyo-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/availability_strategy.py
+-rw-r--r--   0        0        0      865 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/components/datetime_based_cursor.py
+-rw-r--r--   0        0        0      196 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/exceptions.py
+-rw-r--r--   0        0        0     6817 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/run.py
+-rw-r--r--   0        0        0      167 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns.json
+-rw-r--r--   0        0        0     1921 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns_detailed.json
+-rw-r--r--   0        0        0      935 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/email_templates.json
+-rw-r--r--   0        0        0     2136 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/events.json
+-rw-r--r--   0        0        0     2262 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/flows.json
+-rw-r--r--   0        0        0     3931 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/global_exclusions.json
+-rw-r--r--   0        0        0      163 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/lists.json
+-rw-r--r--   0        0        0      561 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/lists_detailed.json
+-rw-r--r--   0        0        0      787 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/metrics.json
+-rw-r--r--   0        0        0     3931 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/profiles.json
+-rw-r--r--   0        0        0     4091 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/campaign_properties.json
+-rw-r--r--   0        0        0     1591 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/list_properties.json
+-rw-r--r--   0        0        0     2892 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/subscriptions.json
+-rw-r--r--   0        0        0     1183 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/source.py
+-rw-r--r--   0        0        0     1114 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/spec.json
+-rw-r--r--   0        0        0    11531 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/streams.py
+-rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.6.0/PKG-INFO
```

### Comparing `airbyte_source_klaviyo-2.5.0/README.md` & `airbyte_source_klaviyo-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/pyproject.toml` & `airbyte_source_klaviyo-2.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.0"
+version = "2.6.0"
 name = "airbyte-source-klaviyo"
 description = "Source implementation for Klaviyo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/availability_strategy.py` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/components/datetime_based_cursor.py` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/components/datetime_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/manifest.yaml` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/manifest.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: 0.81.3
+version: 0.81.6
 type: DeclarativeSource
 
 definitions:
   # Authenticator
   authenticator:
     type: ApiKeyAuthenticator
     api_token: "Klaviyo-API-Key {{ config['api_key'] }}"
@@ -15,19 +15,25 @@
   requester:
     type: HttpRequester
     url_base: "https://a.klaviyo.com/api/"
     authenticator: "#/definitions/authenticator"
     http_method: GET
     error_handler:
       type: DefaultErrorHandler
+      backoff_strategies:
+        - type: WaitTimeFromHeader
+          header: "Retry-After"
       response_filters:
         - type: HttpResponseFilter
           action: FAIL
           http_codes: [401, 403]
           error_message: Please provide a valid API key and make sure it has permissions to read specified streams.
+        - type: HttpResponseFilter
+          action: RETRY
+          http_codes: [429]
     request_headers:
       Accept: "application/json"
       Revision: "2023-10-15"
 
   # Selector
   selector:
     type: RecordSelector
@@ -173,22 +179,43 @@
   lists_stream:
     # Docs: https://developers.klaviyo.com/en/reference/get_lists
     name: "lists"
     $ref: "#/definitions/base_semi_incremental_stream"
     $parameters:
       path: "lists"
 
+  lists_detailed_stream:
+    # Docs: https://developers.klaviyo.com/en/reference/get_list
+    name: "lists_detailed"
+    $ref: "#/definitions/base_semi_incremental_stream"
+    retriever:
+      $ref: "#/definitions/base_retriever"
+      requester:
+        $ref: "#/definitions/requester"
+        request_parameters:
+          "additional-fields[list]": "profile_count"
+      partition_router:
+        type: SubstreamPartitionRouter
+        parent_stream_configs:
+          - type: ParentStreamConfig
+            parent_key: "id"
+            stream: "#/definitions/lists_stream"
+            partition_field: "id"
+    $parameters:
+      path: "lists/{{ stream_slice.id }}"
+
 streams:
   # Incremental streams
   - "#/definitions/profiles_stream"
   - "#/definitions/global_exclusions_stream"
   - "#/definitions/events_stream"
   - "#/definitions/email_templates_stream"
 
   # Semi-Incremental streams
   - "#/definitions/metrics_stream"
   - "#/definitions/lists_stream"
+  - "#/definitions/lists_detailed_stream"
 
 check:
   type: CheckStream
   stream_names:
     - metrics
```

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/campaigns.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/campaign_properties.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.05555555555555555%*

 * *Differences: {"'attributes'": "OrderedDict([('type', ['null', 'object']), ('additionalProperties', True), "*

 * *                 "('properties', OrderedDict([('name', OrderedDict([('type', 'string')])), "*

 * *                 "('status', OrderedDict([('type', 'string')])), ('archived', "*

 * *                 "OrderedDict([('type', 'boolean')])), ('channel', OrderedDict([('type', "*

 * *                 "'string')])), ('audiences', OrderedDict([('type', ['null', 'object']), "*

 * *                 "('additionalProperties', True), ('properties […]*

```diff
@@ -1,297 +1,292 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
-    "properties": {
-        "attributes": {
-            "additionalProperties": true,
-            "properties": {
-                "archived": {
-                    "type": "boolean"
-                },
-                "audiences": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "excluded": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
+    "attributes": {
+        "additionalProperties": true,
+        "properties": {
+            "archived": {
+                "type": "boolean"
+            },
+            "audiences": {
+                "additionalProperties": true,
+                "properties": {
+                    "excluded": {
+                        "items": {
                             "type": [
                                 "null",
-                                "array"
+                                "string"
                             ]
                         },
-                        "included": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "array"
+                        ]
                     },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "channel": {
-                    "type": "string"
-                },
-                "created_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "message": {
-                    "type": "string"
-                },
-                "name": {
-                    "type": "string"
-                },
-                "scheduled_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "send_options": {
-                    "properties": {
-                        "ignore_unsubscribes": {
+                    "included": {
+                        "items": {
                             "type": [
                                 "null",
-                                "boolean"
+                                "string"
                             ]
                         },
-                        "use_smart_sending": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "channel": {
+                "type": "string"
+            },
+            "created_at": {
+                "format": "date-time",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "message": {
+                "type": "string"
+            },
+            "name": {
+                "type": "string"
+            },
+            "scheduled_at": {
+                "format": "date-time",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "send_options": {
+                "properties": {
+                    "ignore_unsubscribes": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
                     },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "send_strategy": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "method": {
-                            "type": "string"
-                        },
-                        "options_static": {
-                            "properties": {
-                                "datetime": {
-                                    "airbyte_type": "timestamp_without_timezone",
-                                    "format": "date-time",
-                                    "type": "string"
-                                },
-                                "is_local": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                },
-                                "send_past_recipients_immediately": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                }
+                    "use_smart_sending": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "send_strategy": {
+                "additionalProperties": true,
+                "properties": {
+                    "method": {
+                        "type": "string"
+                    },
+                    "options_static": {
+                        "properties": {
+                            "datetime": {
+                                "airbyte_type": "timestamp_without_timezone",
+                                "format": "date-time",
+                                "type": "string"
                             },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
+                            "is_local": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "send_past_recipients_immediately": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            }
                         },
-                        "options_sto": {
-                            "properties": {
-                                "date": {
-                                    "format": "date",
-                                    "type": "string"
-                                }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "options_sto": {
+                        "properties": {
+                            "date": {
+                                "format": "date",
+                                "type": "string"
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "options_throttled": {
+                        "properties": {
+                            "datetime": {
+                                "airbyte_type": "timestamp_without_timezone",
+                                "format": "date-time",
+                                "type": "string"
                             },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
+                            "throttle_percentage": {
+                                "type": "integer"
+                            }
                         },
-                        "options_throttled": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "send_time": {
+                "format": "date-time",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "status": {
+                "type": "string"
+            },
+            "tracking_options": {
+                "additionalProperties": true,
+                "properties": {
+                    "is_add_utm": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "is_tracking_clicks": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "is_tracking_opens": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "utm_params": {
+                        "items": {
                             "properties": {
-                                "datetime": {
-                                    "airbyte_type": "timestamp_without_timezone",
-                                    "format": "date-time",
+                                "name": {
                                     "type": "string"
                                 },
-                                "throttle_percentage": {
-                                    "type": "integer"
+                                "value": {
+                                    "type": "string"
                                 }
                             },
                             "type": [
                                 "null",
                                 "object"
                             ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "send_time": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "status": {
-                    "type": "string"
-                },
-                "tracking_options": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "is_add_utm": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "is_tracking_clicks": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "is_tracking_opens": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
                         },
-                        "utm_params": {
-                            "items": {
-                                "properties": {
-                                    "name": {
-                                        "type": "string"
-                                    },
-                                    "value": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "updated_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "id": {
-            "type": "string"
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "updated_at": {
+                "format": "date-time",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            }
         },
-        "links": {
-            "additionalProperties": true,
-            "properties": {
-                "self": {
-                    "type": "string"
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
+        "type": [
+            "null",
+            "object"
+        ]
+    },
+    "id": {
+        "type": "string"
+    },
+    "links": {
+        "additionalProperties": true,
+        "properties": {
+            "self": {
+                "type": "string"
+            }
         },
-        "relationships": {
-            "additionalProperties": true,
-            "properties": {
-                "tags": {
-                    "properties": {
-                        "data": {
-                            "items": {
-                                "properties": {
-                                    "id": {
-                                        "type": "string"
-                                    },
-                                    "type": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "type": "array"
-                        },
-                        "links": {
+        "type": [
+            "null",
+            "object"
+        ]
+    },
+    "relationships": {
+        "additionalProperties": true,
+        "properties": {
+            "tags": {
+                "properties": {
+                    "data": {
+                        "items": {
                             "properties": {
-                                "related": {
+                                "id": {
                                     "type": "string"
                                 },
-                                "self": {
+                                "type": {
                                     "type": "string"
                                 }
                             },
                             "type": [
                                 "null",
                                 "object"
                             ]
-                        }
+                        },
+                        "type": "array"
                     },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "type": {
-            "type": "string"
+                    "links": {
+                        "properties": {
+                            "related": {
+                                "type": "string"
+                            },
+                            "self": {
+                                "type": "string"
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            }
         },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        }
+        "type": [
+            "null",
+            "object"
+        ]
+    },
+    "type": {
+        "type": "string"
     },
-    "type": "object"
+    "updated_at": {
+        "format": "date-time",
+        "type": [
+            "null",
+            "string"
+        ]
+    }
 }
```

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/email_templates.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/email_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/events.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/flows.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/flows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/global_exclusions.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/global_exclusions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/lists.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns_detailed.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('$ref', 'campaign_properties.json'), "*

 * *                 "('estimated_recipient_count', OrderedDict([('type', ['null', 'integer'])])), "*

 * *                 "('campaign_message', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('type', OrderedDict([('type', 'string')])), ('id', "*

 * *                 "OrderedDict([('type', 'string')])), ('attributes', OrderedDict([('type', "*

 * *                 "['null', 'object']), ('properties', Ord […]*

```diff
@@ -1,133 +1,150 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "attributes": {
+        "$ref": "campaign_properties.json",
+        "campaign_message": {
             "properties": {
-                "created": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "name": {
-                    "type": "string"
-                },
-                "opt_in_process": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "updated": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "id": {
-            "type": "string"
-        },
-        "links": {
-            "additionalProperties": true,
-            "properties": {
-                "self": {
-                    "type": "string"
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "relationships": {
-            "additionalProperties": true,
-            "properties": {
-                "profiles": {
+                "attributes": {
                     "properties": {
-                        "links": {
+                        "campaign_id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "channel": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "content": {
                             "properties": {
-                                "related": {
-                                    "type": "string"
+                                "from_email": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "from_label": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "preview_text": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
                                 },
-                                "self": {
-                                    "type": "string"
+                                "subject": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "template_id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "template_name": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
                                 }
                             },
                             "type": [
                                 "null",
                                 "object"
                             ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "tags": {
-                    "properties": {
-                        "data": {
+                        },
+                        "created_at": {
+                            "format": "date-time",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "label": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "send_times": {
                             "items": {
                                 "properties": {
-                                    "id": {
-                                        "type": "string"
+                                    "datetime": {
+                                        "format": "date-time",
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
                                     },
-                                    "type": {
-                                        "type": "string"
+                                    "is_local": {
+                                        "type": [
+                                            "null",
+                                            "boolean"
+                                        ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": "array"
+                            "type": [
+                                "null",
+                                "array"
+                            ]
                         },
-                        "links": {
-                            "properties": {
-                                "related": {
-                                    "type": "string"
-                                },
-                                "self": {
-                                    "type": "string"
-                                }
-                            },
+                        "updated_at": {
+                            "format": "date-time",
                             "type": [
                                 "null",
-                                "object"
+                                "string"
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
+                },
+                "id": {
+                    "type": "string"
+                },
+                "links": {
+                    "properties": {
+                        "self": {
+                            "type": "string"
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "type": {
+                    "type": "string"
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "type": {
-            "type": "string"
-        },
-        "updated": {
-            "format": "date-time",
+        "estimated_recipient_count": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/metrics.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/profiles.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/profiles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/schemas/shared/subscriptions.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/source.py` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/source.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 
 
 from typing import Any, List, Mapping
 
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
-from source_klaviyo.streams import Campaigns, Flows
+from source_klaviyo.streams import Campaigns, CampaignsDetailed, Flows
 
 
 class SourceKlaviyo(YamlDeclarativeSource):
     def __init__(self) -> None:
         super().__init__(**{"path_to_yaml": "manifest.yaml"})
 
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
@@ -19,12 +19,18 @@
         Discovery method, returns available streams
         :param config: A Mapping of the user input configuration as defined in the connector spec.
         """
 
         api_key = config["api_key"]
         start_date = config.get("start_date")
         streams = super().streams(config)
-        streams.extend([Campaigns(api_key=api_key, start_date=start_date), Flows(api_key=api_key, start_date=start_date)])
+        streams.extend(
+            [
+                Campaigns(api_key=api_key, start_date=start_date),
+                CampaignsDetailed(api_key=api_key, start_date=start_date),
+                Flows(api_key=api_key, start_date=start_date),
+            ]
+        )
         return streams
 
     def continue_sync_on_stream_failure(self) -> bool:
         return True
```

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/spec.json` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.5.0/source_klaviyo/streams.py` & `airbyte_source_klaviyo-2.6.0/source_klaviyo/streams.py`

 * *Files 21% similar despite different names*

```diff
@@ -160,58 +160,16 @@
                 # and allows our 'abnormal_state' acceptance test to pass.
                 latest_cursor = min(latest_cursor, pendulum.now().subtract(seconds=3))
                 params["filter"] = f"greater-than({self.cursor_field},{latest_cursor.isoformat()})"
             params["sort"] = self.cursor_field
         return params
 
 
-class ArchivedRecordsStream(IncrementalKlaviyoStream):
-    def __init__(
-        self,
-        path: str,
-        cursor_field: str,
-        start_date: Optional[str] = None,
-        api_revision: Optional[str] = None,
-        **kwargs: Any,
-    ) -> None:
-        super().__init__(start_date=start_date, **kwargs)
-        self._path = path
-        self._cursor_field = cursor_field
-        if api_revision:
-            self.api_revision = api_revision
-
-    @property
-    def cursor_field(self) -> Union[str, List[str]]:
-        return self._cursor_field
-
-    def path(self, **kwargs) -> str:
-        return self._path
-
-    def request_params(
-        self,
-        stream_state: Optional[Mapping[str, Any]],
-        stream_slice: Optional[Mapping[str, Any]] = None,
-        next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> MutableMapping[str, Any]:
-        archived_stream_state = stream_state.get("archived") if stream_state else None
-        params = super().request_params(stream_state=archived_stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
-        archived_filter = "equals(archived,true)"
-        if "filter" in params and archived_filter not in params["filter"]:
-            params["filter"] = f"and({params['filter']},{archived_filter})"
-        elif "filter" not in params:
-            params["filter"] = archived_filter
-        return params
-
-
-class ArchivedRecordsMixin(IncrementalKlaviyoStream, ABC):
-    """A mixin class which should be used when archived records need to be read"""
-
-    @property
-    def archived_stream(self) -> ArchivedRecordsStream:
-        return ArchivedRecordsStream(self.path(), self.cursor_field, self._start_ts, self.api_revision, api_key=self._api_key)
+class IncrementalKlaviyoStreamWithArchivedRecords(IncrementalKlaviyoStream, ABC):
+    """A base class which should be used when archived records need to be read"""
 
     def get_updated_state(self, current_stream_state: MutableMapping[str, Any], latest_record: Mapping[str, Any]) -> Mapping[str, Any]:
         """
         Extend the stream state with `archived` property to store such records' state separately from the stream state
         """
 
         if latest_record.get("attributes", {}).get("archived", False):
@@ -220,36 +178,83 @@
             if current_archived_stream_cursor_value:
                 latest_archived_cursor = max(latest_archived_cursor, pendulum.parse(current_archived_stream_cursor_value))
             current_stream_state["archived"] = {self.cursor_field: latest_archived_cursor.isoformat()}
             return current_stream_state
         else:
             return super().get_updated_state(current_stream_state, latest_record)
 
-    def read_records(
+    def stream_slices(
         self,
         sync_mode: SyncMode,
         cursor_field: Optional[List[str]] = None,
-        stream_slice: Optional[Mapping[str, Any]] = None,
         stream_state: Optional[Mapping[str, Any]] = None,
-    ) -> Iterable[StreamData]:
-        yield from super().read_records(sync_mode, cursor_field, stream_slice, stream_state)
-        yield from self.archived_stream.read_records(sync_mode, cursor_field, stream_slice, stream_state)
+    ) -> Iterable[Optional[Mapping[str, Any]]]:
+        return [{"archived": flag} for flag in (False, True)]
+
+    def request_params(
+        self,
+        stream_state: Optional[Mapping[str, Any]],
+        stream_slice: Optional[Mapping[str, Any]] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> MutableMapping[str, Any]:
+        state = (stream_state or {}).get("archived") if stream_slice.get("archived") else stream_state
+        params = super().request_params(stream_state=state, stream_slice=stream_slice, next_page_token=next_page_token)
+        if stream_slice.get("archived"):
+            archived_filter = "equals(archived,true)"
+            if "filter" in params and archived_filter not in params["filter"]:
+                params["filter"] = f"and({params['filter']},{archived_filter})"
+            elif "filter" not in params:
+                params["filter"] = archived_filter
+        return params
 
 
-class Campaigns(ArchivedRecordsMixin, IncrementalKlaviyoStream):
+class Campaigns(IncrementalKlaviyoStreamWithArchivedRecords):
     """Docs: https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaigns"""
 
     cursor_field = "updated_at"
     api_revision = "2023-06-15"
 
     def path(self, **kwargs) -> str:
         return "campaigns"
 
 
-class Flows(ArchivedRecordsMixin, IncrementalKlaviyoStream):
+class CampaignsDetailed(Campaigns):
+    raise_on_http_errors = False
+
+    def parse_response(self, response: Response, **kwargs: Mapping[str, Any]) -> Iterable[Mapping[str, Any]]:
+        for record in super().parse_response(response, **kwargs):
+            yield self._transform_record(record)
+
+    def _transform_record(self, record: Mapping[str, Any]) -> Mapping[str, Any]:
+        self._set_recipient_count(record)
+        self._set_campaign_message(record)
+        return record
+
+    def _set_recipient_count(self, record: Mapping[str, Any]) -> None:
+        campaign_id = record["id"]
+        recipient_count_request = self._create_prepared_request(
+            path=f"{self.url_base}campaign-recipient-estimations/{campaign_id}",
+            headers=self.request_headers(),
+        )
+        recipient_count_response = self._send_request(recipient_count_request, {})
+        record["estimated_recipient_count"] = (
+            recipient_count_response.json().get("data", {}).get("attributes", {}).get("estimated_recipient_count", 0)
+        )
+
+    def _set_campaign_message(self, record: Mapping[str, Any]) -> None:
+        message_id = record.get("attributes", {}).get("message")
+        if message_id:
+            campaign_message_request = self._create_prepared_request(
+                path=f"{self.url_base}campaign-messages/{message_id}", headers=self.request_headers()
+            )
+            campaign_message_response = self._send_request(campaign_message_request, {})
+            record["campaign_message"] = campaign_message_response.json().get("data")
+
+
+class Flows(IncrementalKlaviyoStreamWithArchivedRecords):
     """Docs: https://developers.klaviyo.com/en/reference/get_flows"""
 
     cursor_field = "updated"
     state_checkpoint_interval = 50  # API can return maximum 50 records per page
 
     def path(self, **kwargs) -> str:
         return "flows"
```

### Comparing `airbyte_source_klaviyo-2.5.0/PKG-INFO` & `airbyte_source_klaviyo-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-klaviyo
-Version: 2.5.0
+Version: 2.6.0
 Summary: Source implementation for Klaviyo.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

