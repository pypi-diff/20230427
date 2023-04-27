# Comparing `tmp/teamscale_cli-8.7.5-py3-none-any.whl.zip` & `tmp/teamscale_cli-8.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13809 bytes, number of entries: 11
+Zip file size: 14120 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      153 b- defN 23-Apr-12 09:15 teamscale_precommit_client/__init__.py
 -rw-r--r--  2.0 unx     2141 b- defN 23-Apr-12 09:15 teamscale_precommit_client/client_configuration_utils.py
 -rw-r--r--  2.0 unx      672 b- defN 23-Apr-12 09:15 teamscale_precommit_client/data.py
--rw-r--r--  2.0 unx     5509 b- defN 23-Apr-12 09:15 teamscale_precommit_client/git_utils.py
--rw-r--r--  2.0 unx    19455 b- defN 23-Apr-12 09:15 teamscale_precommit_client/precommit_client.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      554 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       82 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1014 b- defN 23-Apr-13 08:22 teamscale_cli-8.7.5.dist-info/RECORD
-11 files, 41056 bytes uncompressed, 12055 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx     6308 b- defN 23-Apr-27 06:15 teamscale_precommit_client/git_utils.py
+-rw-r--r--  2.0 unx    20280 b- defN 23-Apr-27 06:15 teamscale_precommit_client/precommit_client.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      554 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       82 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1014 b- defN 23-Apr-27 06:16 teamscale_cli-8.8.0.dist-info/RECORD
+11 files, 42680 bytes uncompressed, 12366 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: teamscale_precommit_client/git_utils.py
 Comment: 
 
 Filename: teamscale_precommit_client/precommit_client.py
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/LICENSE
+Filename: teamscale_cli-8.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/METADATA
+Filename: teamscale_cli-8.8.0.dist-info/METADATA
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/WHEEL
+Filename: teamscale_cli-8.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/entry_points.txt
+Filename: teamscale_cli-8.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/top_level.txt
+Filename: teamscale_cli-8.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teamscale_cli-8.7.5.dist-info/RECORD
+Filename: teamscale_cli-8.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teamscale_precommit_client/git_utils.py

```diff
@@ -2,15 +2,15 @@
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import locale
 import os
 from io import open
 
-from git import Repo, InvalidGitRepositoryError
+from git import Repo, InvalidGitRepositoryError, Diffable
 
 # [M]odified, [A]dded, [C]opied, [T]ype changed, [R]enamed (R092 should be R according to
 # https://gitpython.readthedocs.io/en/stable/reference.html#git.diff.DiffIndex, but testing it locally gave R092)
 _CHANGE_TYPES_CONSIDERED_FOR_PRECOMMIT = ['M', 'A', 'C', 'T', 'R', 'R092']
 _CHANGE_TYPE_DELETED = 'D'
 
 def get_current_branch(path_to_repository):
@@ -70,14 +70,17 @@
     """Filters the provided list of changed files.
 
     Non UTF-8 files and files larger than 1 MB are ignored.
     """
     filtered_files = []
     for changed_file in changed_files:
         file_is_valid = True
+        if (os.path.isdir(os.path.join(path_to_repository, changed_file))):
+            #ignore directories (e.g., git submodule folders)
+            continue
         if os.path.getsize(os.path.join(path_to_repository, changed_file)) > 1 * 1024 * 1024:
             print('File too large for precommit analysis. Ignoring: %s' % changed_file)
             file_is_valid = False
 
         try:
             with open(os.path.join(path_to_repository, changed_file), encoding=file_encoding) as file:
                 file.read()
@@ -93,63 +96,70 @@
 
         if file_is_valid:
             filtered_files.append(changed_file)
 
     return filtered_files
 
 
-def get_changed_files_and_content(path_to_repository, file_encoding):
+def get_changed_files_and_content(path_to_repository, file_encoding, ignore_subrepositories):
     """Utility method for getting the currently changed files from a Git repository.
 
     Filters the changed files using `filter_changed_files`.
 
         Args:
             path_to_repository (str): Path to the Git repository
             file_encoding (str): Encoding of the files in the repository (c.f. https://docs.python.org/3/library/codecs.html#standard-encodings)
 
         Returns:
             dict: Mapping of filename to file content for all changed files in the provided repository.
+            :param ignore_subrepositories:
     """
-    changed_files = filter_changed_files(get_changed_files(path_to_repository), path_to_repository, file_encoding)
+    changed_files = filter_changed_files(get_changed_files(path_to_repository, ignore_subrepositories),
+                                         path_to_repository, file_encoding)
     return {filename: open(os.path.join(path_to_repository, filename), encoding=file_encoding).read() for filename in
             changed_files}
 
 
-def get_changed_files(path_to_repository):
+def get_changed_files(path_to_repository, ignore_subrepositories):
     """Utility method for getting the currently changed files from a Git repository.
 
         Args:
             path_to_repository (str): Path to the Git repository
 
         Returns:
             List(str): List of filenames of all changed files in the provided repository.
     """
-    diff = _get_diff_to_last_commit(path_to_repository)
+    diff = _get_diff_to_last_commit(path_to_repository, ignore_subrepositories)
     return [item.b_path for item in diff if item.change_type in _CHANGE_TYPES_CONSIDERED_FOR_PRECOMMIT]
 
 
-def get_deleted_files(path_to_repository):
+def get_deleted_files(path_to_repository, ignore_subrepositories):
     """Utility method for getting the deleted files from a Git repository.
 
         Args:
             path_to_repository (str): Path to the Git repository
 
         Returns:
             List(str): List of filenames of all deleted files in the provided repository.
     """
-    diff = _get_diff_to_last_commit(path_to_repository)
+    diff = _get_diff_to_last_commit(path_to_repository, ignore_subrepositories)
     return [item.b_path for item in diff if item.change_type == _CHANGE_TYPE_DELETED]
 
 
-def _get_diff_to_last_commit(path_to_repository):
+def _get_diff_to_last_commit(path_to_repository, ignore_subrepositories):
     """ Utility method for getting a diff between the working copy and the HEAD commit
 
         Args:
             path_to_repository (str): Path to the Git repository
 
         Returns:
             List(git.diff.Diff): List of Diff objects for every file
     """
     repo = Repo(path_to_repository)
-    unstaged_diff = repo.index.diff(None)
-    staged_diff = repo.head.commit.diff()
+    if ignore_subrepositories==True:
+        unstaged_diff = repo.index.diff(other=None, paths=None, create_patch=False, ignore_submodules="all")
+        staged_diff = repo.head.commit.diff(other=Diffable.Index, paths=None, create_patch=False, ignore_submodules="all")
+    else:
+        unstaged_diff = repo.index.diff(other=None, paths=None, create_patch=False)
+        staged_diff = repo.head.commit.diff(other=Diffable.Index, paths=None, create_patch=False)
+
     return unstaged_diff + staged_diff
```

## teamscale_precommit_client/precommit_client.py

```diff
@@ -28,15 +28,16 @@
     """Client for precommit analysis"""
     # Number of seconds the client waits until fetching precommit results from the server.
     PRECOMMIT_WAITING_TIME_IN_SECONDS = 2
 
     def __init__(self, teamscale_config, repository_path, path_prefix=DEFAULT_PATH_PREFIX, project_subpath='',
                  analyzed_file=None, verify=True, omit_links_to_findings=False, exclude_findings_in_changed_code=False,
                  fetch_existing_findings=False, fetch_all_findings=False, fetch_existing_findings_in_changes=False,
-                 fail_on_red_findings=False, log_to_stderr=False, file_encoding=DEFAULT_FILE_ENCODING):
+                 fail_on_red_findings=False, log_to_stderr=False, file_encoding=DEFAULT_FILE_ENCODING,
+                 ignore_subrepositories=False):
         """Constructor"""
         self.teamscale_client = TeamscaleClient(teamscale_config.url, teamscale_config.username,
                                                 teamscale_config.access_token, teamscale_config.project_id, verify)
         self.repository_path = repository_path
 
         # calling os.path.join ensures a tailing '/'
         self.path_prefix = os.path.join(path_prefix, '')
@@ -55,14 +56,15 @@
         self.added_findings = []
         self.removed_findings = []
         self.existing_findings = []
         self.findings_in_changed_code = []
         self.current_branch = ''
         self.parent_commit_timestamp = 0
         self.file_encoding = file_encoding
+        self.ignore_subrepositories = ignore_subrepositories
 
     def run(self):
         """Performs the precommit analysis. Depending on the modifications made and the flags provided to the client,
         this triggers precommit analysis or just queries existing findings."""
         self._calculate_modifications()
         self._retrieve_current_branch()
         self._retrieve_parent_commit_timestamp()
@@ -85,16 +87,17 @@
             exit(1)
 
     def _calculate_modifications(self):
         """Calculates the changed and deleted files in the repository."""
         if not self.repository_path or not os.path.exists(self.repository_path) or not os.path.isdir(
                 self.repository_path):
             raise RuntimeError('Invalid path to file in repository: %s' % self.repository_path)
-        self.changed_files = get_changed_files_and_content(self.repository_path, self.file_encoding)
-        self.deleted_files = get_deleted_files(self.repository_path)
+        self.changed_files = get_changed_files_and_content(self.repository_path, self.file_encoding,
+                                                           self.ignore_subrepositories)
+        self.deleted_files = get_deleted_files(self.repository_path, self.ignore_subrepositories)
 
     def _retrieve_current_branch(self):
         """Retrieves the current branch from the repository."""
         self.current_branch = get_current_branch(self.repository_path)
 
     def _retrieve_parent_commit_timestamp(self):
         """Retrieves the commit timestamp from the repository."""
@@ -311,16 +314,20 @@
     parser.add_argument('--path-prefix', metavar='PATH_PREFIX', type=str,
                         help='Path prefix on Teamscale as configured with "Prepend repository identifier" or '
                              '"Path prefix transformation". Please use "/" to separate folders.',
                         default=DEFAULT_PATH_PREFIX)
     parser.add_argument('--file-encoding', metavar='FILE_ENCODING', type=str,
                         help='The encoding of your files '
                              '(c.f. https://docs.python.org/3/library/codecs.html#standard-encodings).'
-                             ' By default, the system encoding will be used.',
-                        default=DEFAULT_FILE_ENCODING)
+                             ' By default, the system encoding will be used.', default=DEFAULT_FILE_ENCODING)
+    parser.add_argument('--ignore-subrepositories', dest='ignore_subrepositories', action='store_const', const=True, default=False,
+                        help='When this option is set, then we ignore subrepositories '
+                             '(git submodules) in the current repository when determining which files changed. This '
+                             'affects the files considered for precommit analysis. It does not affect the retrieval '
+                             'of "existing" findings from the Teamscale server.')
     return parser.parse_args()
 
 
 def _bool_or_string(string):
     """Helper to interpret different ways of specifying boolean values."""
     if string in ['t', 'true', 'True']:
         return True
@@ -340,15 +347,16 @@
                            verify=parsed_args.verify, omit_links_to_findings=parsed_args.omit_links_to_findings,
                            exclude_findings_in_changed_code=parsed_args.exclude_findings_in_changed_code,
                            fetch_existing_findings=parsed_args.fetch_existing_findings,
                            fetch_all_findings=parsed_args.fetch_all_findings,
                            fetch_existing_findings_in_changes=parsed_args.fetch_existing_findings_in_changes,
                            fail_on_red_findings=parsed_args.fail_on_red_findings,
                            log_to_stderr=parsed_args.log_to_stderr,
-                           file_encoding=parsed_args.file_encoding)
+                           file_encoding=parsed_args.file_encoding,
+                           ignore_subrepositories=parsed_args.ignore_subrepositories)
 
 
 def run():
     """Performs precommit analysis."""
     parsed_args = _parse_args()
     precommit_client = _configure_precommit_client(parsed_args)
     precommit_client.run()
```

## Comparing `teamscale_cli-8.7.5.dist-info/LICENSE` & `teamscale_cli-8.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teamscale_cli-8.7.5.dist-info/METADATA` & `teamscale_cli-8.8.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamscale-cli
-Version: 8.7.5
+Version: 8.8.0
 Summary: Client for performing precommit analysis with Teamscale.
 Home-page: https://github.com/cqse/teamscale-cli
 Author: Thomas Kinnen - CQSE GmbH
 Author-email: kinnen@cqse.eu
 License: Apache
 Keywords: teamscale client precommit
 Classifier: Topic :: Utilities
```

