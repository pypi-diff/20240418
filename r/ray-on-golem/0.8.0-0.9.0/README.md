# Comparing `tmp/ray_on_golem-0.8.0.tar.gz` & `tmp/ray_on_golem-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ray_on_golem-0.8.0.tar", max compression
+gzip compressed data, was "ray_on_golem-0.9.0.tar", max compression
```

## Comparing `ray_on_golem-0.8.0.tar` & `ray_on_golem-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35149 2024-02-26 09:52:13.918230 ray_on_golem-0.8.0/LICENSE
--rw-r--r--   0        0        0     6326 2024-02-26 09:52:13.918230 ray_on_golem-0.8.0/README.md
--rw-r--r--   0        0        0     3439 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/__init__.py
--rw-r--r--   0        0        0       43 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/__main__.py
--rw-r--r--   0        0        0       89 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/client/__init__.py
--rw-r--r--   0        0        0     8553 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/client/client.py
--rw-r--r--   0        0        0      434 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/client/exceptions.py
--rw-r--r--   0        0        0       74 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/ctl/__init__.py
--rw-r--r--   0        0        0     8969 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/ctl/ctl.py
--rw-r--r--   0        0        0      932 2024-02-26 09:52:13.938231 ray_on_golem-0.8.0/ray_on_golem/ctl/log.py
--rw-r--r--   0        0        0       43 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/exceptions.py
--rw-r--r--   0        0        0      866 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/log.py
--rw-r--r--   0        0        0      473 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/main.py
--rw-r--r--   0        0        0       70 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/network_stats/__init__.py
--rw-r--r--   0        0        0     3237 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/network_stats/main.py
--rw-r--r--   0        0        0       82 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/network_stats/services/__init__.py
--rw-r--r--   0        0        0     8983 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/network_stats/services/network_stats.py
--rw-r--r--   0        0        0        0 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/provider/__init__.py
--rw-r--r--   0        0        0      115 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/provider/exceptions.py
--rw-r--r--   0        0        0      490 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/provider/log.py
--rw-r--r--   0        0        0    12869 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/provider/node_provider.py
--rw-r--r--   0        0        0      459 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/provider/ssh_command_runner.py
--rw-r--r--   0        0        0      110 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/__init__.py
--rw-r--r--   0        0        0      960 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/exceptions.py
--rw-r--r--   0        0        0     8795 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/main.py
--rw-r--r--   0        0        0      823 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/middlewares.py
--rw-r--r--   0        0        0     4273 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/models.py
--rw-r--r--   0        0        0      283 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/__init__.py
--rw-r--r--   0        0        0      190 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/__init__.py
--rw-r--r--   0        0        0    17420 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/golem.py
--rw-r--r--   0        0        0     4929 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/helpers/demand_config.py
--rw-r--r--   0        0        0     3294 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/helpers/manager_stack.py
--rw-r--r--   0        0        0     1586 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/manager_stack.py
--rw-r--r--   0        0        0     1200 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/manifest.py
--rw-r--r--   0        0        0     1201 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/golem/provider_data.py
--rw-r--r--   0        0        0    14524 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/ray.py
--rw-r--r--   0        0        0      625 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/utils.py
--rw-r--r--   0        0        0     8435 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/services/yagna.py
--rw-r--r--   0        0        0     4907 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/settings.py
--rw-r--r--   0        0        0     8319 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/server/views.py
--rw-r--r--   0        0        0     1754 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/utils.py
--rw-r--r--   0        0        0      691 2024-02-26 09:52:13.942231 ray_on_golem-0.8.0/ray_on_golem/version.py
--rw-r--r--   0        0        0     7243 1970-01-01 00:00:00.000000 ray_on_golem-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-26 14:09:31.449365 ray_on_golem-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6326 2024-03-26 14:09:31.449365 ray_on_golem-0.9.0/README.md
+-rw-r--r--   0        0        0     3449 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/__init__.py
+-rw-r--r--   0        0        0       43 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/__main__.py
+-rw-r--r--   0        0        0       89 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/client/__init__.py
+-rw-r--r--   0        0        0     8553 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/client/client.py
+-rw-r--r--   0        0        0      434 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/client/exceptions.py
+-rw-r--r--   0        0        0       74 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/ctl/__init__.py
+-rw-r--r--   0        0        0     8969 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/ctl/ctl.py
+-rw-r--r--   0        0        0      932 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/ctl/log.py
+-rw-r--r--   0        0        0       43 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/exceptions.py
+-rw-r--r--   0        0        0      866 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/log.py
+-rw-r--r--   0        0        0      473 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/main.py
+-rw-r--r--   0        0        0       70 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/network_stats/__init__.py
+-rw-r--r--   0        0        0     3237 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/network_stats/main.py
+-rw-r--r--   0        0        0       82 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/network_stats/services/__init__.py
+-rw-r--r--   0        0        0     9837 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/network_stats/services/network_stats.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/provider/__init__.py
+-rw-r--r--   0        0        0      115 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/provider/exceptions.py
+-rw-r--r--   0        0        0      490 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/provider/log.py
+-rw-r--r--   0        0        0    12929 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/provider/node_provider.py
+-rw-r--r--   0        0        0      459 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/provider/ssh_command_runner.py
+-rw-r--r--   0        0        0      110 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/__init__.py
+-rw-r--r--   0        0        0      960 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/exceptions.py
+-rw-r--r--   0        0        0     8814 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/main.py
+-rw-r--r--   0        0        0      823 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/middlewares.py
+-rw-r--r--   0        0        0     4341 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/models.py
+-rw-r--r--   0        0        0      283 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/__init__.py
+-rw-r--r--   0        0        0      190 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/__init__.py
+-rw-r--r--   0        0        0    18592 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/golem.py
+-rw-r--r--   0        0        0     4997 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/helpers/demand_config.py
+-rw-r--r--   0        0        0     6048 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/helpers/manager_stack.py
+-rw-r--r--   0        0        0     1003 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/manager_stack.py
+-rw-r--r--   0        0        0     1200 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/manifest.py
+-rw-r--r--   0        0        0     1201 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/golem/provider_data.py
+-rw-r--r--   0        0        0    15174 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/ray.py
+-rw-r--r--   0        0        0      625 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/utils.py
+-rw-r--r--   0        0        0     8589 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/services/yagna.py
+-rw-r--r--   0        0        0     4942 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/settings.py
+-rw-r--r--   0        0        0     8319 2024-03-26 14:09:31.469365 ray_on_golem-0.9.0/ray_on_golem/server/views.py
+-rw-r--r--   0        0        0     1754 2024-03-26 14:09:31.473365 ray_on_golem-0.9.0/ray_on_golem/utils.py
+-rw-r--r--   0        0        0      691 2024-03-26 14:09:31.473365 ray_on_golem-0.9.0/ray_on_golem/version.py
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 ray_on_golem-0.9.0/PKG-INFO
```

### Comparing `ray_on_golem-0.8.0/LICENSE` & `ray_on_golem-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/README.md` & `ray_on_golem-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/pyproject.toml` & `ray_on_golem-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [tool.poetry]
 name = "ray-on-golem"
-version = "0.8.0"
+version = "0.9.0"
 description = "Golem Network integration with Ray"
 authors = ["Golem Factory <contact@golem.network>"]
 readme = "README.md"
 packages = [{include = "ray_on_golem"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
-ray = {version="^2.9.2", extras=["default"]}
-# golem-core = { path="../golem-core-python", develop=true }
-# golem-core = {git="https://github.com/golemfactory/golem-core-python.git", branch="main"}
-golem-core = "^0.5.0"
+ray = {version="~2.9.3", extras=["default"]}
+#golem-core = {path="../golem-core-python", develop=true}
+#golem-core = {git="https://github.com/golemfactory/golem-core-python.git", branch="main"}
+golem-core = "^0.6.0"
 aiohttp = "^3"
 requests = "^2"
 click = "^8"
 pydantic = "<2"
 toml = "^0.10.2"
 dpath = "^2.1.6"
 appdirs = "^1.4.4"
 
 websocat = "^1.12.0"
-golem-node = "0.14.0"
+golem-node = "0.13.3"
 
 setuptools = "*"
+psutil = "^5.9.8"
 
 [tool.poetry.group.ray.dependencies]
 python = "^3.8.1"
 
-ray = {version="==2.9.2", extras=["default"]}
-# golem-core = { path="../golem-core-python", develop=true }
-# golem-core = {git="https://github.com/golemfactory/golem-core-python.git", branch="main"}
-golem-core = "^0.5.0"
+ray = {version="==2.9.3", extras=["default"]}
+#golem-core = {path="../golem-core-python", develop=true}
+#golem-core = {git="https://github.com/golemfactory/golem-core-python.git", branch="main"}
+golem-core = "^0.6.0"
 aiohttp = "^3"
 requests = "^2"
 click = "^8"
 pydantic = "<2"
 toml = "^0.10.2"
 dpath = "^2.1.6"
 appdirs = "^1.4.4"
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/client/client.py` & `ray_on_golem-0.9.0/ray_on_golem/client/client.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/ctl/ctl.py` & `ray_on_golem-0.9.0/ray_on_golem/ctl/ctl.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/ctl/log.py` & `ray_on_golem-0.9.0/ray_on_golem/ctl/log.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/log.py` & `ray_on_golem-0.9.0/ray_on_golem/log.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/network_stats/main.py` & `ray_on_golem-0.9.0/ray_on_golem/network_stats/main.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/network_stats/services/network_stats.py` & `ray_on_golem-0.9.0/ray_on_golem/network_stats/services/network_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,35 @@
 import re
 from collections import defaultdict
 from datetime import timedelta
 from typing import Dict, Optional, Sequence
 
 from golem.managers import (
     BlacklistProviderIdPlugin,
+    DefaultPaymentManager,
     DefaultProposalManager,
     NegotiatingPlugin,
-    PayAllPaymentManager,
     PaymentPlatformNegotiator,
     ProposalBuffer,
     ProposalManagerPlugin,
     ProposalScoringBuffer,
-    RefreshingDemandManager,
 )
-from golem.managers.base import ManagerPluginException, PaymentManager, ProposalNegotiator
+from golem.managers.base import (
+    ManagerPluginException,
+    PaymentManager,
+    ProposalNegotiator,
+    ProposalScorer,
+)
 from golem.node import GolemNode
 from golem.resources import DemandData, Proposal
 from golem.resources.proposal.exceptions import ProposalRejected
 from ya_market import ApiException
 
 from ray_on_golem.server.models import NodeConfigData
+from ray_on_golem.server.services.golem.golem import DEFAULT_DEMAND_LIFETIME
 from ray_on_golem.server.services.golem.helpers.demand_config import DemandConfigHelper
 from ray_on_golem.server.services.golem.helpers.manager_stack import ManagerStackNodeConfigHelper
 from ray_on_golem.server.services.golem.manager_stack import ManagerStack
 from ray_on_golem.server.services.golem.provider_data import PROVIDERS_BLACKLIST
 
 logger = logging.getLogger(__name__)
 
@@ -142,21 +147,34 @@
 
         logger.info("Stopping NetworkStatsService done")
 
     async def run(self, config: Dict, node_type: str, duration_minutes: int) -> None:
         provider_parameters: Dict = config["provider"]["parameters"]
 
         payment_network: str = provider_parameters["payment_network"]
+        payment_driver: str = provider_parameters["payment_driver"]
         total_budget: float = provider_parameters["total_budget"]
         node_config = NodeConfigData(**config["available_node_types"][node_type]["node_config"])
 
-        stack = await self._create_stack(node_config, total_budget, payment_network)
+        is_head_node = node_type == config.get("head_node_type")
+
+        stack = await self._create_stack(
+            node_config=node_config,
+            total_budget=total_budget,
+            payment_network=payment_network,
+            payment_driver=payment_driver,
+            is_head_node=is_head_node,
+        )
         await stack.start()
 
-        print(f"Gathering stats data for {duration_minutes} minutes for `{node_type}`...")
+        print(
+            "Gathering stats data for {} minutes for `{}`{}...".format(
+                duration_minutes, node_type, " (head node)" if is_head_node else ""
+            )
+        )
         consume_proposals_task = asyncio.create_task(self._consume_draft_proposals(stack))
         try:
             await asyncio.wait(
                 [consume_proposals_task],
                 timeout=timedelta(minutes=duration_minutes).total_seconds(),
             )
         finally:
@@ -169,15 +187,15 @@
             print("Gathering stats data done")
             self._stats_plugin_factory.print_gathered_stats()
 
     async def _consume_draft_proposals(self, stack: ManagerStack) -> None:
         drafts = []
         try:
             while True:
-                draft = await stack.proposal_manager.get_draft_proposal()
+                draft = await stack._managers[-1].get_draft_proposal()
                 drafts.append(draft)
         except asyncio.CancelledError:
             return
         finally:
             await asyncio.gather(
                 # FIXME better reason message
                 *[draft.reject(reason="No more needed") for draft in drafts],
@@ -185,63 +203,75 @@
             )
 
     async def _create_stack(
         self,
         node_config: NodeConfigData,
         total_budget: float,
         payment_network: str,
+        payment_driver: str,
+        is_head_node: bool,
     ) -> ManagerStack:
         if not self._payment_manager:
-            self._payment_manager = PayAllPaymentManager(
-                self._golem, budget=total_budget, network=payment_network
+            self._payment_manager = DefaultPaymentManager(
+                self._golem, budget=total_budget, network=payment_network, driver=payment_driver
             )
             await self._payment_manager.start()
 
         stack = ManagerStack()
+        extra_proposal_plugins: Dict[str, ProposalManagerPlugin] = {}
+        extra_proposal_scorers: Dict[str, ProposalScorer] = {}
 
         payloads = await self._demand_config_helper.get_payloads_from_demand_config(
             node_config.demand
         )
 
-        ManagerStackNodeConfigHelper.apply_budget_control_expected_usage(stack, node_config)
-        ManagerStackNodeConfigHelper.apply_budget_control_hard_limits(stack, node_config)
+        ManagerStackNodeConfigHelper.apply_budget_control_expected_usage(
+            extra_proposal_plugins, extra_proposal_scorers, node_config
+        )
+        ManagerStackNodeConfigHelper.apply_budget_control_hard_limits(
+            extra_proposal_plugins, node_config
+        )
 
-        stack.demand_manager = RefreshingDemandManager(
-            self._golem,
-            self._payment_manager.get_allocation,
+        demand_manager = ManagerStackNodeConfigHelper.prepare_demand_manager_for_node_type(
+            stack,
             payloads,
-            demand_lifetime=timedelta(hours=8),
-            subnet_tag=node_config.subnet_tag,
+            DEFAULT_DEMAND_LIFETIME,
+            node_config,
+            is_head_node,
+            self._golem,
+            self._payment_manager,
         )
 
         plugins = [
             self._stats_plugin_factory.create_counter_plugin("Initial"),
             BlacklistProviderIdPlugin(PROVIDERS_BLACKLIST.get(payment_network, set())),
             self._stats_plugin_factory.create_counter_plugin("Not blacklisted"),
         ]
 
-        for plugin_tag, plugin in stack.extra_proposal_plugins.items():
+        for plugin_tag, plugin in extra_proposal_plugins.items():
             plugins.append(plugin)
             plugins.append(self._stats_plugin_factory.create_counter_plugin(f"Passed {plugin_tag}"))
 
         plugins.extend(
             [
                 ProposalScoringBuffer(
                     min_size=500,
                     max_size=1000,
                     fill_at_start=True,
-                    proposal_scorers=(*stack.extra_proposal_scorers.values(),),
+                    proposal_scorers=(*extra_proposal_scorers.values(),),
                     scoring_debounce=timedelta(seconds=10),
                 ),
                 self._stats_plugin_factory.create_counter_plugin("Negotiation initialized"),
                 self._stats_plugin_factory.create_negotiating_plugin(),
                 self._stats_plugin_factory.create_counter_plugin("Negotiated successfully"),
                 ProposalBuffer(min_size=800, max_size=1000, fill_concurrency_size=16),
             ]
         )
-        stack.proposal_manager = DefaultProposalManager(
-            self._golem,
-            stack.demand_manager.get_initial_proposal,
-            plugins=plugins,
+        stack.add_manager(
+            DefaultProposalManager(
+                self._golem,
+                demand_manager.get_initial_proposal,
+                plugins=plugins,
+            )
         )
 
         return stack
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/provider/node_provider.py` & `ray_on_golem-0.9.0/ray_on_golem/provider/node_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ray_on_golem.client import RayOnGolemClient
 from ray_on_golem.ctl import RayOnGolemCtl
 from ray_on_golem.provider.log import NodeProviderCliLogger
 from ray_on_golem.provider.ssh_command_runner import SSHCommandRunner
 from ray_on_golem.server.models import NodeData, NodeId, NodeState
 from ray_on_golem.server.settings import (
     PAYMENT_DRIVER_ERC20,
-    PAYMENT_NETWORK_GOERLI,
+    PAYMENT_NETWORK_HOLESKY,
     PAYMENT_NETWORK_MAINNET,
     PAYMENT_NETWORK_POLYGON,
     TMP_PATH,
 )
 from ray_on_golem.utils import get_default_ssh_key_name, is_running_on_golem_network
 from ray_on_golem.version import get_version
 
@@ -37,18 +37,19 @@
     "on the Polygon blockchain (see: https://docs.golem.network/docs/creators/ray/mainnet).",
 }
 
 PROVIDER_DEFAULTS = {
     "webserver_port": 4578,
     "webserver_datadir": None,
     "enable_registry_stats": True,
-    "payment_network": PAYMENT_NETWORK_GOERLI,
+    "payment_network": PAYMENT_NETWORK_HOLESKY,
     "payment_driver": PAYMENT_DRIVER_ERC20,
     "node_config": {
         "subnet_tag": "public",
+        "priority_head_subnet_tag": "ray-on-golem-heads",
     },
     "total_budget": 1.0,
 }
 
 
 class GolemNodeProvider(NodeProvider):
     def __init__(self, provider_config: Dict[str, Any], cluster_name: str):
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/exceptions.py` & `ray_on_golem-0.9.0/ray_on_golem/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/main.py` & `ray_on_golem-0.9.0/ray_on_golem/server/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,17 @@
 
 async def startup_print(app: web.Application) -> None:
     logger.info("Starting server done, listening on port {}".format(app["port"]))
 
 
 async def shutdown_print(app: web.Application) -> None:
     print("")  # explicit new line to console to visually better handle ^C
-    logger.info("Stopping server gracefully, forcing after `%s`...", RAY_ON_GOLEM_SHUTDOWN_TIMEOUT)
+    logger.info(
+        "Waiting up to `%s` for current connections to close...", RAY_ON_GOLEM_SHUTDOWN_TIMEOUT
+    )
 
 
 async def yagna_service_ctx(app: web.Application) -> None:
     yagna_service: YagnaService = app["yagna_service"]
 
     await yagna_service.init()
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/middlewares.py` & `ray_on_golem-0.9.0/ray_on_golem/server/middlewares.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/models.py` & `ray_on_golem-0.9.0/ray_on_golem/server/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     image_tag: Optional[str] = None
     capabilities: List[str] = ["vpn", "inet"]
     outbound_urls: List[AnyUrl] = []
     min_mem_gib: float = 0.0
     min_cpu_threads: int = 0
     min_storage_gib: float = 0.0
     max_cpu_threads: Optional[int] = None
+    runtime: str = "vm"
 
 
 class PerCpuExpectedUsageData(BaseModel):
     cpu_load: float
     duration_hours: float
     max_cost: Optional[float] = None
 
@@ -87,14 +88,15 @@
     max_env_per_hour_price: Optional[float] = None
 
     payment_interval_hours: Optional[PaymentIntervalHours] = None
 
 
 class NodeConfigData(BaseModel):
     subnet_tag: str
+    priority_head_subnet_tag: Optional[str]
     demand: DemandConfigData = Field(default_factory=DemandConfigData)
     budget_control: Optional[BudgetControlData] = Field(default_factory=BudgetControlData)
 
 
 class ProviderConfigData(BaseModel):
     payment_network: str
     payment_driver: str
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/golem/golem.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/golem/golem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import asyncio
-import hashlib
 import logging
 from collections import defaultdict
 from datetime import datetime, timedelta, timezone
 from functools import partial
 from pathlib import Path
-from typing import Awaitable, Callable, Dict, Optional, Tuple
+from typing import Awaitable, Callable, DefaultDict, Dict, Optional, Tuple
 
 from golem.exceptions import GolemException
 from golem.managers import (
     BlacklistProviderIdPlugin,
     DefaultAgreementManager,
+    DefaultPaymentManager,
     DefaultProposalManager,
     MapScore,
     MidAgreementPaymentsNegotiator,
     NegotiatingPlugin,
-    PayAllPaymentManager,
     PaymentManager,
     PaymentPlatformNegotiator,
     ProposalBuffer,
+    ProposalManagerPlugin,
+    ProposalScorer,
     ProposalScoringBuffer,
     RandomScore,
-    RefreshingDemandManager,
     WorkContext,
 )
 from golem.managers.base import ManagerException
 from golem.node import GolemNode
 from golem.payload import PaymentInfo
 from golem.resources import Activity, Network, Proposal, ProposalData
 from yarl import URL
@@ -50,16 +50,16 @@
     def __init__(self, websocat_path: Path, registry_stats: bool):
         self._websocat_path = websocat_path
 
         self._demand_config_helper: DemandConfigHelper = DemandConfigHelper(registry_stats)
         self._golem: Optional[GolemNode] = None
         self._network: Optional[Network] = None
         self._yagna_appkey: Optional[str] = None
-        self._stacks: Dict[str, ManagerStack] = {}
-        self._stacks_locks = defaultdict(asyncio.Lock)
+        self._stacks: Dict[(str, bool), ManagerStack] = {}
+        self._stacks_locks: DefaultDict[(str, bool), asyncio.Lock] = defaultdict(asyncio.Lock)
         self._payment_manager: Optional[PaymentManager] = None
 
     async def init(self, yagna_appkey: str) -> None:
         logger.info("Starting GolemService...")
 
         self._golem = GolemNode(app_key=yagna_appkey)
         self._yagna_appkey = yagna_appkey
@@ -104,57 +104,75 @@
         logger.info(f"Removing stack `{stack_hash}` done")
 
     async def _get_or_create_stack_from_node_config(
         self,
         node_config: NodeConfigData,
         total_budget: float,
         payment_network: str,
+        payment_driver: str,
+        node_type: str,
+        is_head_node: bool,
     ) -> ManagerStack:
-        stack_hash = self._get_hash_from_node_config(node_config)
+        stack_key = (node_type, is_head_node)
 
-        async with self._stacks_locks[stack_hash]:
-            stack = self._stacks.get(stack_hash)
+        async with self._stacks_locks[stack_key]:
+            stack = self._stacks.get(stack_key)
             if stack is None:
                 logger.info(
-                    f"Creating new stack `{stack_hash}`... {total_budget=}, {payment_network=}"
+                    "Creating new stack `{%s}`: {%s}/{%s}, total_budget={%s}",
+                    stack_key,
+                    payment_driver,
+                    payment_network,
+                    total_budget,
                 )
-                self._stacks[stack_hash] = stack = await self._create_stack(
-                    node_config, total_budget, payment_network
+                self._stacks[stack_key] = stack = await self._create_stack(
+                    node_config=node_config,
+                    total_budget=total_budget,
+                    payment_network=payment_network,
+                    payment_driver=payment_driver,
+                    is_head_node=is_head_node,
                 )
                 await stack.start()
 
-                logger.info(f"Creating new stack `{stack_hash}` done")
+                logger.info(f"Creating new stack `{stack_key}` done")
 
             return stack
 
-    @staticmethod
-    def _get_hash_from_node_config(node_config: NodeConfigData) -> str:
-        return hashlib.md5(node_config.json().encode()).hexdigest()
-
     async def _create_stack(
         self,
         node_config: NodeConfigData,
         total_budget: float,
         payment_network: str,
+        payment_driver: str,
+        is_head_node: bool,
     ) -> ManagerStack:
         if not self._payment_manager:
-            self._payment_manager = PayAllPaymentManager(
-                self._golem, budget=total_budget, network=payment_network
+            self._payment_manager = DefaultPaymentManager(
+                self._golem, budget=total_budget, network=payment_network, driver=payment_driver
             )
             await self._payment_manager.start()
 
         stack = ManagerStack()
+        extra_proposal_plugins: Dict[str, ProposalManagerPlugin] = {}
+        extra_proposal_scorers: Dict[str, ProposalScorer] = {}
 
         payloads = await self._demand_config_helper.get_payloads_from_demand_config(
             node_config.demand
         )
         demand_lifetime = DEFAULT_DEMAND_LIFETIME
 
-        ManagerStackNodeConfigHelper.apply_budget_control_expected_usage(stack, node_config)
-        ManagerStackNodeConfigHelper.apply_budget_control_hard_limits(stack, node_config)
+        ManagerStackNodeConfigHelper.apply_budget_control_expected_usage(
+            extra_proposal_plugins, extra_proposal_scorers, node_config
+        )
+        ManagerStackNodeConfigHelper.apply_budget_control_hard_limits(
+            extra_proposal_plugins, node_config
+        )
+        ManagerStackNodeConfigHelper.apply_priority_head_node_scoring(
+            extra_proposal_scorers, node_config
+        )
 
         proposal_negotiators = [PaymentPlatformNegotiator()]
         if node_config.budget_control.payment_interval_hours is not None:
             logger.debug(
                 "Adding mid agreement payments based on given payment_interval: %s",
                 node_config.budget_control.payment_interval_hours,
             )
@@ -182,56 +200,61 @@
                     min_debit_note_interval=DEFAULT_DEBIT_NOTE_INTERVAL,
                     optimal_debit_note_interval=DEFAULT_DEBIT_NOTE_INTERVAL,
                     min_payment_timeout=minimal_payment_timeout,
                     optimal_payment_timeout=optimal_payment_timeout,
                 )
             )
 
-        stack.demand_manager = RefreshingDemandManager(
-            self._golem,
-            self._payment_manager.get_allocation,
+        demand_manager = ManagerStackNodeConfigHelper.prepare_demand_manager_for_node_type(
+            stack,
             payloads,
-            demand_lifetime=demand_lifetime,
-            subnet_tag=node_config.subnet_tag,
-        )
-        stack.proposal_manager = DefaultProposalManager(
+            demand_lifetime,
+            node_config,
+            is_head_node,
             self._golem,
-            stack.demand_manager.get_initial_proposal,
-            plugins=(
-                BlacklistProviderIdPlugin(PROVIDERS_BLACKLIST.get(payment_network, set())),
-                *stack.extra_proposal_plugins.values(),
-                ProposalScoringBuffer(
-                    min_size=50,
-                    max_size=1000,
-                    fill_at_start=True,
-                    proposal_scorers=(
-                        *stack.extra_proposal_scorers.values(),
-                        MapScore(
-                            partial(self._score_with_provider_data, payment_network=payment_network)
+            self._payment_manager,
+        )
+
+        proposal_manager = stack.add_manager(
+            DefaultProposalManager(
+                self._golem,
+                demand_manager.get_initial_proposal,
+                plugins=(
+                    BlacklistProviderIdPlugin(PROVIDERS_BLACKLIST.get(payment_network, set())),
+                    *extra_proposal_plugins.values(),
+                    ProposalScoringBuffer(
+                        min_size=50,
+                        max_size=1000,
+                        fill_at_start=True,
+                        proposal_scorers=(
+                            *extra_proposal_scorers.values(),
+                            MapScore(
+                                partial(
+                                    self._score_with_provider_data, payment_network=payment_network
+                                )
+                            ),
+                            (0.1, RandomScore()),
                         ),
-                        (0.1, RandomScore()),
+                        scoring_debounce=timedelta(seconds=10),
+                        get_expiration_func=self._get_proposal_expiration,
+                    ),
+                    NegotiatingPlugin(
+                        proposal_negotiators=proposal_negotiators,
+                        proposal_response_timeout=DEFAULT_PROPOSAL_RESPONSE_TIMEOUT,
+                    ),
+                    ProposalBuffer(
+                        min_size=0,
+                        max_size=4,
+                        fill_concurrency_size=4,
+                        get_expiration_func=self._get_proposal_expiration,
                     ),
-                    scoring_debounce=timedelta(seconds=10),
-                    get_expiration_func=self._get_proposal_expiration,
-                ),
-                NegotiatingPlugin(
-                    proposal_negotiators=proposal_negotiators,
-                    proposal_response_timeout=DEFAULT_PROPOSAL_RESPONSE_TIMEOUT,
-                ),
-                ProposalBuffer(
-                    min_size=0,
-                    max_size=4,
-                    fill_concurrency_size=4,
-                    get_expiration_func=self._get_proposal_expiration,
                 ),
-            ),
-        )
-        stack.agreement_manager = DefaultAgreementManager(
-            self._golem, stack.proposal_manager.get_draft_proposal
+            )
         )
+        stack.add_manager(DefaultAgreementManager(self._golem, proposal_manager.get_draft_proposal))
 
         return stack
 
     async def _get_proposal_expiration(self, proposal: Proposal) -> timedelta:
         return await proposal.get_expiration_date() - datetime.now(timezone.utc)
 
     def _score_with_provider_data(
@@ -363,18 +386,26 @@
         *,
         node_config: NodeConfigData,
         public_ssh_key: str,
         ssh_user: str,
         ssh_private_key_path: Path,
         total_budget: float,
         payment_network: str,
+        payment_driver: str,
         add_state_log: Callable[[str], Awaitable[None]],
+        node_type: str,
+        is_head_node: bool,
     ) -> Tuple[Activity, str, str]:
         stack = await self._get_or_create_stack_from_node_config(
-            node_config, total_budget, payment_network
+            node_config=node_config,
+            total_budget=total_budget,
+            payment_network=payment_network,
+            payment_driver=payment_driver,
+            node_type=node_type,
+            is_head_node=is_head_node,
         )
 
         while True:
             try:
                 return await self._create_activity(
                     stack,
                     public_ssh_key,
@@ -400,15 +431,15 @@
         add_state_log: Callable[[str], Awaitable[None]],
     ) -> Tuple[Activity, str, str]:
         logger.info(f"Creating new activity...")
 
         await add_state_log("[1/9] Getting agreement...")
 
         try:
-            agreement = await stack.agreement_manager.get_agreement()
+            agreement = await stack._managers[-1].get_agreement()
         except Exception as e:
             logger.error(f"Creating new activity failed with `{e}`")
             raise
 
         proposal = agreement.proposal
         provider_desc = f"{await proposal.get_provider_name()} ({await proposal.get_provider_id()})"
         await add_state_log(f"[2/9] Creating activity on provider: {provider_desc}...")
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/golem/helpers/demand_config.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/golem/helpers/demand_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ray_on_golem.server.services.golem.manifest import get_manifest
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class MaxCpuThreadsPayload(Payload):
-    max_cpu_threads: int = constraint(defaults.INF_CPU_THREADS, "<=", default=None)
+    max_cpu_threads: int = constraint(defaults.PROP_INF_CPU_THREADS, "<=", default=None)
 
 
 class DemandConfigHelper:
     def __init__(self, registry_stats: bool):
         self._registry_stats = registry_stats
 
     async def get_payloads_from_demand_config(
@@ -61,14 +61,15 @@
     ) -> Payload:
         manifest = get_manifest(
             image_url,
             image_hash,
             list(set([url.scheme for url in demand_config.outbound_urls])),
             demand_config.outbound_urls,
         )
+        logger.debug("Generated manifest:  %s", str(manifest))
         manifest = base64.b64encode(json.dumps(manifest).encode("utf-8")).decode("utf-8")
 
         params = demand_config.dict(
             exclude={"image_hash", "image_tag", "outbound_urls", "subnet_tag", "max_cpu_threads"}
         )
         params["manifest"] = manifest
         return ManifestVmPayload(**params)
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/golem/manifest.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/golem/manifest.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/golem/provider_data.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/golem/provider_data.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/ray.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/ray.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from contextlib import asynccontextmanager
 from functools import partial
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 from golem.utils.asyncio import create_task_with_logging, ensure_cancelled_many
 from golem.utils.logging import get_trace_id_name
-from ray.autoscaler.tags import NODE_KIND_HEAD, TAG_RAY_NODE_KIND
+from ray.autoscaler.tags import NODE_KIND_HEAD, TAG_RAY_NODE_KIND, TAG_RAY_USER_NODE_TYPE
 
 from ray_on_golem.exceptions import RayOnGolemError
 from ray_on_golem.server.exceptions import NodeNotFound
 from ray_on_golem.server.models import (
     Node,
     NodeConfigData,
     NodeData,
@@ -140,36 +140,46 @@
                 self._nodes[node_id] = Node(
                     node_id=node_id,
                     tags=tags,
                 )
 
                 self._create_node_tasks.append(
                     create_task_with_logging(
-                        self._create_node(node_id, NodeConfigData(**node_config)),
+                        self._create_node(
+                            node_id,
+                            NodeConfigData(**node_config),
+                            node_type=self._get_node_type(tags),
+                            is_head_node=self._is_head_node(tags),
+                        ),
                         trace_id=get_trace_id_name(self, f"create-node-{node_id}"),
                     )
                 )
 
         logger.info(f"Requested {count} nodes")
         logger.debug(f"{self._provider_config=}")
 
         return created_node_ids
 
-    async def _create_node(self, node_id: NodeId, node_config: NodeConfigData) -> None:
+    async def _create_node(
+        self, node_id: NodeId, node_config: NodeConfigData, node_type: str, is_head_node: bool
+    ) -> None:
         logger.info("Creating node `%s`...", node_id)
 
         try:
             activity, ip, ssh_proxy_command = await self._golem_service.create_activity(
                 node_config=node_config,
                 public_ssh_key=self._ssh_public_key,
                 ssh_user=self._ssh_user,
                 ssh_private_key_path=self._ssh_private_key_path,
                 total_budget=self._provider_config.total_budget,
                 payment_network=self._provider_config.payment_network,
+                payment_driver=self._provider_config.payment_driver,
                 add_state_log=partial(self._add_node_state_log, node_id),
+                node_type=node_type,
+                is_head_node=is_head_node,
             )
 
             self._print_ssh_command(
                 ip, ssh_proxy_command, self._ssh_user, self._ssh_private_key_path
             )
 
             async with self._get_node_context(node_id) as node:  # type: Node
@@ -303,19 +313,27 @@
                 raise NodeNotFound
 
             yield node
 
     async def _get_head_node(self) -> Node:
         async with self._nodes_lock:
             for node in self._nodes.values():
-                if node.tags.get(TAG_RAY_NODE_KIND) == NODE_KIND_HEAD:
+                if self._is_head_node(node.tags):
                     return node
 
             raise NodeNotFound
 
+    @staticmethod
+    def _is_head_node(tags: Tags) -> bool:
+        return tags.get(TAG_RAY_NODE_KIND) == NODE_KIND_HEAD
+
+    @staticmethod
+    def _get_node_type(tags: Tags) -> str:
+        return tags.get(TAG_RAY_USER_NODE_TYPE)
+
     def _print_ssh_command(
         self, ip: str, ssh_proxy_command: str, ssh_user: str, ssh_private_key_path: Path
     ) -> None:
         logger.debug(
             f"Connect to `{ip}` with:\n"
             f"{get_ssh_command(ip, ssh_proxy_command, ssh_user, ssh_private_key_path)}"
         )
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/utils.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/utils.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/services/yagna.py` & `ray_on_golem-0.9.0/ray_on_golem/server/services/yagna.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,31 +156,37 @@
 
         self._yagna_process.terminate()
         await self._yagna_process.wait()
 
         logger.info("Stopping Yagna done")
 
     async def run_payment_fund(self, network: str, driver: str) -> Dict:
-        logger.debug("Preparing `%s` funds with a timeout up to %s...", network, YAGNA_FUND_TIMEOUT)
+        platform = f"{driver}/{network}"
+        logger.debug(
+            "Preparing `%s` funds with a timeout up to %s...",
+            platform,
+            YAGNA_FUND_TIMEOUT,
+        )
 
+        is_mainnet = network in (PAYMENT_NETWORK_MAINNET, PAYMENT_NETWORK_POLYGON)
         fund_deadline = datetime.now() + YAGNA_FUND_TIMEOUT
         check_seconds = int(YAGNA_CHECK_INTERVAL.total_seconds())
         while datetime.now() < fund_deadline:
             try:
                 await run_subprocess_output(
                     self._yagna_path,
                     "payment",
-                    "fund",
+                    "fund" if not is_mainnet else "init",
                     "--network",
                     network,
                     "--driver",
                     driver,
                 )
             except RayOnGolemError as e:
-                logger.error("Preparing `%s` funds failed with error: %s", network, e)
+                logger.error("Preparing `%s` funds failed with error: %s", platform, e)
             else:
                 output = json.loads(
                     await run_subprocess_output(
                         self._yagna_path,
                         "payment",
                         "status",
                         "--network",
@@ -189,32 +195,32 @@
                         driver,
                         "--json",
                     )
                 )
 
                 amount = float(output["amount"])
 
-                if amount or network in (PAYMENT_NETWORK_MAINNET, PAYMENT_NETWORK_POLYGON):
+                if amount or is_mainnet:
                     logger.debug(
                         "Preparing `%s` funds done with balance of %.2f %s",
-                        network,
+                        platform,
                         amount,
                         output["token"],
                     )
                     return output
                 else:
                     logger.debug(
                         "Prepared funds seems not yet available, waiting additional `%s` seconds...",
                         check_seconds,
                     )
 
             await asyncio.sleep(check_seconds)
 
         raise YagnaServiceError(
-            f"Can't prepare `{network}` funds! Timeout of `{YAGNA_FUND_TIMEOUT}` reached."
+            f"Can't prepare `{platform}` funds! Timeout of `{YAGNA_FUND_TIMEOUT}` reached."
         )
 
     async def fetch_payment_status(self, network: str, driver: str) -> str:
         output = await run_subprocess_output(
             self._yagna_path, "payment", "status", "--network", network, "--driver", driver
         )
         return output.decode()
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/settings.py` & `ray_on_golem-0.9.0/ray_on_golem/server/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 RAY_ON_GOLEM_SHUTDOWN_TIMEOUT = timedelta(seconds=60)
 
 # how long we wait for the webserver process to exit
 RAY_ON_GOLEM_STOP_TIMEOUT = timedelta(minutes=3)
 
 RAY_ON_GOLEM_PID_FILENAME = "ray_on_golem.pid"
 
-
 URL_STATUS = "/"
 URL_CREATE_CLUSTER = "/create_cluster"
 URL_NON_TERMINATED_NODES = "/non_terminated_nodes"
 URL_IS_RUNNING = "/is_running"
 URL_IS_TERMINATED = "/is_terminated"
 URL_NODE_TAGS = "/tags"
 URL_GET_CLUSTER_DATA = "/cluster_data"
@@ -45,14 +44,15 @@
 URL_GET_SSH_PROXY_COMMAND = "/ssh_proxy_command"
 URL_GET_OR_CREATE_DEFAULT_SSH_KEY = "/ger_or_create_default_ssh_key"
 URL_SHUTDOWN = "/shutdown"
 
 PAYMENT_NETWORK_MAINNET = "mainnet"
 PAYMENT_NETWORK_POLYGON = "polygon"
 PAYMENT_NETWORK_GOERLI = "goerli"
+PAYMENT_NETWORK_HOLESKY = "holesky"
 PAYMENT_DRIVER_ERC20 = "erc20"
 
 RAY_ON_GOLEM_PATH = Path(os.getenv("RAY_ON_GOLEM_PATH", "ray-on-golem"))
 YAGNA_PATH = Path(os.getenv("YAGNA_PATH", "yagna"))
 WEBSOCAT_PATH = Path(os.getenv("WEBSOCAT_PATH", "websocat"))
 TMP_PATH = Path("/tmp/ray_on_golem")
 LOGGING_BACKUP_COUNT = 99
```

### Comparing `ray_on_golem-0.8.0/ray_on_golem/server/views.py` & `ray_on_golem-0.9.0/ray_on_golem/server/views.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/utils.py` & `ray_on_golem-0.9.0/ray_on_golem/utils.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/ray_on_golem/version.py` & `ray_on_golem-0.9.0/ray_on_golem/version.py`

 * *Files identical despite different names*

### Comparing `ray_on_golem-0.8.0/PKG-INFO` & `ray_on_golem-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: ray-on-golem
-Version: 0.8.0
+Version: 0.9.0
 Summary: Golem Network integration with Ray
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: dpath (>=2.1.6,<3.0.0)
-Requires-Dist: golem-core (>=0.5.0,<0.6.0)
-Requires-Dist: golem-node (==0.14.0)
+Requires-Dist: golem-core (>=0.6.0,<0.7.0)
+Requires-Dist: golem-node (==0.13.3)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (<2)
-Requires-Dist: ray[default] (>=2.9.2,<3.0.0)
+Requires-Dist: ray[default] (>=2.9.3,<2.10.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: setuptools
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: websocat (>=1.12.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Ray on Golem
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ray-on-golem Version: 0.8.0 Summary: Golem Network
+Metadata-Version: 2.1 Name: ray-on-golem Version: 0.9.0 Summary: Golem Network
 integration with Ray Author: Golem Factory Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: aiohttp
 (>=3,<4) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: click (>=8,<9)
 Requires-Dist: dpath (>=2.1.6,<3.0.0) Requires-Dist: golem-core
-(>=0.5.0,<0.6.0) Requires-Dist: golem-node (==0.14.0) Requires-Dist: pydantic
-(<2) Requires-Dist: ray[default] (>=2.9.2,<3.0.0) Requires-Dist: requests
-(>=2,<3) Requires-Dist: setuptools Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: websocat (>=1.12.0,<2.0.0) Description-Content-Type: text/
-markdown # Ray on Golem
+(>=0.6.0,<0.7.0) Requires-Dist: golem-node (==0.13.3) Requires-Dist: psutil
+(>=5.9.8,<6.0.0) Requires-Dist: pydantic (<2) Requires-Dist: ray[default]
+(>=2.9.3,<2.10.0) Requires-Dist: requests (>=2,<3) Requires-Dist: setuptools
+Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: websocat
+(>=1.12.0,<2.0.0) Description-Content-Type: text/markdown # Ray on Golem
 ## What is Golem, Ray and Ray on Golem [Golem](https://golem.network) is a
 decentralized marketplace for computing power, where providers let requestors
 use their machines for a small fee. Ray on Golem makes it super easy to set up
 and use Golem Network to run your Ray applications. [Ray](https://ray.io) on
 the other hand is an open-source framework dedicated to scaling Python
 workloads. It specializes in tooling for AI/ML applications, but at the same
 time, it is based on Ray Core which understands every piece of generic Python
```

