# Comparing `tmp/lazy_env_configurator-0.2.0.tar.gz` & `tmp/lazy_env_configurator-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_env_configurator-0.2.0.tar", max compression
+gzip compressed data, was "lazy_env_configurator-0.3.0a0.tar", max compression
```

## Comparing `lazy_env_configurator-0.2.0.tar` & `lazy_env_configurator-0.3.0a0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0      400 2023-04-17 08:24:04.187817 lazy_env_configurator-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-04-17 08:57:37.536535 lazy_env_configurator-0.2.0/LICENSE
--rw-r--r--   0        0        0     6563 2023-04-17 08:58:24.042867 lazy_env_configurator-0.2.0/README.md
--rw-r--r--   0        0        0     7718 2023-04-17 08:24:04.188348 lazy_env_configurator-0.2.0/lazy_env_configurator/__init__.py
--rw-r--r--   0        0        0      149 2023-04-17 08:24:04.188494 lazy_env_configurator-0.2.0/lazy_env_configurator/custom_warnings.py
--rw-r--r--   0        0        0     1399 2023-04-17 08:59:02.520760 lazy_env_configurator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-04-16 09:58:51.605661 lazy_env_configurator-0.2.0/pytest.ini
--rw-r--r--   0        0        0     1466 2023-04-17 08:46:56.544079 lazy_env_configurator-0.2.0/requirements-test.txt
--rw-r--r--   0        0        0       10 2023-04-17 08:24:04.188983 lazy_env_configurator-0.2.0/tests/.env.contained
--rw-r--r--   0        0        0       33 2023-04-17 08:24:04.189132 lazy_env_configurator-0.2.0/tests/.env.test
--rw-r--r--   0        0        0     1372 2023-04-17 08:24:04.189301 lazy_env_configurator-0.2.0/tests/test_contained_values.py
--rw-r--r--   0        0        0     1463 2023-04-17 08:24:04.189431 lazy_env_configurator-0.2.0/tests/test_env_configurator.py
--rw-r--r--   0        0        0      461 2023-04-17 08:24:04.189637 lazy_env_configurator-0.2.0/tests/test_invalid_env_file.py
--rw-r--r--   0        0        0      481 2023-04-17 08:24:04.189818 lazy_env_configurator-0.2.0/tests/test_invalid_iterable.py
--rw-r--r--   0        0        0      340 2023-04-17 05:32:48.770621 lazy_env_configurator-0.2.0/tox.ini
--rw-r--r--   0        0        0     7773 1970-01-01 00:00:00.000000 lazy_env_configurator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-04-27 08:49:57.899605 lazy_env_configurator-0.3.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-04-17 08:57:37.536535 lazy_env_configurator-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0    14181 2023-04-27 08:49:57.900261 lazy_env_configurator-0.3.0a0/README.md
+-rw-r--r--   0        0        0     8259 2023-04-27 08:49:57.900771 lazy_env_configurator-0.3.0a0/lazy_env_configurator/__init__.py
+-rw-r--r--   0        0        0      149 2023-04-17 08:24:04.188494 lazy_env_configurator-0.3.0a0/lazy_env_configurator/custom_warnings.py
+-rw-r--r--   0        0        0     3999 2023-04-27 08:49:57.901116 lazy_env_configurator-0.3.0a0/lazy_env_configurator/env.py
+-rw-r--r--   0        0        0     3041 2023-04-27 08:49:57.901420 lazy_env_configurator-0.3.0a0/lazy_env_configurator/validations.py
+-rw-r--r--   0        0        0     1426 2023-04-27 08:49:57.902361 lazy_env_configurator-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-04-16 09:58:51.605661 lazy_env_configurator-0.3.0a0/pytest.ini
+-rw-r--r--   0        0        0     1614 2023-04-27 08:49:57.902720 lazy_env_configurator-0.3.0a0/requirements-test.txt
+-rw-r--r--   0        0        0       10 2023-04-17 08:24:04.188983 lazy_env_configurator-0.3.0a0/tests/.env.contained
+-rw-r--r--   0        0        0       33 2023-04-17 08:24:04.189132 lazy_env_configurator-0.3.0a0/tests/.env.test
+-rw-r--r--   0        0        0      774 2023-04-27 08:49:57.903382 lazy_env_configurator-0.3.0a0/tests/test_contained_values.py
+-rw-r--r--   0        0        0     1131 2023-04-27 08:49:57.903672 lazy_env_configurator-0.3.0a0/tests/test_eager_validation.py
+-rw-r--r--   0        0        0     2943 2023-04-27 08:49:57.904047 lazy_env_configurator-0.3.0a0/tests/test_env_configurator.py
+-rw-r--r--   0        0        0      461 2023-04-17 08:24:04.189637 lazy_env_configurator-0.3.0a0/tests/test_invalid_env_file.py
+-rw-r--r--   0        0        0      481 2023-04-17 08:24:04.189818 lazy_env_configurator-0.3.0a0/tests/test_invalid_iterable.py
+-rw-r--r--   0        0        0      340 2023-04-17 05:32:48.770621 lazy_env_configurator-0.3.0a0/tox.ini
+-rw-r--r--   0        0        0    15435 1970-01-01 00:00:00.000000 lazy_env_configurator-0.3.0a0/PKG-INFO
```

### Comparing `lazy_env_configurator-0.2.0/LICENSE` & `lazy_env_configurator-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_env_configurator-0.2.0/lazy_env_configurator/__init__.py` & `lazy_env_configurator-0.3.0a0/lazy_env_configurator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,41 @@
 import os
 import dotenv
 import warnings
+from .env import Env
 from pathlib import Path
-from dataclasses import dataclass
-from typing import Iterable, Union
-from .custom_warnings import EnvWarning
+from pydantic import BaseModel
+from pydantic.fields import FieldInfo
+from .validations import ValidationOptions
+from pydantic.error_wrappers import ValidationError
+from typing import Iterable, Union, Dict, Optional, Sequence
 
 
-@dataclass(frozen=True)
 class BaseConfig:
     """
     Base Config required for env creation
 
     - `envs` (typing.Iterable[typing.Union[tuple[str, str], str]]): List of env variables to be created.
         Elements in `envs` can be either a tuple of (name, default) or just the name.
         If the element is a tuple, the first element is the name of the env variable and the
         second element is the default value.
     - `dot_env_path` (typing.Union[str, 'os.PathLike[str]']): Path to the .env file
     - `contained` (bool): If True, the env variables loaded from the .env file will be contained within instance and
-     not set as env variables.
+     not set as env variables. default: True
      This is helpful when you do not want to populate global env variables and maintain a clean env.
+    - `validations` (typing.Dict[str, ValidationOptions]): Dict of validations to be applied to the env variables.
+        The key of the dict is the name of the env variable and the value is the validation options.
+        The validation options are the same as the pydantic field info.
+    - `eagerly_validate` (bool): If True, the env variables will be validated on class creation.
     """
     envs: Iterable[Union[tuple[str, str], str]] = tuple()
     dot_env_path: Union[str, 'os.PathLike[str]'] = None
-    contained: bool = False
-
-
-class Env(object):
-    """
-    Env descriptor for env variables. This class populates env
-    variables on first access and caches the value for subsequent access.
-    If the env variable is not set, it uses the default value provided.
-    Values can be overriden by setting the value on the instance.
-    """
-    __slots__ = ('__name', '__value', '__default', '__calculated')
-
-    def __init__(self, default=None):
-        """
-        Initalizer for Env
-        Captures the default value and name of the env variable
-
-        Args:
-            default (typing.Any, optional): Default to override in case of unset Env. Defaults to None.
-        """
-        self.__name = None
-        self.__value = None
-        self.__default = default
-        # flag to check if the value is already calculated
-        self.__calculated = False
-
-    def __get__(self, instance, obj_type=None):
-        '''
-        descriptor __get__ method
-
-        Returns:
-            typing.Any: value of the env variable
-        '''
-        contained_ = getattr(instance, '__contained__', {})
-        # using the cached value if already calculated
-        if not self.__calculated:
-            self.__value = contained_.get(self.__name) or os.getenv(self.__name, self.__default)
-            self.__calculated = True
-        return self.__value
-
-    def __set__(self, _, value):
-        self.__value = value
-
-    def __set_name__(self, _, name):
-        self.__name = name
+    contained: bool = True
+    validations: Dict[str, ValidationOptions] = {}
+    eagerly_validate: bool = False
 
 
 class EnvMeta(type):
     """
     Metaclass for populating env variables
     as class attributes to the child class.
     if the child class has a Config class, it will
@@ -102,31 +66,44 @@
         >>> ABC.instance.test
         >>> ABC.instance.prd
     """
     def __new__(mcs, name, bases, attrs: dict):
         config_attrs = attrs.pop('Config', BaseConfig)  # type: BaseConfig
         if config_attrs:
             mcs.validate_envs(config_attrs)
-            # patching the class attrs with env variables
-            attrs.update(mcs.process_config_attrs(config_attrs))
             mcs.validate_dotenv_path(config_attrs)
             # loading env variables from file
             dot_env_path = getattr(config_attrs, 'dot_env_path', None)
+            __contained__ = {}
             if not config_attrs.contained:
                 dotenv.load_dotenv(dot_env_path)
             else:
                 __contained__ = dotenv.dotenv_values(dot_env_path)
                 if __contained__:
                     attrs['__contained__'] = __contained__
-                else:
-                    warnings.warn(
-                        ('Cannot Contain, No env variables found in dot env or no'
-                         ' dot env file present or specified. This option should be used'
-                         ' exclusively with the .env files. '),
-                        EnvWarning)
+            # patching the class attrs with env variables
+            env_attr_ = mcs.process_config_attrs(config_attrs)
+            if config_attrs.eagerly_validate:
+                errs_ = []
+                name_space_, __annotations__ = {}, {}
+                for k, v in env_attr_.items():
+                    _, errors_ = v.validate(name, contained=__contained__)
+                    if errors_:
+                        name_space_[k] = FieldInfo(default=v.default, **v.extras)
+                        __annotations__[k] = v.type
+                        if isinstance(errors_, Sequence):
+                            errs_.extend(errors_)
+                        else:
+                            errs_.append(errors_)
+                name_space_['__annotations__'] = __annotations__
+                if errs_:
+                    raise ValidationError(errors=errs_,
+                                          model=type(name, (BaseModel,),
+                                                     name_space_))
+            attrs.update(env_attr_)
         cls_ = super().__new__(mcs, name, bases, attrs)
         # initializing the instance
         cls_.instance = cls_()
         return cls_
 
     def validate_envs(config_attrs: BaseConfig):
         """
@@ -163,21 +140,35 @@
 
         Args:
             config_attrs (BaseConfig): _description_
 
         Returns:
             _type_: _description_
         """
+        validation_map = config_attrs.validations
+        default_type = Optional[str]
         c_ = {}
         for attr_name in getattr(config_attrs, 'envs', tuple()):
             name_ = attr_name
             default_ = None
             if isinstance(attr_name, (tuple, list)):
                 [name_, default_] = attr_name
-            c_[name_] = Env(default_)
+            validation_kwargs = validation_map.get(name_, {})
+            default_ = default_ or validation_kwargs.pop('default', None)
+            # selecting the type of the env variable
+            required_ = validation_kwargs.get('required', False)
+            type_ = validation_kwargs.pop('type', default_type)
+            if required_ and type_ is default_type:
+                warnings.warn(
+                    f"Optional types cannot be required. {default_type}, will update required to False."
+                )
+                validation_kwargs['required'] = False
+            env_ = Env(default_, type_=type_, **validation_kwargs)
+            env_.__set_name__(None, name_)
+            c_[name_] = env_
         return c_
 
 
 class BaseEnv(metaclass=EnvMeta):
     """
     Base class for env variables
     This can be used as a base class for env variables.
```

### Comparing `lazy_env_configurator-0.2.0/pyproject.toml` & `lazy_env_configurator-0.3.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy_env_configurator"
-version = "0.2.0"
+version = "0.3.0-alpha"
 description = "Dynamic Config Class Creation using Environment Variables"
 authors = ["satyam soni <satyam.soni@hotmail.co.uk>"]
 readme = "README.md"
 packages = [{include = "lazy_env_configurator"}]
 homepage = "https://github.com/satyamsoni2211/lazy_env_configurator"
 repository = "https://github.com/satyamsoni2211/lazy_env_configurator"
 license = "MIT"
@@ -30,14 +30,15 @@
     "tox.ini",
     "LICENSE"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
+pydantic = "^1.10.7"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `lazy_env_configurator-0.2.0/requirements-test.txt` & `lazy_env_configurator-0.3.0a0/requirements-test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 flake8==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
 iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0"
 packaging==23.1 ; python_version >= "3.9" and python_version < "4.0"
 platformdirs==3.2.0 ; python_version >= "3.9" and python_version < "4.0"
 pluggy==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 pycodestyle==2.10.0 ; python_version >= "3.9" and python_version < "4.0"
+pydantic==1.10.7 ; python_version >= "3.9" and python_version < "4.0"
 pyflakes==3.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pyproject-api==1.5.1 ; python_version >= "3.9" and python_version < "4.0"
 pytest==7.3.1 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11"
 tox==4.4.12 ; python_version >= "3.9" and python_version < "4.0"
+typing-extensions==4.5.0 ; python_version >= "3.9" and python_version < "4.0"
 virtualenv==20.21.0 ; python_version >= "3.9" and python_version < "4.0"
```

