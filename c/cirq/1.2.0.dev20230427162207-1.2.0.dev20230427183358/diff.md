# Comparing `tmp/cirq-1.2.0.dev20230427162207-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230427183358-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7970 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 16:22 cirq-1.2.0.dev20230427162207.dist-info/LICENSE
--rw-r--r--  2.0 unx     7771 b- defN 23-Apr-27 16:22 cirq-1.2.0.dev20230427162207.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 16:22 cirq-1.2.0.dev20230427162207.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-27 16:22 cirq-1.2.0.dev20230427162207.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      461 b- defN 23-Apr-27 16:22 cirq-1.2.0.dev20230427162207.dist-info/RECORD
-5 files, 19682 bytes uncompressed, 7100 bytes compressed:  63.9%
+Zip file size: 7974 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 18:34 cirq-1.2.0.dev20230427183358.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7781 b- defN 23-Apr-27 18:34 cirq-1.2.0.dev20230427183358.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 18:34 cirq-1.2.0.dev20230427183358.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-27 18:34 cirq-1.2.0.dev20230427183358.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      461 b- defN 23-Apr-27 18:34 cirq-1.2.0.dev20230427183358.dist-info/RECORD
+5 files, 19692 bytes uncompressed, 7104 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: cirq-1.2.0.dev20230427162207.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230427183358.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230427162207.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230427183358.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230427162207.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230427183358.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230427162207.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230427183358.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.2.0.dev20230427162207.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230427183358.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230427162207.dist-info/LICENSE` & `cirq-1.2.0.dev20230427183358.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230427162207.dist-info/METADATA` & `cirq-1.2.0.dev20230427183358.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230427162207
+Version: 1.2.0.dev20230427183358
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-core (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-google (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230427162207)
-Requires-Dist: cirq-web (==1.2.0.dev20230427162207)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-core (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-google (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230427183358)
+Requires-Dist: cirq-web (==1.2.0.dev20230427183358)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
 Requires-Dist: pytest ; extra == 'dev_env'
@@ -154,15 +154,15 @@
 
 We welcome contributions! Before opening your first PR, a good place to start is to read our
 `guidelines <https://github.com/quantumlib/cirq/blob/master/CONTRIBUTING.md>`__.
 
 We are dedicated to cultivating an open and inclusive community to build software for near term quantum computers.
 Please read our `code of conduct <https://github.com/quantumlib/cirq/blob/master/CODE_OF_CONDUCT.md>`__ for the rules of engagement within our community.
 
-For real time informal discussions about Cirq, join our `cirqdev <https://gitter.im/cirqdev>`__ Gitter channel, come hangout with us!
+For real time informal discussions about Cirq, join our `cirqdev <https://gitter.im/cirqdev/community>`__ Gitter channel, come hangout with us!
 
 **Cirq Cynque** is our weekly meeting for contributors to discuss upcoming features, designs, issues, community and status of different efforts.
 To get an invitation please join the `cirq-dev email list <https://groups.google.com/forum/#!forum/cirq-dev>`__ which also serves as yet another platform to discuss contributions and design ideas.
 
 
 See Also
 --------
```

