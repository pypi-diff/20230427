# Comparing `tmp/neoaccess-4.0.3.tar.gz` & `tmp/neoaccess-4.1.0.tar.gz`

## Comparing `neoaccess-4.0.3.tar` & `neoaccess-4.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.0.3/LICENSE.txt
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 neoaccess-4.0.3/README.md
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 neoaccess-4.0.3/pyproject.toml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.0.3/src/neoaccess/__init__.py
--rwxr-xr-x   0        0        0    24221 2020-02-02 00:00:00.000000 neoaccess-4.0.3/src/neoaccess/cypher_utils.py
--rwxr-xr-x   0        0        0   154340 2020-02-02 00:00:00.000000 neoaccess-4.0.3/src/neoaccess/neoaccess.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 neoaccess-4.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.1.0/LICENSE.txt
+-rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 neoaccess-4.1.0/README.md
+-rwxr-xr-x   0        0        0      974 2020-02-02 00:00:00.000000 neoaccess-4.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/__init__.py
+-rwxr-xr-x   0        0        0    24221 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/cypher_utils.py
+-rwxr-xr-x   0        0        0   157741 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/neoaccess.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 neoaccess-4.1.0/PKG-INFO
```

### Comparing `neoaccess-4.0.3/LICENSE.txt` & `neoaccess-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neoaccess-4.0.3/pyproject.toml` & `neoaccess-4.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "neoaccess"
-version = "4.0.3"
+version = "4.1.0"
 authors = [
-  { name = "Julian West" },
+  { name = "Julian West BrainAnnex.org" },
 ]
 maintainers = [
   { email = "julian@brainannex.org" },
 ]
 description = "High-level interface to the Neo4j graph database"
 readme = "README.md"
 license = "MIT"
@@ -31,9 +31,9 @@
   "neo4j",
 ]
 
 [project.urls]
 Homepage = "https://brainannex.org/guide.php"
 "Home-page" = "https://brainannex.org/guide.php"
 "Bug Tracker" = "https://github.com/BrainAnnex/brain-annex/issues"
-Source = "https://github.com/BrainAnnex/brain-annex/tree/main/BrainAnnex/modules/neo_access"
+Source = "https://github.com/BrainAnnex/neoaccess"
 Documentation = "https://brainannex.org/guide.php"
```

### Comparing `neoaccess-4.0.3/src/neoaccess/cypher_utils.py` & `neoaccess-4.1.0/src/neoaccess/cypher_utils.py`

 * *Files identical despite different names*

### Comparing `neoaccess-4.0.3/src/neoaccess/neoaccess.py` & `neoaccess-4.1.0/src/neoaccess/neoaccess.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import sys
 import json
 from typing import Union, List
 
 
 class NeoAccess:
     """
-    VERSION 4.0.3   (for Neo 4.x database versions)
+    IMPORTANT : for versions 4.x of the Neo4j database
 
     High-level class to interface with the Neo4j graph database from Python.
 
-    Mostly tested on version 4.3 of Neo4j Community version, but should work with other 4.x versions, too.
-    NOT tested on any other major version of Neo4j; in particular, not tested with version 5
+    Mostly tested on versions 4.3 and 4.4 of Neo4j Community version, but should work with other 4.x versions, too.
+    NOT tested on any other major version of Neo4j; in particular, NOT tested with version 5
 
     Conceptually, there are two parts to NeoAccess:
         1) A thin wrapper around the Neo4j python connectivity library "Neo4j Python Driver"
           that is documented at: https://neo4j.com/docs/api/python-driver/current/api.html
 
         2) A layer above, providing higher-level functionality for common database operations,
            such as lookup, creation, deletion, modification, import, indices, etc.
@@ -200,15 +200,16 @@
         if self.driver is not None:
             self.driver.close()
 
 
 
     def assert_valid_internal_id(self, internal_id: int) -> None:
         """
-        Raise an Exception if the argument is not a valid Neo4j ID
+        Raise an Exception if the argument is not a valid database internal ID
+
         :param internal_id: Alleged Neo4j internal database ID
         :return:            None
         """
         CypherUtils.assert_valid_internal_id(internal_id)
 
 
 
@@ -342,17 +343,17 @@
                                     that wishes to drop.  No harm in listing fields that aren't present
 
         :return:        A (possibly empty) list of dictionaries, if flatten is True,
                         or a list of list, if flatten is False.
                         Each item in the lists is a dictionary, with details that will depend on which Graph Data Types
                                     were returned in the Cypher query.
                                     EXAMPLE of individual items - for a returned NODE
-                                        {'gender': 'M', 'age': 20, 'neo4j_id': 123, 'neo4j_labels': ['patient']}
+                                        {'gender': 'M', 'age': 20, 'internal_id': 123, 'neo4j_labels': ['patient']}
                                     EXAMPLE of individual items - for a returned RELATIONSHIP
-                                        {'price': 7500, 'neo4j_id': 2,
+                                        {'price': 7500, 'internal_id': 2,
                                          'neo4j_start_node': <Node id=11 labels=frozenset() properties={}>,
                                          'neo4j_end_node': <Node id=14 labels=frozenset() properties={}>,
                                          'neo4j_type': 'bought_by'}]
         """
         # Start a new session, use it, and then immediately close it
         with self.driver.session() as new_session:
             result = new_session.run(q, params)
@@ -391,19 +392,19 @@
                     # EXAMPLES of item:
                     #       <Node id=95 labels=frozenset({'car'}) properties={'color': 'white', 'make': 'Toyota'}>
                     #       <Relationship id=12 nodes=(<Node id=147 labels=frozenset() properties={}>, <Node id=150 labels=frozenset() properties={}>) type='bought_by' properties={'price': 7500}>
 
                     neo4j_properties = dict(item.items())   # EXAMPLE: {'gender': 'M', 'age': 99}
 
                     if isinstance(item, neo4j.graph.Node):
-                        neo4j_properties["neo4j_id"] = item.id                  # Example: 227
+                        neo4j_properties["internal_id"] = item.id               # Example: 227
                         neo4j_properties["neo4j_labels"] = list(item.labels)    # Example: ['person', 'client']
 
                     elif isinstance(item, neo4j.graph.Relationship):
-                        neo4j_properties["neo4j_id"] = item.id                  # Example: 227
+                        neo4j_properties["internal_id"] = item.id               # Example: 227
                         neo4j_properties["neo4j_start_node"] = item.start_node  # A neo4j.graph.Node object with "id", "labels" and "properties"
                         neo4j_properties["neo4j_end_node"] = item.end_node      # A neo4j.graph.Node object with "id", "labels" and "properties"
                                                                                 #   Example: <Node id=118 labels=frozenset({'car'}) properties={'color': 'white'}>
                         neo4j_properties["neo4j_type"] = item.type              # The name of the relationship
 
                     elif isinstance(item, neo4j.graph.Path):
                         neo4j_properties["neo4j_nodes"] = item.nodes            # The sequence of Node objects in this path
@@ -429,31 +430,31 @@
     def update_query(self, cypher: str, data_binding=None) -> dict:
         """
         Run a Cypher query and return statistics about its actions (such number of nodes created, etc.)
         Typical use is for queries that update the database.
         If the query returns any values, a list of them is also made available, as the value of the key 'returned_data'.
 
         Note: if the query creates nodes and one wishes to obtain their Neo4j internal ID's,
-              one can include Cypher code such as "RETURN id(n) AS neo4j_id" (where n is the dummy name of the newly-created node)
+              one can include Cypher code such as "RETURN id(n) AS internal_id" (where n is the dummy name of the newly-created node)
 
-        EXAMPLE:  result = update_query("CREATE(n :CITY {name: 'San Francisco'}) RETURN id(n) AS neo4j_id")
+        EXAMPLE:  result = update_query("CREATE(n :CITY {name: 'San Francisco'}) RETURN id(n) AS internal_id")
 
                   result will be {'nodes_created': 1, 'properties_set': 1, 'labels_added': 1,
-                                  'returned_data': [{'neo4j_id': 123}]
+                                  'returned_data': [{'internal_id': 123}]
                                  } , assuming 123 is the Neo4j internal ID of the newly-created node
 
         :param cypher:      Any Cypher query, but typically one that doesn't return anything
         :param data_binding: Data-binding dictionary for the Cypher query
         :return:            A dictionary of statistics (counters) about the query just run
                             EXAMPLES -
                                 {}      The query had no effect
                                 {'nodes_deleted': 3}    The query resulted in the deletion of 3 nodes
                                 {'properties_set': 2}   The query had the effect of setting 2 properties
                                 {'relationships_created': 1}    One new relationship got created
-                                {'returned_data': [{'neo4j_id': 123}]}  'returned_data' contains the results of the query,
+                                {'returned_data': [{'internal_id': 123}]}  'returned_data' contains the results of the query,
                                                                         if it returns anything, as a list of dictionaries
                                                                         - akin to the value returned by query()
                                 {'returned_data': []}  Gets returned by SET QUERIES with no return statement
                             OTHER KEYS include:
                                 nodes_created, nodes_deleted, relationships_created, relationships_deleted,
                                 properties_set, labels_added, labels_removed,
                                 indexes_added, indexes_removed, constraints_added, constraints_removed
@@ -530,15 +531,15 @@
 
         If more than one record is found, an Exception is raised.
         If no record is found, return None.
 
         :param labels:              A string or list/tuple of strings.  Use None if not to be included in search
         :param primary_key_name:    The name of the primary key by which to look the record up
         :param primary_key_value:   The desired value of the primary key
-        :param return_internal_id:       If True, an extra entry is present in the dictionary, with the key "neo4j_id"
+        :param return_internal_id:  If True, an extra entry is present in the dictionary, with the key "internal_id"
 
         :return:                    A dictionary, if a unique record was found; or None if not found
         """
         assert primary_key_name, \
             f"NeoAccess.get_record_by_primary_key(): the primary key name cannot be absent or empty (value: {primary_key_name})"
 
         assert primary_key_value is not None, \
@@ -555,35 +556,36 @@
         return result[0]
 
 
 
     def exists_by_key(self, labels: str, key_name: str, key_value) -> bool:
         """
         Return True if a node with the given labels and key_name/key_value exists, or False otherwise
-
+        TODO: test for multiple labels
         :param labels:
         :param key_name:
         :param key_value:
-        :return:
+        :return:            True if a node with the given labels and key_name/key_value exists,
+                                or False otherwise
         """
         record = self.get_record_by_primary_key(labels, key_name, key_value)
 
         if record is None:
             return False
         else:
             return True
 
 
 
-    def exists_by_internal_id(self, internal_id) -> bool:         # TODO: test
+    def exists_by_internal_id(self, internal_id) -> bool:
         """
         Return True if a node with the given internal Neo4j exists, or False otherwise
 
-        :param internal_id:
-        :return:        True if a node with the given internal Neo4j exists, or False otherwise
+        :param internal_id: An integer with a node's internal database ID
+        :return:            True if a node with the given internal Neo4j exists, or False otherwise
         """
         q = f'''
         MATCH (n) 
         WHERE id(n) = {internal_id} 
         RETURN count(n) AS number_of_nodes
         '''
 
@@ -624,16 +626,16 @@
         """
         RETURN a list of the records (as dictionaries of ALL the key/value node properties)
         corresponding to all the Neo4j nodes specified by the given match data.
 
         :param match:           EITHER an integer with a Neo4j node id,
                                 OR a dictionary of data to identify a node, or set of nodes, as returned by match()
 
-        :param return_internal_id:   Flag indicating whether to also include the Neo4j internal node ID in the returned data
-                                    (using "neo4j_id" as its key in the returned dictionary)
+        :param return_internal_id:  Flag indicating whether to also include the Neo4j internal node ID in the returned data
+                                    (using "internal_id" as its key in the returned dictionary)
         :param return_labels:   Flag indicating whether to also include the Neo4j label names in the returned data
                                     (using "neo4j_labels" as its key in the returned dictionary)
 
         :param order_by:        Optional string with the key (field) name to order by, in ascending order
                                     Note: lower and uppercase names are treated differently in the sort order
         :param limit:           Optional integer to specify the maximum number of nodes returned
 
@@ -650,20 +652,20 @@
                                 Otherwise, return a list whose entries are dictionaries with each record's information
                                     (the node's attribute names are the keys)
                                     EXAMPLE: [  {"gender": "M", "age": 42, "condition_id": 3},
                                                 {"gender": "M", "age": 76, "location": "Berkeley"}
                                              ]
                                     Note that ALL the attributes of each node are returned - and that they may vary across records.
                                     If the flag return_nodeid is set to True, then an extra key/value pair is included in the dictionaries,
-                                            of the form     "neo4j_id": some integer with the Neo4j internal node ID
+                                            of the form     "internal_id": some integer with the Neo4j internal node ID
                                     If the flag return_labels is set to True, then an extra key/value pair is included in the dictionaries,
                                             of the form     "neo4j_labels": [list of Neo4j label(s) attached to that node]
                                     EXAMPLE using both of the above flags:
-                                        [  {"neo4j_id": 145, "neo4j_labels": ["person", "client"], "gender": "M", "condition_id": 3},
-                                           {"neo4j_id": 222, "neo4j_labels": ["person"], "gender": "M", "location": "Berkeley"}
+                                        [  {"internal_id": 145, "neo4j_labels": ["person", "client"], "gender": "M", "condition_id": 3},
+                                           {"internal_id": 222, "neo4j_labels": ["person"], "gender": "M", "location": "Berkeley"}
                                         ]
         # TODO: provide an option to specify the desired fields
 
         """
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
@@ -683,21 +685,21 @@
 
         self.debug_query_print(cypher, data_binding, "get_nodes")
 
 
         # Note: the flatten=True takes care of returning just the fields of the matched node "n", rather than dictionaries indexes by "n"
         if return_internal_id and return_labels:
             result_list = self.query_extended(cypher, data_binding, flatten=True)
-            # Note: query_extended() provides both 'neo4j_id' and 'neo4j_labels'
+            # Note: query_extended() provides both 'internal_id' and 'neo4j_labels'
         elif return_internal_id:     # but not return_labels
             result_list = self.query_extended(cypher, data_binding, flatten=True, fields_to_exclude=['neo4j_labels'])
         elif return_labels:     # but not return_internal_id
-            result_list = self.query_extended(cypher, data_binding, flatten=True, fields_to_exclude=['neo4j_id'])
+            result_list = self.query_extended(cypher, data_binding, flatten=True, fields_to_exclude=['internal_id'])
         else:
-            result_list = self.query_extended(cypher, data_binding, flatten=True, fields_to_exclude=['neo4j_id', 'neo4j_labels'])
+            result_list = self.query_extended(cypher, data_binding, flatten=True, fields_to_exclude=['internal_id', 'neo4j_labels'])
 
         # Deal with empty result lists
         if len(result_list) == 0:   # If no results were produced
             if single_row:
                 return None             # representing a record not found (different from a record with no fields, which will be {})
             if single_cell:
                 return None             # representing a field not found
@@ -855,17 +857,17 @@
         TODO: maybe also accept a "match" structure as argument
 
         :param internal_id: An integer with a Neo4j node id
         :return:            A list of strings with the names of all the labels of the given node
         """
         CypherUtils.assert_valid_internal_id(internal_id)
 
-        q = "MATCH (n) WHERE id(n)=$neo4j_id RETURN labels(n) AS all_labels"
+        q = "MATCH (n) WHERE id(n)=$internal_id RETURN labels(n) AS all_labels"
 
-        return self.query(q, data_binding={"neo4j_id": internal_id}, single_cell="all_labels")
+        return self.query(q, data_binding={"internal_id": internal_id}, single_cell="all_labels")
 
 
 
 
     #####################################################################################################
 
     '''                                 ~   CREATE NODES   ~                                          '''
@@ -905,15 +907,15 @@
 
         self.debug_query_print(q, data_dictionary, "create_node")
 
         result_list = self.query_extended(q, data_dictionary, flatten=True)  # TODO: switch to update_query(), and verify the creation
         if len(result_list) != 1:
             raise Exception("NeoAccess.create_node(): failed to create the requested new node")
 
-        return result_list[0]['neo4j_id']           # Return the Neo4j internal ID of the node just created
+        return result_list[0]['internal_id']           # Return the Neo4j internal ID of the node just created
 
 
 
     def merge_node(self, labels, properties=None) -> dict:  # TODO: test
         """
         The node gets created only if no other node with same labels and properties exists.
 
@@ -1378,29 +1380,29 @@
 
         #print("q_MERGE:\n", q_MERGE)
         # EXAMPLE of q_MERGE:
         '''(n)<-[:EMPLOYS ]-(ex0)
         (n)-[:OWNS {since: $NODE1_par_1}]->(ex1)'''
 
         # Put all the parts of the Cypher query together
-        q = q_MATCH + "\n" + q_CREATE + "\n" + q_MERGE + "RETURN id(n) AS neo4j_id"
+        q = q_MATCH + "\n" + q_CREATE + "\n" + q_MERGE + "RETURN id(n) AS internal_id"
         #print("\n", q)
         #print("\n", data_binding)
         # EXAMPLE of q:
         '''MATCH (ex0 :`DEPARTMENT` { dept_name: $NODE0_VAL }), (ex1 :`CAR`:`INVENTORY` { vehicle_id: $NODE1_VAL })
         CREATE (n :`PERSON` {`name`: $par_1, `city`: $par_2})
         MERGE (n)<-[:EMPLOYS ]-(ex0)
         MERGE (n)-[:OWNS {`since`: $NODE1_par_1}]->(ex1)
-        RETURN id(n) AS neo4j_id
+        RETURN id(n) AS internal_id
         '''
         # EXAMPLE of data_binding : {'par_1': 'Julian', 'par_2': 'Berkeley', 'NODE0_VAL': 'IT', 'NODE1_VAL': 12345, 'NODE1_par_1': 2021}
 
         result = self.update_query(q, data_binding)
         #print("Result of update_query in create_node_with_relationships(): ", result)
-        # EXAMPLE: {'labels_added': 1, 'relationships_created': 2, 'nodes_created': 1, 'properties_set': 3, 'returned_data': [{'neo4j_id': 604}]}
+        # EXAMPLE: {'labels_added': 1, 'relationships_created': 2, 'nodes_created': 1, 'properties_set': 3, 'returned_data': [{'internal_id': 604}]}
 
 
         # Assert that the query produced the expected actions
         if result.get("nodes_created") != 1:
             raise Exception("Failed to create 1 new node")
 
         if result.get("relationships_created") != len(connections):
@@ -1414,25 +1416,25 @@
             raise Exception(f"Failed to set all the {number_props_to_set} properties on the new node and its relationships")
 
         returned_data = result.get("returned_data")
         #print("returned_data", returned_data)
         if len(returned_data) == 0:
             raise Exception("Unable to extract internal ID of the newly-created node")
 
-        neo4j_id = returned_data[0].get("neo4j_id", None)
-        if neo4j_id is None:    # Note: neo4j_id might be zero
+        internal_id = returned_data[0].get("internal_id", None)
+        if internal_id is None:    # Note: internal_id might be zero
             raise Exception("Unable to extract internal ID of the newly-created node")
 
-        return neo4j_id    # Return the Neo4j ID of the new node
+        return internal_id    # Return the Neo4j ID of the new node
 
 
 
     #####################################################################################################
 
-    '''                                      ~   DELETE NODES   ~                                            '''
+    '''                                      ~   DELETE NODES   ~                                     '''
 
     def ________DELETE_NODES________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
     def delete_nodes(self, match: Union[int, dict]) -> int:
@@ -2313,15 +2315,15 @@
         :param including_constraints:   Flag indicating whether to also ditch all the constraints
         :return:                        None
         """
         if including_constraints:
             if self.apoc:
                 self.query("call apoc.schema.assert({},{})")
             else:
-                self.drop_all_constraints()    # TODO: it doesn't work in version 5.5 of the database
+                self.drop_all_constraints()    # TODO: it doesn't work in version 5.5 of the Neo4j database
 
         indexes = self.get_indexes()
         for name in indexes['name']:
             self.drop_index(name)
 
 
 
@@ -2809,93 +2811,130 @@
         if self.debug:
             print(f"{indent_str}list_importer() is returning: {list_of_child_ids}")
 
         return list_of_child_ids
 
 
 
-
-    def import_json_dump(self, json_str: str) -> str:
+    def import_json_dump(self, json_str: str, extended_validation = True) -> str:
         """
-        Used to import data from a database dump done with export_dbase_json() or export_nodes_rels_json()
-        Import nodes and/or relationships into the database, as directed by the given data dump in JSON form.
-        Note: the id's of the nodes need to be shifted,
+        Used to import data from a database dump that was done with export_dbase_json() or export_nodes_rels_json().
+
+        Import nodes and relationships into the database, as specified in the JSON code
+        that was created by the earlier data dump.
+
+        IMPORTANT: the internal id's of the nodes need to be shifted,
               because one cannot force the Neo4j internal id's to be any particular value...
               and, besides (if one is importing into an existing database), particular id's may already be taken.
-        :param json_str:    A JSON string with the format specified under export_dbase_json()
-        :return:            A status message with import details if successful, or raise an Exception if not
+
+        :param json_str:            A JSON string with the format specified under export_dbase_json()
+        :param extended_validation: If True, an attempt is made to try to avoid partial imports,
+                                        by running extended validations prior to importing
+                                        (it will make a first pass thru the data, and hence take longer)
+
+        :return:                    A status message with import details if successful;
+                                        or raise an Exception if not.
+                                        If an error does occur during import then the import is aborted -
+                                        and the number of imported nodes & relationships is returned in the Exception raised.
         """
 
         try:
-            json_list = json.loads(json_str)    # Turn the string (representing a JSON list) into a list
+            json_list = json.loads(json_str)    # Turn the string (which represents a JSON list) into a list
         except Exception as ex:
-            raise Exception(f"Incorrectly-formatted JSON string. {ex}")
+            raise Exception(f"import_json_dump(): incorrectly-formatted JSON string. {ex}")
 
         if self.debug:
             print("json_list: ", json_list)
 
-        assert type(json_list) == list, "The JSON string does not represent the expected list"
+        assert type(json_list) == list, \
+            "import_json_dump(): the JSON string does not represent a list"
+
 
         id_shifting = {}    # To map the Neo4j internal ID's specified in the JSON data dump
                             #       into the ID's of newly-created nodes
 
-        # Do an initial pass for correctness, to try to avoid partial imports
-        for i, item in enumerate(json_list):
-            # We use item.get(key_name) to handle without error situation where the key is missing
-            if (item.get("type") != "node") and (item.get("type") != "relationship"):
-                raise Exception(f"Item in list index {i} must have a 'type' of either 'node' or 'relationship'.  Nothing imported.  Item: {item}")
-
-            if item["type"] == "node":
-                if "id" not in item:
-                    raise Exception(f"Item in list index {i} is marked as 'node' but it lacks an 'id'.  Nothing imported.  Item: {item}")
-
-            elif item["type"] == "relationship":
-                if "label" not in item:
-                    raise Exception(f"Item in list index {i} is marked as 'relationship' but lacks a 'label'.  Nothing imported.  Item: {item}")
-                if "start" not in item:
-                    raise Exception(f"Item in list index {i} is marked as 'relationship' but lacks a 'start' value.  Nothing imported.  Item: {item}")
-                if "end" not in item:
-                    raise Exception(f"Item in list index {i} is marked as 'relationship' but lacks a 'end' value.  Nothing imported.  Item: {item}")
-                if "id" not in item["start"]:
-                    raise Exception(f"Item in list index {i} is marked as 'relationship' but its 'start' value lacks an 'id'.  Nothing imported.  Item: {item}")
-                if "id" not in item["end"]:
-                    raise Exception(f"Item in list index {i} is marked as 'relationship' but its 'end' value lacks an 'id'.  Nothing imported.  Item: {item}")
+        if extended_validation:
+            # Do an initial pass for correctness, to help avoid partial imports.
+            # TODO: maybe also check the validity of the start and end nodes of relationships
+            for i, item in enumerate(json_list):
+                assert type(item) == dict, \
+                    f"import_json_dump(): Item in list index {i} should be a dict, but instead it's of type {type(item)}.  Nothing imported.  Item: {item}"
+                # We use item.get(key_name) to handle without error situation where the key is missing
+                if (item.get("type") != "node") and (item.get("type") != "relationship"):
+                    raise Exception(f"import_json_dump(): Item in list index {i} must be a dict with a 'type' key, "
+                                    f"whose value is either 'node' or 'relationship'.  Nothing imported.  Item: {item}")
+
+                if item["type"] == "node":
+                    if "id" not in item:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'node' but it lacks an 'id'.  Nothing imported.  Item: {item}")
+                    try:
+                        int(item["id"])
+                    except ValueError:
+                        raise Exception(f"import_json_dump(): Item in list index {i} has an 'id' key whose value ({item['id']}) doesn't correspond to an integer.  "
+                                        f"Nothing imported.  Item: {item}")
+
+                elif item["type"] == "relationship":
+                    if "label" not in item:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'relationship' but lacks a 'label'.  Nothing imported.  Item: {item}")
+                    if "start" not in item:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'relationship' but lacks a 'start' value.  Nothing imported.  Item: {item}")
+                    if "end" not in item:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'relationship' but lacks a 'end' value.  Nothing imported.  Item: {item}")
+                    if "id" not in item["start"]:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'relationship' but its 'start' value lacks an 'id'.  Nothing imported.  Item: {item}")
+                    if "id" not in item["end"]:
+                        raise Exception(f"import_json_dump(): Item in list index {i} is marked as 'relationship' but its 'end' value lacks an 'id'.  Nothing imported.  Item: {item}")
 
 
-        # First, process all the nodes, and in the process create the id_shifting map
+        # First, process all the node data, and create the nodes; while doing that, generate the id_shifting map
         num_nodes_imported = 0
-        for item in json_list:
-            if item["type"] == "node":
-                #print("ADDING NODE: ", item)
-                #print(f'     Creating node with label `{item["labels"][0]}` and properties {item["properties"]}')
-                old_id = int(item["id"])
-                new_id = self.create_node(item["labels"][0], item["properties"])  # TODO: Only the 1st label is used for now
-                id_shifting[old_id] = new_id
-                num_nodes_imported += 1
+        try:
+            for item in json_list:
+                if item["type"] == "node":
+                    #print("ADDING NODE: ", item)
+                    #print(f'     Creating node with labels `{item["labels"]}` and properties {item["properties"]}')
+                    old_id = int(item["id"])
+                    new_id = self.create_node(item["labels"], item["properties"])  # Note: any number of labels can be imported
+                    id_shifting[old_id] = new_id
+                    num_nodes_imported += 1
+        except Exception as ex:
+            raise Exception(f"import_json_dump(): the import process was INTERRUPTED "
+                            f"after importing {num_nodes_imported} node(s) and 0 relationship(s). Reason: " + str(ex))
+
 
         #print("id_shifting map:", id_shifting)
 
         # Then process all the relationships, linking to the correct (newly-created) nodes by using the id_shifting map
+        # (node: item types that aren't either "node" nor "relationship" are currently being ignored during the import)
         num_rels_imported = 0
-        for item in json_list:
-            if item["type"] == "relationship":
-                #print("ADDING RELATIONSHIP: ", item)
-                rel_name = item["label"]
-                #rel_props = item["properties"]
-                rel_props = item.get("properties")      # Also works if no "properties" is present (relationships may lack it)
-
-                start_id_original = int(item["start"]["id"])
-                end_id_original = int(item["end"]["id"])
-
-                start_id_shifted = id_shifting[start_id_original]
-                end_id_shifted = id_shifting[end_id_original]
-                #print(f'     Creating relationship named `{rel_name}` from node {start_id_shifted} to node {end_id_shifted},  with properties {rel_props}')
-
-                self.link_nodes_by_ids(start_id_shifted, end_id_shifted, rel_name, rel_props)
-                num_rels_imported += 1
+        try:
+            for item in json_list:
+                if item["type"] == "relationship":
+                    #print("ADDING RELATIONSHIP: ", item)
+                    rel_name = item["label"]
+                    #rel_props = item["properties"]
+                    rel_props = item.get("properties")      # Also works if no "properties" is present (relationships may lack it)
+
+                    start_id_original = int(item["start"]["id"])
+                    end_id_original = int(item["end"]["id"])
+
+                    if start_id_original not in id_shifting:
+                        raise Exception(f"cannot add a relationship `{rel_name}` starting at node with id {start_id_original}, because no node with that id was imported")
+                    if end_id_original not in id_shifting:
+                        raise Exception(f"cannot add a relationship `{rel_name}` ending at node with id {start_id_original}, because no node with that id was imported")
+
+                    start_id_shifted = id_shifting[start_id_original]
+                    end_id_shifted = id_shifting[end_id_original]
+
+                    #print(f'     Creating relationship named `{rel_name}` from node {start_id_shifted} to node {end_id_shifted},  with properties {rel_props}')
+                    self.link_nodes_by_ids(start_id_shifted, end_id_shifted, rel_name, rel_props)
+                    num_rels_imported += 1
+        except Exception as ex:
+            raise Exception(f"import_json_dump(): the import process was INTERRUPTED "
+                            f"after importing {num_nodes_imported} node(s) and {num_rels_imported} relationship(s). Reason: " + str(ex))
 
 
         return f"Successful import of {num_nodes_imported} node(s) and {num_rels_imported} relationship(s)"
 
 
 
 
@@ -2992,7 +3031,17 @@
 
         :param level:
         :return:
         """
         indent_spaces = level*4
         indent_str = " " * indent_spaces        # Repeat a blank character the specified number of times
         return indent_str
+
+
+
+    def _debug_local(self) -> str:
+        """
+        Use to test the switch from a local to remote repository, for debugging
+
+        :return:
+        """
+        return "remote"
```

