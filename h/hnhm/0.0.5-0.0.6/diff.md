# Comparing `tmp/hnhm-0.0.5.tar.gz` & `tmp/hnhm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnhm-0.0.5.tar", max compression
+gzip compressed data, was "hnhm-0.0.6.tar", max compression
```

## Comparing `hnhm-0.0.5.tar` & `hnhm-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      707 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/__init__.py
--rw-r--r--   0        0        0     5725 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/cli.py
--rw-r--r--   0        0        0      600 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/__init__.py
--rw-r--r--   0        0        0     1084 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/attribute.py
--rw-r--r--   0        0        0      554 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/entity.py
--rw-r--r--   0        0        0       80 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/error.py
--rw-r--r--   0        0        0      311 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/group.py
--rw-r--r--   0        0        0      543 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/layout.py
--rw-r--r--   0        0        0      654 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/link.py
--rw-r--r--   0        0        0     2493 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/mutations.py
--rw-r--r--   0        0        0       80 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/priority.py
--rw-r--r--   0        0        0      511 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/sql.py
--rw-r--r--   0        0        0      621 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/storage.py
--rw-r--r--   0        0        0     1545 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/tasks.py
--rw-r--r--   0        0        0      564 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/file_storage.py
--rw-r--r--   0        0        0     7561 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/flow.py
--rw-r--r--   0        0        0    11451 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm.py
--rw-r--r--   0        0        0      902 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_attribute.py
--rw-r--r--   0        0        0     3865 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_entity.py
--rw-r--r--   0        0        0     2547 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_link.py
--rw-r--r--   0        0        0     1297 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_registry.py
--rw-r--r--   0        0        0        0 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/__init__.py
--rw-r--r--   0        0        0    13167 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql.py
--rw-r--r--   0        0        0      459 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/__init__.py
--rw-r--r--   0        0        0      528 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_attribute.py
--rw-r--r--   0        0        0      549 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_group.py
--rw-r--r--   0        0        0      344 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_hub.py
--rw-r--r--   0        0        0      576 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_link.py
--rw-r--r--   0        0        0      228 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_stage.py
--rw-r--r--   0        0        0      507 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_hub.py
--rw-r--r--   0        0        0      983 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_ignore.py
--rw-r--r--   0        0        0     4563 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_new.py
--rw-r--r--   0        0        0     2139 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_update.py
--rw-r--r--   0        0        0      707 2023-04-22 10:35:50.042288 hnhm-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/__init__.py
+-rw-r--r--   0        0        0     1481 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/cli.py
+-rw-r--r--   0        0        0      602 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/attribute.py
+-rw-r--r--   0        0        0      554 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/entity.py
+-rw-r--r--   0        0        0       80 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/error.py
+-rw-r--r--   0        0        0      311 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/group.py
+-rw-r--r--   0        0        0      543 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/layout.py
+-rw-r--r--   0        0        0      654 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/link.py
+-rw-r--r--   0        0        0     2461 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/migrations.py
+-rw-r--r--   0        0        0       80 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/priority.py
+-rw-r--r--   0        0        0      517 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/sql.py
+-rw-r--r--   0        0        0     2725 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/storage.py
+-rw-r--r--   0        0        0     1545 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/tasks.py
+-rw-r--r--   0        0        0      564 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/file_storage.py
+-rw-r--r--   0        0        0     8343 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/flow.py
+-rw-r--r--   0        0        0    10802 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/hnhm.py
+-rw-r--r--   0        0        0      902 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/hnhm_attribute.py
+-rw-r--r--   0        0        0     3865 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_entity.py
+-rw-r--r--   0        0        0     2465 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_link.py
+-rw-r--r--   0        0        0     1297 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_registry.py
+-rw-r--r--   0        0        0     6902 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/plan_printer.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/__init__.py
+-rw-r--r--   0        0        0    13179 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql.py
+-rw-r--r--   0        0        0      459 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/__init__.py
+-rw-r--r--   0        0        0      528 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_attribute.py
+-rw-r--r--   0        0        0      549 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_group.py
+-rw-r--r--   0        0        0      344 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_hub.py
+-rw-r--r--   0        0        0      576 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_link.py
+-rw-r--r--   0        0        0      228 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_stage.py
+-rw-r--r--   0        0        0      507 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_hub.py
+-rw-r--r--   0        0        0      983 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_ignore.py
+-rw-r--r--   0        0        0     4563 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_new.py
+-rw-r--r--   0        0        0     2139 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_update.py
+-rw-r--r--   0        0        0      707 2023-04-27 17:50:39.726219 hnhm-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.6/PKG-INFO
```

### Comparing `hnhm-0.0.5/hnhm/__init__.py` & `hnhm-0.0.6/hnhm/__init__.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/core/__init__.py` & `hnhm-0.0.6/hnhm/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from .error import HnhmError
 from .sql import Sql, FakeSql
 from .link import Link, LinkElement
 from .layout import Layout, LayoutType
 from .attribute import Type, Attribute, ChangeType
 from .storage import Storage, InMemStorage, HnhmStorageData
 from .tasks import Task, LoadHub, LoadLink, LoadGroup, LoadAttribute
-from .mutations import (
-    Mutation,
+from .migrations import (
+    Migration,
     CreateLink,
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
```

### Comparing `hnhm-0.0.5/hnhm/core/attribute.py` & `hnhm-0.0.6/hnhm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/core/entity.py` & `hnhm-0.0.6/hnhm/core/entity.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/core/layout.py` & `hnhm-0.0.6/hnhm/core/layout.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/core/link.py` & `hnhm-0.0.6/hnhm/core/link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/core/mutations.py` & `hnhm-0.0.6/hnhm/core/migrations.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,73 +3,71 @@
 from .link import Link
 from .group import Group
 from .entity import Entity
 from .priority import Priority
 from .attribute import Attribute
 
 
-class Mutation(pydantic.BaseModel):
-    """Mutation represents DWH change."""
-
+class Migration(pydantic.BaseModel):
     priority: Priority
 
 
-class CreateEntity(Mutation):
+class CreateEntity(Migration):
     priority = Priority.FIRST
     entity: Entity
 
     def __str__(self):
         return f"<CreateEntity '{self.entity.name}'>"
 
 
-class RemoveEntity(Mutation):
+class RemoveEntity(Migration):
     priority = Priority.SECOND
     entity: Entity
 
     def __str__(self):
         return f"<RemoveEntity '{self.entity.name}'>"
 
 
-class CreateAttribute(Mutation):
+class CreateAttribute(Migration):
     priority = Priority.SECOND
     entity: Entity
     attribute: Attribute
 
     def __str__(self):
         return f"<CreateAttribute '{self.attribute.name}' entity='{self.entity.name}'>"
 
 
-class RemoveAttribute(Mutation):
+class RemoveAttribute(Migration):
     priority = Priority.FIRST
     entity: Entity
     attribute: Attribute
 
     def __str__(self):
         return f"<RemoveAttribute '{self.attribute.name}' entity='{self.entity.name}'>"
 
 
-class CreateGroup(Mutation):
+class CreateGroup(Migration):
     priority = Priority.SECOND
     entity: Entity
     group: Group
 
     def __str__(self):
         return f"<CreateGroup '{self.group.name}' entity='{self.entity.name}'>"
 
 
-class RemoveGroup(Mutation):
+class RemoveGroup(Migration):
     priority = Priority.FIRST
     entity: Entity
     group: Group
 
     def __str__(self):
         return f"<RemoveGroup '{self.group.name}' entity='{self.entity.name}'>"
 
 
-class AddGroupAttribute(Mutation):
+class AddGroupAttribute(Migration):
     """Add an Attribute to an existing Group."""
 
     priority = Priority.SECOND
     entity: Entity
     group: Group
     attribute: Attribute
 
@@ -77,15 +75,15 @@
         return (
             f"<AddGroupAttribute '{self.group.name}'"
             f" entity='{self.entity.name}'"
             f" attribute='{self.attribute.name}'>"
         )
 
 
-class RemoveGroupAttribute(Mutation):
+class RemoveGroupAttribute(Migration):
     """Remove an Attribute from an existing Group."""
 
     priority = Priority.SECOND
     entity: Entity
     group: Group
     attribute: Attribute
 
@@ -93,21 +91,21 @@
         return (
             f"<RemoveGroupAttribute '{self.group.name}'"
             f" entity='{self.entity.name}'"
             f" attribute='{self.attribute.name}'>"
         )
 
 
-class CreateLink(Mutation):
+class CreateLink(Migration):
     priority = Priority.SECOND
     link: Link
 
     def __str__(self):
         return f"<CreateLink '{self.link.name}'>"
 
 
-class RemoveLink(Mutation):
+class RemoveLink(Migration):
     priority = Priority.FIRST
     link: Link
 
     def __str__(self):
         return f"<RemoveLink '{self.link.name}'>"
```

### Comparing `hnhm-0.0.5/hnhm/core/tasks.py` & `hnhm-0.0.6/hnhm/core/tasks.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/file_storage.py` & `hnhm-0.0.6/hnhm/file_storage.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/flow.py` & `hnhm-0.0.6/hnhm/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,18 +134,33 @@
                     if attribute_target in target_entity.keys:
                         keys_mapping[attribute_target] = attribute_source
                     elif attribute_target.group:
                         group_name = attribute_target.group
                         if group_name not in groups_mapping:
                             groups_mapping[group_name] = {}
                         groups_mapping[group_name][attribute_target] = attribute_source
-                        # todo: check all attributes for group were mapped
                     else:
                         attributes_mapping[attribute_target] = attribute_source
 
+                # Check all attributes for a Group were mapped
+                for group_name, group in target_entity.groups.items():
+                    group_mapping = groups_mapping.get(group_name)
+                    if not group_mapping:
+                        continue
+
+                    for attribute in group.attributes.values():
+                        if attribute not in group_mapping:
+                            attribute_full_name = (
+                                f"{target_entity.name}.{group_name}.{attribute.name}"
+                            )
+                            raise HnhmError(
+                                f"Mapping not found for the attribute '{attribute_full_name}'."
+                                f" Please, provide all mappings for the group: '{target_entity.name}.{group_name}'."
+                            )
+
                 missing_keys = set(target_entity.keys) - set(keys_mapping.keys())
                 if missing_keys:
                     missing_keys_names = [key.name for key in missing_keys]
                     raise HnhmError(
                         f"Found missing mappings for entity='{target_entity.name}' keys."
                         f" Missing mappings for keys: {missing_keys_names}."
                     )
```

### Comparing `hnhm-0.0.5/hnhm/hnhm.py` & `hnhm-0.0.6/hnhm/hnhm.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import pydantic
 
 from hnhm.core import (
     Sql,
     Entity,
     Storage,
-    Mutation,
     HnhmError,
+    Migration,
     CreateLink,
     LayoutType,
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
@@ -29,33 +29,33 @@
     CREATE = "CREATE"
     REMOVE = "REMOVE"
     UPDATE = "UPDATE"
 
 
 class PlanCollection(pydantic.BaseModel):
     type: PlanType
-    mutations: list[Mutation]
+    migrations: list[Migration]
 
 
 class Plan(pydantic.BaseModel):
-    entities_mutations: dict[str, PlanCollection]
-    links_mutations: dict[str, PlanCollection]
+    entities_migrations: dict[str, PlanCollection]
+    links_migrations: dict[str, PlanCollection]
 
     def is_empty(self):
-        return not self.entities_mutations and not self.links_mutations
+        return not self.entities_migrations and not self.links_migrations
 
     @property
-    def mutations_all(self):
-        mutations: list[Mutation] = []
-        for collection in self.entities_mutations.values():
-            mutations.extend(collection.mutations)
-        for collection in self.links_mutations.values():
-            mutations.extend(collection.mutations)
-        mutations = sorted(mutations, key=lambda m: m.priority)
-        return mutations
+    def migrations_all(self):
+        migrations: list[Migration] = []
+        for collection in self.entities_migrations.values():
+            migrations.extend(collection.migrations)
+        for collection in self.links_migrations.values():
+            migrations.extend(collection.migrations)
+        migrations = sorted(migrations, key=lambda m: m.priority)
+        return migrations
 
 
 class HnHm:
     def __init__(self, *, sql: Sql, storage: Storage):
         self.sql = sql
         self.storage = storage
         self.data = self.storage.load()
@@ -78,140 +78,140 @@
             core_entities[entity_core.name] = entity_core
 
         core_links = {}
         for link in links or []:
             link_core = link.to_core()
             core_links[link_core.name] = link_core
 
-        plan = Plan(entities_mutations={}, links_mutations={})
+        plan = Plan(entities_migrations={}, links_migrations={})
 
         # Entity: create if not exists
         for entity in core_entities.values():
             if entity.name in self.data.entities:
                 continue
 
             # Create Entity
-            mutations = [CreateEntity(entity=entity)]
+            migrations = [CreateEntity(entity=entity)]
 
             if entity.layout.type == LayoutType.HNHM:
                 # Create Attribute
                 for attribute in entity.attributes.values():
-                    mutations.append(CreateAttribute(entity=entity, attribute=attribute))
+                    migrations.append(CreateAttribute(entity=entity, attribute=attribute))
                 # Create Group
                 for group in entity.groups.values():
-                    mutations.append(CreateGroup(entity=entity, group=group))
+                    migrations.append(CreateGroup(entity=entity, group=group))
 
-            plan.entities_mutations[entity.name] = PlanCollection(
+            plan.entities_migrations[entity.name] = PlanCollection(
                 type=PlanType.CREATE,
-                mutations=mutations,
+                migrations=migrations,
             )
 
         # Entity: create/remove/update Attribute/Group
         for entity in core_entities.values():
             if entity.name not in self.data.entities:
                 continue
 
             attributes_state = self.data.entities[entity.name].attributes
             groups_state = self.data.entities[entity.name].groups
 
-            mutations = []
+            migrations = []
             # Create Attribute
             for attribute_name, attribute in entity.attributes.items():
                 if attribute_name not in attributes_state:
-                    mutations.append(CreateAttribute(entity=entity, attribute=attribute))
+                    migrations.append(CreateAttribute(entity=entity, attribute=attribute))
 
             # Remove Attribute
             for attribute_name, attribute in attributes_state.items():
                 if attribute_name not in entity.attributes:
-                    mutations.append(RemoveAttribute(entity=entity, attribute=attribute))
+                    migrations.append(RemoveAttribute(entity=entity, attribute=attribute))
 
             # Create/Update Group
             for group_name, group in entity.groups.items():
                 # Update
                 if group_name in groups_state:
                     group_state = groups_state[group_name]
                     # Add an Attribute to a Group
                     for attribute_name, attribute in group.attributes.items():
                         if attribute_name not in group_state.attributes:
-                            mutations.append(
+                            migrations.append(
                                 AddGroupAttribute(
                                     entity=entity, group=group, attribute=attribute
                                 )
                             )
                     # Remove an Attribute from a Group
                     for attribute_name, attribute in group_state.attributes.items():
                         if attribute_name not in group.attributes:
-                            mutations.append(
+                            migrations.append(
                                 RemoveGroupAttribute(
                                     entity=entity, group=group, attribute=attribute
                                 )
                             )
                 # Create
                 else:
-                    mutations.append(CreateGroup(entity=entity, group=group))
+                    migrations.append(CreateGroup(entity=entity, group=group))
 
             # Remove Group
             for group_name, group in groups_state.items():
                 if group_name not in entity.groups:
-                    mutations.append(RemoveGroup(entity=entity, group=group))
+                    migrations.append(RemoveGroup(entity=entity, group=group))
 
-            if mutations:
-                plan.entities_mutations[entity.name] = PlanCollection(
+            if migrations:
+                plan.entities_migrations[entity.name] = PlanCollection(
                     type=PlanType.UPDATE,
-                    mutations=mutations,
+                    migrations=migrations,
                 )
 
         # Link: remove
         for link_name, link in self.data.links.items():
             if link_name not in core_links:
-                plan.links_mutations[link_name] = PlanCollection(
+                plan.links_migrations[link_name] = PlanCollection(
                     type=PlanType.REMOVE,
-                    mutations=[RemoveLink(link=link)],
+                    migrations=[RemoveLink(link=link)],
                 )
 
         # Entity: remove
         for entity_name, entity in self.data.entities.items():
             if entity_name not in core_entities:
-                mutations = []
+                migrations = []
 
                 if entity.layout.type == LayoutType.HNHM:
                     attributes_state = self.data.entities[entity_name].attributes
                     groups_state = self.data.entities[entity_name].groups
                     # Remove Attribute
                     for _, attribute_state in attributes_state.items():
-                        mutations.append(
+                        migrations.append(
                             RemoveAttribute(entity=entity, attribute=attribute_state)
                         )
                     # Remove Group
                     for group_name, group in groups_state.items():
-                        mutations.append(RemoveGroup(entity=entity, group=group))
+                        migrations.append(RemoveGroup(entity=entity, group=group))
 
-                mutations.append(RemoveEntity(entity=entity))
-                plan.entities_mutations[entity_name] = PlanCollection(
+                migrations.append(RemoveEntity(entity=entity))
+                plan.entities_migrations[entity_name] = PlanCollection(
                     type=PlanType.REMOVE,
-                    mutations=mutations,
+                    migrations=migrations,
                 )
 
         # Link: create
         for link_name, link in core_links.items():
             if link_name not in self.data.links:
-                plan.links_mutations[link.name] = PlanCollection(
+                plan.links_migrations[link.name] = PlanCollection(
                     type=PlanType.CREATE,
-                    mutations=[CreateLink(link=link)],
+                    migrations=[CreateLink(link=link)],
                 )
 
         return plan
 
     def apply(self, plan: Plan):
-        for mutation in plan.mutations_all:
-            sql = self.sql.generate_sql(mutation)
+        for migration in plan.migrations_all:
+            sql = self.sql.generate_sql(migration)
 
-            match mutation:
+            match migration:
                 case CreateEntity(entity=entity):
-                    assert entity.name not in self.data.entities
+                    self.data.check_entity_not_exists(entity.name)
                     self.sql.execute(sql)
                     if entity.layout.type == LayoutType.HNHM:
                         attributes = {}
                         groups = {}
                     else:
                         attributes = entity.attributes
                         groups = entity.groups
@@ -221,79 +221,65 @@
                         doc=entity.doc,
                         keys=entity.keys,
                         attributes=attributes,
                         groups=groups,
                     )
 
                 case RemoveEntity(entity=entity):
-                    assert entity.name in self.data.entities
+                    self.data.check_entity_exists(entity.name)
                     self.sql.execute(sql)
                     del self.data.entities[entity.name]
 
                 case CreateAttribute(entity=entity, attribute=attribute):
-                    assert entity.name in self.data.entities
-                    assert (
-                        attribute.name not in self.data.entities[entity.name].attributes
-                    )
+                    self.data.check_attribute_not_exists(entity.name, attribute.name)
                     self.sql.execute(sql)
                     self.data.entities[entity.name].attributes[attribute.name] = attribute
 
                 case RemoveAttribute(entity=entity, attribute=attribute):
-                    assert entity.name in self.data.entities
-                    assert attribute.name in self.data.entities[entity.name].attributes
+                    self.data.check_attribute_exists(entity.name, attribute.name)
                     self.sql.execute(sql)
                     del self.data.entities[entity.name].attributes[attribute.name]
 
                 case CreateGroup(entity=entity, group=group):
-                    assert entity.name in self.data.entities
-                    assert group.name not in self.data.entities[entity.name].groups
+                    self.data.check_group_not_exists(entity.name, group.name)
                     self.sql.execute(sql)
                     self.data.entities[entity.name].groups[group.name] = group
 
                 case RemoveGroup(entity=entity, group=group):
-                    assert entity.name in self.data.entities
-                    assert group.name in self.data.entities[entity.name].groups
+                    self.data.check_group_exists(entity.name, group.name)
                     self.sql.execute(sql)
                     del self.data.entities[entity.name].groups[group.name]
 
                 case AddGroupAttribute(entity=entity, group=group, attribute=attribute):
-                    assert entity.name in self.data.entities
-                    assert group.name in self.data.entities[entity.name].groups
-                    assert (
-                        attribute.name
-                        not in self.data.entities[entity.name]
-                        .groups[group.name]
-                        .attributes
+                    self.data.check_group_attribute_not_exists(
+                        entity.name, group.name, attribute.name
                     )
                     self.sql.execute(sql)
                     self.data.entities[entity.name].groups[group.name].attributes[
                         attribute.name
                     ] = attribute
 
                 case RemoveGroupAttribute(
                     entity=entity, group=group, attribute=attribute
                 ):
-                    assert entity.name in self.data.entities
-                    assert group.name in self.data.entities[entity.name].groups
-                    assert (
-                        attribute.name
-                        in self.data.entities[entity.name].groups[group.name].attributes
+                    self.data.check_group_attribute_exists(
+                        entity.name, group.name, attribute.name
                     )
                     self.sql.execute(sql)
                     del (
                         self.data.entities[entity.name]
                         .groups[group.name]
                         .attributes[attribute.name]
                     )
 
                 case CreateLink(link=link):
-                    assert link.name not in self.data.links
+                    self.data.check_link_not_exists(link.name)
                     self.sql.execute(sql)
                     self.data.links[link.name] = link
 
                 case RemoveLink(link=link):
-                    assert link.name in self.data.links
+                    self.data.check_link_exists(link.name)
                     self.sql.execute(sql)
                     del self.data.links[link.name]
 
                 case _:
-                    raise HnhmError(f"Unknown mutation: '{mutation}'")
+                    raise HnhmError(f"Unknown migration: '{migration}'")
```

### Comparing `hnhm-0.0.5/hnhm/hnhm_attribute.py` & `hnhm-0.0.6/hnhm/hnhm_attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/hnhm_entity.py` & `hnhm-0.0.6/hnhm/hnhm_entity.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/hnhm_link.py` & `hnhm-0.0.6/hnhm/hnhm_link.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,31 +31,31 @@
 class HnhmLink(abc.ABC):
     __layout__: Layout
     __keys__: list[HnhmEntity]
 
     def to_core(self) -> Link:
         inspected = dict(inspect.getmembers(self))
 
-        if "__layout__" not in inspected or not inspected["__layout__"]:
+        if not inspected.get("__layout__"):
             raise HnhmError(
                 f"Layout not found for link: '{self}'."
                 " Please, specify Layout via '__layout__' attribute."
             )
         layout: Layout = inspected["__layout__"]
 
         name = layout.name
 
-        if "__doc__" not in inspected or not inspected["__doc__"]:
+        if not inspected.get("__doc__"):
             raise HnhmError(
                 f"Doc not found or empty for link: '{name}'."
                 " Please, write a documentation for your link."
             )
         doc: str = inspected["__doc__"]
 
-        if "__keys__" not in inspected or not inspected["__keys__"]:
+        if not inspected.get("__keys__"):
             raise HnhmError(
                 f"At least one Key is required for link='{name}'."
                 " Please, specify link's keys via the '__keys__' attribute."
             )
         keys = inspected["__keys__"]
         keys = [key.to_core() for key in keys]
```

### Comparing `hnhm-0.0.5/hnhm/hnhm_registry.py` & `hnhm-0.0.6/hnhm/hnhm_registry.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql.py` & `hnhm-0.0.6/hnhm/postgres/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from hnhm.core import (
     Sql,
     Task,
     Type,
     LoadHub,
     LoadLink,
-    Mutation,
     HnhmError,
     LoadGroup,
+    Migration,
     ChangeType,
     CreateLink,
     LayoutType,
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
@@ -42,16 +42,16 @@
 PG_TYPES = {
     Type.STRING: "TEXT",
     Type.INTEGER: "INTEGER",
     Type.TIMESTAMP: "TIMESTAMPTZ",
 }
 
 
-def generate_sql(mutation_or_task: Mutation | Task, jinja: jinja2.Environment) -> str:
-    match mutation_or_task:
+def generate_sql(migration_or_task: Migration | Task, jinja: jinja2.Environment) -> str:
+    match migration_or_task:
         case CreateEntity(entity=entity):
             if entity.layout.type == LayoutType.HNHM:
                 template = jinja.from_string(SQL_TEMPLATE__CREATE_HUB)
                 columns = []
                 columns_types = []
                 for key in entity.keys:
                     columns.append(key.name)
@@ -302,17 +302,17 @@
                 target_sks=target_sks,
                 target_attributes=[],
                 business_time_field=business_time_field.name,
                 extra_sks=["valid_from"],
             )
 
         case _:
-            mutation_or_task_type = type(mutation_or_task)
+            migration_or_task_type = type(migration_or_task)
             raise HnhmError(
-                f"Unknown mutation or task: '{mutation_or_task}' with type='{mutation_or_task_type}'."
+                f"Unknown migration or task: '{migration_or_task}' with type='{migration_or_task_type}'."
             )
 
 
 class PostgresSqlalchemySql(Sql):
     def __init__(
         self,
         *,
@@ -343,16 +343,16 @@
     def with_engine(cls, engine: Engine):
         if engine.url.drivername != "postgresql+psycopg2":
             raise HnhmError(
                 f"Wrong driver name '{engine.url.drivername}'. Required: 'postgresql+psycopg2'."
             )
         return cls(engine=engine)
 
-    def generate_sql(self, mutation_or_task: Mutation | Task) -> str:
-        return generate_sql(mutation_or_task, self.jinja)
+    def generate_sql(self, migration_or_task: Migration | Task) -> str:
+        return generate_sql(migration_or_task, self.jinja)
 
     def execute(self, sql: str, debug: bool = False):
         if debug:
             print(dedent(sql).strip())
 
         conn = None
         try:
```

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/create_attribute.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/create_attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/create_group.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/create_group.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/create_link.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/create_link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/load_ignore.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/load_ignore.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/load_new.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/load_new.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/hnhm/postgres/sql_templates/load_update.py` & `hnhm-0.0.6/hnhm/postgres/sql_templates/load_update.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.5/pyproject.toml` & `hnhm-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hnhm"
-version = "0.0.5"
+version = "0.0.6"
 description = "hNhM – highly Normalized hybrid Model."
 authors = ["Arseny Egorov <egoroff-ars@yandex.ru>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "1.10.7"
 click = "8.1.3"
@@ -13,15 +13,15 @@
 psycopg2-binary = "2.9.6"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "3.2.2"
 pytest = "7.3.1"
 pytest-cov = "4.0.0"
 pygount = "1.5.1"
-pandas = "2.0.0"
+pandas = "2.0.1"
 
 [tool.poetry.scripts]
 hnhm = "hnhm.cli:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

