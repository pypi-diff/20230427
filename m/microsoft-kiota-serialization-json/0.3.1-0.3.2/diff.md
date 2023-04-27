# Comparing `tmp/microsoft-kiota-serialization-json-0.3.1.tar.gz` & `tmp/microsoft-kiota-serialization-json-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-serialization-json-0.3.1.tar", last modified: Thu Mar 30 13:05:10 2023, max compression
+gzip compressed data, was "microsoft-kiota-serialization-json-0.3.2.tar", last modified: Thu Apr 27 15:39:12 2023, max compression
```

## Comparing `microsoft-kiota-serialization-json-0.3.1.tar` & `microsoft-kiota-serialization-json-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0       82 2023-03-30 13:05:06.752439 microsoft-kiota-serialization-json-0.3.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-03-30 13:05:06.752439 microsoft-kiota-serialization-json-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-03-30 13:05:06.752439 microsoft-kiota-serialization-json-0.3.1/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1870 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/.gitignore
--rw-r--r--   0        0        0    15958 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/.pylintrc
--rw-r--r--   0        0        0      663 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/LICENSE
--rw-r--r--   0        0        0      350 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/Pipfile
--rw-r--r--   0        0        0    35220 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/README.md
--rw-r--r--   0        0        0     2757 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    10250 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1433 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    17554 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0       67 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      105 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/helpers/office_location.py
--rw-r--r--   0        0        0     5681 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/helpers/user.py
--rw-r--r--   0        0        0        0 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     5885 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1678 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     6947 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1101 2023-03-30 13:05:06.756439 microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft-kiota-serialization-json-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1870 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.gitignore
+-rw-r--r--   0        0        0    15976 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.pylintrc
+-rw-r--r--   0        0        0      775 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/LICENSE
+-rw-r--r--   0        0        0      350 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/Pipfile
+-rw-r--r--   0        0        0    35877 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/README.md
+-rw-r--r--   0        0        0     2757 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    10526 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1433 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    17554 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1710 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/entity.py
+-rw-r--r--   0        0        0      105 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     5687 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/user.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5926 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1678 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     6947 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1101 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft-kiota-serialization-json-0.3.2/PKG-INFO
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/.github/workflows/auto-merge-dependabot.yml` & `microsoft-kiota-serialization-json-0.3.2/.github/workflows/auto-merge-dependabot.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.3.6
+        uses: dependabot/fetch-metadata@v1.4.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/.github/workflows/build_publish.yml` & `microsoft-kiota-serialization-json-0.3.2/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/.github/workflows/codeql-analysis.yml` & `microsoft-kiota-serialization-json-0.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/.github/workflows/conflicting-pr-label.yml` & `microsoft-kiota-serialization-json-0.3.2/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/.gitignore` & `microsoft-kiota-serialization-json-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/.pylintrc` & `microsoft-kiota-serialization-json-0.3.2/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -511,9 +511,9 @@
 preferred-modules=
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "BaseException, Exception".
-overgeneral-exceptions=BaseException,
-                       Exception
+overgeneral-exceptions=builtins.BaseException,
+                       builtins.Exception
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/CHANGELOG.md` & `microsoft-kiota-serialization-json-0.3.2/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.2] - 2023-04-27
+
+### Added
+
+### Changed
+
+- Fixed a bug with deserializing models with additional data.
+
 ## [0.3.1] - 2023-03-20
 
 ### Added
 
 ### Changed
 
 - Fixed a bug with deserializing bytes responses.
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/LICENSE` & `microsoft-kiota-serialization-json-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/Pipfile.lock` & `microsoft-kiota-serialization-json-0.3.2/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9595588235294118%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'f1900de773732b7c88935c182f6612df050dab20b558bcda2311cd66c1e9bdda'}}",*

 * * "'develop'": "{'astroid': {'hashes': "*

 * *              "['sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347', "*

 * *              "'sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8'], "*

 * *              "'version': '==2.15.4'}, 'charset-normalizer': {'markers': "*

 * *              '"python_full_version >= \'3.7.0\'"}, \'coverage\': {\'hashes\': '*

 * *            […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "39b636818e450d9efbbdc3d3da92b38e3eb3a3ae618ecffe9f90309730f2209c"
+            "sha256": "f1900de773732b7c88935c182f6612df050dab20b558bcda2311cd66c1e9bdda"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -46,27 +46,19 @@
             "markers": "python_version >= '3.6'",
             "version": "==4.1.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:89860bda98fe2bbd1f5d262229be7629d778ce280de68d95d4a73d1f592ad268",
-                "sha256:af4e0aff46e2868218502789898269ed95b663fba49e65d91c1e09c966266c34"
+                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
+                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.1"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "version": "==2.15.4"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
@@ -146,93 +138,109 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
+        "colorama": {
+            "hashes": [
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
+            ],
+            "markers": "sys_platform == 'win32'",
+            "version": "==0.4.6"
+        },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
-                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
-                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
-                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
-                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
-                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
-                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
-                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
-                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
-                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
-                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
-                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
-                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
-                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
-                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
-                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
-                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
-                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
-                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
-                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
-                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
-                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
-                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
-                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
-                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
-                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
-                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
-                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
-                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
-                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
-                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
-                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
-                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
-                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
-                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
-                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
-                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
-                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
-                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
-                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
-                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
-                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
-                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
-                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
-                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
-                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
-                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
-                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
-                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
-                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
-                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.2"
+            "version": "==7.2.3"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19"
         },
+        "exceptiongroup": {
+            "hashes": [
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==1.1.1"
+        },
         "flit": {
             "hashes": [
                 "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
                 "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
             ],
             "index": "pypi",
             "version": "==3.8.0"
@@ -317,139 +325,147 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5",
-                "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598",
-                "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5",
-                "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389",
-                "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a",
-                "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9",
-                "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78",
-                "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af",
-                "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f",
-                "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4",
-                "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c",
-                "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2",
-                "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e",
-                "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1",
-                "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51",
-                "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f",
-                "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a",
-                "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54",
-                "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f",
-                "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5",
-                "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707",
-                "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b",
-                "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b",
-                "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c",
-                "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799",
-                "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"
+                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
+                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
+                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
+                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
+                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
+                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
+                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
+                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
+                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
+                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
+                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
+                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
+                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
+                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
+                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
+                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
+                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
+                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
+                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
+                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
+                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
+                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
+                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
+                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
+                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
+                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
             ],
             "index": "pypi",
-            "version": "==1.1.1"
+            "version": "==1.2.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a",
+                "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.4.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:8660a54e3f696243d644fca98f79013a959c03f979992c1ab59c24d3f4ec2700",
-                "sha256:d4d009b0116e16845533bc2163493d6681846ac725eab8ca8014afb520178ddd"
+                "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5",
+                "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"
             ],
             "index": "pypi",
-            "version": "==2.17.1"
+            "version": "==2.17.3"
         },
         "pytest": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.3.1"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "index": "pypi",
             "version": "==4.0.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
+                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.29.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "tomli-w": {
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
-                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.7"
+            "version": "==0.11.8"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:357553f8056cfbb8ce8ea0ca4a6a3480268596748360df73a94c2b8c113a5b06",
-                "sha256:de66222c54318c2e05ceb4956976d16696240a45fc2c98e54bfe9a56ce5e1eff"
+                "sha256:355b2cb82b31e556fd18e7b074de7c350c680ab80608f0cc55ba6770d986d67d",
+                "sha256:fe5b545e678ec13e3ddc83a0eee1545c1b5e2fba4cfc39b276ab6f4e7604a923"
             ],
             "index": "pypi",
-            "version": "==2.8.19.11"
+            "version": "==2.8.19.12"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
@@ -537,20 +553,20 @@
                 "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
                 "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
                 "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
                 "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
                 "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:8fea849025584e486fd06d6ba2bed717f396080fd3cc236ba10cb97c4c51cf32",
-                "sha256:a3f5085d37ef7e3e004c4ba9f9b3e40c54ff1901cd111f05145ae313a7c67d1b"
+                "sha256:4c2b59bd5ffe46f3a7da48df87596877189148226ce267c16e8b44240e51578d",
+                "sha256:da62bdfea3df3673553351e6246abed26d9fe6780e548a5af9e70f6d2b4f5b9a"
             ],
             "index": "pypi",
-            "version": "==0.32.0"
+            "version": "==0.33.0"
         }
     }
 }
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/README.md` & `microsoft-kiota-serialization-json-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/SECURITY.md` & `microsoft-kiota-serialization-json-0.3.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/SUPPORT.md` & `microsoft-kiota-serialization-json-0.3.2/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_parse_node.py` & `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import base64
 import json
 import re
+import warnings
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 from typing import Any, Callable, Dict, Generic, List, Optional, Type, TypeVar
 from uuid import UUID
 
 from dateutil import parser
 from kiota_abstractions.serialization import (
@@ -265,24 +266,32 @@
         Args:
             value (Callable[[Parsable], None]): the callback called after the node is
             deserialized.
         """
         self.on_after_assign_field_values = value
 
     def _assign_field_values(self, item: U) -> None:
-        fields = item.get_field_deserializers()
-
-        if isinstance(item, AdditionalDataHolder):
-            item_additional_data = item.additional_data
 
         object_dict = self._json_node
+
+        item_additional_data = None
+
         # if object is null
         if not object_dict:
             return
 
+        if isinstance(item, AdditionalDataHolder):
+            item_additional_data = item.additional_data
+
+        field_deserializers = item.get_field_deserializers()
+
         for key, val in object_dict.items():
-            deserializer = fields.get(key)
+            deserializer = field_deserializers.get(key)
             if deserializer:
                 deserializer(JsonParseNode(val))
-            else:
-                # if item_additional_data:
+            elif item_additional_data is not None:
                 item_additional_data[key] = val
+            else:
+                warnings.warn(
+                    f"Found additional property {key} to \
+                    deserialize but the model doesn't support additional data"
+                )
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_parse_node_factory.py` & `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_serialization_writer.py` & `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/pyproject.toml` & `microsoft-kiota-serialization-json-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/tests/helpers/user.py` & `microsoft-kiota-serialization-json-0.3.2/tests/helpers/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,27 +136,27 @@
         Returns:
             Dict[str, Callable[[ParseNode], None]]: The deserialization information for this
             object where each entry is a property key with its deserialization callback.
         """
         return {
             "id":
             lambda n: setattr(self, 'id', n.get_uuid_value()),
-            "displayName":
+            "display_name":
             lambda n: setattr(self, 'display_name', n.get_str_value()),
-            "officeLocation":
+            "office_location":
             lambda n: setattr(self, 'office_location', n.get_enum_value(OfficeLocation)),
-            "updatedAt":
+            "updated_at":
             lambda n: setattr(self, 'updated_at', n.get_datetime_value()),
             "birthday":
             lambda n: setattr(self, 'birthday', n.get_date_value()),
-            "businessPhones":
+            "business_phones":
             lambda n: setattr(self, 'business_phones', n.get_collection_of_primitive_values(str)),
-            "mobilePhone":
+            "mobile_phone":
             lambda n: setattr(self, 'mobile_phone', n.get_str_value()),
-            "isActive":
+            "is_active":
             lambda n: setattr(self, 'is_active', n.get_bool_value()),
             "age":
             lambda n: setattr(self, 'age', n.get_int_value()),
             "gpa":
             lambda n: setattr(self, 'gpa', n.get_float_value())
         }
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_parse_node.py` & `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 import json
+from dataclasses import asdict,dataclass
 from datetime import date, datetime, time, timedelta
 from uuid import UUID
+from typing import Optional
 
 import pytest
 
 from kiota_serialization_json.json_parse_node import JsonParseNode
 
-from ..helpers import OfficeLocation, User
+from ..helpers import Entity, OfficeLocation, User
 
+url: str = "https://graph.microsoft.com/v1.0/$metadata#users/$entity"
 
+@dataclass
+class UserClass:
+    odata_context: str
+    business_phones: list[str]
+    display_name: str
+    mobile_phone: Optional[str]
+    office_location: str
+    updated_at: str
+    birthday: str
+    is_active: bool
+    age: int
+    gpa: float
+    id: str
+    
+user1 = UserClass(
+        url,
+        ["+1 205 555 0108"],
+        "Diego Siciliani",
+        None,
+        "dunhill",
+        "2021 -07-29T03:07:25Z",
+        "2000-09-04",
+        True,21,3.2,
+        "8f841f30-e6e3-439a-a812-ebd369559c36"
+        )
+user2 = UserClass(
+        url,
+        ["425-555-0100"],
+        "MOD Administrator",
+        None,
+        "oval",
+        "2020 -07-29T03:07:25Z",
+        "1990-09-04",
+        True,
+        32,
+        3.9,
+        "f58411c7-ae78-4d3c-bb0d-3f24d948de41"
+        )
 @pytest.fixture
 def sample_user_json():
+    user_json = json.dumps(asdict(user1))
+    return user_json
+
+@pytest.fixture
+def sample_users_json():
+    users_json = json.dumps([asdict(user1), asdict(user2)])
+    return users_json
+
+@pytest.fixture
+def sample_entity_json():
 
-    user_json = json.dumps(
+    entity_json = json.dumps(
         {
-            "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
-            "businessPhones": ["+1 205 555 0108"],
-            "displayName": "Diego Siciliani",
-            "mobilePhone": None,
-            "officeLocation": "dunhill",
-            "updatedAt": "2021 -07-29T03:07:25Z",
-            "birthday": "2000-09-04",
-            "isActive": True,
-            "age": 21,
-            "gpa": 3.2,
+            "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#$entity",
             "id": "8f841f30-e6e3-439a-a812-ebd369559c36"
         }
     )
-    return user_json
+    return entity_json
 
 
-@pytest.fixture
-def sample_users_json():
-    users_json = json.dumps(
-        [
-            {
-                "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
-                "businessPhones": ["+1 425 555 0109"],
-                "displayName": "Adele Vance",
-                "mobilePhone": None,
-                "officeLocation": "dunhill",
-                "updatedAt": "2017 -07-29T03:07:25Z",
-                "birthday": "2000-09-04",
-                "isActive": True,
-                "age": 21,
-                "gpa": 3.7,
-                "id": "76cabd60-f9aa-4d23-8958-64f5539b826a"
-            },
-            {
-                "businessPhones": ["425-555-0100"],
-                "displayName": "MOD Administrator",
-                "mobilePhone": None,
-                "officeLocation": "oval",
-                "updatedAt": "2020 -07-29T03:07:25Z",
-                "birthday": "1990-09-04",
-                "isActive": True,
-                "age": 32,
-                "gpa": 3.9,
-                "id": "f58411c7-ae78-4d3c-bb0d-3f24d948de41"
-            },
-        ]
-    )
-    return users_json
 
 
 def test_get_str_value():
     parse_node = JsonParseNode("Diego Siciliani")
     result = parse_node.get_str_value()
     assert result == "Diego Siciliani"
 
@@ -157,25 +167,32 @@
     assert isinstance(result.updated_at, datetime)
     assert isinstance(result.birthday, date)
     assert result.business_phones == ["+1 205 555 0108"]
     assert result.age == 21
     assert result.gpa == 3.2
     assert result.is_active == True
     assert result.mobile_phone == None
-    assert "@odata.context" in result.additional_data
+    assert "odata_context" in result.additional_data
 
 
 def test_get_collection_of_object_values(sample_users_json):
     parse_node = JsonParseNode(json.loads(sample_users_json))
     result = parse_node.get_collection_of_object_values(User)
     assert isinstance(result[0], User)
-    assert result[0].id == UUID("76cabd60-f9aa-4d23-8958-64f5539b826a")
-    assert result[0].display_name == "Adele Vance"
+    assert result[0].id == UUID("8f841f30-e6e3-439a-a812-ebd369559c36")
+    assert result[0].display_name == "Diego Siciliani"
     assert result[0].office_location == OfficeLocation.Dunhill
     assert isinstance(result[0].updated_at, datetime)
     assert isinstance(result[0].birthday, date)
-    assert result[0].business_phones == ["+1 425 555 0109"]
+    assert result[0].business_phones == ["+1 205 555 0108"]
     assert result[0].age == 21
-    assert result[0].gpa == 3.7
+    assert result[0].gpa == 3.2
     assert result[0].is_active == True
     assert result[0].mobile_phone == None
-    assert "@odata.context" in result[0].additional_data
+    assert "odata_context" in result[0].additional_data
+    
+def test_get_object_value_no_additional_data(sample_entity_json):
+    with pytest.warns(UserWarning):
+        parse_node = JsonParseNode(json.loads(sample_entity_json))
+        result = parse_node.get_object_value(Entity)
+        assert isinstance(result, Entity)
+        assert result.id == UUID("8f841f30-e6e3-439a-a812-ebd369559c36")
```

### Comparing `microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_parse_node_factory.py` & `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_serialization_writer.py` & `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/tests/unit/test_json_serialization_writer_factory.py` & `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.1/PKG-INFO` & `microsoft-kiota-serialization-json-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.1
+Version: 0.3.2
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

