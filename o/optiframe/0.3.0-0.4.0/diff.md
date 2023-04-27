# Comparing `tmp/optiframe-0.3.0.tar.gz` & `tmp/optiframe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optiframe-0.3.0.tar", max compression
+gzip compressed data, was "optiframe-0.4.0.tar", max compression
```

## Comparing `optiframe-0.3.0.tar` & `optiframe-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-03-12 14:09:36.025204 optiframe-0.3.0/LICENSE
--rw-r--r--   0        0        0     2109 2023-04-16 17:31:05.640958 optiframe-0.3.0/README.md
--rw-r--r--   0        0        0      385 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/__init__.py
--rw-r--r--   0        0        0      414 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/__init__.py
--rw-r--r--   0        0        0     2561 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/default_tasks.py
--rw-r--r--   0        0        0      267 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/errors.py
--rw-r--r--   0        0        0      527 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/metrics.py
--rw-r--r--   0        0        0     8788 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/optimizer.py
--rw-r--r--   0        0        0     1036 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/framework/tasks.py
--rw-r--r--   0        0        0        0 2023-04-01 14:13:27.609904 optiframe-0.3.0/optiframe/py.typed
--rw-r--r--   0        0        0      306 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/__init__.py
--rw-r--r--   0        0        0      495 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/errors.py
--rw-r--r--   0        0        0     6858 2023-04-16 20:21:48.040887 optiframe-0.3.0/optiframe/workflow_engine/step.py
--rw-r--r--   0        0        0     1054 2023-04-16 20:21:48.044887 optiframe-0.3.0/optiframe/workflow_engine/task.py
--rw-r--r--   0        0        0     2283 2023-04-16 20:21:48.044887 optiframe-0.3.0/optiframe/workflow_engine/workflow.py
--rw-r--r--   0        0        0     1087 2023-04-16 20:22:42.018131 optiframe-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 optiframe-0.3.0/setup.py
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 optiframe-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-12 14:09:36.025204 optiframe-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2108 2023-04-27 09:43:25.701305 optiframe-0.4.0/README.md
+-rw-r--r--   0        0        0      385 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-27 09:43:25.705305 optiframe-0.4.0/optiframe/framework/__init__.py
+-rw-r--r--   0        0        0     2561 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/framework/default_tasks.py
+-rw-r--r--   0        0        0      267 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/framework/errors.py
+-rw-r--r--   0        0        0     1042 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/metrics.py
+-rw-r--r--   0        0        0     8957 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/optimizer.py
+-rw-r--r--   0        0        0     1042 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-01 14:13:27.609904 optiframe-0.4.0/optiframe/py.typed
+-rw-r--r--   0        0        0      306 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/workflow_engine/__init__.py
+-rw-r--r--   0        0        0      496 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/errors.py
+-rw-r--r--   0        0        0     6909 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/step.py
+-rw-r--r--   0        0        0     1055 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/task.py
+-rw-r--r--   0        0        0     2322 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/workflow.py
+-rw-r--r--   0        0        0     1087 2023-04-27 10:42:09.187081 optiframe-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 optiframe-0.4.0/setup.py
+-rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 optiframe-0.4.0/PKG-INFO
```

### Comparing `optiframe-0.3.0/LICENSE` & `optiframe-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optiframe-0.3.0/README.md` & `optiframe-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -14,19 +14,19 @@
   4. **Solving** is a pre-defined step that obtains an optimal solution for the problem.
   5. **Solution extraction** allows you to process the variable values of the solution into something more meaningful.
 - **Tasks** are the core components that allow you to implement functionality for each step.
   - The constructor of a task allows you to define *dependencies* for that task,
     which are automatically injected by the optimizer based on their type annotation.
   - The **execute** method allows you to implement the functionality.
     It may return data which can then be used by other tasks as a dependency.
-- **Packages** combine tasks that belong together.
-    Each package must contain a task for building the MIP and can additionally contain tasks
+- **Modules** combine tasks that belong together.
+    Each module must contain a task for building the MIP and can additionally contain tasks
     for validation, pre-processing and solution extraction.
-    The packages are what makes Optiframe so modular:
-    You can define extensions of a problem in a separate package and only include it if needed.
+    The modules are what makes Optiframe so extendable:
+    You can define extensions of a problem in a separate module and only include it if needed.
 - The **optimizer** allows you to configure the packages that you need.
     Afterwards, you can initialize it with the instance data and then solve the optimization problem.
 
 ## Installation & Usage
 
 ```cli
 pip install optiframe
```

### Comparing `optiframe-0.3.0/optiframe/framework/default_tasks.py` & `optiframe-0.4.0/optiframe/framework/default_tasks.py`

 * *Files identical despite different names*

### Comparing `optiframe-0.3.0/optiframe/framework/optimizer.py` & `optiframe-0.4.0/optiframe/framework/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,81 +19,89 @@
     ProblemSettings,
 )
 from .metrics import StepTimes, ModelSize
 from .tasks import BuildMipTask, ValidateTask, PreProcessingTask, ExtractSolutionTask
 
 
 @dataclass
-class OptimizationPackage:
-    """A package bundling tasks for each step of the optimization process."""
+class OptimizationModule:
+    """A modules bundling tasks for each steps of the optimization process."""
 
     build_mip: Type[BuildMipTask[Any]]
     validate: Optional[Type[ValidateTask]] = None
     pre_processing: Optional[Type[PreProcessingTask[Any]]] = None
     extract_solution: Optional[Type[ExtractSolutionTask[Any]]] = None
 
 
 class Optimizer:
     """An optimizer for an optimization problem.
 
-    Can be configured by adding optimization packages,
+    Can be configured by adding optimization modules,
     which implement the actual optimization process.
     """
 
     name: str
     sense: LpMinimize | LpMaximize
-    packages: list[OptimizationPackage]
+    modules: list[OptimizationModule]
 
     def __init__(self, name: str, sense: LpMinimize | LpMaximize):
         """Create a new optimizer.
 
         :param name: The name of the optimization problem.
         :param sense: Whether to minimize or maximize the objective.
         Defaults to minimize.
         """
         self.name = name
         self.sense = sense
-        self.packages = []
+        self.modules = []
+
+    def add_modules(self, *modules: OptimizationModule) -> Self:
+        """Add optimization modules to the optimizer.
+
+        The modules implement the entire functionality,
+        without any modules, the optimizer doesn't do anything useful.
+        """
+        for module in modules:
+            self.modules.append(module)
 
-    def add_package(self, package: OptimizationPackage) -> Self:
-        """Add an optimization package to the optimizer."""
-        self.packages.append(package)
         return self
 
     def initialize(self, *data: Any) -> InitializedOptimizer:
         """Initialize the optimizer with the data defining the problem instance.
 
-        Which data classes need to be added here depends on the packages
+        Which data classes need to be added here depends on the modules
         that have been added to the optimizer.
         """
         validate_step = Step("validate")
         pre_processing_step = Step("pre_processing")
-        build_mip_step = Step("build_mip").add_task(CreateProblemTask)
-        solve_step = Step("solve").add_task(SolveTask)
-        extract_solution_step = Step("extract_solution").add_task(ExtractSolutionObjValueTask)
+        build_mip_step = Step("build_mip").add_tasks(CreateProblemTask)
+        solve_step = Step("solve").add_tasks(SolveTask)
+        extract_solution_step = Step("extract_solution").add_tasks(ExtractSolutionObjValueTask)
 
-        for package in self.packages:
-            if package.validate is not None:
-                validate_step.add_task(package.validate)
+        for module in self.modules:
+            if module.validate is not None:
+                validate_step.add_tasks(module.validate)
 
-            if package.pre_processing is not None:
-                pre_processing_step.add_task(package.pre_processing)
+            if module.pre_processing is not None:
+                pre_processing_step.add_tasks(module.pre_processing)
 
-            build_mip_step.add_task(package.build_mip)
+            build_mip_step.add_tasks(module.build_mip)
 
-            if package.extract_solution is not None:
-                extract_solution_step.add_task(package.extract_solution)
+            if module.extract_solution is not None:
+                extract_solution_step.add_tasks(module.extract_solution)
 
         workflow = (
             Workflow()
-            .add_step(validate_step)
-            .add_step(pre_processing_step)
-            .add_step(build_mip_step)
-            .add_step(solve_step)
-            .add_step(extract_solution_step)
+            .add_steps(
+                validate_step,
+                pre_processing_step,
+                build_mip_step,
+                solve_step,
+                extract_solution_step,
+            )
             .initialize(*data)
             .add_data(ProblemSettings(name=self.name, sense=self.sense))
         )
         return InitializedOptimizer(workflow)
 
 
 class InitializedOptimizer:
```

### Comparing `optiframe-0.3.0/optiframe/framework/tasks.py` & `optiframe-0.4.0/optiframe/framework/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The abstract task types for each optimization step."""
+"""The abstract task types for each optimization steps."""
 import abc
 from typing import TypeVar, Generic
 
 from optiframe import Task
 
 T = TypeVar("T")
 
@@ -24,15 +24,15 @@
 
     pass
 
 
 class BuildMipTask(Task[T], abc.ABC, Generic[T]):
     """A task to construct (or modify) the mixed integer program.
 
-    This is the central of the optimization package as it modifies the final result.
+    This is the central part of the optimization modules as it modifies the final result.
     """
 
     pass
 
 
 class ExtractSolutionTask(Task[T], abc.ABC):
     """A task to extract the relevant information from the solution of the MIP.
```

### Comparing `optiframe-0.3.0/optiframe/workflow_engine/step.py` & `optiframe-0.4.0/optiframe/workflow_engine/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The steps of a workflow.
 
 Steps are executed sequentially in the optimization process.
-Each step can contain multiple tasks, which are ordered based on their dependencies.
+Each steps can contain multiple tasks, which are ordered based on their dependencies.
 """
 
 from __future__ import annotations
 
 import inspect
 import logging
 from dataclasses import dataclass
@@ -37,75 +37,77 @@
 
 # Data which can be injected into a task.
 # The keys should be class objects which define the type of the data.
 StepData = dict[Any, Any]
 
 
 class Step:
-    """One step in the workflow process.
+    """One steps in the workflow process.
 
-    Each step is composed of multiple tasks which will be executed within this step.
+    Each steps is composed of multiple tasks which will be executed within this steps.
     Multiple steps are executed sequentially.
     """
 
     name: str
     tasks: list[Type[Task[Any]]]
 
     def __init__(self, name: str):
         self.name = name
         self.tasks = []
 
-    def add_task(self, task: Type[Task[Any]]) -> Self:
+    def add_tasks(self, *tasks: Type[Task[Any]]) -> Self:
         """Register a task to run in this step.
 
-        :param task: The task to register.
-        :return: The same step, to use for function chaining.
+        :param tasks: The tasks to register.
+        :return: The same steps, to use for function chaining.
         """
-        self.tasks.append(task)
+        for task in tasks:
+            self.tasks.append(task)
+
         return self
 
     def initialize(self, step_data: StepData) -> InitializedStep:
-        """Initialize a step with data from previous steps.
+        """Initialize a steps with data from previous steps.
 
         This allows data to be passed between steps and be added from the user.
         """
         return InitializedStep(self, step_data)
 
 
 class InitializedStep:
-    """A step that has been initialized with data."""
+    """A steps that has been initialized with data."""
 
     step: Step
     step_data: StepData
 
     def __init__(self, step: Step, step_data: StepData):
         self.step = step
         self.step_data = step_data
 
     def name(self) -> str:
-        """Get the name of the step."""
+        """Get the name of the steps."""
         return self.step.name
 
     def tasks(self) -> list[Type[Task[Any]]]:
-        """Get the tasks that have to be executed during this step."""
+        """Get the tasks that have to be executed during this steps."""
         return self.step.tasks
 
     def execute(self) -> StepData:
-        """Execute the step by executing the action of all tasks within it.
+        """Execute the steps by executing the action of all tasks within it.
 
         The dependencies of each task are injected automatically.
 
         :raises InjectionError: If the `__init__` or `action` methods are missing type annotations.
         This is necessary to inject the dependencies automatically.
         :raises ScheduleError: If the tasks can't be scheduled,
         e.g. due to circular dependencies.
-        :return: The step data, including the one generated during this step.
+        :return: The steps data, including the one generated during this steps.
         """
         start_time = datetime.now()
-        logger.info(f"Executing step {self.name()}...")
+        logger.info(f"Executing steps {self.name()}...")
 
         dependencies = self._task_dependencies()
 
         tasks_to_execute = [ext for ext in self.tasks()]
 
         while len(tasks_to_execute) > 0:
             has_executed = False
@@ -155,15 +157,15 @@
                     "The tasks could not be scheduled, "
                     f"{ext_strs} have unfulfilled dependencies:\n"
                     f"{missing_deps_strs}"
                 )
 
         duration = datetime.now() - start_time
 
-        logger.info(f"Finished step {self.name()} in {duration.total_seconds():.2f}s.")
+        logger.info(f"Finished steps {self.name()} in {duration.total_seconds():.2f}s.")
 
         return self.step_data
 
     def _task_dependencies(self) -> dict[Type[Task[Any]], list[TaskDependency]]:
         """Determine which task depends on which type of data.
 
         :return: For each task, a list of its dependencies.
```

### Comparing `optiframe-0.3.0/optiframe/workflow_engine/task.py` & `optiframe-0.4.0/optiframe/workflow_engine/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """A task in the workflow which executes a specific action.
 
     The task can generate data and return it from the `execute` function.
     This data will be made available to the other tasks of the workflow.
 
     The task can also depend on data by other tasks by specifying dependencies in the constructor.
     The type annotation of the constructor parameters determine which dependency will be injected.
-    If the data is generated by a task in the same step, the task will be executed before this one.
+    If the data is generated by a task in the same steps, the task will be executed before this one.
     """
 
     @abc.abstractmethod
     def execute(self) -> T:
         """Execute the action of this task.
 
         This method is called once all the dependencies of the task have been gathered.
```

### Comparing `optiframe-0.3.0/optiframe/workflow_engine/workflow.py` & `optiframe-0.4.0/optiframe/workflow_engine/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from .step import Step, StepData
 
 
 class Workflow:
     """A complete workflow.
 
     The workflow is composed of steps, which are executed sequentially.
-    Each step is composed of tasks, which can depend on each other.
+    Each steps is composed of tasks, which can depend on each other.
     """
 
     steps: list[Step]
 
     def __init__(self) -> None:
         self.steps = list()
 
-    def add_step(self, step: Step) -> Self:
-        """Add a step to the workflow.
+    def add_steps(self, *steps: Step) -> Self:
+        """Add steps to the workflow.
 
         The order in which the steps are added determines the order in which they are executed.
         """
-        self.steps.append(step)
+        for step in steps:
+            self.steps.append(step)
+
         return self
 
     def initialize(self, *args: Any) -> InitializedWorkflow:
         """Initialize the workflow with data.
 
         The data that needs to be added here is the data required by the tasks
         that is not generated by any other tasks.
@@ -54,22 +56,22 @@
         be provided by other tasks, but is also not available at initialization.
         """
         data_type = type(data)
         self.step_data[data_type] = data
         return self
 
     def execute_step(self, index: int) -> StepData:
-        """Execute the step at the given index.
+        """Execute the steps at the given index.
 
-        The indexes start at 0, so 0 is the first step.
+        The indexes start at 0, so 0 is the first steps.
         """
         step = self.workflow.steps[index]
         self.step_data = step.initialize(self.step_data).execute()
         return self.step_data
 
     def execute(self) -> StepData:
         """Execute all steps sequentially."""
         for step in self.workflow.steps:
-            # Execute each step sequentially and update the step data
+            # Execute each steps sequentially and update the steps data
             self.step_data = step.initialize(self.step_data).execute()
 
         return self.step_data
```

### Comparing `optiframe-0.3.0/pyproject.toml` & `optiframe-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optiframe"
-version = "0.3.0"
+version = "0.4.0"
 description = "A modular framework for mixed integer programming."
 authors = ["Tim Jentzsch <optiframe.projects@timjen.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TimJentzsch/optiframe"
 exclude = ["examples", "tests"]
```

### Comparing `optiframe-0.3.0/setup.py` & `optiframe-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pulp>=2.7.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['knapsack = examples.knapsack:demo']}
 
 setup_kwargs = {
     'name': 'optiframe',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'A modular framework for mixed integer programming.',
-    'long_description': '# Optiframe [![PyPI Version](https://img.shields.io/pypi/v/optiframe)](https://pypi.org/project/optiframe/) [![License](https://img.shields.io/pypi/l/optiframe)](LICENSE)\n\nOptiframe is an **opti**mization **frame**work for writing mixed integer programs (MIPs).\n\nIt allows you to structure your MIPs in a way that allows clear separation of concerns,\nhigh modularity and testability.\n\n## Core Concepts\n\n- The optimization process is divided into multiple **steps** which are clearly separated:\n  1. **Validation** allows you to validate the input data.\n  2. **Pre-processing** allows you to optimize the provided data to reduce the size of the final model.\n  3. **MIP building** allows you to modify the MIP to define the optimization problem.\n  4. **Solving** is a pre-defined step that obtains an optimal solution for the problem.\n  5. **Solution extraction** allows you to process the variable values of the solution into something more meaningful.\n- **Tasks** are the core components that allow you to implement functionality for each step.\n  - The constructor of a task allows you to define *dependencies* for that task,\n    which are automatically injected by the optimizer based on their type annotation.\n  - The **execute** method allows you to implement the functionality.\n    It may return data which can then be used by other tasks as a dependency.\n- **Packages** combine tasks that belong together.\n    Each package must contain a task for building the MIP and can additionally contain tasks\n    for validation, pre-processing and solution extraction.\n    The packages are what makes Optiframe so modular:\n    You can define extensions of a problem in a separate package and only include it if needed.\n- The **optimizer** allows you to configure the packages that you need.\n    Afterwards, you can initialize it with the instance data and then solve the optimization problem.\n\n## Installation & Usage\n\n```cli\npip install optiframe\n```\n\nTake a look at the `examples` folder for examples on how to use Optiframe!\n\n## License\n\nThis project is available under the terms of the [MIT license](LICENSE).\n',
+    'long_description': '# Optiframe [![PyPI Version](https://img.shields.io/pypi/v/optiframe)](https://pypi.org/project/optiframe/) [![License](https://img.shields.io/pypi/l/optiframe)](LICENSE)\n\nOptiframe is an **opti**mization **frame**work for writing mixed integer programs (MIPs).\n\nIt allows you to structure your MIPs in a way that allows clear separation of concerns,\nhigh modularity and testability.\n\n## Core Concepts\n\n- The optimization process is divided into multiple **steps** which are clearly separated:\n  1. **Validation** allows you to validate the input data.\n  2. **Pre-processing** allows you to optimize the provided data to reduce the size of the final model.\n  3. **MIP building** allows you to modify the MIP to define the optimization problem.\n  4. **Solving** is a pre-defined step that obtains an optimal solution for the problem.\n  5. **Solution extraction** allows you to process the variable values of the solution into something more meaningful.\n- **Tasks** are the core components that allow you to implement functionality for each step.\n  - The constructor of a task allows you to define *dependencies* for that task,\n    which are automatically injected by the optimizer based on their type annotation.\n  - The **execute** method allows you to implement the functionality.\n    It may return data which can then be used by other tasks as a dependency.\n- **Modules** combine tasks that belong together.\n    Each module must contain a task for building the MIP and can additionally contain tasks\n    for validation, pre-processing and solution extraction.\n    The modules are what makes Optiframe so extendable:\n    You can define extensions of a problem in a separate module and only include it if needed.\n- The **optimizer** allows you to configure the packages that you need.\n    Afterwards, you can initialize it with the instance data and then solve the optimization problem.\n\n## Installation & Usage\n\n```cli\npip install optiframe\n```\n\nTake a look at the `examples` folder for examples on how to use Optiframe!\n\n## License\n\nThis project is available under the terms of the [MIT license](LICENSE).\n',
     'author': 'Tim Jentzsch',
     'author_email': 'optiframe.projects@timjen.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TimJentzsch/optiframe',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `optiframe-0.3.0/PKG-INFO` & `optiframe-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optiframe
-Version: 0.3.0
+Version: 0.4.0
 Summary: A modular framework for mixed integer programming.
 Home-page: https://github.com/TimJentzsch/optiframe
 License: MIT
 Author: Tim Jentzsch
 Author-email: optiframe.projects@timjen.net
 Requires-Python: >=3.11.0rc1
 Classifier: License :: OSI Approved :: MIT License
@@ -30,19 +30,19 @@
   4. **Solving** is a pre-defined step that obtains an optimal solution for the problem.
   5. **Solution extraction** allows you to process the variable values of the solution into something more meaningful.
 - **Tasks** are the core components that allow you to implement functionality for each step.
   - The constructor of a task allows you to define *dependencies* for that task,
     which are automatically injected by the optimizer based on their type annotation.
   - The **execute** method allows you to implement the functionality.
     It may return data which can then be used by other tasks as a dependency.
-- **Packages** combine tasks that belong together.
-    Each package must contain a task for building the MIP and can additionally contain tasks
+- **Modules** combine tasks that belong together.
+    Each module must contain a task for building the MIP and can additionally contain tasks
     for validation, pre-processing and solution extraction.
-    The packages are what makes Optiframe so modular:
-    You can define extensions of a problem in a separate package and only include it if needed.
+    The modules are what makes Optiframe so extendable:
+    You can define extensions of a problem in a separate module and only include it if needed.
 - The **optimizer** allows you to configure the packages that you need.
     Afterwards, you can initialize it with the instance data and then solve the optimization problem.
 
 ## Installation & Usage
 
 ```cli
 pip install optiframe
```

