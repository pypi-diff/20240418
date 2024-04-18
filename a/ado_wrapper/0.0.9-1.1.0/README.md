# Comparing `tmp/ado_wrapper-0.0.9.tar.gz` & `tmp/ado_wrapper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.9.tar", max compression
+gzip compressed data, was "ado_wrapper-1.1.0.tar", max compression
```

## Comparing `ado_wrapper-0.0.9.tar` & `ado_wrapper-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.9/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.9/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.9/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-0.0.9/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2163 2024-04-14 14:14:45.873869 ado_wrapper-0.0.9/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.9/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.9/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.9/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.9/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      816 2024-04-14 14:23:57.502121 ado_wrapper-0.0.9/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.9/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    13458 2024-04-14 10:58:44.110259 ado_wrapper-0.0.9/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-14 10:58:41.445364 ado_wrapper-0.0.9/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3432 2024-04-14 10:58:38.698564 ado_wrapper-0.0.9/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    14566 2024-04-14 14:27:10.406329 ado_wrapper-0.0.9/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.9/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14602 2024-04-14 14:15:32.045150 ado_wrapper-0.0.9/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12740 2024-04-14 10:58:27.795680 ado_wrapper-0.0.9/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10172 2024-04-14 14:16:37.472201 ado_wrapper-0.0.9/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5972 2024-04-14 10:59:00.916715 ado_wrapper-0.0.9/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-0.0.9/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8313 2024-04-14 09:38:20.128931 ado_wrapper-0.0.9/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4877 2024-04-14 10:59:52.033985 ado_wrapper-0.0.9/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8422 2024-04-14 11:01:12.740028 ado_wrapper-0.0.9/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-14 14:54:01.312144 ado_wrapper-0.0.9/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4353 2024-04-14 14:25:02.772871 ado_wrapper-0.0.9/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2213 2024-04-14 14:51:56.622094 ado_wrapper-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.1.0/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.1.0/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.1.0/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.1.0/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.1.0/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.1.0/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.1.0/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.1.0/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.1.0/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      936 2024-04-17 20:35:57.592719 ado_wrapper-1.1.0/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.1.0/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.1.0/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14358 2024-04-18 10:11:16.564382 ado_wrapper-1.1.0/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.1.0/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     4878 2024-04-18 10:11:58.176749 ado_wrapper-1.1.0/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.1.0/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    14785 2024-04-15 19:15:13.133919 ado_wrapper-1.1.0/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.1.0/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.1.0/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.1.0/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10086 2024-04-15 15:16:12.399073 ado_wrapper-1.1.0/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.1.0/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.1.0/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.1.0/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4877 2024-04-14 10:59:52.033985 ado_wrapper-1.1.0/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8749 2024-04-18 09:52:24.036512 ado_wrapper-1.1.0/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-18 10:06:27.938348 ado_wrapper-1.1.0/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4412 2024-04-18 10:11:16.535800 ado_wrapper-1.1.0/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2446 2024-04-18 10:08:47.532362 ado_wrapper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.1.0/PKG-INFO
```

### Comparing `ado_wrapper-0.0.9/LICENSE` & `ado_wrapper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/README.md` & `ado_wrapper-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/__main__.py` & `ado_wrapper-1.1.0/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/client.py` & `ado_wrapper-1.1.0/ado_wrapper/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class AdoClient:
     def __init__(  # pylint: disable=too-many-arguments
         self, ado_email: str, ado_pat: str, ado_org: str, ado_project: str,
         state_file_name: str | None = "main.state", bypass_initialisation: bool = False,
         action: Literal["plan", "apply"] = "apply"  # fmt: skip
     ) -> None:
         """Takes an email, PAT, org, project, and state file name. The state file name is optional, and if not provided,
-        state will not be stored in "main.state" """
+        state will be stored in "main.state" (can be disabled using None)"""
         self.ado_email = ado_email
         self.ado_pat = ado_pat
         self.ado_org = ado_org
         self.ado_project = ado_project
 
         self.plan_mode = action == "plan"
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/dumps.py` & `ado_wrapper-1.1.0/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from ado_wrapper.resources.annotated_tags import AnnotatedTag
 from ado_wrapper.resources.branches import Branch
 from ado_wrapper.resources.builds import Build, BuildDefinition
 from ado_wrapper.resources.commits import Commit
+from ado_wrapper.resources.environment import Environment
 from ado_wrapper.resources.groups import Group
 from ado_wrapper.resources.merge_policies import MergePolicies, MergeBranchPolicy, MergePolicyDefaultReviewer
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
 from ado_wrapper.resources.repo import Repo, BuildRepository
 from ado_wrapper.resources.service_endpoint import ServiceEndpoint
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/builds.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/builds.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,26 +46,23 @@
 @dataclass
 class Build(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/builds?view=azure-devops-rest-7.1"""
 
     build_id: str = field(metadata={"is_id_field": True})
     build_number: str
     status: BuildStatus = field(metadata={"editable": True})  # Only this is editable ):
-    requested_by: Member
-    build_repo: BuildRepository
-    parameters: dict[str, str]
+    requested_by: Member = field(repr=False)
+    build_repo: BuildRepository = field(repr=False)
+    parameters: dict[str, str] = field(repr=False)
     definition: "BuildDefinition | None" = field(repr=False)
-    start_time: datetime | None = None
-    finish_time: datetime | None = None
+    start_time: datetime | None = field(repr=False)
+    finish_time: datetime | None = field(repr=False)
     queue_time: datetime | None = field(repr=False, default=None)
-    reason: str = "An automated build created with the ado_wrapper Python library"
-    priority: QueuePriority = "normal"
-
-    def __str__(self) -> str:
-        return f"{self.build_number} ({self.build_id}), {self.status}"
+    reason: str = field(default="An automated build created with the ado_wrapper Python library", repr=False)
+    priority: QueuePriority = field(default="normal", repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Build":
         requested_by = Member.from_request_payload(data["requestedBy"])
         build_repo = BuildRepository.from_request_payload(data["repository"])
         build_definition = BuildDefinition.from_request_payload(data["definition"]) if "definition" in data else None
         return cls(str(data["id"]), str(data["buildNumber"]), data["status"], requested_by, build_repo, data.get("templateParameters", {}),
@@ -108,25 +105,25 @@
     def update(self, ado_client: "AdoClient", attribute_name: str, attribute_value: Any) -> None:  # type: ignore[override]
         return super().update(
             ado_client, "patch",
             f"/{ado_client.ado_project}/_apis/build/builds/{self.build_id}?api-version=7.1",
             attribute_name, attribute_value, {attribute_name: attribute_value}  # fmt: skip
         )
 
-    # ============ End of requirement set by all state managed resources ================== #
-    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-    # =============== Start of additional methods included with class ===================== #
-
     @classmethod
-    def get_all_by_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Build]":
+    def get_all(cls, ado_client: "AdoClient") -> "list[Build]":  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"/{ado_client.ado_project}/_apis/build/builds?definitions={definition_id}&api-version=7.1",
+            f"/{ado_client.ado_project}/_apis/build/builds?api-version=7.1",
         )  # type: ignore[return-value]
 
+    # ============ End of requirement set by all state managed resources ================== #
+    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+    # =============== Start of additional methods included with class ===================== #
+
     @classmethod
     def create_and_wait_until_completion(cls, ado_client: "AdoClient", definition_id: str, branch_name: str = "main",
                                          max_timeout_seconds: int = 300) -> "Build":  # fmt: skip
         """Creates a build and waits until it is completed, or raises a TimeoutError if it takes too long.
         WARNING: This is a blocking operation, it will not return until the build is completed or the timeout is reached."""
         build = cls.create(ado_client, definition_id, branch_name, True)
         start_time = datetime.now()
@@ -150,14 +147,30 @@
         leases = leases_request.json()["value"]
         for lease in leases:
             lease_response = ado_client.session.delete(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/retention/leases?ids={lease['leaseId']}&api-version=6.1",
             )
             assert lease_response.status_code <= 204
 
+    @classmethod
+    def get_all_by_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Build]":
+        return super().get_all(
+            ado_client,
+            f"/{ado_client.ado_project}/_apis/build/builds?definitions={definition_id}&api-version=7.1",
+        )  # type: ignore[return-value]
+
+    @classmethod
+    def allow_approvers(cls, ado_client: "AdoClient", build_definition_id: str, approvers_ids: str) -> None:
+        """This is a PATCH request, so it doesn't return anything."""
+        return NotImplementedError("This method is not implemented yet!")  # type: ignore[return-value]
+        # ado_client.session.patch(
+        #     f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/pipelines/pipelinePermissions/approvers?api-version=7.1",
+        #     json={"approvers": [{"id": approvers_ids}]},
+        # )
+
 
 # ========================================================================================================
 
 
 @dataclass
 class BuildDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/definitions?view=azure-devops-rest-7.1"""
@@ -193,19 +206,20 @@
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: "AdoClient", name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
         description: str, agent_pool_id: str, variable_groups: list[str], branch_name: str = "main",  # fmt: skip
     ) -> "BuildDefinition":
+        payload = get_build_definition(name, repo_id, repo_name, path_to_pipeline, description,
+                                       ado_client.ado_project, agent_pool_id, branch_name)  # fmt: skip
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
-            payload=get_build_definition(name, repo_id, repo_name, path_to_pipeline, description, ado_client.ado_project,
-                                         agent_pool_id, branch_name)  # fmt: skip
+            payload=payload,
         )  # type: ignore[return-value]
         #  | {"variableGroups": [{"id": x for x in variable_groups}]},
 
     def update(self, ado_client: "AdoClient", attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         if self.build_repo is None or self.process is None:
             raise ValueError("This build definition does not have a (repository or process) in its data, it cannot be updated")
         payload = (
@@ -227,25 +241,25 @@
             build.delete(ado_client)  # Can't remove from state because retention policies etc.
         return super().delete_by_id(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions/{resource_id}?forceDelete=true&api-version=7.1",
             resource_id,
         )
 
-    # ============ End of requirement set by all state managed resources ================== #
-    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-    # =============== Start of additional methods included with class ===================== #
-
     @classmethod
     def get_all(cls, ado_client: "AdoClient") -> "list[BuildDefinition]":  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
+    # ============ End of requirement set by all state managed resources ================== #
+    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+    # =============== Start of additional methods included with class ===================== #
+
     def get_all_builds_by_definition(self, ado_client: "AdoClient") -> "list[Build]":
         return Build.get_all_by_definition(ado_client, self.build_definition_id)
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: "AdoClient", repo_id: str) -> "list[BuildDefinition]":
         return super().get_all(
             ado_client,
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/commits.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/groups.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from dataclasses import dataclass, field
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 
-# from ado_wrapper.resources.users import GroupMember
-
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
 @dataclass
 class Group(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/graph/groups?view=azure-devops-rest-7.1"""
@@ -18,17 +16,14 @@
     group_descriptor: str = field(metadata={"is_id_field": True})  # None are editable
     name: str = field(metadata={"internal_name": "displayName"})  # Not editable
     description: str
     group_id: str  # Not editable, don't use
     origin_id: str = field(metadata={"internal_name": "originId"})  # Not editable, don't use
     # group_members: list[GroupMember] = field(default_factory=list)
 
-    def __str__(self) -> str:
-        return repr(self)
-
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "Group":
         return cls(data["url"].split("/_apis/Graph/Groups/", maxsplit=1)[1], data["displayName"], data.get("description", ""),
                    data["domain"].removeprefix("vstfs:///Classification/TeamProject/"), data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, group_descriptor: str) -> "Group":
@@ -56,19 +51,19 @@
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, group_name: str) -> "Group | None":
         return cls.get_by_abstract_filter(ado_client, lambda group: group.name == group_name)  # type: ignore[return-value, attr-defined]
 
+    # @classmethod
+    # def get_all_by_member(cls, ado_client: AdoClient, member_descriptor_id: str) -> list["Group"]:
+    #     raise NotImplementedError
+    # Will finish this later
+    # return [group for group in cls.get_all(ado_client) if group.group_descriptor == member_descriptor_id]
+
     # def get_members(self, ado_client: AdoClient) -> list["GroupMember"]:
     #     request = ado_client.session.get(
     #         f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/groups/{self.group_id}/members?api-version=7.1-preview.2",
     #     ).json()
     #     rint(request)
     #     # return [GroupMember.from_request_payload(member) for member in request]
-
-    @classmethod
-    def get_all_by_member(cls, ado_client: AdoClient, member_descriptor_id: str) -> list["Group"]:
-        raise NotImplementedError
-        # Will finish this later
-        # return [group for group in cls.get_all(ado_client) if group.group_descriptor == member_descriptor_id]
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/merge_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,27 @@
 from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 WhenChangesArePushed = Literal["require_revote_on_each_iteration", "require_revote_on_last_iteration",
                                "reset_votes_on_source_push", "reset_rejections_on_source_push", "do_nothing"]  # fmt: skip
-name_mapping = {
+merge_complete_name_mapping = {
     "requireVoteOnEachIteration": "require_revote_on_each_iteration",
     "requireVoteOnLastIteration": "require_revote_on_last_iteration",
     "resetOnSourcePush": "reset_votes_on_source_push",
     "resetRejectionsOnSourcePush": "reset_rejections_on_source_push",
     "do_nothing": "do_nothing",
 }
+limit_merge_type_mapping = {
+    "allowSquash": "allow_squash",
+    "allowNoFastForward": "allow_no_fast_forward",
+    "allowRebase": "allow_rebase",
+    "allowRebaseMerge": "allow_rebase_merge",
+}
 
 
 def _get_type_id(ado_client: AdoClient, action_type: str) -> str:
     """Used internally to get a specific update request ID"""
     request = ado_client.session.get(
         f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/types?api-version=6.0"
     )
@@ -105,16 +111,16 @@
     when_new_changes_are_pushed: WhenChangesArePushed
     created_date: datetime = field(repr=False)
     is_inherited: bool = field(default=False, repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any], is_inherited: bool) -> "MergeBranchPolicy":  # type: ignore[override]
         settings = data["settings"]
-        when_new_changes_are_pushed = name_mapping[
-            ([x for x in name_mapping if settings.get(x, False)] or ["do_nothing"])[0]
+        when_new_changes_are_pushed = merge_complete_name_mapping[
+            ([x for x in merge_complete_name_mapping if settings.get(x, False)] or ["do_nothing"])[0]
         ]  # Any or "do_nothing"  # fmt: skip
         branch_name: str | None = settings["scope"][0]["refName"]
         return cls(
             data["id"], settings["scope"][0]["repositoryId"], (branch_name.removeprefix("refs/heads/") if branch_name else None),
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
             when_new_changes_are_pushed, from_ado_date_string(data["createdDate"]),  # type: ignore[arg-type]
             is_inherited  # fmt: skip
@@ -167,15 +173,15 @@
         """Used internally to get a list of all policies."""
         policy_groups: dict[str, Any] = data["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"] or {}  # fmt: skip
         all_policies = []
         for policy_group in policy_groups.values():
             for policy in policy_group["currentScopePolicies"] or []:  # If it's None, don't loop
                 settings = policy["settings"]
                 # Limit merge types
-                if any(x in settings for x in ("allowSquash", "allowNoFastForward", "allowRebase", "allowRebaseMerge")):
+                if any(x in settings for x in limit_merge_type_mapping):
                     continue
                 # Build Validation {'buildDefinitionId': 4, 'queueOnSourceUpdateOnly': True, 'manualQueueOnly': False, 'displayName': None, 'validDuration': 720.0
                 if "buildDefinitionId" in settings:
                     continue
                 # Automatically included reviewers
                 if "requiredReviewerIds" in settings:
                     all_policies.append(MergePolicyDefaultReviewer.from_request_payload(policy))
@@ -210,15 +216,17 @@
             if policies is not None else None
         )  # fmt: skip
 
     @classmethod
     def get_default_reviewers_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergePolicyDefaultReviewer] | None:  # fmt: skip
         policies = cls.get_all_by_repo_id(ado_client, repo_id, branch_name)
         return (
-            [x for x in policies if isinstance(x, MergePolicyDefaultReviewer)] if policies is not None else None  # pylint: disable=not-an-iterable
+            [x for x in policies if isinstance(x, MergePolicyDefaultReviewer)]  # pylint: disable=not-an-iterable
+            if policies is not None
+            else None
         )
 
     # ================== Default Reviewers ================== #
     @staticmethod
     def add_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
         return MergePolicyDefaultReviewer.add_default_reviewer(ado_client, repo_id, reviewer_id, is_required, branch_name)
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/projects.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/pull_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, Literal, TYPE_CHECKING
 from dataclasses import dataclass, field
 
-from ado_wrapper.utils import from_ado_date_string, ResourceNotFound
+from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member, Reviewer
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
     from ado_wrapper.resources.repo import Repo
 
@@ -21,15 +21,15 @@
 
 @dataclass
 class PullRequest(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-requests?view=azure-devops-rest-7.1"""
 
     pull_request_id: str = field(metadata={"is_id_field": True})
     title: str = field(metadata={"editable": True})
-    description: str = field(metadata={"editable": True})
+    description: str = field(repr=False, metadata={"editable": True})
     source_branch: str = field(repr=False)
     target_branch: str = field(repr=False)
     author: Member
     creation_date: datetime = field(repr=False)
     repo: Repo
     close_date: datetime | None = field(default=None, repr=False)
     is_draft: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDraft"})
@@ -75,15 +75,14 @@
             raise ValueError("The branch you are trying to create a pull request from does not exist.")
         obj = cls.from_request_payload(request)
         ado_client.state_manager.add_resource_to_state(cls.__name__, obj.pull_request_id, obj.to_json())  # type: ignore[arg-type]
         return obj
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> None:  # type: ignore[override]
-        # raise NotImplementedError("You can't delete pull requests, only close them.")
         pr = cls.get_by_id(ado_client, pull_request_id)
         pr.update(ado_client, "merge_status", "abandoned")
         ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request_id)
 
     def update(self, ado_client: AdoClient, attribute_name: PullRequestEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         return super().update(
             ado_client, "patch",
@@ -127,24 +126,22 @@
         request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/reviewers?api-version=7.1",
         ).json()
         return [Member.from_request_payload(reviewer) for reviewer in request["value"]]
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list[PullRequest]:
-        pull_requests = ado_client.session.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?searchCriteria.status={status}&api-version=7.1",
-        ).json()
         try:
-            return [PullRequest.from_request_payload(pr) for pr in pull_requests["value"]]
+            return super().get_all(
+                ado_client,
+                f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?searchCriteria.status={status}&api-version=7.1",
+            )  # type: ignore[return-value]
         except KeyError:
-            if pull_requests.get("message", "").startswith("TF401019"):
-                print(f"Repo `{pull_requests['message'].split('identifier')[1].split(' ')[0]}` was disabled, or you had no access.")
-                return []
-            raise ResourceNotFound(pull_requests)  # pylint: disable=raise-missing-from
+            print(f"Repo with id `{repo_id}` was disabled, or you had no access.")
+            return []
 
     @classmethod
     def get_all_by_author(cls, ado_client: AdoClient, author_email: str, status: PullRequestStatus = "all") -> list[PullRequest]:
         return [pr for pr in cls.get_all(ado_client, status) if pr.author.email == author_email]
 
     @classmethod
     def get_my_pull_requests(cls, ado_client: AdoClient) -> list[PullRequest]:
@@ -154,18 +151,15 @@
         request = ado_client.session.get(f"https://dev.azure.com/{ado_client.ado_org}/_pulls")
         raw_data = (
             request.text.split("application/json")[1].split('pullRequests"')[1].split("queries")[0].removeprefix(":").removesuffix(',"')
         )
         return [cls.from_request_payload(pr) for pr in json.loads(raw_data).values()]
 
     def get_comment_threads(self, ado_client: AdoClient, ignore_system_messages: bool = True) -> list[PullRequestCommentThread]:
-        request = ado_client.session.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/threads?api-version=7.1",
-        ).json()["value"]
-        comments = [PullRequestCommentThread.from_request_payload(data) for data in request]
+        comments = PullRequestCommentThread.get_all(ado_client, self.repo.repo_id, self.pull_request_id)
         if ignore_system_messages:
             comments = [comment for comment in comments if comment.comments[0].comment_type != "system"]
         return comments
 
     def get_comments(self, ado_client: AdoClient, ignore_system_messages: bool = True) -> list[PullRequestComment]:
         """Gets a list of comments on a pull request, optionally ignoring system messages."""
         return [comment for thread in self.get_comment_threads(ado_client, ignore_system_messages) for comment in thread.comments]
@@ -237,15 +231,15 @@
     creation_date: datetime = field(repr=False)
     comment_type: CommentType
     is_deleted: bool = field(repr=False)
     liked_users: list[Member] = field(repr=False)
 
     def __str__(self) -> str:
         return (
-            f"PullRequestComment(id={self.comment_id}, author_email=`{self.author.email}`, content=`{self.content}`, "
+            f"PullRequestComment(comment_id={self.comment_id}, author_email=`{self.author.email}`, content=`{self.content}`, "
             f"creation_date={self.creation_date}, comment_type={self.comment_type}{', is_deleted=True' if self.is_deleted else ''})"
         )
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "PullRequestComment":
         author = Member.from_request_payload(data["author"])
         liked_users = [Member.from_request_payload(user) for user in data.get("usersLiked", [])]
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/releases.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/releases.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 ReleaseDefinitionEditableAttribute = Literal["name", "description", "release_name_format", "variable_groups"]
 ReleaseStatus = Literal["active", "abandoned", "draft", "undefined"]
 
 # ========================================================================================================
-# WARNING: THIS FILE IS MAINLY UNTESTED, AND MAY NOT WORK AS EXPECTED
+# WARNING: THIS FILE IS NOT MASSIVELY UNTESTED, AND MAY NOT WORK AS EXPECTED
 # FEEL FREE TO MAKE A PR TO FIX/IMPROVE THIS FILE
 # ========================================================================================================
 
 
 def get_release_definition(
     ado_client: "AdoClient", name: str, variable_group_ids: list[int], agent_pool_id: str, revision: str = "1", _id: str = ""
 ) -> dict[str, Any]:
@@ -87,24 +87,21 @@
 @dataclass
 class Release(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/release/releases?view=azure-devops-rest-7.1"""
 
     release_id: str = field(metadata={"is_id_field": True})
     name: str
     status: ReleaseStatus
-    created_on: datetime
-    created_by: Member
-    description: str
+    created_on: datetime = field(repr=False)
+    created_by: Member = field(repr=False)
+    description: str = field(repr=False)
     variables: list[dict[str, Any]] | None = field(default_factory=list, repr=False)  # type: ignore[assignment]
     variable_groups: list[int] | None = field(default_factory=list, repr=False)  # type: ignore[assignment]
     keep_forever: bool = field(default=False, repr=False)
 
-    def __str__(self) -> str:
-        return f"{self.name} ({self.release_id}), {self.status}"
-
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Release":
         created_by = Member.from_request_payload(data["createdBy"])
         return cls(str(data["id"]), data["name"], data["status"], from_ado_date_string(data["createdOn"]), created_by, data["description"],
                    data.get("variables", None), data.get("variableGroups", None), data["keepForever"])  # fmt: skip
 
     @classmethod  # TO-DO: Test
@@ -199,47 +196,45 @@
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.0",
             get_release_definition(ado_client, name, variable_group_ids, agent_pool_id),
         )  # type: ignore[return-value]
 
     @classmethod
     def delete_by_id(cls, ado_client: "AdoClient", release_definition_id: str) -> None:  # type: ignore[override]
         for release in ReleaseDefinition.get_all_releases_for_definition(ado_client, release_definition_id):
-            ado_client.state_manager.remove_resource_from_state("Release", release.release_id)
+            # ado_client.state_manager.remove_resource_from_state("Release", release.release_id)
+            release.delete(ado_client)
         return super().delete_by_id(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{release_definition_id}?forceDelete=True&api-version=7.1",
             release_definition_id,
         )
 
     def update(self, ado_client: "AdoClient", attribute_name: ReleaseDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         self.revision = str(int(self.revision) + 1)
         return super().update(
             ado_client, "put",
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{self.release_definition_id}?api-version=7.1",
             attribute_name, attribute_value, self._raw_data,  # fmt: skip
         )
 
-    # ============ End of requirement set by all state managed resources ================== #
-    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-    # =============== Start of additional methods included with class ===================== #
-
-    @classmethod
-    def get_all_releases_for_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Release]":
-        response = ado_client.session.get(
-            f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases?api-version=7.1&definitionId={definition_id}",
-        ).json()
-        return [Release.from_request_payload(release) for release in response["value"]]
-
     @classmethod
     def get_all(cls, ado_client: "AdoClient") -> "list[ReleaseDefinition]":  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
+    # ============ End of requirement set by all state managed resources ================== #
+    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+    # =============== Start of additional methods included with class ===================== #
+
+    @classmethod
+    def get_all_releases_for_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Release]":
+        return Release.get_all(ado_client, definition_id)
+
 
 # ========================================================================================================
 
 # @dataclass
 # class ReleaseEnvironment:
 #     """https://learn.microsoft.com/en-us/rest/api/azure/devops/release/definitions/list?view=azure-devops-rest-7.1&tabs=HTTP#releasedefinitionenvironment"""
 #     release_environment_id: str = field(metadata={"is_id_field": True})
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/repo.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 
     repo_id: str = field(metadata={"is_id_field": True})
     name: str = field(metadata={"editable": True})
     default_branch: str = field(default="main", repr=False, metadata={"editable": True, "internal_name": "defaultBranch"})
     is_disabled: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDisabled"})
     # WARNING, disabling a repo means it's not able to be deleted, proceed with caution.
 
-    def __str__(self) -> str:
-        return f"Repo(name={self.name}, id={self.repo_id})"
-
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "Repo":
         return cls(
             data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
         )
 
     @classmethod
@@ -104,15 +101,15 @@
         if request.status_code != 200:
             raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
         return request.text  # This is the file content
 
     def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
         """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
         This function downloads the contents of a repo, and returns a dictionary of the files and their contents
-        The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
+        The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"] etc."""
         try:
             request = ado_client.session.get(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
             )
         except requests.exceptions.ConnectionError:
             print(f"=== Connection error, failed to download {self.repo_id}")
             return {}
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/teams.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/users.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 # ======================================================================================================= #
 # ------------------------------------------------------------------------------------------------------- #
 # ======================================================================================================= #
 
 
 @dataclass
 class Member(StateManagedResource):
-    """A stripped down member class which is often returned by the API, for example in build requests."""
+    """A stripped down member class which is often returned by the API, for example in build requests or PRs."""
 
     name: str
     email: str
     member_id: str = field(metadata={"is_id_field": True}, repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Member":
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.1.0/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.9/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.1.0/ado_wrapper/state_managed_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,33 +80,37 @@
         cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None
     ) -> "StateManagedResource | PlannedStateManagedResource":
         if ado_client.plan_mode:
             return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = ado_client.session.post(url, json=payload or {})  # Create a brand new dict
-        if request.status_code == 401:
-            raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
-        if request.status_code == 409:
-            raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
+        if request.status_code >= 300:
+            if request.status_code == 401:
+                raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
+            if request.status_code == 409:
+                raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
+            raise ValueError(f"Error creating {cls.__name__}: {request.status_code} - {request.text}")
         resource = cls.from_request_payload(request.json())
         ado_client.state_manager.add_resource_to_state(cls.__name__, extract_id(resource), resource.to_json())  # type: ignore[arg-type]
         return resource
 
     @classmethod
     def delete_by_id(cls, ado_client: "AdoClient", url: str, resource_id: str) -> None:
         """Deletes an object by its id. The id is passed so it can be removed from state"""
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = ado_client.session.delete(url)
         if request.status_code != 204:
             if request.status_code == 404:
                 print("[ADO_WRAPPER] Resource not found, probably already deleted, removing from state")
             else:
-                raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
+                if "message" in request.json():
+                    raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
+                raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.text}")
         ado_client.state_manager.remove_resource_from_state(cls.__name__, resource_id)  # type: ignore[arg-type]
 
     def delete(self, ado_client: "AdoClient") -> None:
         return self.delete_by_id(ado_client, extract_id(self))  # type: ignore[call-arg]  # pylint: disable=no-value-for-parameter
 
     def update(self, ado_client: "AdoClient", update_action: Literal["put", "patch"], url: str,  # pylint: disable=too-many-arguments
                attribute_name: str, attribute_value: Any, params: dict[str, Any]) -> None:  # fmt: skip
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/state_manager.py` & `ado_wrapper-1.1.0/ado_wrapper/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, TypedDict, TYPE_CHECKING, Literal
 
 from ado_wrapper.utils import DeletionFailed, get_resource_variables, ResourceType
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
-STATE_FILE_VERSION = "1.5"
+STATE_FILE_VERSION = "1.6"
 
 
 class StateFileType(TypedDict):
     state_file_version: str
     resources: dict[ResourceType, dict[str, Any]]
```

### Comparing `ado_wrapper-0.0.9/ado_wrapper/utils.py` & `ado_wrapper-1.1.0/ado_wrapper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from datetime import datetime, timezone
 from typing import overload, TYPE_CHECKING, Literal
 from dataclasses import fields
 
 if TYPE_CHECKING:
     from ado_wrapper.state_managed_abc import StateManagedResource
 
-ResourceType = Literal[
-    "Branch", "Build", "BuildDefinition", "Commit", "Group", "MergePolicies", "MergeBranchPolicy", "MergePolicyDefaultReviewer",
-    "Project", "PullRequest", "Release", "ReleaseDefinition",
-    "Repo", "Team", "AdoUser", "Member", "ServiceEndpoint", "Reviewer", "VariableGroup"  # fmt: skip
-]
-
 
 @overload
 def from_ado_date_string(date_string: str) -> datetime:
     ...
 
 
 @overload
@@ -125,13 +119,20 @@
 class AuthenticationError(Exception):
     pass
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
-        Branch, Build, BuildDefinition, Commit, Group, MergePolicies, MergeBranchPolicy, MergePolicyDefaultReviewer, Project,
-        PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
+        AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
+        MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
         AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
     )
 
     return locals()
+
+
+ResourceType = Literal[
+    "AnnotatedTag", "Branch", "Build", "BuildDefinition", "Commit", "Environment", "Group", "MergePolicies", "MergeBranchPolicy",
+    "MergePolicyDefaultReviewer", "Project", "PullRequest", "Release", "ReleaseDefinition",
+    "Repo", "Team", "AdoUser", "Member", "ServiceEndpoint", "Reviewer", "VariableGroup"  # fmt: skip
+]
```

### Comparing `ado_wrapper-0.0.9/pyproject.toml` & `ado_wrapper-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.9"
+version = "1.1.0"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -72,15 +72,27 @@
 markers = [
     "wip: mark test as a work in progress",
     "from_request_payload: mark test which convert payloads to resources",
     "update: Tests which are used to update the API",
     "create_delete: Tests which are used to create and delete resources",
     "get_by_id: Tests which are used to get resources by their ID",
     "get_all: Tests which are used to get all resources",
+    "get_all_by_name: Tests which are used to get resources by their name",
     "integrations: Tests which are used to test full integrations of multiple resources",
 ]
 
 [tool.black]
 line_length = 140
 
 [tool.isort]
 profile = "black"
+
+[tool.coverage.run]
+omit = [
+    "tests/*",
+    "dist/*",
+    "__pycache__/*",
+    ".mypy_cache/*",
+    ".pytest_cache/*",
+    ".vscode/*",
+    "/opt/*",
+]
```

### Comparing `ado_wrapper-0.0.9/PKG-INFO` & `ado_wrapper-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.9
+Version: 1.1.0
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

