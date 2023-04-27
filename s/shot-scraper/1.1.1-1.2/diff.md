# Comparing `tmp/shot-scraper-1.1.1.tar.gz` & `tmp/shot-scraper-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shot-scraper-1.1.1.tar", last modified: Mon Jan 30 02:36:58 2023, max compression
+gzip compressed data, was "shot-scraper-1.2.tar", last modified: Thu Apr 27 03:05:22 2023, max compression
```

## Comparing `shot-scraper-1.1.1.tar` & `shot-scraper-1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:36:58.819953 shot-scraper-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-01-30 02:36:58.819953 shot-scraper-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 02:36:58.819953 shot-scraper-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:36:58.819953 shot-scraper-1.1.1/shot_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/shot_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30903 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/shot_scraper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-30 02:36:43.000000 shot-scraper-1.1.1/shot_scraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:36:58.819953 shot-scraper-1.1.1/shot_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-30 02:36:58.000000 shot-scraper-1.1.1/shot_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:05:22.925693 shot-scraper-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 03:05:09.000000 shot-scraper-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 03:05:22.925693 shot-scraper-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-27 03:05:09.000000 shot-scraper-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:05:22.925693 shot-scraper-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-27 03:05:09.000000 shot-scraper-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:05:22.925693 shot-scraper-1.2/shot_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:05:09.000000 shot-scraper-1.2/shot_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31900 2023-04-27 03:05:09.000000 shot-scraper-1.2/shot_scraper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-27 03:05:09.000000 shot-scraper-1.2/shot_scraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:05:22.925693 shot-scraper-1.2/shot_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 03:05:22.000000 shot-scraper-1.2/shot_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:05:22.925693 shot-scraper-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-27 03:05:09.000000 shot-scraper-1.2/tests/test_shot_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-27 03:05:09.000000 shot-scraper-1.2/tests/test_utils.py
```

### Comparing `shot-scraper-1.1.1/LICENSE` & `shot-scraper-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shot-scraper-1.1.1/PKG-INFO` & `shot-scraper-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shot-scraper
-Version: 1.1.1
+Version: 1.2
 Summary: A command-line utility for taking automated screenshots of websites
 Home-page: https://github.com/simonw/shot-scraper
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/shot-scraper/issues
 Project-URL: CI, https://github.com/simonw/shot-scraper/actions
 Project-URL: Changelog, https://github.com/simonw/shot-scraper/releases
@@ -15,14 +15,15 @@
 
 # shot-scraper
 
 [![PyPI](https://img.shields.io/pypi/v/shot-scraper.svg)](https://pypi.org/project/shot-scraper/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/shot-scraper?include_prereleases&label=changelog)](https://github.com/simonw/shot-scraper/releases)
 [![Tests](https://github.com/simonw/shot-scraper/workflows/Test/badge.svg)](https://github.com/simonw/shot-scraper/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/shot-scraper/blob/master/LICENSE)
+[![discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://discord.gg/EE7Hx4Kbny)
 
 A command-line utility for taking automated screenshots of websites
 
 For background on this project see [shot-scraper: automated screenshots for documentation, built on Playwright](https://simonwillison.net/2022/Mar/10/shot-scraper/).
 
 ## Documentation
```

### Comparing `shot-scraper-1.1.1/README.md` & `shot-scraper-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # shot-scraper
 
 [![PyPI](https://img.shields.io/pypi/v/shot-scraper.svg)](https://pypi.org/project/shot-scraper/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/shot-scraper?include_prereleases&label=changelog)](https://github.com/simonw/shot-scraper/releases)
 [![Tests](https://github.com/simonw/shot-scraper/workflows/Test/badge.svg)](https://github.com/simonw/shot-scraper/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/shot-scraper/blob/master/LICENSE)
+[![discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://discord.gg/EE7Hx4Kbny)
 
 A command-line utility for taking automated screenshots of websites
 
 For background on this project see [shot-scraper: automated screenshots for documentation, built on Playwright](https://simonwillison.net/2022/Mar/10/shot-scraper/).
 
 ## Documentation
```

### Comparing `shot-scraper-1.1.1/setup.py` & `shot-scraper-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "1.1.1"
+VERSION = "1.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `shot-scraper-1.1.1/shot_scraper/cli.py` & `shot-scraper-1.2/shot_scraper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 def log_console_option(fn):
     click.option("--log-console", is_flag=True, help="Write console.log() to stderr")(
         fn
     )
     return fn
 
 
+def silent_option(fn):
+    click.option("--silent", is_flag=True, help="Do not output any messages")(fn)
+    return fn
+
+
 def skip_fail_options(fn):
     click.option("--skip", is_flag=True, help="Skip pages that return HTTP errors")(fn)
     click.option(
         "--fail",
         is_flag=True,
         help="Fail with an error code if a page returns an HTTP error",
     )(fn)
@@ -147,14 +152,19 @@
     "--padding",
     type=int,
     help="When using selectors, add this much padding in pixels",
     default=0,
 )
 @click.option("-j", "--javascript", help="Execute this JS prior to taking the shot")
 @click.option("--retina", is_flag=True, help="Use device scale factor of 2")
+@click.option(
+    "--omit-background",
+    is_flag=True,
+    help="Omit the default browser background from the shot, making it possible take advantage of transparence. Does not work with JPEGs or when using --quality.",
+)
 @click.option("--quality", type=int, help="Save as JPEG with this quality, e.g. 80")
 @click.option(
     "--wait", type=int, help="Wait this many milliseconds before taking the screenshot"
 )
 @click.option("--wait-for", help="Wait until this JS expression returns true")
 @click.option(
     "--timeout",
@@ -178,40 +188,43 @@
     help="Log details of all requests to this file",
 )
 @log_console_option
 @browser_option
 @user_agent_option
 @reduced_motion_option
 @skip_fail_options
+@silent_option
 def shot(
     url,
     auth,
     output,
     width,
     height,
     selectors,
     selectors_all,
     js_selectors,
     js_selectors_all,
     padding,
     javascript,
     retina,
+    omit_background,
     quality,
     wait,
     wait_for,
     timeout,
     interactive,
     devtools,
     log_requests,
     log_console,
     browser,
     user_agent,
     reduced_motion,
     skip,
     fail,
+    silent,
 ):
     """
     Take a single screenshot of a page or portion of a page.
 
     Usage:
 
         shot-scraper www.example.com
@@ -248,14 +261,15 @@
         "width": width,
         "height": height,
         "quality": quality,
         "wait": wait,
         "wait_for": wait_for,
         "timeout": timeout,
         "padding": padding,
+        "omit_background": omit_background,
         "retina": retina,
     }
     interactive = interactive or devtools
     with sync_playwright() as p:
         use_existing_page = False
         context, browser_obj = _browser_context(
             p,
@@ -282,26 +296,28 @@
                 shot = take_shot(
                     context,
                     shot,
                     return_bytes=True,
                     use_existing_page=use_existing_page,
                     log_requests=log_requests,
                     log_console=log_console,
+                    silent=silent,
                 )
                 sys.stdout.buffer.write(shot)
             else:
                 shot["output"] = str(output)
                 shot = take_shot(
                     context,
                     shot,
                     use_existing_page=use_existing_page,
                     log_requests=log_requests,
                     log_console=log_console,
                     skip=skip,
                     fail=fail,
+                    silent=silent,
                 )
         except TimeoutError as e:
             raise click.ClickException(str(e))
         browser_obj.close()
 
 
 def _browser_context(
@@ -374,28 +390,30 @@
     multiple=True,
 )
 @browser_option
 @user_agent_option
 @reduced_motion_option
 @log_console_option
 @skip_fail_options
+@silent_option
 def multi(
     config,
     auth,
     retina,
     timeout,
     fail_on_error,
     noclobber,
     outputs,
     browser,
     user_agent,
     reduced_motion,
     log_console,
     skip,
     fail,
+    silent,
 ):
     """
     Take multiple screenshots, defined by a YAML file
 
     Usage:
 
         shot-scraper multi config.yml
@@ -435,14 +453,15 @@
             try:
                 take_shot(
                     context,
                     shot,
                     log_console=log_console,
                     skip=skip,
                     fail=fail,
+                    silent=silent,
                 )
             except TimeoutError as e:
                 if fail or fail_on_error:
                     raise click.ClickException(str(e))
                 else:
                     click.echo(str(e), err=True)
                     continue
@@ -641,14 +660,15 @@
     "--scale",
     type=click.FloatRange(min=0.1, max=2.0),
     help="Scale of the webpage rendering",
 )
 @click.option("--print-background", is_flag=True, help="Print background graphics")
 @log_console_option
 @skip_fail_options
+@silent_option
 def pdf(
     url,
     auth,
     output,
     javascript,
     wait,
     media_screen,
@@ -657,14 +677,15 @@
     width,
     height,
     scale,
     print_background,
     log_console,
     skip,
     fail,
+    silent,
 ):
     """
     Create a PDF of the specified page
 
     Usage:
 
         shot-scraper pdf https://datasette.io/
@@ -706,18 +727,16 @@
         if media_screen:
             page.emulate_media(media="screen")
 
         pdf = page.pdf(**kwargs)
 
         if output == "-":
             sys.stdout.buffer.write(pdf)
-        else:
-            click.echo(
-                "Screenshot of '{}' written to '{}'".format(url, output), err=True
-            )
+        elif not silent:
+            click.echo("PDF of '{}' written to '{}'".format(url, output), err=True)
 
         browser_obj.close()
 
 
 @cli.command()
 @click.argument("url")
 @click.option(
@@ -741,26 +760,28 @@
 @click.option(
     "--wait", type=int, help="Wait this many milliseconds before taking the snapshot"
 )
 @log_console_option
 @browser_option
 @user_agent_option
 @skip_fail_options
+@silent_option
 def html(
     url,
     auth,
     output,
     javascript,
     selector,
     wait,
     log_console,
     browser,
     user_agent,
     skip,
     fail,
+    silent,
 ):
     """
     Output the final HTML of the specified page
 
     Usage:
 
         shot-scraper html https://datasette.io/
@@ -791,17 +812,19 @@
         else:
             html = page.content()
 
         if output == "-":
             sys.stdout.write(html)
         else:
             open(output, "w").write(html)
-            click.echo(
-                "HTML snapshot of '{}' written to '{}'".format(url, output), err=True
-            )
+            if not silent:
+                click.echo(
+                    "HTML snapshot of '{}' written to '{}'".format(url, output),
+                    err=True,
+                )
 
         browser_obj.close()
 
 
 @cli.command()
 @click.option(
     "--browser",
@@ -869,43 +892,49 @@
         with open(context_file, "w") as fp:
             fp.write(context_json)
         # chmod 600 to avoid other users on the shared machine reading it
         pathlib.Path(context_file).chmod(0o600)
 
 
 def _check_and_absolutize(filepath):
-    path = pathlib.Path(filepath)
-    if path.exists():
-        return path.absolute()
-    return False
+    try:
+        path = pathlib.Path(filepath)
+        if path.exists():
+            return path.absolute()
+        return False
+    except OSError:
+        # On Windows, instantiating a Path object on `http://` or `https://` will raise an exception
+        return False
 
 
 def take_shot(
     context_or_page,
     shot,
     return_bytes=False,
     use_existing_page=False,
     log_requests=None,
     log_console=False,
     skip=False,
     fail=False,
+    silent=False,
 ):
     url = shot.get("url") or ""
     if not url:
         raise click.ClickException("url is required")
 
     if skip and fail:
         raise click.ClickException("--skip and --fail cannot be used together")
 
     url = url_or_file_path(url, file_exists=_check_and_absolutize)
 
     output = shot.get("output", "").strip()
     if not output and not return_bytes:
         output = filename_for_url(url, ext="png", file_exists=os.path.exists)
     quality = shot.get("quality")
+    omit_background = shot.get("omit_background")
     wait = shot.get("wait")
     wait_for = shot.get("wait_for")
     padding = shot.get("padding") or 0
 
     selectors = shot.get("selectors") or []
     selectors_all = shot.get("selectors_all") or []
     js_selectors = shot.get("js_selectors") or []
@@ -981,14 +1010,16 @@
 
     if wait_for:
         page.wait_for_function(wait_for)
 
     screenshot_args = {}
     if quality:
         screenshot_args.update({"quality": quality, "type": "jpeg"})
+    if omit_background:
+        screenshot_args.update({"omit_background": True})
     if not return_bytes:
         screenshot_args["path"] = output
 
     if (
         not selectors
         and not js_selectors
         and not selectors_all
@@ -1031,15 +1062,16 @@
     else:
         # Whole page
         if return_bytes:
             return page.screenshot(**screenshot_args)
         else:
             page.screenshot(**screenshot_args)
             message = "Screenshot of '{}' written to '{}'".format(url, output)
-    click.echo(message, err=True)
+    if not silent:
+        click.echo(message, err=True)
 
 
 def _js_selector_javascript(js_selectors, js_selectors_all):
     extra_selectors = []
     extra_selectors_all = []
     js_blocks = []
     for js_selector in js_selectors:
```

### Comparing `shot-scraper-1.1.1/shot_scraper/utils.py` & `shot-scraper-1.2/shot_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `shot-scraper-1.1.1/shot_scraper.egg-info/PKG-INFO` & `shot-scraper-1.2/shot_scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shot-scraper
-Version: 1.1.1
+Version: 1.2
 Summary: A command-line utility for taking automated screenshots of websites
 Home-page: https://github.com/simonw/shot-scraper
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/shot-scraper/issues
 Project-URL: CI, https://github.com/simonw/shot-scraper/actions
 Project-URL: Changelog, https://github.com/simonw/shot-scraper/releases
@@ -15,14 +15,15 @@
 
 # shot-scraper
 
 [![PyPI](https://img.shields.io/pypi/v/shot-scraper.svg)](https://pypi.org/project/shot-scraper/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/shot-scraper?include_prereleases&label=changelog)](https://github.com/simonw/shot-scraper/releases)
 [![Tests](https://github.com/simonw/shot-scraper/workflows/Test/badge.svg)](https://github.com/simonw/shot-scraper/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/shot-scraper/blob/master/LICENSE)
+[![discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://discord.gg/EE7Hx4Kbny)
 
 A command-line utility for taking automated screenshots of websites
 
 For background on this project see [shot-scraper: automated screenshots for documentation, built on Playwright](https://simonwillison.net/2022/Mar/10/shot-scraper/).
 
 ## Documentation
```

