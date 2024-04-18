# Comparing `tmp/pylotus_rpc-0.3.tar.gz` & `tmp/pylotus_rpc-0.4.tar.gz`

## Comparing `pylotus_rpc-0.3.tar` & `pylotus_rpc-0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pytest.ini
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/requirements.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/http_json_rpc_connector.py
--rw-r--r--   0        0        0    10970 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/lotus_client.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/methods/__init__.py
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/methods/chain.py
--rw-r--r--   0        0        0    68223 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/methods/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/actor.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/actor_state.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/address.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/block_header.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/cid.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/deadline.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/deadline_info.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/deal_proposal.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/deal_state.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/execution_trace.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/gas_trace.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/invocation_result.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/loc.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/message.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/message_gas_cost.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/message_lookup.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/message_receipt.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/miner_info.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/miner_partition.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/miner_power.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/sector.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/sector_pre_commit_info.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/signature.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/state_compute_output.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/types/tip_set.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pylotus_rpc/util/sector_util.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/tests/__init__.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/tests/test_chain.py
--rw-r--r--   0        0        0    22879 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/tests/test_state.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/tests/test_util.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/.gitignore
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/LICENSE
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/pyproject.toml
--rw-r--r--   0        0        0    17474 2020-02-02 00:00:00.000000 pylotus_rpc-0.3/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pytest.ini
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/requirements.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/http_json_rpc_connector.py
+-rw-r--r--   0        0        0    10970 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/lotus_client.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/methods/__init__.py
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/methods/chain.py
+-rw-r--r--   0        0        0    68223 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/methods/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/actor.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/actor_state.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/address.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/block_header.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/cid.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/deadline.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/deadline_info.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/deal_proposal.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/deal_state.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/execution_trace.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/gas_trace.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/invocation_result.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/loc.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/message.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/message_gas_cost.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/message_lookup.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/message_receipt.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/miner_info.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/miner_partition.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/miner_power.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/sector.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/sector_pre_commit_info.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/signature.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/state_compute_output.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/types/tip_set.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pylotus_rpc/util/sector_util.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/tests/test_chain.py
+-rw-r--r--   0        0        0    22879 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/tests/test_state.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/tests/test_util.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/.gitignore
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/LICENSE
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/pyproject.toml
+-rw-r--r--   0        0        0    17474 2020-02-02 00:00:00.000000 pylotus_rpc-0.4/PKG-INFO
```

### Comparing `pylotus_rpc-0.3/pylotus_rpc/http_json_rpc_connector.py` & `pylotus_rpc-0.4/pylotus_rpc/http_json_rpc_connector.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/lotus_client.py` & `pylotus_rpc-0.4/pylotus_rpc/lotus_client.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/methods/chain.py` & `pylotus_rpc-0.4/pylotus_rpc/methods/chain.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/methods/state.py` & `pylotus_rpc-0.4/pylotus_rpc/methods/state.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/actor.py` & `pylotus_rpc-0.4/pylotus_rpc/types/actor.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/block_header.py` & `pylotus_rpc-0.4/pylotus_rpc/types/block_header.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/cid.py` & `pylotus_rpc-0.4/pylotus_rpc/types/cid.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/deadline.py` & `pylotus_rpc-0.4/pylotus_rpc/types/deadline.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/deadline_info.py` & `pylotus_rpc-0.4/pylotus_rpc/types/deadline_info.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/deal_proposal.py` & `pylotus_rpc-0.4/pylotus_rpc/types/deal_proposal.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/execution_trace.py` & `pylotus_rpc-0.4/pylotus_rpc/types/execution_trace.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/gas_trace.py` & `pylotus_rpc-0.4/pylotus_rpc/types/gas_trace.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/invocation_result.py` & `pylotus_rpc-0.4/pylotus_rpc/types/invocation_result.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/loc.py` & `pylotus_rpc-0.4/pylotus_rpc/types/loc.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/message.py` & `pylotus_rpc-0.4/pylotus_rpc/types/message.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/message_gas_cost.py` & `pylotus_rpc-0.4/pylotus_rpc/types/message_gas_cost.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/message_lookup.py` & `pylotus_rpc-0.4/pylotus_rpc/types/message_lookup.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/message_receipt.py` & `pylotus_rpc-0.4/pylotus_rpc/types/message_receipt.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/miner_info.py` & `pylotus_rpc-0.4/pylotus_rpc/types/miner_info.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/miner_partition.py` & `pylotus_rpc-0.4/pylotus_rpc/types/miner_partition.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/miner_power.py` & `pylotus_rpc-0.4/pylotus_rpc/types/miner_power.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/sector.py` & `pylotus_rpc-0.4/pylotus_rpc/types/sector.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/sector_pre_commit_info.py` & `pylotus_rpc-0.4/pylotus_rpc/types/sector_pre_commit_info.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/state_compute_output.py` & `pylotus_rpc-0.4/pylotus_rpc/types/state_compute_output.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/types/tip_set.py` & `pylotus_rpc-0.4/pylotus_rpc/types/tip_set.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pylotus_rpc/util/sector_util.py` & `pylotus_rpc-0.4/pylotus_rpc/util/sector_util.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/tests/test_chain.py` & `pylotus_rpc-0.4/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/tests/test_state.py` & `pylotus_rpc-0.4/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/LICENSE` & `pylotus_rpc-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/README.md` & `pylotus_rpc-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pylotus_rpc-0.3/pyproject.toml` & `pylotus_rpc-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pylotus-rpc"
-version = "0.3"
+version = "0.4"
 description = "Python client for interacting with the Lotus JSON-RPC API."
 readme = "README.md"
 license = { file="LICENSE" }
 keywords = ["lotus", "filecoin", "rpc", "json-rpc", "api", "client", "python"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -24,8 +24,8 @@
 
 
 [project.urls]
 Homepage = "https://github.com/FilForge/pylotus-rpc"
 Issues = "https://github.com/FilForge/pylotus-rpc/issues"
 
 [tool.hatch.build.targets.wheel]
-packages = ["pylotus-rpc"]
+packages = ["pylotus_rpc"]
```

### Comparing `pylotus_rpc-0.3/PKG-INFO` & `pylotus_rpc-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pylotus-rpc
-Version: 0.3
+Version: 0.4
 Summary: Python client for interacting with the Lotus JSON-RPC API.
 Project-URL: Homepage, https://github.com/FilForge/pylotus-rpc
 Project-URL: Issues, https://github.com/FilForge/pylotus-rpc/issues
 Author: Jason Byteforgia
 License:                              Apache License
                                Version 2.0, January 2004
                             http://www.apache.org/licenses/
```

