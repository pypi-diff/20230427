# Comparing `tmp/iam_ape-1.0.5.tar.gz` & `tmp/iam_ape-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_ape-1.0.5.tar", max compression
+gzip compressed data, was "iam_ape-1.1.0.tar", max compression
```

## Comparing `iam_ape-1.0.5.tar` & `iam_ape-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-03-21 14:09:32.879473 iam_ape-1.0.5/LICENSE
--rw-r--r--   0        0        0     3032 2023-03-21 14:09:32.879626 iam_ape-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880346 iam_ape-1.0.5/iam_ape/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880510 iam_ape-1.0.5/iam_ape/aws_iam_actions/__init__.py
--rw-r--r--   0        0        0   254744 2023-03-23 15:18:42.493453 iam_ape-1.0.5/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
--rw-r--r--   0        0        0     2773 2023-03-23 15:18:42.493898 iam_ape-1.0.5/iam_ape/aws_iam_actions/scrape_iam_actions.py
--rw-r--r--   0        0        0     1655 2023-03-21 14:09:32.881248 iam_ape-1.0.5/iam_ape/consts.py
--rw-r--r--   0        0        0    30290 2023-03-23 15:18:42.494325 iam_ape-1.0.5/iam_ape/evaluator.py
--rw-r--r--   0        0        0    12009 2023-03-23 15:18:42.494634 iam_ape-1.0.5/iam_ape/expand_policy.py
--rw-r--r--   0        0        0     7866 2023-03-23 15:18:42.495061 iam_ape-1.0.5/iam_ape/helper_functions.py
--rw-r--r--   0        0        0     4774 2023-03-23 15:18:42.495406 iam_ape-1.0.5/iam_ape/helper_types.py
--rw-r--r--   0        0        0     6236 2023-03-23 15:18:42.495778 iam_ape-1.0.5/iam_ape/main.py
--rw-r--r--   0        0        0        0 2023-03-23 15:18:42.495823 iam_ape-1.0.5/iam_ape/py.typed
--rw-r--r--   0        0        0     1195 2023-03-23 15:18:42.496176 iam_ape-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 iam_ape-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-21 14:09:32.879473 iam_ape-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-27 15:10:48.767861 iam_ape-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880346 iam_ape-1.1.0/iam_ape/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880510 iam_ape-1.1.0/iam_ape/aws_iam_actions/__init__.py
+-rw-r--r--   0        0        0   259037 2023-04-27 15:10:48.769019 iam_ape-1.1.0/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
+-rw-r--r--   0        0        0     2773 2023-03-23 15:18:42.493898 iam_ape-1.1.0/iam_ape/aws_iam_actions/scrape_iam_actions.py
+-rw-r--r--   0        0        0     1655 2023-03-21 14:09:32.881248 iam_ape-1.1.0/iam_ape/consts.py
+-rw-r--r--   0        0        0    31885 2023-04-27 15:10:48.769584 iam_ape-1.1.0/iam_ape/evaluator.py
+-rw-r--r--   0        0        0    14524 2023-04-27 15:10:48.769991 iam_ape-1.1.0/iam_ape/expand_policy.py
+-rw-r--r--   0        0        0     3724 2023-04-27 15:10:48.770267 iam_ape-1.1.0/iam_ape/helper_classes.py
+-rw-r--r--   0        0        0     7900 2023-04-27 15:10:48.770543 iam_ape-1.1.0/iam_ape/helper_functions.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:10:48.770874 iam_ape-1.1.0/iam_ape/helper_types.py
+-rw-r--r--   0        0        0     9584 2023-04-27 15:10:48.771237 iam_ape-1.1.0/iam_ape/main.py
+-rw-r--r--   0        0        0        0 2023-03-23 15:18:42.495823 iam_ape-1.1.0/iam_ape/py.typed
+-rw-r--r--   0        0        0     1257 2023-04-27 15:10:48.772004 iam_ape-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.0/PKG-INFO
```

### Comparing `iam_ape-1.0.5/LICENSE` & `iam_ape-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_ape-1.0.5/README.md` & `iam_ape-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 }
 ```
 This statement, having both `Resource` and `NotResource` together, is not supported by AWS but makes more sense when trying to understand what the effective permissions of a user are.
 
 ## Roadmap ##
 - [ ] Add an option to supply a resource policy and evaluate whether the entity has access to that resource 
 - [ ] Support additional permissions inherited by Role assumption
-- [ ] Support SCP Policies
+- [x] Support SCP Policies
```

### Comparing `iam_ape-1.0.5/iam_ape/aws_iam_actions/scrape_iam_actions.py` & `iam_ape-1.1.0/iam_ape/aws_iam_actions/scrape_iam_actions.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.0.5/iam_ape/consts.py` & `iam_ape-1.1.0/iam_ape/consts.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.0.5/iam_ape/evaluator.py` & `iam_ape-1.1.0/iam_ape/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from collections import defaultdict
 from dataclasses import replace
 from fnmatch import fnmatch
 from typing import Any, Dict, List, Optional, Set, Tuple
 
 from iam_ape.consts import PolicyElement
 from iam_ape.expand_policy import PolicyExpander
+from iam_ape.helper_classes import (
+    Action,
+    IneffectiveAction,
+    PermissionsContainer,
+    PolicyWithSource,
+)
 from iam_ape.helper_functions import (
     deep_update,
     get_default_policy_for_managed_policy,
     merge_condition,
     normalize_policy,
 )
-from iam_ape.helper_types import (
-    Action,
-    EntityType,
-    FinalReportT,
-    IneffectiveAction,
-    PermissionsContainer,
-    PolicyWithSource,
-)
+from iam_ape.helper_types import EntityType, FinalReportT
 
 logger = logging.getLogger("IAM-APE:evaluator")
 
 
 def should_deny(
     iam_action: Action, denied_actions: Dict[str, Set[Action]]
 ) -> Tuple[bool, Set[Action], Optional[str]]:
@@ -468,17 +467,26 @@
         }
         self.Policy: Dict[str, Any] = {
             policy["Arn"]: policy for policy in auth_report.get("Policies", [])
         }
 
 
 class EffectivePolicyEvaluator:
-    def __init__(self, authorization_details: AuthorizationDetails) -> None:
+    def __init__(
+        self,
+        authorization_details: AuthorizationDetails,
+        scp_policies: Optional[List[PolicyWithSource]] = None,
+    ) -> None:
         self.auth_details = authorization_details
         self.policy_expander = PolicyExpander()
+        self.scp_policy = (
+            self.policy_expander.expand_policies(scp_policies)
+            if scp_policies
+            else PermissionsContainer()
+        )
 
     def create_json_report(
         self, permissions_container: PermissionsContainer
     ) -> FinalReportT:
         def action_to_service(action: str) -> str:
             return action.split(":")[0]
 
@@ -552,55 +560,78 @@
         }
         # for section in ("allowed_permissions", "denied_permissions"):
         for action_tuple_set in permissions_container.allowed_permissions.values():
             for action_tuple in action_tuple_set:
                 service = action_to_service(action_tuple.action)
                 resource = action_tuple.resource or "*"
                 if action_tuple.not_resource:
-                    resource += f" EXCEPT {action_tuple.not_resource}"
+                    if res["allowed_permissions"][service][resource].get("NotResource"):
+                        res["allowed_permissions"][service][resource][
+                            "NotResource"
+                        ].append(action_tuple.not_resource)
+                    else:
+                        res["allowed_permissions"][service][resource]["NotResource"] = [
+                            action_tuple.not_resource
+                        ]
                 access_level = self.policy_expander.get_action_access_level(
                     action_tuple.action
                 )
-                res["allowed_permissions"][service][resource][access_level][
-                    action_tuple.action
-                ]["Condition"] = merge_condition(
-                    res["allowed_permissions"][service][resource][access_level].get(
-                        action_tuple.action
-                    ),
+                if cond := merge_condition(
+                    res["allowed_permissions"][service][resource][access_level]
+                    .get(action_tuple.action, {})
+                    .get("Condition", {}),
                     action_tuple.condition,
                     negate=False,
-                )
+                ):
+                    res["allowed_permissions"][service][resource][access_level][
+                        action_tuple.action
+                    ]["Condition"] = cond
                 res["allowed_permissions"][service][resource][access_level][
                     action_tuple.action
                 ]["source"].add(action_tuple.source)
 
         for action_tuple_set in permissions_container.denied_permissions.values():
             for action_tuple in action_tuple_set:
                 service = action_to_service(action_tuple.action)
                 resource = action_tuple.resource or "*"
                 if action_tuple.not_resource:
-                    resource += f" EXCEPT {action_tuple.not_resource}"
+                    if res["denied_permissions"][service][resource].get("NotResource"):
+                        res["denied_permissions"][service][resource][
+                            "NotResource"
+                        ].append(action_tuple.not_resource)
+                    else:
+                        res["denied_permissions"][service][resource]["NotResource"] = [
+                            action_tuple.not_resource
+                        ]
                 access_level = self.policy_expander.get_action_access_level(
                     action_tuple.action
                 )
-                res["denied_permissions"][service][resource][access_level][
-                    action_tuple.action
-                ]["Condition"] = merge_condition(
-                    res["denied_permissions"][service][resource][access_level].get(
-                        action_tuple.action
-                    ),
+                if cond := merge_condition(
+                    res["denied_permissions"][service][resource][access_level]
+                    .get(action_tuple.action, {})
+                    .get("Condition", {}),
                     action_tuple.condition,
                     negate=False,
-                )
+                ):
+                    res["denied_permissions"][service][resource][access_level][
+                        action_tuple.action
+                    ]["Condition"] = cond
 
         for action_tuple in permissions_container.ineffective_permissions:
             service = action_to_service(action_tuple.action)
             resource = action_tuple.resource or "*"
             if action_tuple.not_resource:
-                resource += f" EXCEPT {action_tuple.not_resource}"
+                if res["ineffective_permissions"][service][resource].get("NotResource"):
+                    res["ineffective_permissions"][service][resource][
+                        "NotResource"
+                    ].append(action_tuple.not_resource)
+                else:
+                    res["ineffective_permissions"][service][resource]["NotResource"] = [
+                        action_tuple.not_resource
+                    ]
             access_level = self.policy_expander.get_action_access_level(
                 action_tuple.action
             )
             res["ineffective_permissions"][service][resource][access_level][
                 action_tuple.action
             ]["denied_by"].add(action_tuple.denied_by)
 
@@ -669,26 +700,25 @@
         direct_permissions = self.policy_expander.expand_policies(
             direct_policies + indirect_policies
         )
         permission_boundary = self.get_permission_boundary(entity_obj)
 
         final_permissions, ineffective_permissions = explicitly_deny(direct_permissions)
 
-        if (
-            permission_boundary.allowed_permissions
-            or permission_boundary.denied_permissions
-        ):
-            final_permissions, more_ineffective_permissions = apply_permission_boundary(
-                final_permissions, permission_boundary
+        for boundary in (permission_boundary, self.scp_policy):
+            if boundary.allowed_permissions or boundary.denied_permissions:
+                (
+                    final_permissions,
+                    more_ineffective_permissions,
+                ) = apply_permission_boundary(final_permissions, boundary)
+                ineffective_permissions.update(more_ineffective_permissions)
+
+            denied_permissions = deep_update(
+                direct_permissions.denied_permissions,
+                boundary.denied_permissions,
             )
-            ineffective_permissions.update(more_ineffective_permissions)
-
-        denied_permissions = deep_update(
-            direct_permissions.denied_permissions,
-            permission_boundary.denied_permissions,
-        )
 
         return PermissionsContainer(
             allowed_permissions=final_permissions,
             denied_permissions=denied_permissions,
             ineffective_permissions=ineffective_permissions,
         )
```

### Comparing `iam_ape-1.0.5/iam_ape/expand_policy.py` & `iam_ape-1.1.0/iam_ape/expand_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import tarfile
 from collections import defaultdict
 from fnmatch import fnmatch
 from typing import Any, Dict, FrozenSet, List, Literal, Optional, Set, Tuple
 
+from requests.structures import CaseInsensitiveDict
+
 from iam_ape.consts import PolicyElement, actions_json_location
-from iam_ape.helper_functions import as_list, normalize_policy
-from iam_ape.helper_types import (
+from iam_ape.helper_classes import (
     Action,
-    AwsPolicyStatementType,
-    AwsPolicyType,
     HashableDict,
+    HashableList,
     PermissionsContainer,
     PolicyWithSource,
 )
+from iam_ape.helper_functions import as_list, normalize_policy
+from iam_ape.helper_types import AwsPolicyStatementType, AwsPolicyType
 
 logger = logging.getLogger("policy expander")
 
 
 def _append_action(
     res: Dict[str, Set[Action]],
     action: str,
@@ -71,27 +73,35 @@
                     source=source,
                 )
             )
 
 
 class PolicyExpander:
     def __init__(self) -> None:
-        self.all_iam_actions: Dict[str, Any] = self._init_iam_actions()
+        self.all_iam_actions: CaseInsensitiveDict = self._init_iam_actions()
         self._all_service_wildcards: List[str] = [
             f"{k}:*" for k, v in self.all_iam_actions.items() if len(v) > 0
         ]
 
     @staticmethod
-    def _init_iam_actions() -> Dict[str, Dict[str, Dict[str, str]]]:
+    def _init_iam_actions() -> CaseInsensitiveDict:
+        res: CaseInsensitiveDict = CaseInsensitiveDict()
         try:
             with tarfile.open(actions_json_location) as f:
-                return json.load(f.extractfile("actions.json"))  # type: ignore
+                data = json.load(f.extractfile("actions.json"))  # type: ignore
+                for k, v in data.items():
+                    res[k] = CaseInsensitiveDict(v)
         except Exception as e:
             logger.exception(f"Failed to load AWS IAM Actions due to {e}")
-        return {}
+        return res
+
+    def normalize_action(self, action: str) -> str:
+        service, permission = action.split(":", maxsplit=1)
+        permission = self.all_iam_actions[service]._store[permission.lower()][0]
+        return f"{service}:{permission}"
 
     def expand_policies(self, policies: List[PolicyWithSource]) -> PermissionsContainer:
         allow_actions_dict: Dict[str, Set[Action]] = defaultdict(set)
         deny_actions_dict: Dict[str, Set[Action]] = defaultdict(set)
 
         all_actions: Dict[Literal["Allow", "Deny"], Dict[str, Set[Action]]] = {
             PolicyElement.ALLOW: allow_actions_dict,
@@ -142,37 +152,37 @@
                         action=f"{service}:{action}",
                         resources=as_list(iam_action.resource),
                         not_resources=as_list(iam_action.not_resource),
                         condition=iam_action.condition,
                         source=iam_action.source,
                     )
         elif PolicyElement.WILDCARD in iam_action.action:  # {"Action": ["iam:*"]}
-            assert (
-                iam_action.action.count(":") == 1
-            ), f"Got an invalid wildcard action: {iam_action.action}"
-            service, wildcard_action = iam_action.action.split(":")
+            service, wildcard_action = iam_action.action.split(":", maxsplit=1)
             for action in self.all_iam_actions[service].keys():
-                if fnmatch(action, wildcard_action):
+                if fnmatch(action.lower(), wildcard_action.lower()):
                     _append_action(
                         res=res,
                         action=f"{service}:{action}",
                         resources=as_list(iam_action.resource),
                         not_resources=as_list(iam_action.not_resource),
                         condition=iam_action.condition,
                         source=iam_action.source,
                     )
         else:  # {"Action": ["sts:GetCallerIdentity"]}
-            _append_action(
-                res=res,
-                action=iam_action.action,
-                resources=as_list(iam_action.resource),
-                not_resources=as_list(iam_action.not_resource),
-                condition=iam_action.condition,
-                source=iam_action.source,
-            )
+            try:
+                _append_action(
+                    res=res,
+                    action=self.normalize_action(iam_action.action),
+                    resources=as_list(iam_action.resource),
+                    not_resources=as_list(iam_action.not_resource),
+                    condition=iam_action.condition,
+                    source=iam_action.source,
+                )
+            except KeyError:  # not a valid action
+                logger.debug(f"Got an invalid action: {iam_action.action}")
 
         return res
 
     def expand_not_action(
         self, statement: AwsPolicyStatementType, sid: str
     ) -> Dict[str, Set[Action]]:
         res: Dict[str, Set[Action]] = defaultdict(set)
@@ -182,41 +192,45 @@
         ):  # {"NotAction": ["*"]}
             # This is here as a safeguard. No sane person should write a policy like this. It has no effect.
             pass
         else:  # {"NotAction": ["ec2:*", "iam:Get*", "sts:GetCallerIdentity"]}
             for iam_service, action_dicts in self.all_iam_actions.items():
                 for action in action_dicts.keys():
                     curr_action = f"{iam_service}:{action}"
+                    curr_action_lower = curr_action.lower()
                     if any(
-                        [fnmatch(curr_action, not_action) for not_action in notactions]
+                        [
+                            fnmatch(curr_action_lower, not_action.lower())
+                            for not_action in notactions
+                        ]
                     ):
                         continue
                     _append_action(
                         res=res,
                         action=curr_action,
                         resources=statement.get(PolicyElement.RESOURCE),
                         not_resources=statement.get(PolicyElement.NOTRESOURCE),
                         condition=statement.get(PolicyElement.CONDITION),
                         source=sid,
                     )
 
         return res
 
     def get_action_access_level(self, action: str) -> str:
-        service, action_key = action.split(":")
+        service, action_key = action.split(":", maxsplit=1)
         return self.all_iam_actions[service][action_key]["access"]
 
     def deflate_policy_statements(
         self,
         policy_statements: List[AwsPolicyStatementType],
     ) -> List[AwsPolicyStatementType]:
         for statement in policy_statements:
             action_dict = defaultdict(list)
             for action in statement.get(PolicyElement.ACTION) or []:
-                service, action_key = action.split(":")
+                service, action_key = action.split(":", maxsplit=1)
                 action_dict[service].append(action_key)
             for service, action_keys in action_dict.items():
                 try:
                     if all(
                         [
                             action in action_keys
                             for action in self.all_iam_actions[service]
@@ -239,22 +253,24 @@
 
     def shrink_policy(self, allow_actions: Dict[str, Set[Action]]) -> AwsPolicyType:
         policy_res: AwsPolicyType = {"Statement": []}
         squashed_policies: Set[Action] = set()
         for allow_action_set in allow_actions.values():
             squashed_policies.update(allow_action_set)
 
+        # Arrange by Resource/NotResource
         by_resource_notresource: Dict[
             Tuple[Optional[str], Optional[str]], Dict[Optional[HashableDict], Set[str]]
         ] = defaultdict(lambda: defaultdict(set))
         for action_tuple in squashed_policies:
             by_resource_notresource[(action_tuple.resource, action_tuple.not_resource)][
                 HashableDict.recursively(action_tuple.condition)
             ].add(action_tuple.action)
 
+        # Arrange by Action/Condition/NotResource
         by_action_condition_notresource: Dict[
             Tuple[FrozenSet[str], Optional[HashableDict], Optional[str]], Set[str]
         ] = defaultdict(set)
         for resource_notresource, condition_actions in by_resource_notresource.items():
             resource, notresource = resource_notresource
             for condition, actions_set in condition_actions.items():
                 key = frozenset(actions_set), condition, notresource
@@ -277,9 +293,48 @@
                 statement[PolicyElement.RESOURCE] = sorted([r for r in resources])
             if notresource:
                 statement[PolicyElement.NOTRESOURCE] = as_list(notresource)
             if condition:
                 statement[PolicyElement.CONDITION] = condition
             statements.append(statement)
 
-        policy_res["Statement"] = self.deflate_policy_statements(statements)
+        deflated_statements = self.deflate_policy_statements(statements)
+
+        final_statements: Dict[int, AwsPolicyStatementType] = {}
+        for statement in deflated_statements:
+            statement_key = hash(
+                (
+                    HashableList(statement[PolicyElement.ACTION] or []),
+                    HashableDict.recursively(statement.get(PolicyElement.CONDITION)),
+                )
+            )
+            if statement_key in final_statements.keys():
+                rsrc = (
+                    final_statements[statement_key].get(PolicyElement.RESOURCE) or []
+                ) + (statement.get(PolicyElement.RESOURCE) or [])
+                if rsrc:
+                    final_statements[statement_key][PolicyElement.RESOURCE] = list(
+                        set(rsrc)
+                    )
+                not_rsrc = (
+                    final_statements[statement_key].get(PolicyElement.NOTRESOURCE) or []
+                ) + (statement.get(PolicyElement.NOTRESOURCE) or [])
+                if not_rsrc:
+                    final_statements[statement_key][PolicyElement.NOTRESOURCE] = list(
+                        set(not_rsrc)
+                    )
+            else:
+                final_statements[statement_key] = statement
+
+        admin_statement: AwsPolicyStatementType = {
+            PolicyElement.EFFECT: PolicyElement.ALLOW,
+            PolicyElement.ACTION: [PolicyElement.WILDCARD],
+            PolicyElement.RESOURCE: [PolicyElement.WILDCARD],
+        }
+        if any(
+            [statement == admin_statement for statement in final_statements.values()]
+        ):
+            policy_res["Statement"] = [admin_statement]
+        else:
+            policy_res["Statement"] = list(final_statements.values())
+
         return normalize_policy(policy_res)
```

### Comparing `iam_ape-1.0.5/iam_ape/helper_functions.py` & `iam_ape-1.1.0/iam_ape/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from copy import deepcopy
 from typing import Any, Dict, List, Literal, Optional, Set, TypeVar
 
 from iam_ape.consts import CONDITIONS_NEGATIONS
-from iam_ape.helper_types import AwsPolicyType, HashableDict, HashableList
+from iam_ape.helper_classes import HashableDict, HashableList
+from iam_ape.helper_types import AwsPolicyType
 
 logger = logging.getLogger(__name__)
 
 KeyType = TypeVar("KeyType")
 
 
 def as_list(element: Optional[Any]) -> List[Any]:
```

### Comparing `iam_ape-1.0.5/iam_ape/helper_types.py` & `iam_ape-1.1.0/iam_ape/helper_classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,18 @@
 from collections import namedtuple
 from dataclasses import dataclass, field
-from enum import Enum
-from typing import Any, Dict, List, Optional, Set, TypedDict
+from typing import Any, Dict, List, Optional, Set
 
 from iam_ape.consts import PolicyElement
-
-
-class FinalReportT(TypedDict):
-    allowed_permissions: Dict[str, Any]
-    denied_permissions: Dict[str, Any]
-    ineffective_permissions: Dict[str, Any]
-
-
-class AwsPolicyStatementType(TypedDict, total=False):
-    Effect: str
-    Sid: Optional[str]
-    Action: Optional[List[str]]
-    NotAction: Optional[List[str]]
-    Resource: Optional[List[str]]
-    NotResource: Optional[List[str]]
-    Principal: Optional[Dict[str, Any]]
-    NotPrincipal: Optional[Dict[str, Any]]
-    Condition: Optional[Dict[str, Any]]
-
-
-class AwsPolicyType(TypedDict, total=False):
-    Version: Optional[str]
-    Id: Optional[str]
-    Statement: List[AwsPolicyStatementType]
-
-
-class EntityType(Enum):
-    user: str = "User"
-    group: str = "Group"
-    role: str = "Role"
+from iam_ape.helper_types import (
+    ActionDict,
+    AwsPolicyType,
+    IneffectiveActionDict,
+    PermissionsContainerDict,
+)
 
 
 class HashableList(List[Any]):
     def flatten(self, list_obj: List[Any]) -> List[Any]:
         all_items = []
         for item in list_obj:
             if hasattr(item, "__hash__"):
@@ -64,26 +39,14 @@
             if isinstance(value, dict):
                 dict_obj[key] = HashableDict.recursively(value)
             elif isinstance(value, list):
                 dict_obj[key] = HashableList(value)
         return HashableDict(dict_obj)
 
 
-class ActionDict(TypedDict):
-    Action: str
-    Resource: Optional[str]
-    NotResource: Optional[str]
-    Condition: Optional[Dict[str, Any]]
-    Source: str
-
-
-class IneffectiveActionDict(ActionDict):
-    DeniedBy: str
-
-
 @dataclass(unsafe_hash=True)
 class Action:
     action: str
     resource: Optional[str]
     not_resource: Optional[str]
     condition: Optional[Dict[str, Any]]
     source: str
@@ -117,20 +80,14 @@
 
 
 class PolicyWithSource(namedtuple("PolicyWithSource", ["source", "policy"])):
     source: str
     policy: AwsPolicyType
 
 
-class PermissionsContainerDict(TypedDict):
-    allowed_permissions: List[ActionDict]
-    denied_permissions: List[ActionDict]
-    ineffective_permissions: List[ActionDict]
-
-
 @dataclass
 class PermissionsContainer:
     allowed_permissions: Dict[str, Set[Action]] = field(default_factory=dict)
     denied_permissions: Dict[str, Set[Action]] = field(default_factory=dict)
     ineffective_permissions: Set[IneffectiveAction] = field(default_factory=set)
 
     def to_dict(self) -> PermissionsContainerDict:
```

### Comparing `iam_ape-1.0.5/iam_ape/main.py` & `iam_ape-1.1.0/iam_ape/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import argparse
 import json
 import logging
 import os
 import re
 import sys
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-import boto3  # type: ignore
-from botocore.exceptions import ProfileNotFound  # type: ignore
+import boto3
+from botocore.exceptions import ClientError, ProfileNotFound
 
 from iam_ape.aws_iam_actions.scrape_iam_actions import scrape_iam_actions
 from iam_ape.evaluator import AuthorizationDetails, EffectivePolicyEvaluator
+from iam_ape.helper_classes import PolicyWithSource
 from iam_ape.helper_functions import deep_update
 from iam_ape.helper_types import AwsPolicyType, EntityType, FinalReportT
 
 logger = logging.getLogger("IAM-APE")
-entity_regex_string = r"arn:aws(-cn|-us-gov)?:iam::\d{12}:(user|group|role)/[\w-]+"
+logging.getLogger("botocore").setLevel(logging.WARNING)  # suppress botocore logs
+entity_regex_string = r"arn:aws(-cn|-us-gov)?:iam::(?P<account>\d{12}):(?P<entity_type>user|group|role)/[\w-]+"
 entity_regex = re.compile(entity_regex_string)
 
 banner = """
   __   __   _  _        __   ____  ____ 
  (  ) / _\ ( \/ ) ___  / _\ (  _ \(  __)
   )( /    \/ \/ \(___)/    \ ) __/ ) _) 
  (__)\_/\_/\_)(_/     \_/\_/(__)  (____)
@@ -62,28 +64,32 @@
     format = LogFormatter()
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(format)
     logging.root.addHandler(handler)
     logging.root.setLevel(logging.INFO)
 
 
-def validate_arn(arn: str) -> EntityType:
+def validate_arn(arn: str) -> Tuple[EntityType, str]:
+    regex_match = entity_regex.fullmatch(arn)
     try:
-        assert entity_regex.match(arn)
+        assert regex_match
     except AssertionError:
         raise ValueError(
             f'Invalid ARN format: "{arn}". Expected: "{entity_regex_string}"'
         )
 
-    if ":user/" in arn:
-        return EntityType.user
-    elif ":group/" in arn:
-        return EntityType.group
+    entity_type = regex_match.group("entity_type")
+    account_id = regex_match.group("account")
+
+    if entity_type == "user":
+        return EntityType.user, account_id
+    elif entity_type == "group":
+        return EntityType.group, account_id
     else:
-        return EntityType.role
+        return EntityType.role, account_id
 
 
 def load_auth_details_from_json(inp: str) -> AuthorizationDetails:
     with open(inp, "r") as f:
         auth_report = json.load(f)
     return AuthorizationDetails(auth_report)
 
@@ -99,14 +105,89 @@
     paginator = iam_client.get_paginator("get_account_authorization_details")
     for page in paginator.paginate():
         auth_report = deep_update(auth_report, page)
     a = AuthorizationDetails(auth_report)
     return a
 
 
+def load_scp_from_json(inp: str) -> PolicyWithSource:
+    with open(inp) as f:
+        policy_description = json.load(f)
+        return PolicyWithSource(
+            policy_description["Policy"]["PolicySummary"]["Arn"],
+            json.loads(policy_description["Policy"]["Content"]),
+        )
+
+
+def load_scp_from_aws(
+    account_id: str, profile: Optional[str] = None
+) -> List[PolicyWithSource]:
+    logger.info("Attempting to fetch service control policies from AWS...")
+    profile = profile or os.environ.get("AWS_PROFILE")
+    policies = []
+
+    if not profile:
+        raise ValueError("No AWS profile found")
+
+    boto3.setup_default_session(profile_name=profile)
+    org_client = boto3.client("organizations")
+    paginator = org_client.get_paginator("list_policies_for_target")
+
+    for page in paginator.paginate(
+        TargetId=account_id, Filter="SERVICE_CONTROL_POLICY"
+    ):
+        for policy in page["Policies"]:
+            policy_description = org_client.describe_policy(PolicyId=policy["Id"])
+            policies.append(
+                PolicyWithSource(
+                    policy_description["Policy"]["PolicySummary"]["Arn"],
+                    json.loads(policy_description["Policy"]["Content"]),
+                )
+            )
+
+    return policies
+
+
+def get_auth_details(input_path: str, profile: str) -> AuthorizationDetails:
+    if input_path:
+        auth_details = load_auth_details_from_json(input_path)
+    else:
+        auth_details = load_auth_details_from_aws(profile)
+    return auth_details
+
+
+def get_scp_policies(
+    scp_policy_arg: Optional[str], profile: Optional[str], entity_account: str
+) -> List[PolicyWithSource]:
+    policy_jsons = []
+    if scp_policy_arg:
+        scp_policy_paths = (
+            scp_policy_arg.split(",")
+            if "," in scp_policy_arg
+            else scp_policy_arg.split(" ")
+        )
+        for policy_path in scp_policy_paths:
+            policy_jsons.append(load_scp_from_json(inp=policy_path))
+
+    elif profile:
+        try:
+            policy_jsons.extend(
+                load_scp_from_aws(profile=profile, account_id=entity_account)
+            )
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "AWSOrganizationsNotInUseException":
+                logger.debug("SCP Policies not in use for this account")
+            elif e.response["Error"]["Code"] == "AccessDeniedException":
+                logger.info(
+                    "Could not fetch SCP policies due to insufficient permissions"
+                )
+
+    return policy_jsons
+
+
 def build_arg_parser() -> argparse.ArgumentParser:
     arg_parser = argparse.ArgumentParser()
     basic_usage = arg_parser.add_argument_group()
     adv_usage = arg_parser.add_argument_group()
     misc_usage = arg_parser.add_argument_group()
 
     basic_usage.add_argument(
@@ -117,14 +198,20 @@
     adv_usage.add_argument(
         "-i",
         "--input",
         help='Path to report generated by "aws iam get-account-authorization-details"',
         required=False,
     )
     adv_usage.add_argument(
+        "-s",
+        "--scp-policy",
+        help='Path to report(s) generated by "aws organizations describe-policy --policy-id <SCP_Policy_ID>"',
+        required=False,
+    )
+    adv_usage.add_argument(
         "-o",
         "--output",
         help="File path to write the output to (default: stdout)",
         default="stdout",
     )
     adv_usage.add_argument(
         "-f",
@@ -171,33 +258,35 @@
 
     if arguments.update:
         scrape_iam_actions()
         if not arguments.arn:
             return 0
 
     try:
-        entity_type = validate_arn(arguments.arn)
+        entity_type, entity_account = validate_arn(arguments.arn)
     except ValueError as e:
         logger.error(e)
         return -1
 
-    if arguments.input:
-        auth_details = load_auth_details_from_json(arguments.input)
-    else:
-        try:
-            auth_details = load_auth_details_from_aws(arguments.profile)
-        except ValueError as e:
-            logger.error(e)
-            return -1
-        except ProfileNotFound as e:
-            logger.error(e)
-            return -1
+    try:
+        auth_details = get_auth_details(arguments.input, arguments.profile)
+    except (ValueError, ProfileNotFound) as e:
+        logger.error(e)
+        return -1
+
+    scp_policies = None
+    if arguments.input is None or arguments.scp_policy is not None:
+        scp_policies = get_scp_policies(
+            arguments.scp_policy, arguments.profile, entity_account
+        )
 
     logger.info("Evaluating effective permissions")
-    calculator = EffectivePolicyEvaluator(auth_details)
+    calculator = EffectivePolicyEvaluator(
+        authorization_details=auth_details, scp_policies=scp_policies
+    )
 
     try:
         res = calculator.evaluate(arn=arguments.arn, entity_type=entity_type)
     except ValueError as e:
         logger.error(e)
         return -1
 
@@ -208,14 +297,17 @@
         out = calculator.create_json_report(res)
 
     if arguments.output == "stdout":
         logger.info(f"Effective permissions policy for {arguments.arn}\n")
         logger.info(json.dumps(out, indent=2))
     else:
         with open(arguments.output, "w") as f:
-            json.dump(out, f)
+            json.dump(out, f, indent=2)
+        logger.info(
+            f"Wrote effective permissions for {arguments.arn} to {arguments.output}"
+        )
 
     return 0
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `iam_ape-1.0.5/pyproject.toml` & `iam_ape-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-ape"
-version = "1.0.5"
+version = "1.1.0"
 description = "IAM AWS Permissions Evaluator"
 authors = ["Tohar Braun, Orca Security <tohar@orca.security>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 repository = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 keywords = ["aws", "iam"]
@@ -24,17 +24,18 @@
 beautifulsoup4 = "^4.8.2"
 tqdm = "^4.63.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 pytest = "^7.2.1"
 types-requests = "^2.28.11.12"
-mypy = "^1.1.1"
+mypy = "^1.0.0"
 flake8 = "*"
 isort = "*"
+boto3-stubs = {extras = ["essential"], version = "^1.26.115"}
 
 [tool.setuptools.package-data]
 iam-ape = ["iam_ape/aws_iam_actions/*.tar.gz", "iam_ape/py.typed"]
 
 [tool.poetry.scripts]
 iam-ape = "iam_ape.main:main"
```

### Comparing `iam_ape-1.0.5/PKG-INFO` & `iam_ape-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-ape
-Version: 1.0.5
+Version: 1.1.0
 Summary: IAM AWS Permissions Evaluator
 Home-page: https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 License: GPL-3.0-or-later
 Keywords: aws,iam
 Author: Tohar Braun, Orca Security
 Author-email: tohar@orca.security
 Requires-Python: >=3.8,<4.0
@@ -75,9 +75,8 @@
 }
 ```
 This statement, having both `Resource` and `NotResource` together, is not supported by AWS but makes more sense when trying to understand what the effective permissions of a user are.
 
 ## Roadmap ##
 - [ ] Add an option to supply a resource policy and evaluate whether the entity has access to that resource 
 - [ ] Support additional permissions inherited by Role assumption
-- [ ] Support SCP Policies
-
+- [x] Support SCP Policies
```

