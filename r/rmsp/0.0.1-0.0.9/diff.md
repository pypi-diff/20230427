# Comparing `tmp/rmsp-0.0.1.tar.gz` & `tmp/rmsp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmsp-0.0.1.tar", last modified: Sun Aug 28 17:35:28 2022, max compression
+gzip compressed data, was "rmsp-0.0.9.tar", last modified: Thu Apr 27 14:38:12 2023, max compression
```

## Comparing `rmsp-0.0.1.tar` & `rmsp-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2022-08-28 17:35:28.515250 rmsp-0.0.1/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    20098 2022-08-28 17:35:28.515250 rmsp-0.0.1/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    20206 2022-08-28 17:33:21.000000 rmsp-0.0.1/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2022-08-28 17:35:28.514250 rmsp-0.0.1/rmsp/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       94 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/__init__.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    13808 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/mphelper.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    29325 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/rmsbuilder.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    88392 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/rmscore.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2022-08-28 17:35:28.515250 rmsp-0.0.1/rmsp/rmsgui/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/rmsgui/__init__.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    14910 2022-08-28 17:33:35.000000 rmsp-0.0.1/rmsp/rmsutils.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2022-08-28 17:35:28.515250 rmsp-0.0.1/rmsp.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)    20098 2022-08-28 17:35:28.000000 rmsp-0.0.1/rmsp.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      267 2022-08-28 17:35:28.000000 rmsp-0.0.1/rmsp.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2022-08-28 17:35:28.000000 rmsp-0.0.1/rmsp.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       30 2022-08-28 17:35:28.000000 rmsp-0.0.1/rmsp.egg-info/requires.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        5 2022-08-28 17:35:28.000000 rmsp-0.0.1/rmsp.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2022-08-28 17:35:28.515250 rmsp-0.0.1/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      728 2022-08-28 17:35:20.000000 rmsp-0.0.1/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-04-27 14:38:12.182147 rmsp-0.0.9/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    19928 2023-04-27 14:38:12.182147 rmsp-0.0.9/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    19977 2023-04-27 14:36:31.000000 rmsp-0.0.9/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-04-27 14:38:12.164146 rmsp-0.0.9/rmsp/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      201 2023-04-27 14:28:48.000000 rmsp-0.0.9/rmsp/__init__.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     1686 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/commands.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-04-27 14:38:12.182147 rmsp-0.0.9/rmsp/example/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2023-04-24 11:15:38.000000 rmsp-0.0.9/rmsp/example/__init__.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      344 2023-04-24 11:15:38.000000 rmsp-0.0.9/rmsp/example/example1.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     7040 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/interactorhelper.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    13761 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/mphelper.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    33373 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/rmsbuilder.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)   101099 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/rmscore.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    13035 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/rmsinteractor.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     3170 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/rmstemplate.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    16282 2023-04-24 11:14:39.000000 rmsp-0.0.9/rmsp/rmsutils.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2023-04-27 14:38:12.181147 rmsp-0.0.9/rmsp.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    19928 2023-04-27 14:38:11.000000 rmsp-0.0.9/rmsp.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      377 2023-04-27 14:38:11.000000 rmsp-0.0.9/rmsp.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2023-04-27 14:38:11.000000 rmsp-0.0.9/rmsp.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       46 2023-04-27 14:38:11.000000 rmsp-0.0.9/rmsp.egg-info/requires.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        5 2023-04-27 14:38:11.000000 rmsp-0.0.9/rmsp.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2023-04-27 14:38:12.182147 rmsp-0.0.9/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      750 2023-04-27 14:36:39.000000 rmsp-0.0.9/setup.py
```

### Comparing `rmsp-0.0.1/PKG-INFO` & `rmsp-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: rmsp
-Version: 0.0.1
+Version: 0.0.9
 Summary: Resource management system for python
 Home-page: https://github.com/aldenleung/rmsp/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 
 # Resource Management System (RMS) Manual
@@ -25,30 +27,20 @@
 
 RMS record most common python functions and objects, and avoid duplicated jobs. Minimal efforts are needed from the users to avoid repeated jobs.  
 
 ### Effortless incorporation to existing pipelines
 
 Rebuilding an entire analysis into the new system is usually a big hurdle, but not in RMS. RMS provides a simple solution - you can keep using most of your codes in the main body. The only thing to do is to change the import functions.
 
-### Flexible interface for both programmers and non-programmers
 
-TBW
-
-### Multi-processing support on different tasks
-
-TBW
 
 ### Easy but powerful search
 
 Many systems allow you to find out an upstream file required to generate the results. However, not all systems allow more complicated search. For example, can we search for the results based on some input file 1 and input file 2, processed through either pipeline X with the parameter A or pipeline Y with parameter B? Can we find out peak files using peak calling software J with alignment based on alignment software K? RMS enables these searches so that you can always retrieve your results quickly
 
-### Tracking multiple conda environment in bash
-
-TBW
-
 ### Easy Backup / Restore
 
 Backup / Restore is an essential feature to protect a database system from data loss. The core RMS files include all the pipelines used, which are stored in an SQL database. It also allows users to select and backup various files or resource content (For example, only backup the raw file and key result file, and remove any intermediate files). Restoring a database requires. 
 
 ### Integrity check
 
 Since RMS uses the absolute path to link to a file, users could easily access the file as for any downstream analysis or visualization. Users can also move or delete any unused intermediate files. Just like Python culture, nothing prevents you from modifying a file if you really do so. We encourage users to be responsible for their own actions. However, RMS will still do a quick check (based on file size) before using the file. An optional integrity check based on MD5 is also available. 
@@ -56,15 +48,15 @@
 
 
 ## Installation
 
 To install Resource Management System, use the following:
 
 ```python
-pip install resource_management_system
+pip install rmsp
 ```
 
 
 
 ## Quick Start
 
 ### Try-it-out for the first time
@@ -560,28 +552,18 @@
 rmsutils.restore('src_path', 'target_path')
 ```
 
 
 
 ## User Guide - GUI
 
-The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding. 
-
-TBW
-
-### Template
-
-TBW
-
-### Extension
-
-TBW
-
-
+The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding.  Please refer to rmsp-gui for details
 
 ## FAQ / Important Notes
 
 This section includes some of the important notes that one should keep in mind when using RMS. 
 
 - RMS does not store any information about the environment. It does not keep track of any external executables. Rather, it basically relies on the conda environment. Hence when doing the backup / restore, make sure you also backup the environment yourself. 
 
 
+
+
```

### Comparing `rmsp-0.0.1/README.md` & `rmsp-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,20 @@
 
 RMS record most common python functions and objects, and avoid duplicated jobs. Minimal efforts are needed from the users to avoid repeated jobs.  
 
 ### Effortless incorporation to existing pipelines
 
 Rebuilding an entire analysis into the new system is usually a big hurdle, but not in RMS. RMS provides a simple solution - you can keep using most of your codes in the main body. The only thing to do is to change the import functions.
 
-### Flexible interface for both programmers and non-programmers
 
-TBW
-
-### Multi-processing support on different tasks
-
-TBW
 
 ### Easy but powerful search
 
 Many systems allow you to find out an upstream file required to generate the results. However, not all systems allow more complicated search. For example, can we search for the results based on some input file 1 and input file 2, processed through either pipeline X with the parameter A or pipeline Y with parameter B? Can we find out peak files using peak calling software J with alignment based on alignment software K? RMS enables these searches so that you can always retrieve your results quickly
 
-### Tracking multiple conda environment in bash
-
-TBW
-
 ### Easy Backup / Restore
 
 Backup / Restore is an essential feature to protect a database system from data loss. The core RMS files include all the pipelines used, which are stored in an SQL database. It also allows users to select and backup various files or resource content (For example, only backup the raw file and key result file, and remove any intermediate files). Restoring a database requires. 
 
 ### Integrity check
 
 Since RMS uses the absolute path to link to a file, users could easily access the file as for any downstream analysis or visualization. Users can also move or delete any unused intermediate files. Just like Python culture, nothing prevents you from modifying a file if you really do so. We encourage users to be responsible for their own actions. However, RMS will still do a quick check (based on file size) before using the file. An optional integrity check based on MD5 is also available. 
@@ -43,15 +33,15 @@
 
 
 ## Installation
 
 To install Resource Management System, use the following:
 
 ```python
-pip install resource_management_system
+pip install rmsp
 ```
 
 
 
 ## Quick Start
 
 ### Try-it-out for the first time
@@ -547,27 +537,15 @@
 rmsutils.restore('src_path', 'target_path')
 ```
 
 
 
 ## User Guide - GUI
 
-The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding. 
-
-TBW
-
-### Template
-
-TBW
-
-### Extension
-
-TBW
-
-
+The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding.  Please refer to rmsp-gui for details
 
 ## FAQ / Important Notes
 
 This section includes some of the important notes that one should keep in mind when using RMS. 
 
 - RMS does not store any information about the environment. It does not keep track of any external executables. Rather, it basically relies on the conda environment. Hence when doing the backup / restore, make sure you also backup the environment yourself.
```

### Comparing `rmsp-0.0.1/rmsp/mphelper.py` & `rmsp-0.0.9/rmsp/mphelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-'''
-Created on Mar 28, 2021
 
-@author: Alden
-'''
 from enum import Enum
 import multiprocessing
 import threading
 import time
 import datetime
 import queue
 _global_lock = threading.Condition()
```

### Comparing `rmsp-0.0.1/rmsp/rmsbuilder.py` & `rmsp-0.0.9/rmsp/rmsbuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from collections import defaultdict, OrderedDict
 import types
 import dill
 import threading
 from enum import Enum
 import logging
 
-from .rmscore import RMSEntryType, RMSEntry, Pipe, Task, Resource, UnrunTask, VirtualModule
-from. rmscore import RMSUpdateEvent
+from .rmscore import RMSEntryType, RMSEntry, Pipe, Task, Resource, UnrunTask, VirtualModule, FileResource, VirtualResource
+from. rmscore import RMSUpdateEvent, RMSTemplateJobStatus
 from .rmscore import _get_func_ba, _has_resource_content
 from .mphelper import ProcessWrap, ProcessWrapState
 
 _logger = logging.getLogger("rmspool")
 
 
 class RMSUnrunTasksBuilder():
@@ -23,14 +23,15 @@
 	def __init__(self, rmspool):
 		self.rmspool = rmspool
 		self.rms = rmspool.rms
 		self.rms.registerRMSUpdateListener(self)
 		
 		self.vfdb = {}
 		self.unruntasks = []
+		self.template_jobs = []
 		self.vm = VirtualModule()
 		
 	def onRMSUpdate(self, events):
 		'''
 		Builder allows users to specify a virtual file (that is generated by some tasks)
 		
 		The builder receives update from RMS and try to replace these virtual futures.
@@ -40,14 +41,17 @@
 		for event in events:
 			if event[0] == RMSUpdateEvent.INSERT:
 				if event[1][0] is RMSEntryType.FILERESOURCE:
 					f = self.rms.get(event[1])
 					if f.file_path in self.vfdb:
 						vr = self.vfdb.pop(f.file_path)
 						self.rms.replace_virtualresource(vr, f)
+# 				for template_job in self.template_jobs:
+# 					if all(ut)
+			# Track for templatejob
 	@property
 	def sql(self):
 		return self.rms.sql
 	
 	def register_file(self, *args, **kwargs):
 		return self.rms.register_file(*args, **kwargs)
 	
@@ -55,27 +59,27 @@
 		try:
 			return self.rms.file_from_path(file_path)
 		except:
 			file_path = os.path.abspath(file_path)
 			if file_path in self.vfdb:
 				return self.vfdb[file_path]
 			else:
-				vr = self.rms.create_virtualresource()
+				vr = self.rms.create_virtualfileresource(file_path)
 				self.vfdb[file_path] = vr
 				return vr
 	
 	def register_pipe(self, *args, **kwargs):
 		pipe = self.rms.register_pipe(*args, **kwargs)
 		# Create an alternative pipe with self stored as rmsp 
-		pipe_rb = Pipe(pipe.pid, pipe.func, pipe.return_volatile, pipe.is_deterministic, pipe.module_name, pipe.func_name, pipe.output_func, pipe.description, pipe.tags, pipe.info, self)
+		pipe_rb = Pipe(pipe.pid, pipe._func_str, pipe.return_volatile, pipe.is_deterministic, pipe.module_name, pipe.func_name, pipe._output_func_str, pipe.description, pipe.tags, pipe.info, self)
 		return pipe_rb
 	
 	def get_pipe(self, *args, **kwargs):
 		pipe = self.rms.get_pipe(*args, **kwargs)
-		pipe_rb = Pipe(pipe.pid, pipe.func, pipe.return_volatile, pipe.is_deterministic, pipe.module_name, pipe.func_name, pipe.output_func, pipe.description, pipe.tags, pipe.info, self)
+		pipe_rb = Pipe(pipe.pid, pipe._func_str, pipe.return_volatile, pipe.is_deterministic, pipe.module_name, pipe.func_name, pipe._output_func_str, pipe.description, pipe.tags, pipe.info, self)
 		return pipe_rb
 	
 	def rmsimport(self, namespace=None, moduleobj=None, varname = None, altname=None, return_first_module=False):
 		'''
 		Perform a virtual import
 	
 		'''
@@ -230,78 +234,157 @@
 				fileresource_description="", fileresource_tags=set(), fileresource_info={}):
 		'''
 		A virtual run method. Rather than running the RMS pipe, it creates unruntasks and virtualresources. 
 		'''
 		vr = self.rms.create_virtualresource()
 		if self.rms.scriptID is not None:
 			task_info = {"scriptid":self.rms.scriptID, **task_info}
-		
-		u = self.rms.create_unruntask(pipe.pid, args, kwargs, [vr], None,
+		if pipe.output_func is not None:
+			try:
+				def convert(arg):
+					if isinstance(arg, FileResource) or isinstance(arg, VirtualResource):
+						if arg.file_path is not None:
+							return arg.file_path
+						else:
+							return arg
+					elif isinstance(arg, Pipe):
+						return arg.func
+					else:
+						return arg
+				tmp_args = [convert(arg) for arg in args]
+				tmp_kwargs = {key:convert(arg) for key, arg in kwargs.items()}
+# 				print(tmp_args, tmp_kwargs)
+				
+				virtual_output_files = pipe.output_func(*tmp_args, **tmp_kwargs)
+				virtual_vrs = []
+				for file_path in virtual_output_files: 
+					file_path = os.path.abspath(file_path)
+					if file_path in self.vfdb:
+						tvr = self.vfdb[file_path]
+					else:
+						tvr = self.rms.create_virtualfileresource(file_path)
+						self.vfdb[file_path] = tvr
+					virtual_vrs.append(tvr)
+# 				print(virtual_output_files, virtual_vrs)				
+			except:
+				virtual_vrs = []
+		else:
+			virtual_vrs = []
+		u = self.rms.create_unruntask(pipe.pid, args, kwargs, [vr], virtual_vrs,
 									task_description, task_tags, task_info,
 									resource_description, resource_tags, resource_info,
 									fileresource_description, fileresource_tags, fileresource_info
 									)
+		
 		self.unruntasks.append(u)
 		return vr
 
-	def execute_builder(self):
-		self.rmspool.run(*self.unruntasks)
+	def run_template_job(self, template_job):
+		'''
+		This involves running multiple steps in a function
+		'''
+		vrs = []
+		rmsb_wrapper = types.SimpleNamespace()
+		rmsb_wrapper.register_file = self.register_file
+		rmsb_wrapper.file_from_path = self.file_from_path
+		rmsb_wrapper.sql = self.sql
+		def run_wrapper(*args, **kwargs):
+			vr = self.run(*args, **kwargs)
+			vrs.append(vr)
+			return vr
+		rmsb_wrapper.run = run_wrapper
+		rmsb_wrapper.get_pipe = lambda *args, **kwargs: RMSUnrunTasksBuilder.get_pipe(rmsb_wrapper, *args, **kwargs)
+		
+		def _dummy(*args, **kwargs):
+			pipe = self.register_pipe(*args, **kwargs)
+			return Pipe(pipe.pid, pipe._func_str, pipe.return_volatile, pipe.is_deterministic, pipe.module_name, pipe.func_name, pipe._output_func_str, pipe.description, pipe.tags, pipe.info, rmsb_wrapper)
+		rmsb_wrapper.register_pipe = _dummy
+		rmsb_wrapper.rmsimport = lambda *args, **kwargs: RMSUnrunTasksBuilder.rmsimport(rmsb_wrapper, *args, **kwargs) 
+		try:
+			template_job.func(rmsb_wrapper, *template_job.args, **template_job.kwargs)
+			unruntasks = [self.rms.get_unruntask(uid) for uid in set(vr.uid for vr in vrs)]
+		except:
+			import traceback
+			traceback.print_exc()
+			template_job.status = RMSTemplateJobStatus.ERROR
+			raise Exception()
+		self.template_jobs.append(template_job)
+		template_job.unruntasks.extend(unruntasks)
+		
+	def run_template(self, func, args=[], kwargs={}):
+		job = self.rms.create_template_job(func, args, kwargs)
+		self.run_template_job(job)
+		return job
+	
+	def simulate_template(self, func, args=[], kwargs={}):
+		return self.rms.simulate_template(func, args, kwargs)
+	
+	def execute_builder(self, priority=20):
+		self.rmspool.run(*self.unruntasks, priority=priority)
 		l = list(self.unruntasks)
 		self.unruntasks.clear()
+		for template_job in self.template_jobs:
+			if template_job.status == RMSTemplateJobStatus.PENDING:
+				template_job.status = RMSTemplateJobStatus.RUNNING
 		return l
 
-
+	
 class RMSPoolUpdateEvent(Enum):
 	SUBMISSION = 1
 	EXECUTION = 2
 	COMPLETION = 3
 	SKIPPED = 4
 	ERROR = 5
 	CANCELLATION = 6
 	
 
 
 def _dill_load(path):
 	with open(path, "rb") as fr:
 		return dill.load(fr)
+	
+	
 class RMSProcessWrapPool():
 	'''
 	Process is not recycled. Hence this is very inefficient for running many short processes. 
 	However, it benefits from interruptable Process, and not affected by jupyter's "stop"   
 	'''
 	def __init__(self, rms, nthread, use_thread=False): #, use_hybrid_process_thread=False
 		self.rms = rms
 		
 		self.nthread = nthread
 		
+# 		self.run_tasks_assistant_lock = threading.Condition() 
+# 		self.run_tasks_lock = threading.Condition()
+		 
 		self.pending_tasks_lock = threading.Condition() # A lock for accessing pending_tasks and next_pid
 		self.pending_tasks = OrderedDict()
 		self.next_pid = 0
 		
 		self.finished_tasks_lock = threading.Condition() # A lock for accessing finished_tasks and error_tasks
 		self.finished_tasks = set()
 		self.error_tasks = set()
 		
 		self.futures_lock = threading.Condition() # A lock for accessing futures 
 		self.futures = OrderedDict()
 
 		self.resources_to_fetch = set()
 		self.fetch_resource_tasks = OrderedDict()
 		
+		# The update event lock is used related to fireUpdateEvent
 		self.update_event_lock = threading.Condition()
 		self.update_events = list()
 
 		self.closing = False
 		
 		self.use_thread = use_thread
 		# The thread run tills closing is True and no more pending tasks remain.
 		threading.Thread(target=self._run_pending_tasks).start()
 		threading.Thread(target=self._fire_update_events).start()
 		
-		
 		self.listeners = []
 		
 		self.rms.registerRMSUpdateListener(self)
 		
 	def registerListener(self, listener):
 		self.listeners.append(listener)
 		
@@ -332,15 +415,17 @@
 			
 		self.update_event_lock.release()
 	
 	def onRMSUpdate(self, events):
 		'''
 		An unruntask is pending if it still has virtual resources not yet resolved.
 		Hence, upon any update of the virtual resource from RMS, 
-		try to notify pending_tasks_lock to check if any unruntasks can now be submitted   
+		try to notify pending_tasks_lock to check if any unruntasks can now be submitted
+		
+		(This method needs to be updated later, as multiple call to onRMSUpdate actually notify multiple times)
 		'''
 		toNotify = False
 		for event in events:
 			if event[0] == RMSUpdateEvent.DELETE:
 				if event[1][0] == RMSEntryType.VIRTUALRESOURCE:
 					toNotify = True
 		if toNotify:
@@ -362,16 +447,16 @@
 			pid = unruntask.uid # This pid is process id, not pipe id
 			self.pending_tasks[pid] = unruntask, priority
 			registered_pids.append(pid)
 		self.fireUpdateEvent([(RMSPoolUpdateEvent.SUBMISSION, unruntask.uid) for unruntask in unruntasks])
 		self.pending_tasks_lock.notify_all()
 		self.pending_tasks_lock.release()
 		
-		for unruntask in unruntasks:
-			self.fetch_resource_content(*unruntask.input_resources, priority=priority)
+		resources_to_fetch = [r for unruntask in unruntasks for r in unruntask.input_resources]
+		self.fetch_resource_content(*resources_to_fetch, priority=priority)
 		return registered_pids
 	
 	def fetch_resource_content(self, *resources, priority=20):
 		if self.closing:
 			raise ValueError("Invalid state")
 		self.pending_tasks_lock.acquire()
 		self._fetch_resource_content(*resources, priority=priority)
@@ -522,14 +607,20 @@
 								# Perform a new task
 								unruntask = job
 								pipe = self.rms.get_pipe(unruntask.pid)
 								ba = unruntask.ba
 								
 								executed.append(unruntask.uid)
 								func_args, func_kwargs = self.rms._ba_rms_to_func_args_kwargs(ba)
+								
+								output_files = self.rms.compute_output_files(pipe, func_args, func_kwargs)
+								if not self.rms.allow_overwrite:
+									if self.rms.exist_output_files(output_files):
+										raise Exception("Cannot overwrite files")
+								
 								pwcallback=(lambda state, raw_return_value, begin_time, end_time, pid, callback=None,unruntask=unruntask:
 																			self._completion_callback(state, raw_return_value, begin_time, end_time, pid, callback, unruntask))
 								
 								# Attempts to use process first
 								use_thread = self.use_thread
 								if pipe.return_volatile:
 									use_thread = True
@@ -659,27 +750,32 @@
 
 		
 	def _completion_callback(self, state, raw_return_value, begin_time, end_time, pid, callback, unruntask):
 		'''
 		Add pids to finished tasks. 
 		Notify pending tasks
 		'''
+		# Precompile file md5 so that we don't block the locks for too long
+		precompiled_files_md5 = self.rms._compile_files_md5_from_pipe_ba(self.rms.get_pipe(unruntask.pid), unruntask.ba)
+		
 		self.pending_tasks_lock.acquire() # The lock is important since the callback may occassionally triggers run_pending_tasks
 		self.futures_lock.acquire() # I don't think I need this here
 		self.finished_tasks_lock.acquire()
 		try:
 			if self.futures[pid].state == ProcessWrapState.COMPLETE:
 				self.fireUpdateEvent([(RMSPoolUpdateEvent.COMPLETION, pid)])
 				self.finished_tasks.add(pid)
 				
 				pipe = self.rms.get_pipe(unruntask.pid)
 				task = self.rms.register_finished_task(raw_return_value, begin_time, end_time, unruntask.ba, pipe, 
 													unruntask.task_description, unruntask.task_tags, unruntask.task_info,
 													unruntask.resource_description, unruntask.resource_tags, unruntask.resource_info, 
-													unruntask.fileresource_description, unruntask.fileresource_tags, unruntask.fileresource_info)
+													unruntask.fileresource_description, unruntask.fileresource_tags, unruntask.fileresource_info,
+													precompiled_files_md5
+													)
 								
 				self.rms.replace_unruntask(unruntask, task)
 			elif self.futures[pid].state == ProcessWrapState.PICKLING_ERROR:
 				# Try to rerun the process by using thread
 				pipe = self.rms.get_pipe(unruntask.pid)
 				ba = unruntask.ba
 				func_args, func_kwargs = self.rms._ba_rms_to_func_args_kwargs(ba)
@@ -708,15 +804,15 @@
 		self.pending_tasks_lock.release()
 	
 
 
 	def cancel(self, pids):
 		'''
 		Attempts to cancel a task if it is still pending. 
-		If a task is being executed or completed, it will be cancelled.  
+		If a task is being executed or completed, it will not be cancelled.  
 		See also kill. 
 		'''
 		removed_from_pending_tasks = []
 		self.pending_tasks_lock.acquire()
 		for pid in pids:
 			if pid in self.pending_tasks:
 				self.pending_tasks.pop(pid)
@@ -724,26 +820,38 @@
 		self.pending_tasks_lock.notify_all()
 		self.pending_tasks_lock.release()
 		
 # 		logging.info(f"Removed from pending tasks: {join_str(removed_from_pending_tasks, ',')}")
 # 		logging.info(f"Removed from pools: {join_str(removed_from_futures, ',')}")
 	def cancel_all(self):
 		'''
-		Attempts to cancel all pending tasks 
+		Attempts to cancel all pending tasks.
+		
+		If one wants to remove all pending and running tasks, use the following:
+		rmspool.cancel_all()
+		rmspool.kill_all() 
+		
 		'''
 		removed_from_pending_tasks = []
 		self.pending_tasks_lock.acquire()
 		for pid in list(self.pending_tasks.keys()):
 			self.pending_tasks.pop(pid)
 			removed_from_pending_tasks.append(pid)
 		self.pending_tasks_lock.notify_all()
 		self.pending_tasks_lock.release()
 		
 		
 	def kill(self, pids):
+		'''
+		Attempts to kill running tasks
+		If the task is still pending, it will not be killed.
+		
+		See also cancel.  		
+		
+		'''
 		self.pending_tasks_lock.acquire()
 		self.futures_lock.acquire()
 		for pid in pids:
 			self.futures[pid].kill()
 		self.pending_tasks_lock.notify_all()
 		self.pending_tasks_lock.release()
 		self.futures_lock.release()
```

### Comparing `rmsp-0.0.1/rmsp/rmscore.py` & `rmsp-0.0.9/rmsp/rmscore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-'''
-Running a command in a (another) conda environment
-
-Some software must be run within a specific environment (e.g. python 2). We do not support running python functions designed for different environments. 
-
- 
-Created on Jan 28, 2021
-
-@author: Alden
-'''
-
 import sys
 import os
 import subprocess
 import itertools
 import uuid
 import json
 import datetime
 import dateutil.parser
 import types
 import inspect
 import operator
-from enum import Enum
+from enum import IntEnum
 import sqlite3
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
 
 import networkx as nx
 import dill
 
 
 try:
 	import simplevc
@@ -34,24 +23,25 @@
 except:
 	_SUPPORT_SIMPLEVC = False
 	
 ###################################
 # RMS Update events
 ###################################
 
-class RMSUpdateEvent(Enum):
+class RMSUpdateEvent(IntEnum):
 	MODIFY = 1
 	INSERT = 2
 	DELETE = 3
 	CONTENTCHANGE = 4
+	REPLACE = 5
 	
 ###################################
 # RMS Entries and related classes
 ###################################
-class RMSEntryType(Enum):
+class RMSEntryType(IntEnum):
 	NONRMSENTRY = 0
 	PIPE = 1
 	RESOURCE = 2
 	FILERESOURCE = 3
 	TASK = 4
 	UNRUNTASK = 5
 	VIRTUALRESOURCE=6
@@ -103,14 +93,22 @@
 	@property
 	def run_time(self):
 		return self.end_time - self.begin_time
 	def get_type(self):
 		return RMSEntryType.TASK	
 	def get_id(self):
 		return self.tid
+	
+class UnrunTaskState(IntEnum):
+	EDIT = 0
+	LOCKED = 1
+	PENDING = 2
+	RUNNING = 3
+	COMPLETE = 4
+	ERROR = 5
 class UnrunTask(RMSEntry):
 	'''
 	return_values could be None if not specified. 
 	output_files could be None if not specified
 	If the above two are specified (as a list of virtual resources), 
 	an update will be applied to replace virtual resource to resource / fileresource
 	'''
@@ -129,14 +127,15 @@
 		self.resource_description = resource_description
 		self.resource_tags = resource_tags
 		self.resource_info = resource_info
 		self.fileresource_description = fileresource_description
 		self.fileresource_tags = fileresource_tags
 		self.fileresource_info = fileresource_info
 		self.replacement = None
+		self.state = UnrunTaskState.EDIT
 	@property
 	def input_pipes(self):
 		return [arg for arg in self.ba.args if isinstance(arg, Pipe)] + [arg for arg in self.ba.kwargs.values() if isinstance(arg, Pipe)]		
 	@property
 	def input_resources(self):
 		return [arg for arg in self.ba.args if isinstance(arg, Resource)] + [arg for arg in self.ba.kwargs.values() if isinstance(arg, Resource)]
 	@property
@@ -166,43 +165,77 @@
 		An unruntask is ready if all the arguments of ba is set properly.
 		'''
 		try:
 			self.ba.signature.bind(*self.ba.args, **self.ba.kwargs)
 		except TypeError:
 			return False
 		return True
-	
+class UnrunTaskParam:
+	pass	
+	# Remove associated parameter
+	 
 def _invalid_func():
 	'''
 	An indicator for invalid function when loading pipe from database.
 	'''
 	raise Exception("Invalid function")
 
 class Pipe(RMSEntry):
 	#def __init__(self, pid, func, return_tuple, return_volatile, output_func, is_deterministic, description, tags, info, rmsp):
-	def __init__(self, pid, func, return_volatile, is_deterministic, module_name, func_name, output_func, description, tags, info, rms):
+	def __init__(self, pid, func_str, return_volatile, is_deterministic, module_name, func_name, output_func_str, description, tags, info, rms):
 		self.pid = pid
-		self.func = func 
+		self._func_str = func_str
 		self.return_volatile = return_volatile
 		self.is_deterministic = is_deterministic
 		self.module_name = module_name
 		self.func_name = func_name		
-		self.output_func = output_func
+		self._output_func_str = output_func_str
 		self.description = description
 		self.tags = tags
 		self.info = info
 		self.rms = rms
-
+		self._func = None
+		self._output_func = None
+	
+	@property
+	def func(self):
+		if self._func is None:
+			try:
+				self._func = dill.loads(bytes.fromhex(self._func_str))
+			except:
+				self._func = _invalid_func
+		return self._func
+	@property
+	def output_func(self):
+		if self._output_func_str is None:
+			self._output_func = None
+		elif self._output_func is None:
+			try: 
+				self._output_func = dill.loads(bytes.fromhex(self._output_func_str))
+			except:
+				self._output_func = _invalid_func
+		return self._output_func
+			
+			
 	def __call__(self, *args, **kwargs):
 		return self.rms.run(self, args, kwargs)
 	def get_type(self):
 		return RMSEntryType.PIPE	
 	
 	def get_id(self):
 		return self.pid
+	def __getstate__(self):
+		d = dict(self.__dict__)
+		d.pop("rms")
+		return d
+	def __setstate__(self, d):
+		d = dict(d)
+		d["rms"] = None
+		self.__dict__ = d
+	
 class Resource(RMSEntry):
 	def __init__(self, rid, tid, volatile, description, tags, info, content=None, has_content=True):
 		self.rid = rid
 		self.tid = tid
 		self.volatile = volatile
 		self.description = description
 		self.tags = tags
@@ -253,30 +286,54 @@
 	def get_type(self):
 		return RMSEntryType.FILERESOURCE	
 		
 	def get_id(self):
 		return self.fid
 
 class VirtualResource(RMSEntry):
-	def __init__(self, vid, tid, volatile, description, tags, info):
+	def __init__(self, vid, file_path=None):
 		self.vid = vid
+		self.uid = None
 		self.replacement = None
+		self.file_path = file_path
 	def get_type(self):
 		return RMSEntryType.VIRTUALRESOURCE	
 		
 	def get_id(self):
 		return self.vid
 	
+# class VirtualFileResource(VirtualResource):
+# 	def __init__(self, vid, file_path):
+# 		super().__init__(vid)
+# 		self.file_path = file_path
+		
 class ResourceNotReadyException(Exception):
 	'''
 	An exception that is called when accessing a resource without content.
 	'''
 	pass
 	
-	
+class RMSTemplate():
+	pass
+class RMSLibrary():
+	pass
+class RMSTemplateJobStatus(IntEnum):
+	PENDING = 0
+	RUNNING = 1
+	COMPLETE = 2
+	ERROR = 3
+class RMSTemplateJob():
+	def __init__(self, tpid, func, args, kwargs):
+		self.tpid = tpid
+		self.func = func
+		self.args = args
+		self.kwargs = kwargs
+		self.status = RMSTemplateJobStatus.PENDING
+		self.unruntasks = []
+		self.tasks = []
 class VirtualModule():
 	'''
 	A virtual class to hold the imported module
 	'''
 	pass
 	
 ##########################
@@ -516,16 +573,168 @@
 	if os.path.isdir(f):
 		return None
 	try:
 		return subprocess.check_output(["md5sum", f]).decode().split()[0]
 	except:
 		return None
 	
+#####################################
+# Template Simulator
+#####################################	
+class TemplateSimulationResult:
+	def __init__(self, rfdb, vfdb, unruntasks_db, virtualresources_db, pipes_db):
+		self.rfdb = rfdb
+		self.vfdb = vfdb
+		self.unruntasks_db = unruntasks_db
+		self.virtualresources_db = virtualresources_db
+		self.pipes_db = pipes_db
+		
+class TemplateSimulator:
+	def __init__(self):
+		self.rfdb = {}
+		self.vfdb = {}
+		self.unruntasks_db = {}
+		self.virtualresources_db = {}
+		self.pipes_db = {}
+		
+	def _get_new_id(self):
+		return uuid.uuid4().hex
+		
+	def create_virtualfileresource(self, file_path):
+		vid = self._get_new_id()
+		vr = VirtualResource(vid, file_path=file_path)
+		self.vfdb[file_path] = vr
+		self.virtualresources_db[vid] = vr 
+		return vr
+	def create_virtualresource(self,):
+		vid = self._get_new_id()
+		vr = VirtualResource(vid)
+		self.virtualresources_db[vid] = vr
+		return vr
+	
+	def create_unruntask(self, pid, args=[], kwargs={}, return_values=[], output_files=[],
+						task_description="", task_tags=set(), task_info={},
+						resource_description="", resource_tags=set(), resource_info={}, 
+						fileresource_description="", fileresource_tags=set(), fileresource_info={}):
+		uid = self._get_new_id()
+		pipe = self.get_pipe(pid)
+		ba = _get_func_ba(pipe.func, args, kwargs, partial=True)
+		ut = UnrunTask(uid, pid, ba, return_values, output_files,
+					task_description, task_tags, task_info,
+					resource_description, resource_tags, resource_info,
+					fileresource_description, fileresource_tags, fileresource_info
+					)
+		
+		for vr in return_values:
+			vr.uid = uid
+		if output_files is not None:
+			for vr in output_files:
+				vr.uid = uid
+		self.unruntasks_db[uid] = ut
+		return ut
+		
+	
+	def register_file(self, file_path):
+		file_path = os.path.abspath(file_path)
+		if file_path in self.rfdb:
+			return self.rfdb[file_path]
+		else:
+			vr = self.create_virtualfileresource(file_path)
+		self.rfdb[file_path] = vr
+		return vr
+	
+	def file_from_path(self, file_path):
+		file_path = os.path.abspath(file_path)
+		if file_path in self.vfdb:
+			return self.vfdb[file_path]
+		else:
+			vr = self.create_virtualfileresource(file_path)
+		self.vfdb[file_path] = vr
+		return vr
+	
+	def register_pipe(self, func, return_volatile=False, is_deterministic=True, output_func=None, description="", tags={}, pid=None, force=False):
+		if not callable(func):
+			raise Exception("func is not callable, and cannot be registered")
+		info = {}
+		if func.__module__ == "__main__":
+			try:
+				info["sourcecode"] = inspect.getsource(func)
+			except:
+				pass
+			func.__code__ = _modify_func_code(func.__code__)
+		if output_func is not None:
+			if output_func.__module__ == "__main__":
+				try:
+					info["outputfunc_sourcecode"] = inspect.getsource(output_func)
+				except:
+					pass
+				output_func.__code__ = _modify_func_code(output_func.__code__)
+# 		print(func)
+		e = dill.dumps(func)
+# 		print(e)
+		func = dill.loads(e)
+		func_name = func.__name__
+		module_name = func.__module__
+
+		pid = self._get_new_id()
+		pipe = Pipe(pid, dill.dumps(func).hex(), return_volatile, is_deterministic, module_name, func_name, None if output_func is None else dill.dumps(output_func).hex(), description, tags, info, self)
+		self.pipes_db[pid] = pipe
+		return pipe
 	
+	def get_pipe(self, pid):
+		return self.pipes_db[pid]
 	
+	def run(self, pipe, args=(), kwargs={},
+		   task_description="", task_tags=set(), task_info={},
+				resource_description="", resource_tags=set(), resource_info={}, 
+				fileresource_description="", fileresource_tags=set(), fileresource_info={}):
+		uid = self._get_new_id()
+# 		print(uid)
+# 		ba = _get_func_ba(pipe.func, args, kwargs, partial=True)
+		vr = self.create_virtualresource()
+		if pipe.output_func is not None:
+			try:
+				def convert(arg):
+					if isinstance(arg, VirtualResource) or isinstance(arg, FileResource):
+						if arg.file_path is not None:
+							return arg.file_path
+						else:
+							return arg
+					elif isinstance(arg, Pipe):
+						return arg.func
+					else:
+						return arg
+				tmp_args = [convert(arg) for arg in args]
+				tmp_kwargs = {key:convert(arg) for key, arg in kwargs.items()}
+				# print(tmp_args, tmp_kwargs)
+				
+				virtual_output_files = pipe.output_func(*tmp_args, **tmp_kwargs)
+				virtual_vrs = []
+				for file_path in virtual_output_files: 
+					file_path = os.path.abspath(file_path)
+					if file_path in self.vfdb:
+						tvr = self.vfdb[file_path]
+					else:
+						tvr = self.create_virtualfileresource(file_path)
+						self.vfdb[file_path] = tvr
+					virtual_vrs.append(tvr)
+			except:
+				print("BAD")
+				virtual_vrs = []
+		
+		u = self.create_unruntask(pipe.pid, args, kwargs, [vr], virtual_vrs,
+									task_description, task_tags, task_info,
+									resource_description, resource_tags, resource_info,
+									fileresource_description, fileresource_tags, fileresource_info
+									)
+		self.unruntasks_db[u.uid] = u
+		return vr
+
+	def get_result(self):
+		return TemplateSimulationResult(self.rfdb, self.vfdb, self.unruntasks_db, self.virtualresources_db, self.pipes_db)
 #####################################
 # RMS
 #####################################	
 class ResourceManagementSystem():
 	'''
 	A resource management system
 	'''
@@ -537,20 +746,21 @@
 		self.dbfile = dbfile
 		self.resources_db = {}
 		self.pipes_db = {}
 		self.tasks_db = {}
 		self.fileresources_db = {}
 		self.unruntasks_db = {}
 		self.virtualresources_db = {}
+# 		self.virtualfileresources_db = {}
 		self.resource_dump_dir = resource_dump_dir
 		self.tokens = {}
 		self.rms_update_listeners = []
 		self.vm = VirtualModule()
 		self.scriptID = None
-		
+		self.allow_overwrite = False
 	############
 	# RMS Info #
 	############
 	@property
 	def database_id(self):
 		dbid, = self.sql.cursor().execute("SELECT infovalue FROM metainfo WHERE infokey = 'dbid'").fetchone()
 		return dbid
@@ -579,15 +789,34 @@
 	
 	def _obtain_resource_content(self, resource, autofetch=True):
 		if not resource.has_content:
 			try:
 				_load_resource_content(self.resource_dump_dir, resource)
 			except:
 				if autofetch:
-					self.auto_fetch_resource_content([resource])
+					# self.auto_fetch_resource_content([resource])
+					if not resource.has_content:
+						if resource.tid is None:
+							raise Exception("Fail. Unable to retrieve resource tid.")
+						task = self.get_task(resource.tid)
+						pipe = self.get_pipe(task.pid)
+						if not pipe.is_deterministic:
+							raise Exception("Fail. Unable to rerun pipe because it is a non-deterministic pipe.")
+						if not len(task.output_files) == 0:
+							raise Exception("Fail. Re-retrieving the content may overwrite certain files.")
+						if any(not os.path.exists(f.file_path) for f in task.input_fileresources):
+							raise Exception("Fail. Some files are missing")
+						for sub_resource in task.input_resources:
+							self._obtain_resource_content(sub_resource, autofetch)
+						raw_return_value = self._run_pipe(pipe, task.args, task.kwargs)
+						resource.content = raw_return_value
+						self.fireRMSUpdateEvent([(RMSUpdateEvent.CONTENTCHANGE, resource.get_full_id())])
+					
+					
+					
 				else:
 					raise Exception("Resource content not available for " + resource.rid)
 		return resource.content
 	
 	def _obtain_fileresource_file_path(self, fileresource):
 		return fileresource.file_path
 	
@@ -639,14 +868,16 @@
 				try:
 					info["outputfunc_sourcecode"] = inspect.getsource(output_func)
 				except:
 					pass
 				output_func.__code__ = _modify_func_code(output_func.__code__)
 		
 		func = dill.loads(dill.dumps(func))
+		if output_func is not None:
+			output_func = dill.loads(dill.dumps(output_func))
 		func_name = func.__name__
 		module_name = func.__module__
 		c = self.sql.cursor()
 		
 		c.execute('''SELECT pid FROM pipes where return_volatile IS ? AND is_deterministic IS ? AND module_name IS ? AND func_name IS ?;''', 
 				[int(return_volatile), int(is_deterministic), module_name, func_name])
 		
@@ -654,23 +885,25 @@
 		if len(results) > 0:
 			for old_pid, in results:
 				old_pipe = self.get_pipe(old_pid)
 				if (dill.dumps(old_pipe.func).hex() == dill.dumps(func).hex()
 					and ((old_pipe.output_func is None and output_func is None)
 						or (old_pipe.output_func is not None and output_func is not None and dill.dumps(old_pipe.output_func).hex() == dill.dumps(output_func).hex()))):
 					return old_pipe
-				
 		if pid is None:
 			pid = self._get_new_id()
-		pipe = Pipe(pid, func, return_volatile, is_deterministic, module_name, func_name, output_func, description, tags, info, self)
+		pipe = Pipe(pid, dill.dumps(func).hex(), return_volatile, is_deterministic, module_name, func_name, None if output_func is None else dill.dumps(output_func).hex(), description, tags, info, self)
 		_sql_execute_commands(self.sql, _sql_insert_pipe(pipe))
 		self.pipes_db[pid] = pipe
 		self.fireRMSUpdateEvent([(RMSUpdateEvent.INSERT, pipe.get_full_id())])
 		return pipe
 	
+# 	def drp(self, return_volatile=False, is_deterministic=True, output_func=None, description="", tags={}, pid=None, force=False):
+# 		return lambda func: self.register_pipe(func, return_volatile, is_deterministic, output_func, description, tags, pid, force)
+	
 	def register_file(self, file_path, *, description="", tags=set(), tid=None, fid=None, force=False):
 		'''
 		'''
 		file_path = os.path.abspath(file_path)
 		try:
 			existing_fileresource = self.file_from_path(file_path)
 		except:
@@ -709,15 +942,15 @@
 		c = self.sql.cursor()
 		#c.execute('''SELECT fid FROM files where file_patfile_pathh = ? ORDER BY (SELECT end_time FROM tasks WHERE tid = tid) DESC;''', [file_path])
 		c.execute('''SELECT fid FROM files where file_path = ? ORDER BY (SELECT end_time FROM tasks WHERE tid = tid) DESC;''', [file_path])
 		raw_results = c.fetchall()
 		results = [fid for fid, in raw_results if "overwritten" not in self.get_fileresource(fid).info and "deprecated" not in self.get_fileresource(fid).info]
 		if len(results) > 0:
 			if len(results) > 1:
-				raise Exception("Found more than one file.")
+				raise Exception("Found more than one file." + ",".join(results))
 			fid = results[-1]
 			return self.get_fileresource(fid)
 		else:
 			if len(raw_results) > 0:
 				raise Exception("You have requested a deprecated / overwritten file") 
 			else:
 				raise Exception(f"File {file_path} is not registered.")
@@ -884,40 +1117,53 @@
 			objs = [self.get_task(rmsobj.tid)]
 		elif rmsobj.get_type() == RMSEntryType.TASK:
 			objs = rmsobj.input_resources + rmsobj.input_fileresources + rmsobj.input_pipes
 		elif rmsobj.get_type() == RMSEntryType.UNRUNTASK:
 			objs = rmsobj.input_resources + rmsobj.input_fileresources + rmsobj.input_pipes + rmsobj.input_virtualresources
 		elif rmsobj.get_type() == RMSEntryType.VIRTUALRESOURCE:
 			objs = [unruntask for unruntask in self.unruntasks_db.values() if rmsobj in unruntask.output_virtualresources]
+			
+			#if rmsobj.file_path is not None:
+				#potential_unruntasks = [unruntask for unruntask in self.unruntasks_db.values() if rmsobj.file_path in self._guess_unruntask_output(unruntask)]
+				#potential_unruntasks = [unruntask for unruntask in self.unruntasks_db.values() if rmsobj.file_path in unruntask.output_file]
+				#objs += [r for r in potential_unruntasks if r not in objs] 
 		elif rmsobj.get_type() == RMSEntryType.PIPE:
 			objs = []
 		else:
 			raise Exception()
 		if target_rmsobjs is not None:
 			objs = [rmsobj for rmsobj in objs if rmsobj in target_rmsobjs]
 		return objs
 		
 	def _get_next_downstream_objs(self, rmsobj, target_rmsobjs=None):
 		target_tids = None if target_rmsobjs is None else [rmsobj.tid for rmsobj in target_rmsobjs if rmsobj.get_type() == RMSEntryType.TASK]
 		if rmsobj.get_type() == RMSEntryType.FILERESOURCE:
-			objs = self.find_tasks_by_io(iotype="i", fids=[rmsobj.fid], target_tids=target_tids)
+			objs = self.find_tasks_by_io(iotype="i", fids=[rmsobj.fid], target_tids=target_tids) + [unruntask for unruntask in self.unruntasks_db.values() if rmsobj in unruntask.input_fileresources]
 		elif rmsobj.get_type() == RMSEntryType.RESOURCE:
 			objs = self.find_tasks_by_io(iotype="i", rids=[rmsobj.rid], target_tids=target_tids) + [unruntask for unruntask in self.unruntasks_db.values() if rmsobj in unruntask.input_resources]
+			
 		elif rmsobj.get_type() == RMSEntryType.TASK:
 			objs = rmsobj.output_resources + rmsobj.output_fileresources
 		elif rmsobj.get_type() == RMSEntryType.UNRUNTASK:
 			objs = rmsobj.output_resources + rmsobj.output_fileresources + rmsobj.output_virtualresources
+			file_paths = [obj.file_path for obj in objs if obj.file_path is not None]
+# 			file_paths += self._guess_unruntask_output(rmsobj)
+			file_paths = set(file_paths)
+			potential_vrs = [virtualresource for virtualresource in self.virtualresources_db.values() if virtualresource.file_path is not None and virtualresource.file_path in file_paths]
+			objs += [v for v in potential_vrs if v not in objs]
 		elif rmsobj.get_type() == RMSEntryType.VIRTUALRESOURCE:
 			objs = [unruntask for unruntask in self.unruntasks_db.values() if rmsobj in unruntask.input_virtualresources]
 		elif rmsobj.get_type() == RMSEntryType.PIPE:
 			objs = self.find_tasks_by_io(iotype="i", pids=[rmsobj.pid], target_tids=target_tids) + [unruntask for unruntask in self.unruntasks_db.values() if rmsobj in unruntask.input_pipes]
 		else:
 			raise Exception()
+		#for i in self.unruntasks_db.values()
 		if target_rmsobjs is not None:
 			objs = [rmsobj for rmsobj in objs if rmsobj in target_rmsobjs]
+			
 		return objs
 	def _get_next_connected_objs(self, rmsobj, target_rmsobjs=None):
 		return set(self._get_next_upstream_objs(rmsobj, target_rmsobjs) + self._get_next_downstream_objs(rmsobj, target_rmsobjs))
 					
 						
 	############################
 	# Users get RMSEntry by ID #
@@ -973,42 +1219,42 @@
 			bool(r[2]),
 			bool(r[3]),
 			r[4],
 			r[5],
 			r[6],
 			r[7]
 		)
-		try:
-			
-			func = dill.loads(bytes.fromhex(func_str))
-		except:
-			func = _invalid_func
-		if output_func_str is None:
-			output_func = None
-		else:
-			try: 
-				output_func = dill.loads(bytes.fromhex(output_func_str))
-			except:
-				output_func = _invalid_func
+# 		try:
+# 			func = dill.loads(bytes.fromhex(func_str))
+# 		except:
+# 			func = _invalid_func
+# 		if output_func_str is None:
+# 			output_func = None
+# 		else:
+# 			try: 
+# 				output_func = dill.loads(bytes.fromhex(output_func_str))
+# 			except:
+# 				output_func = _invalid_func
 		tags = set(tag_value for tag_value, in tags_results)
 		info = {k:v for k, v in info_results}
 		if pid in self.pipes_db:
-			pipe = self.pipes_db[pid]
-			pipe.pid=pid
-			pipe.func=func
-			pipe.return_volatile=return_volatile
-			pipe.is_deterministic=is_deterministic
-			pipe.output_func=output_func
-			pipe.module_name = module_name
-			pipe.func_name = func_name
-			pipe.description=description
-			pipe.tags=tags
-			pipe.info=info
+			raise Exception()
+# 			pipe = self.pipes_db[pid]
+# 			pipe.pid=pid
+# 			pipe.func=func
+# 			pipe.return_volatile=return_volatile
+# 			pipe.is_deterministic=is_deterministic
+# 			pipe.output_func=output_func
+# 			pipe.module_name = module_name
+# 			pipe.func_name = func_name
+# 			pipe.description=description
+# 			pipe.tags=tags
+# 			pipe.info=info
 		else:
-			pipe = Pipe(pid, func, return_volatile, is_deterministic, module_name, func_name, output_func, description, tags, info, self)
+			pipe = Pipe(pid, func_str, return_volatile, is_deterministic, module_name, func_name, output_func_str, description, tags, info, self)
 			self.pipes_db[pipe.pid] = pipe
 		return pipe
 	
 	def get_resource(self, rid, refetch=False):
 		if rid in self.resources_db and not refetch:
 			return self.resources_db[rid]
 		c = self.sql.cursor()
@@ -1060,15 +1306,15 @@
 		c.execute('''SELECT tag_value FROM file_tags where fid = ?;''', [fid])
 		tags_results = c.fetchall()
 		c.execute('''SELECT info_key, info_value FROM file_info where fid = ?;''', [fid])
 		info_results = c.fetchall()
 		c.execute('''SELECT tid FROM tasks_outputfiles where fid = ?;''', [fid])
 		task_results = c.fetchall()
 		if len(results) != 1:
-			raise Exception()
+			raise Exception("Error in getting files: " + fid)
 		if len(task_results) > 1:
 			raise Exception()
 		elif len(task_results) == 1:
 			tid, = task_results[0]
 		else:
 			tid = None
 		r = results[0]
@@ -1100,15 +1346,14 @@
 		if tid in self.tasks_db and not refetch:
 			return self.tasks_db[tid]
 		c = self.sql.cursor()
 		c.execute('''SELECT * FROM tasks where tid = ?;''', [tid])
 		results = c.fetchall()
 		if len(results) != 1:
 			raise Exception()
-
 		c.execute('''SELECT tag_value FROM task_tags where tid = ?;''', [tid])
 		tags_results = c.fetchall()
 		c.execute('''SELECT info_key, info_value FROM task_info where tid = ?;''', [tid])
 		info_results = c.fetchall()
 		
 		c.execute('''SELECT arg_order, arg_value FROM tasks_args_json where tid = ?;''', [tid])
 		args_json = [(arg_order, json.loads(arg_value)) for arg_order, arg_value in c.fetchall()]
@@ -1249,43 +1494,67 @@
 	# Users run a task #
 	####################
 	def compute_output_files(self, pipe, func_args, func_kwargs):
 		output_file_paths = pipe.output_func(*func_args, **func_kwargs) if pipe.output_func is not None else []
 		output_file_paths = [os.path.abspath(path) for path in output_file_paths] 
 		return output_file_paths
 	
+	def exist_output_files(self, output_files):
+		overlapped_fids = []
+		for output_file in output_files:
+			c = self.sql.cursor()
+			c.execute('''SELECT fid FROM files where file_path = ?;''', [output_file])
+			overlapped_fids.extend([fid for fid, in c.fetchall()])
+		return len(overlapped_fids) > 0
 	
-	
-	def register_finished_task(self, raw_return_value, begin_time, end_time, ba, pipe, 
-							task_description="", task_tags=[], task_info={},
-							resource_description="", resource_tags=[], resource_info={},
-							fileresource_description="", fileresource_tags=[], fileresource_info={}):
-		'''
-		Register a finished task, assuming the task has completed successfully. 
-		'''
+	def _compile_files_md5_from_pipe_ba(self, pipe, ba):
 		func_args, func_kwargs = self._ba_rms_to_func_args_kwargs(ba)
-		
 		# Check for output files
 		output_file_paths = pipe.output_func(*func_args, **func_kwargs) if pipe.output_func is not None else []
 		output_file_paths = [os.path.abspath(path) for path in output_file_paths] 
 		problematic_paths = [p for p in output_file_paths if not os.path.exists(p)]
 		if len(problematic_paths) > 0:
 			print("Warning: the following output files are not detected:")
 			print(problematic_paths)
 			output_file_paths = [p for p in output_file_paths if os.path.exists(p)]
-			
+		return OrderedDict([[file_path,_get_file_md5(file_path)] for file_path in output_file_paths])
+	def register_finished_task(self, raw_return_value, begin_time, end_time, ba, pipe, 
+							task_description="", task_tags=[], task_info={},
+							resource_description="", resource_tags=[], resource_info={},
+							fileresource_description="", fileresource_tags=[], fileresource_info={},
+							precompiled_files_md5=None
+							):
+		'''
+		Register a finished task, assuming the task has completed successfully. 
+		'''
+# 		func_args, func_kwargs = self._ba_rms_to_func_args_kwargs(ba)
+# 		
+# 		# Check for output files
+# 		output_file_paths = pipe.output_func(*func_args, **func_kwargs) if pipe.output_func is not None else []
+# 		output_file_paths = [os.path.abspath(path) for path in output_file_paths] 
+# 		problematic_paths = [p for p in output_file_paths if not os.path.exists(p)]
+# 		if len(problematic_paths) > 0:
+# 			print("Warning: the following output files are not detected:")
+# 			print(problematic_paths)
+# 			output_file_paths = [p for p in output_file_paths if os.path.exists(p)]
+# 			
+		if precompiled_files_md5 is None:
+			file_path_md5_dict = self._compile_files_md5_from_pipe_ba(pipe, ba)
+		else:
+			file_path_md5_dict = precompiled_files_md5
+		output_file_paths = list(file_path_md5_dict.keys())
 		return_value_rid = self._get_new_id()
 		output_file_fids = [self._get_new_id() for _ in output_file_paths]
 		tid = self._get_new_id()
 		
 		# Create resource, fileresource and task
 		new_resources = [Resource(return_value_rid, tid, pipe.return_volatile, resource_description, resource_tags, resource_info, raw_return_value)]
 		
-		new_fileresources = [FileResource(fid, tid, file_path, _get_file_md5(file_path), fileresource_description, fileresource_tags, fileresource_info) for fid, file_path in zip(output_file_fids, output_file_paths)]
-
+# 		new_fileresources = [FileResource(fid, tid, file_path, _get_file_md5(file_path), fileresource_description, fileresource_tags, fileresource_info) for fid, file_path in zip(output_file_fids, output_file_paths)]
+		new_fileresources = [FileResource(fid, tid, file_path, file_path_md5_dict[file_path], fileresource_description, fileresource_tags, fileresource_info) for fid, file_path in zip(output_file_fids, output_file_paths)]
 		task = Task(tid, pipe.pid, ba.args, ba.kwargs, new_resources, new_fileresources, begin_time, end_time, task_description, task_tags, task_info)
 		
 		# Find files that are overwritten
 		# Even if deprecated, it should be marked overwritten
 		old_fids = []
 		for fileresource in new_fileresources:
 			c = self.sql.cursor()
@@ -1351,15 +1620,18 @@
 			return prev_tasks[0].return_values[0]
 		
 		# Conversion to func_args and func_kwargs
 		func_args, func_kwargs = self._ba_rms_to_func_args_kwargs(ba)
 		
 		# Generate output files, this step ensures that the output func works 
 		output_files = self.compute_output_files(pipe, func_args, func_kwargs)
-		
+		if not self.allow_overwrite:
+			if self.exist_output_files(output_files):
+				raise Exception()
+
 		# Add task info
 		if self.scriptID is not None:
 			task_info = {"scriptid":self.scriptID, **task_info}
 		begin_time = datetime.datetime.now()
 		raw_return_value = pipe.func(*func_args, **func_kwargs)
 		end_time = datetime.datetime.now()
 		
@@ -1380,46 +1652,52 @@
 		ba = _get_func_ba(pipe.func, args, kwargs)
 		func_args, func_kwargs = self._ba_rms_to_func_args_kwargs(ba)
 		return pipe.func(*func_args, **func_kwargs)
 
 	def replace_virtualresource(self, virtualresource, resource):
 		'''
 		Replace a virtual resource with the desired resource.
+		Can also replace a virtual filresource with the desired fileresource
 		
 		Should change it to use replace_unruntask_rmsobj 
 		'''
 		virtualresource.replacement = resource
+		self.fireRMSUpdateEvent([(RMSUpdateEvent.REPLACE, virtualresource.get_full_id())])
 		for unruntask in self.find_downstream_objs([virtualresource], 1):
 			original_kv = list(unruntask.ba.arguments.items())
 			for k, v in original_kv:
 				if unruntask.ba.signature.parameters[k].kind == inspect.Parameter.VAR_POSITIONAL:
 					unruntask.ba.arguments[k] = [resource if (isinstance(i, RMSEntry) and i is virtualresource) else i for i in v]
 				elif unruntask.ba.signature.parameters[k].kind == inspect.Parameter.VAR_KEYWORD:
 					unruntask.ba.arguments[k] = {ik:(resource if (isinstance(i, RMSEntry) and i is virtualresource) else i) for ik, i in v.items()}
 				else:
 					if isinstance(v, RMSEntry):
 						if v is virtualresource:
 							unruntask.ba.arguments[k] = resource
-		self.delete(virtualresource.get_full_id())
+		#Temp disable
+# 		self.delete(virtualresource.get_full_id())
 		
 	def replace_unruntask(self, unruntask, task):
 		'''
 		Update all associated virtual resources  
 		'''
 		if unruntask.return_values is not None:
 			if len(task.return_values) == len(unruntask.return_values):
 				for vr, r in zip(unruntask.return_values, task.return_values):
 					self.replace_virtualresource(vr, r)
 		if unruntask.output_files is not None:
 			if len(task.output_files) == len(unruntask.output_files):
 				for vr, r in zip(unruntask.output_files, task.output_files):
 					self.replace_virtualresource(vr, r)
+					
 		
 		unruntask.replacement = task
-		self.delete(unruntask.get_full_id())
+		self.fireRMSUpdateEvent([(RMSUpdateEvent.REPLACE, unruntask.get_full_id())])
+		# Temp disable
+		#self.delete(unruntask.get_full_id())
 
 	def run_unruntask(self, unruntask):
 		pipe = self.get_pipe(unruntask.pid)
 		ba = unruntask.ba
 		prev_tasks = self.find_tasks_by_pipe_and_args(pipe.pid, ba.args, ba.kwargs)
 		if len(prev_tasks) > 0:
 			print("The task has been done before.")
@@ -1435,14 +1713,40 @@
 											unruntask.task_description, unruntask.task_tags, unruntask.task_info,
 											unruntask.resource_description, unruntask.resource_tags, unruntask.resource_info,
 											unruntask.fileresource_description, unruntask.fileresource_tags, unruntask.fileresource_info)
 		
 		self.replace_unruntask(unruntask, task)
 		return task.return_values[0]
 	
+	def create_template_job(self, func, args, kwargs):
+		tpid = self._get_new_id()
+		return RMSTemplateJob(tpid, func, args, kwargs)
+	
+	def run_template_job(self, template_job):
+		'''
+		This involves running multiple steps in a function
+		'''
+		template_job.status = RMSTemplateJobStatus.RUNNING
+# 		try:
+		template_job.func(self, *template_job.args, **template_job.kwargs)
+		template_job.status = RMSTemplateJobStatus.COMPLETE
+		return template_job 
+# 		except:
+# 			print("Here")
+# 			template_job.status = RMSTemplateJobStatus.ERROR
+		
+	def run_template(self, func, args=[], kwargs={}):
+		job = self.create_template_job(func, args, kwargs)
+		return self.run_template_job(job)
+		
+	def simulate_template(self, func, args=[], kwargs={}):
+		simulator = TemplateSimulator()
+		func(simulator, *args, **kwargs)
+		return simulator.get_result()
+	
 	def run_unruntask_chain(self, unruntask):
 		for vr in unruntask.input_virtualresources:
 			prev_unruntasks = self.find_upstream_objs([vr], 1)
 			if len(prev_unruntasks) > 1:
 				assert False
 			if len(prev_unruntasks) == 0:
 				print("Cannot fetch virtual task: " + vr.get_id())
@@ -1485,27 +1789,40 @@
 		ba = _get_func_ba(pipe.func, args, kwargs, partial=True)
 		ut = UnrunTask(uid, pid, ba, return_values, output_files,
 					task_description, task_tags, task_info,
 					resource_description, resource_tags, resource_info,
 					fileresource_description, fileresource_tags, fileresource_info
 					)
 		
-				
+		for vr in return_values:
+			vr.uid = uid
+		if output_files is not None:
+			for vr in output_files:
+				vr.uid = uid
 		self.unruntasks_db[uid] = ut
+		self.fireRMSUpdateEvent([(RMSUpdateEvent.INSERT, ut.get_full_id())])
 		return ut
+	
 	def create_unruntask_from_task(self, task, return_values=[], output_files=[]):
 		uid = self._get_new_id()
 		ba = _get_func_ba(self.get_pipe(task.pid).func, task.args, task.kwargs, partial=True)
 		unruntask = UnrunTask(uid, task.pid, ba, return_values, output_files)
 		self.unruntasks_db[uid] = unruntask
 		return unruntask
 	def create_virtualresource(self):
 		vid = self._get_new_id()
-		vr = VirtualResource(vid, None, None, None, None, None)
+		vr = VirtualResource(vid)
+		self.virtualresources_db[vid] = vr
+		self.fireRMSUpdateEvent([(RMSUpdateEvent.INSERT, vr.get_full_id())])
+		return vr
+	def create_virtualfileresource(self, file_path):
+		vid = self._get_new_id()
+		vr = VirtualResource(vid, file_path)
 		self.virtualresources_db[vid] = vr
+		self.fireRMSUpdateEvent([(RMSUpdateEvent.INSERT, vr.get_full_id())])
 		return vr
 	def create_unruntask_chain(self, args):
 		rmsobjs = list(map(self._as_rmsobj, args))
 		
 		newobjs = []
 		
 		g = self.construct_digraph_from_rmsids(rmsobjs)
@@ -1559,15 +1876,35 @@
 				newobjs.append(unruntask)
 			else:
 				pass
 		
 		self.fireRMSUpdateEvent([(RMSUpdateEvent.INSERT, rmsobj.get_full_id()) for rmsobj in newobjs])
 		return newobjs
 					
-	
+	def _guess_unruntask_output(self, unruntask):
+		'''
+		Based on the current parameter of unruntask, guess the output of the unruntask by adding default or None to missing parameters
+		'''
+		if self.get_pipe(unruntask.pid).output_func is None:
+			return []
+		ba = unruntask.ba.signature.bind_partial(*unruntask.ba.args, **unruntask.ba.kwargs)
+		for p, param in unruntask.ba.signature.parameters.items():
+			if param.kind == inspect.Parameter.VAR_POSITIONAL or param.kind == inspect.Parameter.VAR_KEYWORD:
+				continue
+			if p not in ba.arguments:
+				if param.default is param.empty:
+					ba.arguments[p] = None
+				else:
+					ba.arguments[p] = param.default
+		try:
+			potential_output_files = self.get_pipe(unruntask.pid).output_func(*ba.args, **ba.kwargs)
+			return potential_output_files
+		except:
+			return []
+		
 	def mark_deprecated(self, rmsobj, mark_downstream=True):
 		'''
 		Mark a rmsobj as deprecated. 
 		All downstream rmsobjs will be marked as deprecated too.
 		
 		
 		'''
@@ -1737,15 +2074,15 @@
 		if namespace is None:
 			namespace = dict()
 		if moduleobj is None:
 			moduleobj = "builtins"
 
 		# There are two ways to add bound_method. 
 		# 1. If the class is already registered, set the bound method as the class attr
-		# 2. If the class is not registered, set the class as another virtual module 
+		# 2. If the class is not registered, set the class as another virtual module
 		bound_method_classes = defaultdict(list)
 		for p in pipes:
 			if inspect.ismethod(p.func):
 				if inspect.isclass(p.func.__self__):
 					bound_method_classes[p.func.__self__].append(p)
 		
 	
@@ -1797,15 +2134,14 @@
 							i = k.__name__
 							if i not in to_add:
 								to_add[i] = VirtualModule()
 							for bound_method in bound_methods:
 								setattr(to_add[i], bound_method.func.__name__, bound_method)
 				namespace[altname] = types.SimpleNamespace(**d, **to_add)
 				returnvalue = namespace[altname]
-
 				
 		# Import the variable
 		else:
 			output_pipes = []
 			# wild card case
 			if varname == "*":
 				tmp_returnvalues = {}
@@ -2102,16 +2438,16 @@
 		if len(funcs) > 0:
 			modules.add("dill")
 			
 		print("# The codes are auto-generated from the RMS. Please refer to the original pipeline for details")
 		print("###########")
 		print("# Imports #")
 		print("###########")
-		print(f"from rpms import newrms")
-		print(f'rmsp = newrms.ResourceManagementSystem("/local/storage/kl945/RMS/New_RMS.db", "/local/storage/kl945/RMS/")')
+		print(f"from rmsp import rmscore")
+		print(f'rmsp = rmscore.ResourceManagementSystem("/path/to/test.db", "/path/to/")')
 		print()
 		print("#############")
 		print("# Pipelines #")
 		print("#############")
 		for code in codes:
 			print(code)
 		print()
```

### Comparing `rmsp-0.0.1/rmsp/rmsutils.py` & `rmsp-0.0.9/rmsp/rmsutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-'''
-Created on Aug 7, 2021
-
-@author: kl945
-'''
 
 import os
 import shutil
 import glob
 import uuid
 import sqlite3
 from .rmscore import ResourceManagementSystem
@@ -443,26 +438,27 @@
 		for s in br:
 			fname, fmd5, fid = s.split("\t")
 			entries[fid] = fname, fmd5, fid 
 	return dbid, entries 
 		
 		
 		
-def export_files_to_directory(self, o, *target_files, directorymode='common', rootdirectory='.',):
+def export_files_to_directory(self, o, *target_files, directorymode='common', rootdirectory='.', override_deprecated_files=False):
 	'''
 	Export files from a database to the target directory. 
 	
 	Directory mode: Can be common, root, or basename
 	
 	'''
 		
 	dbid, = self.sql.cursor().execute("SELECT infovalue FROM metainfo WHERE infokey = 'dbid'").fetchone()
 	frs = [self.file_from_path(f) for f in target_files]
 	abspaths = [fr.file_path for fr in frs]
 	
+	print(f"Checking {len(target_files)} files...")
 	# Compile relative path for target_files
 	target_file_dict = None
 	if directorymode == 'common':
 		common_path = os.path.commonpath(abspaths)
 		if not os.path.isdir(common_path):
 			common_path = os.path.dirname(common_path)
 		target_file_dict = {p: os.path.relpath(p, common_path) for p in abspaths}
@@ -478,14 +474,15 @@
 	if len(dup_alt_file_names) > 0:
 		raise Exception("Duplicated file names detected. If you are using directorymode 'basename', consider using other directorymode")
 	
 	# Read the old RMS metainfo file
 	f = os.path.abspath(o + "/" + "RMS_metainfo.txt")
 	if os.path.exists(f):
 		old_dbid, old_entries = _read_meta_info(f)
+		print(f"There are {len(old_entries)} old entries exported.")
 		if old_dbid != dbid:
 			raise Exception(f"The DB IDs are different: {old_dbid} and {dbid}")
 	else:
 		old_entries = {}
 	
 	# Build the current entries
 	entries = {}
@@ -493,50 +490,72 @@
 		entries[fr.fid] = target_file_dict[fr.file_path], fr.md5, fr.fid
 		
 	# Check for inconsistency in old and current entries
 	for fname, fmd5, fid in entries.values():
 		if fid in old_entries:
 			ofname, ofmd5, ofid = old_entries[fid]
 			if fname != ofname or fmd5 != ofmd5:
-				raise Exception(f"Inconsistent file: {fid}")
+				raise Exception(f"Inconsistent file: {fid}" + f"\n{fname}, {ofname}, {fmd5}, {ofmd5}")
+	
+	# Check for deprecated, overlapping entries (by file path)
+	deprecated_entries_to_replace = {} # (old fid: new fid)
+	old_entries_by_fname = {ofname: (ofname, ofmd5, ofid) for ofname, ofmd5, ofid in old_entries.values()}
+	for fname, fmd5, fid in entries.values():
+		if fid not in old_entries:
+			if fname in old_entries_by_fname:
+				ofid = old_entries_by_fname[fname][2]
+				if "overwritten" in self.get_fileresource(ofid).info or "deprecated" in self.get_fileresource(ofid).info: 
+					deprecated_entries_to_replace[ofid] = fid
+	if len(deprecated_entries_to_replace) > 0:
+		if not override_deprecated_files:
+			raise Exception("Deprecated files exist. Change override_deprecated_files to True if you want to replace the entries\n" + "\n".join([old_entries[ofid][0] for ofid in deprecated_entries_to_replace])) 
+		print(f"There are {len(deprecated_entries_to_replace)} deprecated/overwritten files to be replaced...")
+		
 	# Create the metainfo file
 	metainfo_file = tempfile.NamedTemporaryFile(mode='w+', suffix=".txt", delete=False).name
 	with open(metainfo_file, 'w') as fw:
 		fw.write(f"## RMS_DB_ID: {dbid}\n")
 		fw.write(f"#File\tMD5\tRMS_File_ID\n")
 		
 		for fname, fmd5, fid in old_entries.values():
+			if fid in deprecated_entries_to_replace:
+				continue
 			fw.write(f"{fname}\t{fmd5}\t{fid}\n")
 		for fname, fmd5, fid in entries.values():
 			if fid in old_entries:
 				continue
 			fw.write(f"{fname}\t{fmd5}\t{fid}\n")
 
 	
 	# Also add the metainfo file to the dict
 	target_file_dict[metainfo_file] = 'RMS_metainfo.txt'
 	
 	# Update the target file dict
 	target_file_dict = {target_file: os.path.abspath(o + "/" + alt_file_name) for target_file, alt_file_name in target_file_dict.items()}
 	
-	# Check if file exists
+	
+	# Check if file exists to avoid overwritting important files. 
+	# Deprecated files to be replaced do not count towards existing files.
+	if len(deprecated_entries_to_replace) > 0:
+		fids_to_replace_deprecated_entries = set(deprecated_entries_to_replace.values())
+	else:
+		fids_to_replace_deprecated_entries = set()
 	existing_files = []
 	for fr in frs:
 		if fr.fid in old_entries:
 			target_file_dict.pop(fr.file_path)
 		else:
 			if os.path.exists(target_file_dict[fr.file_path]):
-				existing_files.append(target_file_dict[fr.file_path])
-				
+				if fr.fid not in fids_to_replace_deprecated_entries:
+					existing_files.append(target_file_dict[fr.file_path])
 	if len(existing_files) > 0:
 		raise Exception("File(s) exist.\n" + "\n".join(existing_files))
-	print(f"Checking {len(target_files)} files")
-	print(f"There are {len(old_entries)} old entries in last export.")
+
+	# Export the files	
 	print(f"Exporting {len(target_file_dict) - 1} entries...")
-	
 	for src, dst in target_file_dict.items():
 		os.makedirs(os.path.dirname(dst), exist_ok=True)
 		shutil.copyfile(src, dst)
 	shutil.copyfile(src, dst)
 	
 	# remove the temp metainfo file
 	os.unlink(metainfo_file)
```

### Comparing `rmsp-0.0.1/rmsp.egg-info/PKG-INFO` & `rmsp-0.0.9/rmsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: rmsp
-Version: 0.0.1
+Version: 0.0.9
 Summary: Resource management system for python
 Home-page: https://github.com/aldenleung/rmsp/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 
 # Resource Management System (RMS) Manual
@@ -25,30 +27,20 @@
 
 RMS record most common python functions and objects, and avoid duplicated jobs. Minimal efforts are needed from the users to avoid repeated jobs.  
 
 ### Effortless incorporation to existing pipelines
 
 Rebuilding an entire analysis into the new system is usually a big hurdle, but not in RMS. RMS provides a simple solution - you can keep using most of your codes in the main body. The only thing to do is to change the import functions.
 
-### Flexible interface for both programmers and non-programmers
 
-TBW
-
-### Multi-processing support on different tasks
-
-TBW
 
 ### Easy but powerful search
 
 Many systems allow you to find out an upstream file required to generate the results. However, not all systems allow more complicated search. For example, can we search for the results based on some input file 1 and input file 2, processed through either pipeline X with the parameter A or pipeline Y with parameter B? Can we find out peak files using peak calling software J with alignment based on alignment software K? RMS enables these searches so that you can always retrieve your results quickly
 
-### Tracking multiple conda environment in bash
-
-TBW
-
 ### Easy Backup / Restore
 
 Backup / Restore is an essential feature to protect a database system from data loss. The core RMS files include all the pipelines used, which are stored in an SQL database. It also allows users to select and backup various files or resource content (For example, only backup the raw file and key result file, and remove any intermediate files). Restoring a database requires. 
 
 ### Integrity check
 
 Since RMS uses the absolute path to link to a file, users could easily access the file as for any downstream analysis or visualization. Users can also move or delete any unused intermediate files. Just like Python culture, nothing prevents you from modifying a file if you really do so. We encourage users to be responsible for their own actions. However, RMS will still do a quick check (based on file size) before using the file. An optional integrity check based on MD5 is also available. 
@@ -56,15 +48,15 @@
 
 
 ## Installation
 
 To install Resource Management System, use the following:
 
 ```python
-pip install resource_management_system
+pip install rmsp
 ```
 
 
 
 ## Quick Start
 
 ### Try-it-out for the first time
@@ -560,28 +552,18 @@
 rmsutils.restore('src_path', 'target_path')
 ```
 
 
 
 ## User Guide - GUI
 
-The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding. 
-
-TBW
-
-### Template
-
-TBW
-
-### Extension
-
-TBW
-
-
+The GUI is useful to visualize all your tasks, files and resources. It allows instant analysis to certain variables. The template system also allows you to run simple analysis if you are unfamiliar with coding.  Please refer to rmsp-gui for details
 
 ## FAQ / Important Notes
 
 This section includes some of the important notes that one should keep in mind when using RMS. 
 
 - RMS does not store any information about the environment. It does not keep track of any external executables. Rather, it basically relies on the conda environment. Hence when doing the backup / restore, make sure you also backup the environment yourself. 
 
 
+
+
```

### Comparing `rmsp-0.0.1/setup.py` & `rmsp-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
-requirements = ["python-dateutil", "dill", "networkx"]
+requirements = ["python-dateutil", "dill", "networkx", "psutil", "requests"]
 
 setup(
 	name="rmsp",
-	version="0.0.1",
+	version="0.0.9",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="Resource management system for python",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/rmsp/",
 	packages=find_packages(),
```

