# Comparing `tmp/rxnoptgoaliteragent-0.0.4.tar.gz` & `tmp/rxnoptgoaliteragent-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnoptgoaliteragent-0.0.4.tar", last modified: Tue Apr  4 06:30:26 2023, max compression
+gzip compressed data, was "rxnoptgoaliteragent-1.2.0.tar", last modified: Thu Apr 27 21:32:11 2023, max compression
```

## Comparing `rxnoptgoaliteragent-0.0.4.tar` & `rxnoptgoaliteragent-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       44 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/MANIFEST.in
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10842 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10386 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/README.md
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.337260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       36 2023-04-04 06:27:59.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/__init__.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/agent/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      102 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/agent/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7423 2023-03-31 13:49:03.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/agent/rxn_opt_goal_iter_agent.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       90 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1236 2023-03-31 13:49:03.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/iris.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8672 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/ontogoal.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1515 2023-02-07 17:47:30.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/entry_point.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/kg_operations/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       29 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/kg_operations/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    23095 2023-04-02 19:44:05.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/kg_operations/sparql_client.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/__init__.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    17970 2023-03-31 13:49:03.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/conftest.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7787 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_kg_sparql_client.py
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4466 2023-03-16 15:26:11.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_rxn_opt_goal_iter.py
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_triples/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1882 2023-03-31 13:49:03.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_triples/goal_iter.ttl
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1173 2023-03-31 13:49:03.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_triples/plan_step_agent.ttl
-drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10842 2023-04-04 06:30:26.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/PKG-INFO
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      915 2023-04-04 06:30:26.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/SOURCES.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-04-04 06:30:26.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/dependency_links.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      175 2023-04-04 06:30:26.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/requires.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       20 2023-04-04 06:30:26.000000 rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/top_level.txt
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-04-04 06:30:26.347260 rxnoptgoaliteragent-0.0.4/setup.cfg
--rw-r--r--   0 jb2197    (1000) jb2197    (1000)      996 2023-04-04 06:27:59.000000 rxnoptgoaliteragent-0.0.4/setup.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.817283 rxnoptgoaliteragent-1.2.0/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       44 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/MANIFEST.in
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10842 2023-04-27 21:32:11.817283 rxnoptgoaliteragent-1.2.0/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10386 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/README.md
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       36 2023-04-27 21:30:52.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/__init__.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/agent/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      102 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/agent/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7431 2023-04-27 12:28:53.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/agent/rxn_opt_goal_iter_agent.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       90 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1236 2023-04-27 12:27:27.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/iris.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     8672 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/ontogoal.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1515 2023-02-07 17:47:30.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/entry_point.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/kg_operations/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       29 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/kg_operations/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    23224 2023-04-27 12:43:57.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/kg_operations/sparql_client.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        0 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/__init__.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    18077 2023-04-27 21:22:44.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/conftest.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     7787 2023-01-20 09:52:31.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_kg_sparql_client.py
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     4466 2023-03-16 15:26:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_rxn_opt_goal_iter.py
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.817283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_triples/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1878 2023-04-27 12:28:53.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_triples/goal_iter.ttl
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)     1153 2023-04-27 12:28:53.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_triples/plan_step_agent.ttl
+drwxr-xr-x   0 jb2197    (1000) jb2197    (1000)        0 2023-04-27 21:32:11.807283 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)    10842 2023-04-27 21:32:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/PKG-INFO
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      915 2023-04-27 21:32:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/SOURCES.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)        1 2023-04-27 21:32:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/dependency_links.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      175 2023-04-27 21:32:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/requires.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       20 2023-04-27 21:32:11.000000 rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/top_level.txt
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)       38 2023-04-27 21:32:11.817283 rxnoptgoaliteragent-1.2.0/setup.cfg
+-rw-r--r--   0 jb2197    (1000) jb2197    (1000)      996 2023-04-27 21:30:52.000000 rxnoptgoaliteragent-1.2.0/setup.py
```

### Comparing `rxnoptgoaliteragent-0.0.4/PKG-INFO` & `rxnoptgoaliteragent-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnoptgoaliteragent
-Version: 0.0.4
+Version: 1.2.0
 Summary: rxnoptgoaliteragent is capable of conducting one iteration of pursuring the reaction optimisation goal as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/RxnOptGoalIterAgent
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rxnoptgoaliteragent-0.0.4/README.md` & `rxnoptgoaliteragent-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/agent/rxn_opt_goal_iter_agent.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/agent/rxn_opt_goal_iter_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         **kwargs
     ):
         super().__init__(**kwargs)
 
         self.sparql_client = self.get_sparql_client(RxnOptGoalIterSparqlClient)
 
     def agent_input_concepts(self) -> list:
-        return [ONTOGOAL_GOALSET, ONTOCAPE_CHEMICALREACTION, ONTOREACTION_REACTIONEXPERIMENT, ONTOLAB_LABORATORY]
+        return [ONTOGOAL_GOALSET, ONTOREACTION_CHEMICALREACTION, ONTOREACTION_REACTIONEXPERIMENT, ONTOLAB_LABORATORY]
 
     def agent_output_concepts(self) -> list:
         return [ONTOGOAL_RESULT]
 
     def validate_inputs(self, http_request) -> bool:
         return super().validate_inputs(http_request)
 
@@ -33,15 +33,15 @@
             raise Exception(f"Exactly one goal set is expected, but found: {list_goal_set_iri}")
         goal_set_iri = list_goal_set_iri[0]
         goal_set_instance = self.sparql_client.get_goal_set_instance(goal_set_iri)
 
         # II. Get the chemical reaction and reaction experiment
         # NOTE reaction experiment might not in the derivation inputs as this might be the first reaction where no prior data is available
         # Check if the input is in correct format, and return OntoReaction.ReactionExperiment/ReactionVariation instance
-        list_chemical_reaction_iri = derivation_inputs.getIris(ONTOCAPE_CHEMICALREACTION)
+        list_chemical_reaction_iri = derivation_inputs.getIris(ONTOREACTION_CHEMICALREACTION)
         if len(list_chemical_reaction_iri) != 1:
             raise Exception(f"Exactly one chemical reaction is expected, but found: {list_chemical_reaction_iri}")
         chem_rxn_iri = list_chemical_reaction_iri[0]
         chem_rxn_instance = self.sparql_client.get_chemical_reaction_given_iri(chem_rxn_iri)
         if chem_rxn_instance.hasDoETemplate is None:
             raise Exception(f"ChemicalReaction {chem_rxn_iri} does not have a DoE template")
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/iris.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/iris.py`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/data_model/ontogoal.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/data_model/ontogoal.py`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/entry_point.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/entry_point.py`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/kg_operations/sparql_client.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/kg_operations/sparql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             hasRestriction=restriction,
         )
         return goal_set_instance
 
     def generate_doe_instance_from_goal(
         self,
         goal_set: GoalSet,
-        chem_rxn: OntoCAPE_ChemicalReaction,
+        chem_rxn: ChemicalReaction,
         rxn_exp_as_beliefs: List[ReactionExperiment]=None,
     ) -> DesignOfExperiment:
         # get the doe template
         doe_template = self.get_doe_instance(chem_rxn.hasDoETemplate)
 
         # process design variables
         list_design_variables = []
@@ -181,37 +181,37 @@
             if isinstance(var, ContinuousVariable):
                 design_var = ContinuousVariable(
                     instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                     namespace_for_init=getNameSpace(var.instance_iri),
                     upperLimit=var.upperLimit,
                     lowerLimit=var.lowerLimit,
                     positionalID=var.positionalID,
-                    refersTo=OM_Quantity(
+                    refersToQuantity=OM_Quantity(
                         instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
-                        namespace_for_init=getNameSpace(var.refersTo.instance_iri),
-                        clz=var.refersTo.clz,
-                        hasUnit=var.refersTo.hasUnit,
+                        namespace_for_init=getNameSpace(var.refersToQuantity.instance_iri),
+                        clz=var.refersToQuantity.clz,
+                        hasUnit=var.refersToQuantity.hasUnit,
                     ),
                 )
                 list_design_variables.append(design_var)
             elif isinstance(var, CategoricalVariable):
                 list_design_variables.append(
                     CategoricalVariable(
                         instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                         namespace_for_init=getNameSpace(var.instance_iri),
                         positionalID=var.positionalID,
-                        refersTo=OM_Quantity(
+                        refersToQuantity=OM_Quantity(
                             instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                             namespace_for_init=getNameSpace(var.instance_iri),
-                            clz=var.refersTo.clz,
+                            clz=var.refersToQuantity.clz,
                             hasValue=OM_Measure(
                                 instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
-                                namespace_for_init=getNameSpace(var.refersTo.instance_iri),
-                                hasUnit=var.refersTo.hasValue.hasUnit,
-                                hasNumericalValue=var.refersTo.hasValue.hasNumericalValue,
+                                namespace_for_init=getNameSpace(var.refersToQuantity.instance_iri),
+                                hasUnit=var.refersToQuantity.hasValue.hasUnit,
+                                hasNumericalValue=var.refersToQuantity.hasValue.hasNumericalValue,
                             ),
                         ),
                         hasLevel=var.hasLevel,
                     )
                 )
             else:
                 raise NotImplementedError(f"Design variable type {type(var)} is not implemented yet.")
@@ -219,38 +219,38 @@
         # process fixed parameters
         list_fixed_parameters = []
         for param in doe_template.hasDomain.hasFixedParameter:
             fixed_param = FixedParameter(
                 instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                 namespace_for_init=getNameSpace(param.instance_iri),
                 positionalID=param.positionalID,
-                refersTo=OM_Quantity(
+                refersToQuantity=OM_Quantity(
                     instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
-                    namespace_for_init=getNameSpace(param.refersTo.instance_iri),
-                    clz=param.refersTo.clz,
+                    namespace_for_init=getNameSpace(param.refersToQuantity.instance_iri),
+                    clz=param.refersToQuantity.clz,
                     hasValue=OM_Measure(
                         instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
-                        namespace_for_init=getNameSpace(param.refersTo.hasValue.instance_iri),
-                        hasUnit=param.refersTo.hasValue.hasUnit,
-                        hasNumericalValue=param.refersTo.hasValue.hasNumericalValue,
+                        namespace_for_init=getNameSpace(param.refersToQuantity.hasValue.instance_iri),
+                        hasUnit=param.refersToQuantity.hasValue.hasUnit,
+                        hasNumericalValue=param.refersToQuantity.hasValue.hasNumericalValue,
                     ),
                 )
             )
             list_fixed_parameters.append(fixed_param)
 
         # process system responses
         list_system_responses = []
         for goal in goal_set.hasGoal:
             boolean_maximise = True if goal.desiresGreaterThan is not None else False
             sys_res = SystemResponse(
                 instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                 namespace_for_init=getNameSpace(goal_set.instance_iri),
                 maximise=boolean_maximise,
                 # positionalID=None, # TODO [only when we are supporting same type of goal]
-                refersTo=goal.desires().clz,
+                refersToQuantity=goal.desires().clz,
             )
             list_system_responses.append(sys_res)
 
         # construct doe domain
         constructed_domain = Domain(
             instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
             namespace_for_init=getNameSpace(goal_set.instance_iri),
@@ -270,15 +270,15 @@
             # TODO [urgent] make sure the strategy is not duplicated if already exists in the KG - current solution will mess up the TSEMO as duplicated data properties will be created
             usesStrategy=doe_template.usesStrategy,
             hasDomain=constructed_domain,
             hasSystemResponse=list_system_responses,
             utilisesHistoricalData=HistoricalData(
                 instance_iri=INSTANCE_IRI_TO_BE_INITIALISED,
                 namespace_for_init=getNameSpace(goal_set.instance_iri),
-                refersTo=filtered_rxn_exp_as_beliefs,
+                refersToExperiment=filtered_rxn_exp_as_beliefs,
                 # NOTE in utilisesHistoricalData, the default value 1 is used for numOfNewExp
             ),
             designsChemicalReaction=chem_rxn.instance_iri,
         )
 
         return doe_instance
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/conftest.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     return _create_rogi_agent
 
 # fixture used in the test_kg_sparql_client.py
 @pytest.fixture(scope="module")
 def initialise_triple_store():
     # NOTE: requires access to the docker.cmclinnovations.com registry from the machine the test is run on.
     # For more information regarding the registry, see: https://github.com/cambridge-cares/TheWorldAvatar/wiki/Docker%3A-Image-registry
-    blazegraph = DockerContainer('docker.cmclinnovations.com/blazegraph_for_tests:1.0.0')
+    blazegraph = DockerContainer('ghcr.io/cambridge-cares/blazegraph_for_tests:1.0.0')
     # the port is set as 9999 to match with the value set in the docker image
     blazegraph.with_exposed_ports(9999)
     yield blazegraph
 
 # fixture used in the test_kg_sparql_client.py
 @pytest.fixture(scope="module")
 def initialise_test_triples(initialise_triple_store):
@@ -264,15 +264,15 @@
 
 
 # ----------------------------------------------------------------------------------
 # Utility functions and classes
 # ----------------------------------------------------------------------------------
 
 class IRIs(Enum):
-    GOAL_ITER_BASE_IRI = 'http://www.example.com/triplestore/ontogoal/rxnopt/'
+    GOAL_ITER_BASE_IRI = 'https://www.example.com/triplestore/ontogoal/rxnopt/'
     GOALSET_1 = GOAL_ITER_BASE_IRI + 'GoalSet_1'
 
     GOAL_1 = GOAL_ITER_BASE_IRI + 'Goal_1'
     DESIRED_QUANTITY_1 = GOAL_ITER_BASE_IRI + 'Desired_Quantity_1'
     DESIRED_QUANTITY_1_TYPE = ONTOREACTION_YIELD
     DESIRED_QUANTITY_MEASURE_1 = GOAL_ITER_BASE_IRI + 'Desired_Quantity_Measure_1'
     DESIRED_QUANTITY_MEASURE_1_UNIT = OM_PERCENT
@@ -289,22 +289,22 @@
     DESIRED_QUANTITY_MEASURE_2 = GOAL_ITER_BASE_IRI + 'Desired_Quantity_Measure_2'
     DESIRED_QUANTITY_MEASURE_2_UNIT = OM_POUNDSTERLINGPERLITRE
     DESIRED_QUANTITY_MEASURE_2_NUMVAL = 0.01
     RESTRICTION_1 = GOAL_ITER_BASE_IRI + 'Restriction_1'
     RESTRICTION_1_CYCLEALLOWANCE = 5
     RESTRICTION_1_DEADLINE = 4102444800.0
 
-    PLAN_STEP_AGENT_BASE_IRI = 'http://www.theworldavatar.com/resource/plans/RxnOpt/'
+    PLAN_STEP_AGENT_BASE_IRI = 'https://www.theworldavatar.com/kg/plans/RxnOpt/'
     RXN_OPT_PLAN = PLAN_STEP_AGENT_BASE_IRI + 'rxnoptplan'
     STEP_DOE = PLAN_STEP_AGENT_BASE_IRI + 'doe'
-    STEP_DOE_AGENT = 'http://www.theworldavatar.com/resource/agents/Service__DoE/Service'
+    STEP_DOE_AGENT = 'https://www.theworldavatar.com/kg/agents/Service__DoE/Service'
     STEP_SCHEDULEEXE = PLAN_STEP_AGENT_BASE_IRI + 'schedule_exe'
-    STEP_SCHEDULE_AGENT = 'http://www.theworldavatar.com/resource/agents/Service__VapourtecSchedule/Service'
+    STEP_SCHEDULE_AGENT = 'https://www.theworldavatar.com/kg/agents/Service__VapourtecSchedule/Service'
     STEP_POSTPRO = PLAN_STEP_AGENT_BASE_IRI + 'postpro'
-    STEP_POSTPRO_AGENT = 'http://www.theworldavatar.com/resource/agents/Service__HPLC_PostPro/Service'
+    STEP_POSTPRO_AGENT = 'https://www.theworldavatar.com/kg/agents/Service__HPLC_PostPro/Service'
 
     EXP_1_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ReactionExperiment_1/'
     EXP_2_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ReactionExperiment_2/'
     EXP_3_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ReactionExperiment_3/'
     EXP_4_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ReactionExperiment_4/'
     EXP_5_BASE_IRI = 'https://www.example.com/triplestore/ontorxn/ReactionExperiment_5/'
     EXAMPLE_RXN_EXP_1_IRI = EXP_1_BASE_IRI + 'RxnExp_1'
@@ -320,14 +320,18 @@
 
     DERIVATION_INPUTS_NO_PRIOR_DATA = [GOALSET_1, CHEMICAL_REACTION_IRI]
 
 def initialise_triples(sparql_client, derivation_client, derivation_inputs):
     # Delete all triples before initialising prepared triples
     sparql_client.performUpdate("""DELETE WHERE {?s ?p ?o.}""")
 
+    # Upload ontology TBox
+    sparql_client.upload_ontology_tbox(ONTODOE)
+    sparql_client.upload_ontology_tbox(ONTOREACTION)
+
 	# Upload all relevant example triples provided in the resources folder of 'chemistry_and_robots' package to triple store
     for f in [
         'sample_data/rxn_data.ttl', # previous experiment data
         'sample_data/new_exp_data.ttl', # new experiment data
         'sample_data/dummy_lab.ttl', # lab hardware and other information
         'sample_data/doe_template.ttl', # DOE template
     ]:
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_kg_sparql_client.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_kg_sparql_client.py`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_rxn_opt_goal_iter.py` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_rxn_opt_goal_iter.py`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_triples/goal_iter.ttl` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_triples/goal_iter.ttl`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 @prefix rdfs:            <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix rdf:            <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:             <http://www.w3.org/2001/XMLSchema#> .
 @prefix saref:             <https://saref.etsi.org/core/> .
 @prefix om:             <http://www.ontology-of-units-of-measure.org/resource/om-2/> .
 @prefix ontorxn:         <https://www.theworldavatar.com/kg/ontoreaction/> .
 @prefix ontogoal:        <https://www.theworldavatar.com/kg/ontogoal/> .
-@prefix :                <http://www.example.com/triplestore/ontogoal/rxnopt/> .
+@prefix :                <https://www.example.com/triplestore/ontogoal/rxnopt/> .
 
-@prefix rxnopt:          <http://www.theworldavatar.com/resource/plans/RxnOpt/> .
+@prefix rxnopt:          <https://www.theworldavatar.com/kg/plans/RxnOpt/> .
 
 :GoalSet_1
     a ontogoal:GoalSet;
     ontogoal:hasGoal :Goal_1;
     ontogoal:hasGoal :Goal_2;
     ontogoal:hasRestriction :Restriction_1;
 .
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent/tests/test_triples/plan_step_agent.ttl` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent/tests/test_triples/plan_step_agent.ttl`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 @prefix rdfs:            <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix rdf:            <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix xsd:             <http://www.w3.org/2001/XMLSchema#> .
 @prefix saref:             <https://saref.etsi.org/core/> .
 @prefix om:             <http://www.ontology-of-units-of-measure.org/resource/om-2/> .
 @prefix ontogoal:        <https://www.theworldavatar.com/kg/ontogoal/> .
-@prefix :                <http://www.theworldavatar.com/resource/plans/RxnOpt/> .
+@prefix :                <https://www.theworldavatar.com/kg/plans/RxnOpt/> .
 
 :rxnoptplan
     a ontogoal:RxnOptPlan;
     ontogoal:hasStep :doe;
     ontogoal:hasStep :schedule_exe;
     ontogoal:hasStep :postpro;
 .
 
 :doe
     a ontogoal:DesignOfExperiment;
     ontogoal:hasNextStep :schedule_exe;
-    ontogoal:canBePerformedBy <http://www.theworldavatar.com/resource/agents/Service__DoE/Service>;
+    ontogoal:canBePerformedBy <https://www.theworldavatar.com/kg/agents/Service__DoE/Service>;
 .
 
 :schedule_exe
     a ontogoal:RxnExpExecution;
     ontogoal:hasNextStep :postpro;
-    ontogoal:canBePerformedBy <http://www.theworldavatar.com/resource/agents/Service__VapourtecSchedule/Service>;
+    ontogoal:canBePerformedBy <https://www.theworldavatar.com/kg/agents/Service__VapourtecSchedule/Service>;
 .
 
 :postpro
     a ontogoal:PostProcessing;
-    ontogoal:canBePerformedBy <http://www.theworldavatar.com/resource/agents/Service__HPLC_PostPro/Service>;
+    ontogoal:canBePerformedBy <https://www.theworldavatar.com/kg/agents/Service__HPLC_PostPro/Service>;
 .
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/PKG-INFO` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxnoptgoaliteragent
-Version: 0.0.4
+Version: 1.2.0
 Summary: rxnoptgoaliteragent is capable of conducting one iteration of pursuring the reaction optimisation goal as part of The World Avatar project.
 Home-page: https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/RxnOptGoalIterAgent
 Author: Jiaru Bai
 Author-email: jb2197@cam.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rxnoptgoaliteragent-0.0.4/rxnoptgoaliteragent.egg-info/SOURCES.txt` & `rxnoptgoaliteragent-1.2.0/rxnoptgoaliteragent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxnoptgoaliteragent-0.0.4/setup.py` & `rxnoptgoaliteragent-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='rxnoptgoaliteragent',
-    version='0.0.4',
+    version='1.2.0',
     author='Jiaru Bai',
     author_email='jb2197@cam.ac.uk',
     license='MIT',
     python_requires='>=3.8',
     description="rxnoptgoaliteragent is capable of conducting one iteration of pursuring the reaction optimisation goal as part of The World Avatar project.",
     url="https://github.com/cambridge-cares/TheWorldAvatar/tree/main/Agents/RxnOptGoalIterAgent",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(exclude=['tests','tests.*']),
-    install_requires=['pyderivationagent>=1.4.3', 'pandas', 'pydantic==1.9.0', 'chemistry_and_robots>=1.5.0'],
+    install_requires=['pyderivationagent>=1.4.3', 'pandas', 'pydantic==1.9.0', 'chemistry_and_robots>=1.6.0'],
     extras_require={
         "dev": [
             "testcontainers>=3.4.2",
             "pytest>=6.2.3",
             "pytest-docker-compose>=3.2.1",
             "pytest-rerunfailures>=10.2"
         ],
```

