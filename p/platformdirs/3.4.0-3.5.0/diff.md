# Comparing `tmp/platformdirs-3.4.0.tar.gz` & `tmp/platformdirs-3.5.0.tar.gz`

## Comparing `platformdirs-3.4.0.tar` & `platformdirs-3.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/conftest.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_android.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_api.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_main.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.4.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.4.0/LICENSE
--rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.4.0/README.rst
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/android.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/version.py
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 platformdirs-3.5.0/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_android.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_api.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_main.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 platformdirs-3.5.0/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.0/LICENSE
+-rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.5.0/README.rst
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.5.0/PKG-INFO
```

### Comparing `platformdirs-3.4.0/src/platformdirs/__init__.py` & `platformdirs-3.5.0/src/platformdirs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,21 @@
 def user_videos_dir() -> str:
     """
     :returns: videos directory tied to the user
     """
     return PlatformDirs().user_videos_dir
 
 
+def user_music_dir() -> str:
+    """
+    :returns: music directory tied to the user
+    """
+    return PlatformDirs().user_music_dir
+
+
 def user_runtime_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> str:
@@ -490,14 +497,21 @@
 def user_videos_path() -> Path:
     """
     :returns: videos path tied to the user
     """
     return PlatformDirs().user_videos_path
 
 
+def user_music_path() -> Path:
+    """
+    :returns: music path tied to the user
+    """
+    return PlatformDirs().user_music_path
+
+
 def user_runtime_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> Path:
@@ -528,24 +542,26 @@
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
     "user_videos_dir",
+    "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
     "user_data_path",
     "user_config_path",
     "user_cache_path",
     "user_state_path",
     "user_log_path",
     "user_documents_path",
     "user_pictures_path",
     "user_videos_path",
+    "user_music_path",
     "user_runtime_path",
     "site_data_path",
     "site_config_path",
     "site_cache_path",
 ]
```

### Comparing `platformdirs-3.4.0/src/platformdirs/__main__.py` & `platformdirs-3.5.0/src/platformdirs/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
     "user_videos_dir",
+    "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.4.0/src/platformdirs/android.py` & `platformdirs-3.5.0/src/platformdirs/android.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,21 @@
     def user_videos_dir(self) -> str:
         """
         :return: videos directory tied to the user e.g. ``/storage/emulated/0/DCIM/Camera``
         """
         return _android_videos_folder()
 
     @property
+    def user_music_dir(self) -> str:
+        """
+        :return: music directory tied to the user e.g. ``/storage/emulated/0/Music``
+        """
+        return _android_music_folder()
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, same as `user_cache_dir` if not opinionated else ``tmp`` in it,
           e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>/tmp``
         """
         path = self.user_cache_dir
         if self.opinion:
@@ -163,10 +170,26 @@
         videos_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_DCIM).getAbsolutePath()
     except Exception:
         videos_dir = "/storage/emulated/0/DCIM/Camera"
 
     return videos_dir
 
 
+@lru_cache(maxsize=1)
+def _android_music_folder() -> str:
+    """:return: music folder for the Android OS"""
+    # Get directories with pyjnius
+    try:
+        from jnius import autoclass
+
+        Context = autoclass("android.content.Context")  # noqa: N806
+        Environment = autoclass("android.os.Environment")  # noqa: N806
+        music_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_MUSIC).getAbsolutePath()
+    except Exception:
+        music_dir = "/storage/emulated/0/Music"
+
+    return music_dir
+
+
 __all__ = [
     "Android",
 ]
```

### Comparing `platformdirs-3.4.0/src/platformdirs/api.py` & `platformdirs-3.5.0/src/platformdirs/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,19 @@
     @property
     @abstractmethod
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user"""
 
     @property
     @abstractmethod
+    def user_music_dir(self) -> str:
+        """:return: music directory tied to the user"""
+
+    @property
+    @abstractmethod
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user"""
 
     @property
     def user_data_path(self) -> Path:
         """:return: data path tied to the user"""
         return Path(self.user_data_dir)
@@ -190,10 +195,15 @@
 
     @property
     def user_videos_path(self) -> Path:
         """:return: videos path tied to the user"""
         return Path(self.user_videos_dir)
 
     @property
+    def user_music_path(self) -> Path:
+        """:return: music path tied to the user"""
+        return Path(self.user_music_dir)
+
+    @property
     def user_runtime_path(self) -> Path:
         """:return: runtime path tied to the user"""
         return Path(self.user_runtime_dir)
```

### Comparing `platformdirs-3.4.0/src/platformdirs/macos.py` & `platformdirs-3.5.0/src/platformdirs/macos.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user, e.g. ``~/Movies``"""
         return os.path.expanduser("~/Movies")
 
     @property
+    def user_music_dir(self) -> str:
+        """:return: music directory tied to the user, e.g. ``~/Music``"""
+        return os.path.expanduser("~/Music")
+
+    @property
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user, e.g. ``~/Library/Caches/TemporaryItems/$appname/$version``"""
         return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches/TemporaryItems"))
 
 
 __all__ = [
     "MacOS",
```

### Comparing `platformdirs-3.4.0/src/platformdirs/unix.py` & `platformdirs-3.5.0/src/platformdirs/unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,21 @@
     def user_videos_dir(self) -> str:
         """
         :return: videos directory tied to the user, e.g. ``~/Videos``
         """
         return _get_user_media_dir("XDG_VIDEOS_DIR", "~/Videos")
 
     @property
+    def user_music_dir(self) -> str:
+        """
+        :return: music directory tied to the user, e.g. ``~/Music``
+        """
+        return _get_user_media_dir("XDG_MUSIC_DIR", "~/Music")
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g. ``/run/user/$(id -u)/$appname/$version`` or
          ``$XDG_RUNTIME_DIR/$appname/$version``
         """
         path = os.environ.get("XDG_RUNTIME_DIR", "")
         if not path.strip():
```

### Comparing `platformdirs-3.4.0/src/platformdirs/windows.py` & `platformdirs-3.5.0/src/platformdirs/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,61 +112,80 @@
     def user_videos_dir(self) -> str:
         """
         :return: videos directory tied to the user e.g. ``%USERPROFILE%\\Videos``
         """
         return os.path.normpath(get_win_folder("CSIDL_MYVIDEO"))
 
     @property
+    def user_music_dir(self) -> str:
+        """
+        :return: music directory tied to the user e.g. ``%USERPROFILE%\\Music``
+        """
+        return os.path.normpath(get_win_folder("CSIDL_MYMUSIC"))
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g.
          ``%USERPROFILE%\\AppData\\Local\\Temp\\$appauthor\\$appname``
         """
         path = os.path.normpath(os.path.join(get_win_folder("CSIDL_LOCAL_APPDATA"), "Temp"))
         return self._append_parts(path)
 
 
 def get_win_folder_from_env_vars(csidl_name: str) -> str:
     """Get folder from environment variables."""
-    if csidl_name == "CSIDL_PERSONAL":  # does not have an environment name
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")
-
-    if csidl_name == "CSIDL_MYPICTURES":  # does not have an environment name
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")
-
-    if csidl_name == "CSIDL_MYVIDEO":  # does not have an environment name
-        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")
+    result = get_win_folder_if_csidl_name_not_env_var(csidl_name)
+    if result is not None:
+        return result
 
     env_var_name = {
         "CSIDL_APPDATA": "APPDATA",
         "CSIDL_COMMON_APPDATA": "ALLUSERSPROFILE",
         "CSIDL_LOCAL_APPDATA": "LOCALAPPDATA",
     }.get(csidl_name)
     if env_var_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
     result = os.environ.get(env_var_name)
     if result is None:
         raise ValueError(f"Unset environment variable: {env_var_name}")
     return result
 
 
+def get_win_folder_if_csidl_name_not_env_var(csidl_name: str) -> str | None:
+    """Get folder for a CSIDL name that does not exist as an environment variable."""
+    if csidl_name == "CSIDL_PERSONAL":
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")
+
+    if csidl_name == "CSIDL_MYPICTURES":
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")
+
+    if csidl_name == "CSIDL_MYVIDEO":
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")
+
+    if csidl_name == "CSIDL_MYMUSIC":
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Music")
+    return None
+
+
 def get_win_folder_from_registry(csidl_name: str) -> str:
     """Get folder from the registry.
 
     This is a fallback technique at best. I'm not sure if using the
     registry for this guarantees us the correct answer for all CSIDL_*
     names.
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
         "CSIDL_MYPICTURES": "My Pictures",
         "CSIDL_MYVIDEO": "My Video",
+        "CSIDL_MYMUSIC": "My Music",
     }.get(csidl_name)
     if shell_folder_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
     if sys.platform != "win32":  # only needed for mypy type checker to know that this code runs only on Windows
         raise NotImplementedError
     import winreg
 
@@ -180,14 +199,15 @@
     csidl_const = {
         "CSIDL_APPDATA": 26,
         "CSIDL_COMMON_APPDATA": 35,
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
         "CSIDL_MYPICTURES": 39,
         "CSIDL_MYVIDEO": 14,
+        "CSIDL_MYMUSIC": 13,
     }.get(csidl_name)
     if csidl_const is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
 
     buf = ctypes.create_unicode_buffer(1024)
     windll = getattr(ctypes, "windll")  # noqa: B009 # using getattr to avoid false positive with mypy type checker
     windll.shell32.SHGetFolderPathW(None, csidl_const, None, 0, buf)
```

### Comparing `platformdirs-3.4.0/tests/conftest.py` & `platformdirs-3.5.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
     "user_videos_dir",
+    "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.4.0/tests/test_android.py` & `platformdirs-3.5.0/tests/test_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         "user_cache_dir": f"/data/data/com.example/cache{suffix}",
         "site_cache_dir": f"/data/data/com.example/cache{suffix}",
         "user_state_dir": f"/data/data/com.example/files{suffix}",
         "user_log_dir": f"/data/data/com.example/cache{suffix}{'' if params.get('opinion', True) is False else '/log'}",
         "user_documents_dir": "/storage/emulated/0/Documents",
         "user_pictures_dir": "/storage/emulated/0/Pictures",
         "user_videos_dir": "/storage/emulated/0/DCIM/Camera",
+        "user_music_dir": "/storage/emulated/0/Music",
         "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else '/tmp'}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.4.0/tests/test_api.py` & `platformdirs-3.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.4.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.5.0/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.4.0/tests/test_macos.py` & `platformdirs-3.5.0/tests/test_macos.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,12 +31,13 @@
         "user_cache_dir": f"{home}/Library/Caches{suffix}",
         "site_cache_dir": f"/Library/Caches{suffix}",
         "user_state_dir": f"{home}/Library/Application Support{suffix}",
         "user_log_dir": f"{home}/Library/Logs{suffix}",
         "user_documents_dir": f"{home}/Documents",
         "user_pictures_dir": f"{home}/Pictures",
         "user_videos_dir": f"{home}/Movies",
+        "user_music_dir": f"{home}/Music",
         "user_runtime_dir": f"{home}/Library/Caches/TemporaryItems{suffix}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.4.0/tests/test_unix.py` & `platformdirs-3.5.0/tests/test_unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from pytest_mock import MockerFixture
 
 from platformdirs.unix import Unix
 
 
-@pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir"])
+@pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir", "user_music_dir"])
 def test_user_media_dir(mocker: MockerFixture, prop: str) -> None:
     example_path = "/home/example/ExampleMediaFolder"
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = example_path
     assert getattr(Unix(), prop) == example_path
 
 
 @pytest.mark.parametrize(
     ("env_var", "prop"),
     [
         pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", id="user_documents_dir"),
         pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", id="user_pictures_dir"),
         pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", id="user_videos_dir"),
+        pytest.param("XDG_MUSIC_DIR", "user_music_dir", id="user_music_dir"),
     ],
 )
 def test_user_media_dir_env_var(mocker: MockerFixture, env_var: str, prop: str) -> None:
     # Mock media dir not being in user-dirs.dirs file
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = None
 
@@ -42,14 +43,15 @@
 
 @pytest.mark.parametrize(
     ("env_var", "prop", "default_abs_path"),
     [
         pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", "/home/example/Documents", id="user_documents_dir"),
         pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", "/home/example/Pictures", id="user_pictures_dir"),
         pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", "/home/example/Videos", id="user_videos_dir"),
+        pytest.param("XDG_MUSIC_DIR", "user_music_dir", "/home/example/Music", id="user_music_dir"),
     ],
 )
 def test_user_media_dir_default(mocker: MockerFixture, env_var: str, prop: str, default_abs_path: str) -> None:
     # Mock media dir not being in user-dirs.dirs file
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = None
```

### Comparing `platformdirs-3.4.0/LICENSE` & `platformdirs-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.4.0/README.rst` & `platformdirs-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.4.0/pyproject.toml` & `platformdirs-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.4.0/PKG-INFO` & `platformdirs-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.4.0
+Version: 3.5.0
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
```

