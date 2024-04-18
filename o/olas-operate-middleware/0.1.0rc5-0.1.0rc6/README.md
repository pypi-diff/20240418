# Comparing `tmp/olas_operate_middleware-0.1.0rc5.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc5.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc6.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc5.tar` & `olas_operate_middleware-0.1.0rc6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc5/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc5/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc5/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc5/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc5/operate/account/user.py
--rw-r--r--   0        0        0    18550 2024-04-17 09:26:07.366152 olas_operate_middleware-0.1.0rc5/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc5/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc5/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc5/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc5/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc5/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc5/operate/keys.py
--rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc5/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc5/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc5/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc5/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc5/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc5/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc5/operate/services/__init__.py
--rw-r--r--   0        0        0    17523 2024-04-17 09:26:07.367524 olas_operate_middleware-0.1.0rc5/operate/services/manage.py
--rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc5/operate/services/protocol.py
--rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc5/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc5/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc5/operate/utils/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc5/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc5/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8662 2024-04-16 14:21:46.519007 olas_operate_middleware-0.1.0rc5/operate/wallet/master.py
--rw-r--r--   0        0        0     1171 2024-04-17 09:26:07.371553 olas_operate_middleware-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc6/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc6/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc6/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc6/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc6/operate/account/user.py
+-rw-r--r--   0        0        0    18550 2024-04-17 09:26:07.366152 olas_operate_middleware-0.1.0rc6/operate/cli.py
+-rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc6/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc6/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc6/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc6/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc6/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc6/operate/keys.py
+-rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc6/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc6/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc6/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc6/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc6/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc6/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc6/operate/services/__init__.py
+-rw-r--r--   0        0        0    17808 2024-04-17 11:42:50.723943 olas_operate_middleware-0.1.0rc6/operate/services/manage.py
+-rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc6/operate/services/protocol.py
+-rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc6/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc6/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc6/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc6/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc6/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-16 14:21:46.519007 olas_operate_middleware-0.1.0rc6/operate/wallet/master.py
+-rw-r--r--   0        0        0     1171 2024-04-18 10:17:15.241211 olas_operate_middleware-0.1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc6/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc5/LICENSE` & `olas_operate_middleware-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/README.md` & `olas_operate_middleware-0.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/account/user.py` & `olas_operate_middleware-0.1.0rc6/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/cli.py` & `olas_operate_middleware-0.1.0rc6/operate/cli.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/constants.py` & `olas_operate_middleware-0.1.0rc6/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc6/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/keys.py` & `olas_operate_middleware-0.1.0rc6/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc6/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc6/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc6/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc6/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/resource.py` & `olas_operate_middleware-0.1.0rc6/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc6/operate/services/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #   limitations under the License.
 #
 # ------------------------------------------------------------------------------
 """Service manager."""
 
 import asyncio
 import logging
+import traceback
 import typing as t
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from aea.helpers.base import IPFSHash
 from aea.helpers.logging import setup_logger
 from autonomy.chain.base import registry_contracts
@@ -413,22 +414,27 @@
         loop: t.Optional[asyncio.AbstractEventLoop] = None,
     ) -> None:
         """Start a background funding job."""
         loop = loop or asyncio.get_event_loop()
         service = self.create_or_load(hash=hash)
         with ThreadPoolExecutor() as executor:
             while True:
-                await loop.run_in_executor(
-                    executor,
-                    self.fund_service,
-                    hash,
-                    PUBLIC_RPCS[service.ledger_config.chain],
-                    10000000000000000,
-                    50000000000000000,
-                )
+                try:
+                    await loop.run_in_executor(
+                        executor,
+                        self.fund_service,
+                        hash,
+                        PUBLIC_RPCS[service.ledger_config.chain],
+                        10000000000000000,
+                        50000000000000000,
+                    )
+                except Exception:  # pylint: disable=broad-except
+                    logging.info(
+                        f"Error occured while funding the service\n{traceback.format_exc()}"
+                    )
                 await asyncio.sleep(60)
 
     def deploy_service_locally(self, hash: str, force: bool = True) -> Deployment:
         """
         Deploy service locally
 
         :param hash: Service hash
```

### Comparing `olas_operate_middleware-0.1.0rc5/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc6/operate/services/protocol.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/services/service.py` & `olas_operate_middleware-0.1.0rc6/operate/services/service.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/types.py` & `olas_operate_middleware-0.1.0rc6/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc6/operate/utils/gnosis.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc6/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc6/operate/wallet/master.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc5/pyproject.toml` & `olas_operate_middleware-0.1.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc5"
+version = "0.1.0-rc6"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
```

### Comparing `olas_operate_middleware-0.1.0rc5/PKG-INFO` & `olas_operate_middleware-0.1.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

