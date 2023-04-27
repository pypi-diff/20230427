# Comparing `tmp/ansible_later-3.2.3.tar.gz` & `tmp/ansible_later-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_later-3.2.3.tar", max compression
+gzip compressed data, was "ansible_later-3.3.0.tar", max compression
```

## Comparing `ansible_later-3.2.3.tar` & `ansible_later-3.3.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     1123 2023-04-20 07:50:50.803852 ansible_later-3.2.3/LICENSE
--rw-r--r--   0        0        0     3173 2023-04-20 07:50:50.803852 ansible_later-3.2.3/README.md
--rw-r--r--   0        0        0      120 2023-04-20 07:51:04.080358 ansible_later-3.2.3/ansiblelater/__init__.py
--rwxr-xr-x   0        0        0     2892 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/__main__.py
--rw-r--r--   0        0        0     9843 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/candidate.py
--rw-r--r--   0        0        0      666 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/exceptions.py
--rw-r--r--   0        0        0     5180 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/logger.py
--rw-r--r--   0        0        0      834 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckBecomeUser.py
--rw-r--r--   0        0        0     1636 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckBracesSpaces.py
--rw-r--r--   0        0        0     2345 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckChangedInWhen.py
--rw-r--r--   0        0        0     1079 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandHasChanges.py
--rw-r--r--   0        0        0     2650 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py
--rw-r--r--   0        0        0     2031 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfModule.py
--rw-r--r--   0        0        0     1227 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCompareToEmptyString.py
--rw-r--r--   0        0        0     1229 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckCompareToLiteralBool.py
--rw-r--r--   0        0        0      952 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckDeprecated.py
--rw-r--r--   0        0        0     3764 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionMissing.py
--rw-r--r--   0        0        0     3105 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionOctal.py
--rw-r--r--   0        0        0     1156 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckFilterSeparation.py
--rw-r--r--   0        0        0     1920 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckGitHasVersion.py
--rw-r--r--   0        0        0     1162 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckInstallUseLatest.py
--rw-r--r--   0        0        0      941 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckLiteralBoolFormat.py
--rw-r--r--   0        0        0      737 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckLocalAction.py
--rw-r--r--   0        0        0     1182 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckMetaChangeFromDefault.py
--rw-r--r--   0        0        0     1201 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckMetaMain.py
--rw-r--r--   0        0        0      892 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNameFormat.py
--rw-r--r--   0        0        0      897 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNamedTask.py
--rw-r--r--   0        0        0     1679 2023-04-20 07:50:50.803852 ansible_later-3.2.3/ansiblelater/rules/CheckNativeYaml.py
--rw-r--r--   0        0        0     2179 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckNestedJinja.py
--rw-r--r--   0        0        0     1235 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckRelativeRolePaths.py
--rw-r--r--   0        0        0      700 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckScmInSrc.py
--rw-r--r--   0        0        0     1064 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckShellInsteadCommand.py
--rw-r--r--   0        0        0     1601 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckTaskSeparation.py
--rw-r--r--   0        0        0      904 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckUniqueNamedTask.py
--rw-r--r--   0        0        0      590 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckVersion.py
--rw-r--r--   0        0        0      891 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckWhenFormat.py
--rw-r--r--   0        0        0      518 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlColons.py
--rw-r--r--   0        0        0      517 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentEnd.py
--rw-r--r--   0        0        0      525 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentStart.py
--rw-r--r--   0        0        0      524 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlEmptyLines.py
--rw-r--r--   0        0        0      684 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlFile.py
--rw-r--r--   0        0        0      627 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlHasContent.py
--rw-r--r--   0        0        0      521 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlHyphens.py
--rw-r--r--   0        0        0      526 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/rules/CheckYamlIndent.py
--rw-r--r--   0        0        0     7899 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/settings.py
--rw-r--r--   0        0        0    11943 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/standard.py
--rw-r--r--   0        0        0        0 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/__init__.py
--rw-r--r--   0        0        0     2337 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/test_logger.py
--rw-r--r--   0        0        0      527 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/test/unit/test_settings.py
--rw-r--r--   0        0        0     2475 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/utils/__init__.py
--rw-r--r--   0        0        0    19003 2023-04-20 07:50:50.807852 ansible_later-3.2.3/ansiblelater/utils/yamlhelper.py
--rw-r--r--   0        0        0     3475 2023-04-20 07:51:04.080358 ansible_later-3.2.3/pyproject.toml
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 ansible_later-3.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-04-27 06:53:55.111832 ansible_later-3.3.0/LICENSE
+-rw-r--r--   0        0        0     3173 2023-04-27 06:53:55.111832 ansible_later-3.3.0/README.md
+-rw-r--r--   0        0        0      120 2023-04-27 06:54:26.079750 ansible_later-3.3.0/ansiblelater/__init__.py
+-rwxr-xr-x   0        0        0     2892 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/__main__.py
+-rw-r--r--   0        0        0     9843 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/candidate.py
+-rw-r--r--   0        0        0      666 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/logger.py
+-rw-r--r--   0        0        0      834 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckBecomeUser.py
+-rw-r--r--   0        0        0     1636 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckBracesSpaces.py
+-rw-r--r--   0        0        0     2346 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckChangedInWhen.py
+-rw-r--r--   0        0        0     1079 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckCommandHasChanges.py
+-rw-r--r--   0        0        0     2650 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckCommandInsteadOfArgument.py
+-rw-r--r--   0        0        0     2031 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckCommandInsteadOfModule.py
+-rw-r--r--   0        0        0     1227 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckCompareToEmptyString.py
+-rw-r--r--   0        0        0     1229 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckCompareToLiteralBool.py
+-rw-r--r--   0        0        0      952 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckDeprecated.py
+-rw-r--r--   0        0        0     3864 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckDeprecatedBareVars.py
+-rw-r--r--   0        0        0     3764 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckFilePermissionMissing.py
+-rw-r--r--   0        0        0     3106 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckFilePermissionOctal.py
+-rw-r--r--   0        0        0     1156 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckFilterSeparation.py
+-rw-r--r--   0        0        0     1921 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckGitHasVersion.py
+-rw-r--r--   0        0        0     1162 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckInstallUseLatest.py
+-rw-r--r--   0        0        0      941 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckLiteralBoolFormat.py
+-rw-r--r--   0        0        0      737 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckLocalAction.py
+-rw-r--r--   0        0        0     1182 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckMetaChangeFromDefault.py
+-rw-r--r--   0        0        0     1201 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckMetaMain.py
+-rw-r--r--   0        0        0      892 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckNameFormat.py
+-rw-r--r--   0        0        0      897 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckNamedTask.py
+-rw-r--r--   0        0        0     1679 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckNativeYaml.py
+-rw-r--r--   0        0        0     2179 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckNestedJinja.py
+-rw-r--r--   0        0        0     1235 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckRelativeRolePaths.py
+-rw-r--r--   0        0        0      700 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckScmInSrc.py
+-rw-r--r--   0        0        0     1064 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckShellInsteadCommand.py
+-rw-r--r--   0        0        0     1601 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckTaskSeparation.py
+-rw-r--r--   0        0        0      904 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckUniqueNamedTask.py
+-rw-r--r--   0        0        0      590 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckVersion.py
+-rw-r--r--   0        0        0      891 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckWhenFormat.py
+-rw-r--r--   0        0        0      518 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlColons.py
+-rw-r--r--   0        0        0      517 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlDocumentEnd.py
+-rw-r--r--   0        0        0      525 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlDocumentStart.py
+-rw-r--r--   0        0        0      524 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlEmptyLines.py
+-rw-r--r--   0        0        0      684 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlFile.py
+-rw-r--r--   0        0        0      627 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlHasContent.py
+-rw-r--r--   0        0        0      521 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlHyphens.py
+-rw-r--r--   0        0        0      526 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/rules/CheckYamlIndent.py
+-rw-r--r--   0        0        0     7899 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/settings.py
+-rw-r--r--   0        0        0    11943 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/standard.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/test/unit/__init__.py
+-rw-r--r--   0        0        0     2337 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/test/unit/test_logger.py
+-rw-r--r--   0        0        0      527 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/test/unit/test_settings.py
+-rw-r--r--   0        0        0     2909 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/utils/__init__.py
+-rw-r--r--   0        0        0    19003 2023-04-27 06:53:55.111832 ansible_later-3.3.0/ansiblelater/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3475 2023-04-27 06:54:26.079750 ansible_later-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 ansible_later-3.3.0/PKG-INFO
```

### Comparing `ansible_later-3.2.3/LICENSE` & `ansible_later-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/README.md` & `ansible_later-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/__main__.py` & `ansible_later-3.3.0/ansiblelater/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/candidate.py` & `ansible_later-3.3.0/ansiblelater/candidate.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/exceptions.py` & `ansible_later-3.3.0/ansiblelater/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/logger.py` & `ansible_later-3.3.0/ansiblelater/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckBecomeUser.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckBecomeUser.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckBracesSpaces.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckBracesSpaces.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckChangedInWhen.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckChangedInWhen.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
+
 from ansiblelater.standard import StandardBase
 
 
 class CheckChangedInWhen(StandardBase):
 
     sid = "ANSIBLE0026"
     description = "Use handlers instead of `when: changed`"
```

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckCommandHasChanges.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckCommandHasChanges.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckCommandInsteadOfArgument.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckCommandInsteadOfModule.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckCommandInsteadOfModule.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckCompareToEmptyString.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckCompareToEmptyString.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckCompareToLiteralBool.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckCompareToLiteralBool.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckDeprecated.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckDeprecated.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionMissing.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckFilePermissionMissing.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckFilePermissionOctal.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckFilePermissionOctal.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
+
 from ansiblelater.standard import StandardBase
 
 
 class CheckFilePermissionOctal(StandardBase):
 
     sid = "ANSIBLE0019"
     description = "Octal file permissions must contain leading zero or be a string"
```

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckFilterSeparation.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckFilterSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckGitHasVersion.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckGitHasVersion.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
+
 from ansiblelater.standard import StandardBase
 
 
 class CheckGitHasVersion(StandardBase):
 
     sid = "ANSIBLE0020"
     description = "Git checkouts should use explicit version"
```

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckInstallUseLatest.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckInstallUseLatest.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckLiteralBoolFormat.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckLiteralBoolFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckLocalAction.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckLocalAction.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckMetaChangeFromDefault.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckMetaChangeFromDefault.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckMetaMain.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckMetaMain.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckNameFormat.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckNameFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckNamedTask.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckNativeYaml.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckNativeYaml.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckNestedJinja.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckNestedJinja.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckRelativeRolePaths.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckRelativeRolePaths.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckScmInSrc.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckScmInSrc.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckShellInsteadCommand.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckShellInsteadCommand.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckTaskSeparation.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckTaskSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckUniqueNamedTask.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckUniqueNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckVersion.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckWhenFormat.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckWhenFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlColons.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlColons.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentEnd.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlDocumentEnd.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlDocumentStart.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlDocumentStart.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlEmptyLines.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlEmptyLines.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlFile.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlFile.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlHasContent.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlHasContent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlHyphens.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlHyphens.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/rules/CheckYamlIndent.py` & `ansible_later-3.3.0/ansiblelater/rules/CheckYamlIndent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/settings.py` & `ansible_later-3.3.0/ansiblelater/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/standard.py` & `ansible_later-3.3.0/ansiblelater/standard.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/test/unit/test_logger.py` & `ansible_later-3.3.0/ansiblelater/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/test/unit/test_settings.py` & `ansible_later-3.3.0/ansiblelater/test/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/ansiblelater/utils/__init__.py` & `ansible_later-3.3.0/ansiblelater/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Global utils collection."""
 
 import contextlib
+import re
 import sys
 from contextlib import suppress
 from distutils.version import LooseVersion
 
 import yaml
 
 from ansiblelater import logger
@@ -85,14 +86,26 @@
         if len(vector) == 1 \
         else add_dict_branch(tree[key] if key in tree else {},
                              vector[1:],
                              value)
     return tree
 
 
+def has_jinja(value):
+    """Return true if a string seems to contain jinja templating."""
+    re_has_jinja = re.compile(r"{[{%#].*[%#}]}", re.DOTALL)
+    return bool(isinstance(value, str) and re_has_jinja.search(value))
+
+
+def has_glob(value):
+    """Return true if a string looks like having a glob pattern."""
+    re_has_glob = re.compile("[][*?]")
+    return bool(isinstance(value, str) and re_has_glob.search(value))
+
+
 def sysexit(code=1):
     sys.exit(code)
 
 
 def sysexit_with_message(msg, code=1):
     LOG.critical(msg)
     sysexit(code)
```

### Comparing `ansible_later-3.2.3/ansiblelater/utils/yamlhelper.py` & `ansible_later-3.3.0/ansiblelater/utils/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.2.3/pyproject.toml` & `ansible_later-3.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,46 +26,46 @@
 license = "MIT"
 name = "ansible-later"
 packages = [
   {include = "ansiblelater"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-later/"
-version = "3.2.3"
+version = "3.3.0"
 
 [tool.poetry.dependencies]
 PyYAML = "6.0"
-ansible = {version = "7.4.0", optional = true}
-ansible-core = {version = "2.14.4", optional = true}
+ansible = {version = "7.5.0", optional = true}
+ansible-core = {version = "2.14.5", optional = true}
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 jsonschema = "4.17.3"
 nested-lookup = "0.2.25"
 pathspec = "0.11.1"
 python = "^3.9.0"
 python-json-logger = "2.0.7"
 toolz = "0.12.0"
 unidiff = "0.7.5"
-yamllint = "1.30.0"
+yamllint = "1.31.0"
 
 [tool.poetry.extras]
 ansible = ["ansible"]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-later = "ansiblelater.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.261"
+ruff = "0.0.262"
 pytest = "7.3.1"
 pytest-mock = "3.10.0"
 pytest-cov = "4.0.0"
 toml = "0.10.2"
-yapf = "0.32.0"
+yapf = "0.33.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [tool.pytest.ini_options]
```

### Comparing `ansible_later-3.2.3/PKG-INFO` & `ansible_later-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-later
-Version: 3.2.3
+Version: 3.3.0
 Summary: Reviews ansible playbooks, roles and inventories and suggests improvements.
 Home-page: https://ansible-later.geekdocs.de/
 License: MIT
 Keywords: ansible,code,review
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -25,26 +25,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Provides-Extra: ansible
 Provides-Extra: ansible-core
 Requires-Dist: PyYAML (==6.0)
-Requires-Dist: ansible (==7.4.0) ; extra == "ansible"
-Requires-Dist: ansible-core (==2.14.4) ; extra == "ansible-core"
+Requires-Dist: ansible (==7.5.0) ; extra == "ansible"
+Requires-Dist: ansible-core (==2.14.5) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.13.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: python-json-logger (==2.0.7)
 Requires-Dist: toolz (==0.12.0)
 Requires-Dist: unidiff (==0.7.5)
-Requires-Dist: yamllint (==1.30.0)
+Requires-Dist: yamllint (==1.31.0)
 Project-URL: Documentation, https://ansible-later.geekdocs.de/
 Project-URL: Repository, https://github.com/thegeeklab/ansible-later/
 Description-Content-Type: text/markdown
 
 # ansible-later
 
 Another best practice scanner for Ansible roles and playbooks
```

