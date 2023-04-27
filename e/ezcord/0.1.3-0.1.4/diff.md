# Comparing `tmp/ezcord-0.1.3.tar.gz` & `tmp/ezcord-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.1.3.tar", last modified: Sat Apr 15 22:09:38 2023, max compression
+gzip compressed data, was "ezcord-0.1.4.tar", last modified: Thu Apr 27 14:25:08 2023, max compression
```

## Comparing `ezcord-0.1.3.tar` & `ezcord-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 22:09:24.000000 ezcord-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 22:09:38.609271 ezcord-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-15 22:09:24.000000 ezcord-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 22:09:24.000000 ezcord-0.1.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.605271 ezcord-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 22:09:24.000000 ezcord-0.1.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-15 22:09:24.000000 ezcord-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 22:09:24.000000 ezcord-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 22:09:38.609271 ezcord-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.601271 ezcord-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.605271 ezcord-0.1.3/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/emb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/internal/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 14:24:54.000000 ezcord-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-27 14:25:08.178108 ezcord-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-27 14:24:54.000000 ezcord-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 14:24:54.000000 ezcord-0.1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 14:24:54.000000 ezcord-0.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 14:24:54.000000 ezcord-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 14:24:54.000000 ezcord-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:25:08.178108 ezcord-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.174108 ezcord-0.1.4/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 14:24:54.000000 ezcord-0.1.4/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:25:08.178108 ezcord-0.1.4/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 14:25:08.000000 ezcord-0.1.4/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.1.3/LICENSE` & `ezcord-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.3/PKG-INFO` & `ezcord-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.1.3/README.md` & `ezcord-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.3/pyproject.toml` & `ezcord-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.3/src/ezcord/bot.py` & `ezcord-0.1.4/src/ezcord/bot.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from pathlib import Path
 from typing import Any, Literal
 
 import aiohttp
 import discord
 from discord.ext import commands
 
+from .emb import error as error_emb
 from .internal.translation import set_lang, t
-from .logs import DEFAULT_LOG, set_log
-from .times import convert_time
+from .logs import DEFAULT_LOG, custom_log, set_log
+from .times import dc_timestamp
 
 
 class Bot(discord.Bot):
     """Bot class that extends from :class:`discord.Bot`.
 
     Parameters
     ----------
@@ -30,88 +31,110 @@
     error_webhook_url:
         The webhook URL to send error messages to. Defaults to ``None``.
 
         .. note::
             You need to enable the error handler for the webhook to work.
     ignored_errors:
         A list of error types to ignore. Defaults to ``None``.
+    full_error_traceback:
+        Whether to send the full error traceback. If this is ``False``,
+        only the most recent traceback will be sent. Defaults to ``False``.
     language:
         The language to use for the bot. Defaults to ``en``.
     """
 
     def __init__(
         self,
         intents: discord.Intents = discord.Intents.default(),
+        *,
         debug: bool = True,
         error_handler: bool = True,
         error_webhook_url: str | None = None,
         ignored_errors: list[Any] | None = None,
+        full_error_traceback: bool = False,
         language: Literal["en", "de"] = "en",
-        *args,
         **kwargs,
     ):
-        super().__init__(intents=intents, *args, **kwargs)
+        super().__init__(intents=intents, **kwargs)
 
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
             self.logger = logging.getLogger(DEFAULT_LOG)
             self.logger.addHandler(logging.NullHandler())
 
         self.error_webhook_url = error_webhook_url
         self.ignored_errors = ignored_errors or []
+        self.full_error_traceback = full_error_traceback
         set_lang(language)
 
         if error_handler:
             self.add_listener(self._error_event, "on_application_command_error")
         elif error_webhook_url:
             warnings.warn("You need to enable the error handler for the webhook to work.")
 
         self.add_listener(self.ready_event, "on_ready")
 
     def load_cogs(
         self,
         *directories: str,
         subdirectories: bool = False,
         ignored_cogs: list[str] | None = None,
+        custom_logs: bool | str = True,
     ):
         """Load all cogs in the given directories.
 
         Parameters
         ----------
         *directories:
             Names of the directories to load cogs from.
             Defaults to ``cogs``.
         subdirectories:
             Whether to load cogs from subdirectories.
             Defaults to ``False``.
         ignored_cogs:
             A list of cogs to ignore. Defaults to ``None``.
+        custom_logs:
+            Whether to use a custom log format for cogs. Defaults to ``True``.
+            You can also pass in a custom color.
         """
         ignored_cogs = ignored_cogs or []
         if not directories:
             directories = ("cogs",)
 
         for directory in directories:
             path = Path(directory)
 
             for filename in os.listdir(directory):
-                if filename.endswith(".py") and filename not in ignored_cogs:
-                    self.load_extension(f"{'.'.join(path.parts)}.{filename[:-3]}")
-                    self.logger.debug(f"Loaded {filename[:-3]}")
+                name = filename[:-3]
+                if filename.endswith(".py") and name not in ignored_cogs:
+                    self.load_extension(f"{'.'.join(path.parts)}.{name}")
+                    if custom_logs:
+                        custom_log("COG", f"Loaded {name}", color=custom_logs, level=logging.DEBUG)
+                    else:
+                        self.logger.debug(f"Loaded {name}")
 
             if subdirectories:
                 for element in os.scandir(directory):
-                    if element.is_dir():
-                        for sub_file in os.scandir(element.path):
-                            if sub_file.name.endswith(".py") and sub_file.name not in ignored_cogs:
-                                self.load_extension(
-                                    f"{'.'.join(path.parts)}.{element.name}.{sub_file.name[:-3]}"
+                    if not element.is_dir():
+                        continue
+
+                    for sub_file in os.scandir(element.path):
+                        name = sub_file.name[:-3]
+                        if sub_file.name.endswith(".py") and name not in ignored_cogs:
+                            self.load_extension(f"{'.'.join(path.parts)}.{element.name}.{name}")
+                            if custom_logs:
+                                custom_log(
+                                    "COG",
+                                    f"Loaded {element.name}.{name}",
+                                    color=custom_logs,
+                                    level=logging.DEBUG,
                                 )
-                                self.logger.debug(f"Loaded {element.name}.{sub_file.name[:-3]}")
+                            else:
+                                self.logger.debug(f"Loaded {element.name}.{name}")
 
     async def ready_event(self):
         """Prints the bot's information when it's ready."""
         infos = [
             f"User:     {self.user}",
             f"ID:       {self.user.id}",
             f"Pycord:   {discord.__version__}",
@@ -131,61 +154,73 @@
         self.logger.info(start_txt)
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
 
-        embed = discord.Embed(
-            title="Error", description=f"{t('error')}: ```{error}```", color=discord.Color.red()
-        )
-
         if isinstance(error, commands.CommandOnCooldown):
             seconds = round(ctx.command.get_cooldown_retry_after(ctx))
-            embed.title = "Cooldown"
-            embed.description = t("cooldown", convert_time(seconds))
-            await ctx.respond(embed=embed, ephemeral=True)
+            cooldown_txt = t("cooldown", dc_timestamp(seconds))
+            await error_emb(ctx, cooldown_txt, title="Cooldown")
 
         elif isinstance(error, commands.BotMissingPermissions):
             perms = "\n".join(error.missing_permissions)
-            embed.title = t("no_perm_title")
-            embed.description = f"{t('no_perm_desc')} ```\n{perms}```"
-            await ctx.respond(embed=embed, ephemeral=True)
+            perm_txt = f"{t('no_perm_desc')} ```\n{perms}```"
+            await error_emb(ctx, perm_txt, title=t("no_perm_title"))
 
         else:
+            if "original" in error.__dict__ and not self.full_error_traceback:
+                original_error = error.__dict__["original"]
+                error_msg = f"{original_error.__class__.__name__}: {error.__cause__}"
+                error = original_error
+            else:
+                error_msg = f"{error}"
+
+            error_txt = f"{t('error')}: ```{error_msg}```"
             try:
-                await ctx.respond(embed=embed, ephemeral=True)
+                await error_emb(ctx, error_txt, title="Error")
             except discord.HTTPException:
-                raise error
+                pass
 
+            webhook_sent = False
             if self.error_webhook_url:
                 async with aiohttp.ClientSession() as session:
                     webhook = discord.Webhook.from_url(
                         self.error_webhook_url, session=session, bot_token=self.http.token
                     )
                     error_txt = "".join(
                         traceback.format_exception(type(error), error, error.__traceback__)
                     )
                     guild_txt = (
-                        f"\n\n`Guild:` {ctx.guild.name} ({ctx.guild.id})" if ctx.guild else ""
+                        f"\n- **Guild:** {ctx.guild.name} - `{ctx.guild.id}`" if ctx.guild else ""
+                    )
+                    user_txt = (
+                        f"\n- **User:** {ctx.author} - `{ctx.author.id}`" if ctx.author else ""
                     )
-                    user_txt = f"\n\n`User:` {ctx.author} ({ctx.author.id})" if ctx.author else ""
 
                     embed = discord.Embed(
                         title="Error Report",
-                        description=f"`Command:` /{ctx.command.name}"
+                        description=f"- **Command:** /{ctx.command.qualified_name}"
                         f"{guild_txt}{user_txt}"
-                        f"```{error_txt[:3500]}```",
+                        f"\n```py\n{error_txt[:3500]}```",
                         color=discord.Color.red(),
                     )
                     try:
                         await webhook.send(
                             embed=embed,
                             username=f"{self.user.name} Error Report",
                             avatar_url=self.user.display_avatar.url,
                         )
                     except discord.HTTPException:
                         self.logger.error(
                             "Error while sending error report to webhook. "
-                            "Please check if you the URL is correct."
+                            "Please check if the URL is correct."
                         )
-            raise error
+                    else:
+                        webhook_sent = True
+
+            self.logger.exception(
+                f"Error while executing **/{ctx.command.qualified_name}** ```{error_msg}```",
+                exc_info=error,
+                extra={"webhook_sent": webhook_sent},
+            )
```

### Comparing `ezcord-0.1.3/src/ezcord/internal/languages.py` & `ezcord-0.1.4/src/ezcord/internal/languages.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,27 +3,27 @@
         "min": "Minute",
         "sec": "Sekunde",
         "hour": "Stunde",
         "day": "Tag",
     },
     "bot": {
         "error": "Der folgende Fehler ist aufgetreten",
-        "cooldown": "Versuche es in `{}` erneut.",
+        "cooldown": "Versuche es {} erneut.",
         "no_perm_title": "Fehlende Berechtigung",
         "no_perm_desc": "Mir fehlen die folgenden Berechtigungen, um diesen Befehl auszuführen.",
     },
 }
 
 en = {
     "times": {
         "min": "minute",
         "sec": "second",
         "hour": "hour",
         "day": "day",
     },
     "bot": {
         "error": "The following error occurred",
-        "cooldown": "Try again in `{}`.",
+        "cooldown": "Try again {}.",
         "no_perm_title": "Missing permission",
         "no_perm_desc": "I'm missing the following permissions to execute this command.",
     },
 }
```

### Comparing `ezcord-0.1.3/src/ezcord/internal/translation.py` & `ezcord-0.1.4/src/ezcord/internal/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Internal language utilities for the library."""
 
 import inspect
 import os
 from configparser import ConfigParser
+from functools import cache
 from pathlib import Path
 from typing import Literal
 
 from .languages import *
 
 
 def plural_de(amount: int, word: str, relative: bool = True) -> str:
@@ -104,14 +105,15 @@
 
     if lang == "de":
         return de[origin_file][key].format(*args)
     else:
         return en[origin_file][key].format(*args)
 
 
+@cache
 def get_lang():
     """Get the language from the config file."""
     parent = Path(__file__).parent.absolute()
     config = ConfigParser()
     config.read(os.path.join(parent, "config.ini"))
 
     return config["DEFAULT"]["lang"]
```

### Comparing `ezcord-0.1.3/src/ezcord/times.py` & `ezcord-0.1.4/src/ezcord/times.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     if hours < 24:
         return f"{round(hours)} {tp('hour', round(hours))}"
     days = hours / 24
     return f"{round(days)} {tp('day', round(days), relative=relative)}"
 
 
 def convert_dt(dt: datetime | timedelta, relative: bool = True) -> str:
-    """Convert :class:`datetime` or :class:`timedelta` to a human-readable relative time.
+    """Convert :class:`datetime` or :class:`timedelta` to a human-readable time.
 
     This function calls :func:`convert_time`.
 
     Parameters
     ----------
     dt:
         The datetime or timedelta object to convert.
@@ -75,15 +75,17 @@
     if isinstance(dt, timedelta):
         return convert_time(abs(dt.total_seconds()), relative)
 
     if isinstance(dt, datetime):
         return convert_time(abs((dt - utcnow()).total_seconds()), relative)
 
 
-def dc_timestamp(seconds: int, style: Literal["t", "T", "d", "D", "f", "F", "R"] = "R") -> str:
+def dc_timestamp(
+    seconds: int | float, style: Literal["t", "T", "d", "D", "f", "F", "R"] = "R"
+) -> str:
     """Convert seconds to a Discord timestamp.
 
     Parameters
     ----------
     seconds:
         The amount of seconds to convert.
     style: :class:`str`
```

### Comparing `ezcord-0.1.3/src/ezcord/utils.py` & `ezcord-0.1.4/src/ezcord/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,15 @@
         Keyword arguments for :class:`discord.File`.
 
     Returns
     -------
     :class:`discord.File`
     """
     content = json.dumps(dictionary, indent=2).encode()
-    file = discord.File(io.BytesIO(content), filename=filename, **kwargs)
-    return file
+    return discord.File(io.BytesIO(content), filename=filename, **kwargs)
 
 
 def create_text_file(text: str, filename: str = "data.txt", **kwargs):
     """Create a :class:`discord.File` object from a string.
 
     Parameters
     ----------
```

### Comparing `ezcord-0.1.3/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.1.4/src/ezcord.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

