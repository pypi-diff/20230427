# Comparing `tmp/timeturner-0.2.0.tar.gz` & `tmp/timeturner-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeturner-0.2.0.tar", max compression
+gzip compressed data, was "timeturner-0.3.0a0.tar", max compression
```

## Comparing `timeturner-0.2.0.tar` & `timeturner-0.3.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.2.0/LICENSE
--rw-r--r--   0        0        0     5683 2023-04-14 20:04:24.907411 timeturner-0.2.0/README.md
--rw-r--r--   0        0        0     1161 2023-04-14 20:05:50.627664 timeturner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-14 20:06:01.657697 timeturner-0.2.0/timeturner/__init__.py
--rw-r--r--   0        0        0    12333 2023-04-14 14:18:21.859089 timeturner-0.2.0/timeturner/db.py
--rw-r--r--   0        0        0      293 2023-04-14 19:29:21.172846 timeturner-0.2.0/timeturner/helper.py
--rw-r--r--   0        0        0     3015 2023-04-14 14:18:26.695772 timeturner-0.2.0/timeturner/loader.py
--rw-r--r--   0        0        0     2569 2023-04-14 19:30:34.596455 timeturner-0.2.0/timeturner/models.py
--rw-r--r--   0        0        0     8466 2023-04-13 19:58:09.637254 timeturner-0.2.0/timeturner/parser.py
--rw-r--r--   0        0        0     2996 2023-04-14 19:46:59.840550 timeturner-0.2.0/timeturner/rich_output.py
--rw-r--r--   0        0        0     2328 2023-04-14 18:47:24.435713 timeturner-0.2.0/timeturner/run.py
--rw-r--r--   0        0        0     2086 2023-03-29 15:39:11.994974 timeturner-0.2.0/timeturner/settings.py
--rw-r--r--   0        0        0     8515 2023-04-14 19:33:15.290413 timeturner-0.2.0/timeturner/timeturner.py
--rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.2.0/timeturner/tools/boltons_iterutils.py
--rw-r--r--   0        0        0     6699 1970-01-01 00:00:00.000000 timeturner-0.2.0/setup.py
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 timeturner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     6099 2023-04-20 17:44:07.808207 timeturner-0.3.0a0/README.md
+-rw-r--r--   0        0        0     1163 2023-04-27 12:01:12.321609 timeturner-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-27 12:02:37.218708 timeturner-0.3.0a0/timeturner/__init__.py
+-rw-r--r--   0        0        0    12422 2023-04-16 18:53:08.962749 timeturner-0.3.0a0/timeturner/db.py
+-rw-r--r--   0        0        0      674 2023-04-16 19:13:02.245927 timeturner-0.3.0a0/timeturner/helper.py
+-rw-r--r--   0        0        0     3015 2023-04-14 14:18:26.695772 timeturner-0.3.0a0/timeturner/loader.py
+-rw-r--r--   0        0        0     2534 2023-04-20 15:54:26.254760 timeturner-0.3.0a0/timeturner/models.py
+-rw-r--r--   0        0        0     8708 2023-04-20 15:54:38.728125 timeturner-0.3.0a0/timeturner/parser.py
+-rw-r--r--   0        0        0     3048 2023-04-20 15:55:29.878254 timeturner-0.3.0a0/timeturner/rich_output.py
+-rw-r--r--   0        0        0     2614 2023-04-20 19:55:13.187167 timeturner-0.3.0a0/timeturner/run.py
+-rw-r--r--   0        0        0     5890 2023-04-20 19:51:16.822890 timeturner-0.3.0a0/timeturner/settings.py
+-rw-r--r--   0        0        0    16051 2023-04-20 19:54:37.770360 timeturner-0.3.0a0/timeturner/timeturner.py
+-rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.3.0a0/timeturner/tools/boltons_iterutils.py
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 timeturner-0.3.0a0/setup.py
+-rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 timeturner-0.3.0a0/PKG-INFO
```

### Comparing `timeturner-0.2.0/LICENSE` & `timeturner-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeturner-0.2.0/README.md` & `timeturner-0.3.0a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -36,19 +36,28 @@
 
 If you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`
 
 ![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)
 
 ### Adding a public holiday
 
-> **Warning:**
-> This is not final yet.
+To add May 1st as a public holiday, run the following command:
+
+![`timeturner add 05-01 @holiday`](img/add_holiday.svg)
+
+### Adding your vacation
+
+To add your vacation, run the following command:
+
+![`timeturner add 04-25 - 05-14 @vacation`](img/add_vacation.svg)
+
+Adding your vacation will add a segments that are not part of holidays, it will also split
+weekends and only add working days as vacation.
+
 
-If you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after
-the activity times when adding a new event.
 
 
 ## Configuration
 
 | Environment Variable       | Default Value                    | Description                                  |
 | -------------------------- | -------------------------------- | -------------------------------------------- |
 | TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |
@@ -84,60 +93,66 @@
 If you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.
 
 
 
 TODOs:
 - [ ] Add Configuration
   - [ ] ignore seconds
-  - [ ] freeze time, to generate useful images
+  - [ ] freeze time, to generate useful and pretty images for docs
   - [ ] automatic rest periods
+  - [ ] default work time
+  - [ ] default work week days
+- [ ] allow full day activities to coexist with other activities
+  - [ ] travel time and holiday could happen
+- [ ] DB migrations
 - [ ] show and generate tui output
 - [ ] Add section about contributions
 - [ ] Add precommit hook to ensure code is formatted
 - [ ] Generate docstrings for DB methods
 - [ ] Remove import command (it contains assumptions that will not be true for everyone)
   - [ ] Document how to import data from other time trackers
   - [ ] Add mode to convert hamster output to jsonl file.
   - [ ] Add mode to import jsonl file
 - [ ] Add logging
   - [ ] allow different log levels for database and application
 - [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app
 - [ ] README
   - [ ] auto generate config options
-- [ ] db
-  - [ ] add table for tags
 
 
 TODOS by command:
 
-- [ ] add
-  - [ ] allow passive activities
-  - [ ] allow sick days
-  - [ ] allow vacation days
-  - [x] allow for public holidays
+- [x] add
+
 - [ ] end
   - [ ] add tests
 
 - [ ] configure
   - [ ] modify and write configfile
   - [ ] allow to add aliases for commands
     - [ ] e.g. new new add alias with setting passive to true
+  - [ ] add test when holiday tag name is changed in settings
+
 - [ ] list
   - [ ] split up multiday activities
+  - [ ] summaries full day tags differently
   - [x] holidays should not count as work time
     - [x] it should also not count as missing work time
-  - [ ] group by year, month, week, day
+  - [ ] group by year, month, week, daysplit up multiday activities
   - [ ] add option to show only open activities
   - [ ] add tests
+
 - [ ] import holidays
+
 - [ ] export
   - [ ] probably like list --format jsonl
 
 - [ ] undo (revert the last change)
 - [ ] confirm changes that would modify other entries
+
 ### Design Goals
 
 - minimalistic, little to type
 - enforce as little as possible
 - be clear
 - be extensible
   - TODO: support plugins (maybe a later version)
```

### Comparing `timeturner-0.2.0/pyproject.toml` & `timeturner-0.3.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeturner"
-version = "0.2.0"
+version = "0.3.0a0"
 description = ""
 authors = ["Olaf Gladis <olaf@gladis.org>"]
 readme = "README.md"
 packages = [{ include = "timeturner" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timeturner-0.2.0/timeturner/db.py` & `timeturner-0.3.0a0/timeturner/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,23 +315,25 @@
         end: Optional[DateTime] = None,
     ) -> list[PensiveRow]:
         """
         Get all segments between the given start and end times.
 
         This includes segments that start before the given start time and / or end after
         the given end time.
+
+        end is exclusive, i.e. segments that end at the given end time are not included.
         """
         cursor = self.connection.cursor()
         end_is_none = end is None
         if end is None:
             end = start
         cursor.execute(
             f"""
             SELECT pk, start, end, passive, description FROM {self.table_name}
-            WHERE start <= ? AND (end >= ? OR end IS NULL)
+            WHERE start <= ? AND (end > ? OR end IS NULL)
             ORDER BY start ASC
             """,
             (str(end), str(start)),
         )
 
         rows = cursor.fetchall()
         collected_rows = [
```

### Comparing `timeturner-0.2.0/timeturner/loader.py` & `timeturner-0.3.0a0/timeturner/loader.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.2.0/timeturner/models.py` & `timeturner-0.3.0a0/timeturner/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Optional, cast
 
 import pendulum
 from pendulum.date import Date
 from pendulum.datetime import DateTime
 from pendulum.duration import Duration
 from pendulum.parser import parse
-from pendulum.period import Period
 from pendulum.time import Time
 from pydantic import BaseModel, validator
 
 
 class DayType(Enum):
     WORK = auto()
     HOLIDAY = auto()
```

### Comparing `timeturner-0.2.0/timeturner/parser.py` & `timeturner-0.3.0a0/timeturner/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
 
 # from pendulum.tz.timezone import Timezone
 from enum import Enum
-from typing import Any, Literal, TypedDict, cast, overload
+from typing import Any, TypedDict
 
 import pendulum
 from pendulum.datetime import DateTime
 from pendulum.duration import Duration
 
+from timeturner.helper import end_of, end_of_day
 from timeturner.models import NewSegmentParams
+from timeturner.settings import ReportSettings
 
 delta_components = re.compile(r"(?P<sign>[+-])?(?P<value>\d+)(?P<unit>[mhd])")
 range_components = re.compile(r"(?P<value>\d+)?(?P<unit>[dwMyY]|day|week|month|year)s?")
 
 
 class ComponentType(Enum):
     TIME = "time"
@@ -194,34 +196,38 @@
 
 
 def parse_add_args(
     args: list[str],
     *,
     prefer_full_days: bool = False,
     holiday: bool = False,
+    report_settings: ReportSettings,
 ) -> NewSegmentParams:
     args, tags = split_filter_tags(args)
-    if "_holiday" in tags:
-        holiday = True
     if holiday:
-        if "_holiday" not in tags:
-            tags.append("_holiday")
-        prefer_full_days = True
+        if report_settings.holiday_tag not in tags:
+            tags.append(report_settings.holiday_tag)
+    for tag in tags:
+        if tag not in report_settings.tag_settings:
+            continue
+        if report_settings.tag_settings[tag].full_day:
+            prefer_full_days = True
+
     start, end = split_array(args, "-")
     start = single_time_parse(start)
     if end:
         end = single_time_parse(end, now=start)
     else:
         end = None
     if prefer_full_days:
         start = start.start_of("day")
         if not end:
-            end = start.end_of("day")
+            end = end_of_day(start)
         else:
-            end = end.end_of("day")
+            end = end_of_day(end)
     return NewSegmentParams(
         start=start,
         end=end,
         tags=tags,
     )
 
 
@@ -230,53 +236,53 @@
     *,
     now: DateTime | None = None,
 ) -> tuple[DateTime, DateTime]:
     if now is None:
         now = pendulum.now()
     now = now.set(second=0, microsecond=0)
     start = now.start_of("day")
-    end = now.end_of("day")
+    end = end_of_day(now)
     if "-" in args:
         start, end = split_array(args, "-")
         start = single_time_parse(start, now=now)
         end = single_time_parse(end, now=start)
 
         if start.time() == now.time():
             start = start.start_of("day")
         if end.time() == now.time():
-            end = end.end_of("day")
+            end = end_of_day(end)
 
     elif len(args) == 0:
         pass
     elif len(args) == 1:
         arg = args[0]
         if arg in ["week", "month", "year"]:
             start = now.start_of(arg)
-            end = now.end_of(arg)
+            end = end_of(now, arg)
         elif arg == "today":
             pass
         elif arg == "yesterday":
             start = start.subtract(days=1)
             end = end.subtract(days=1)
         elif _match := range_components.match(arg):
             match _match.groupdict():
                 case {"value": value, "unit": "d" | "day" | "days"}:
                     start = start.subtract(days=int(value) - 1)
                 case {"value": value, "unit": "w" | "week" | "weeks"}:
                     start = start.start_of("week").subtract(weeks=int(value) - 1)
-                    end = now.end_of("week")
+                    end = end_of(now, "week")
                 case {"value": value, "unit": "M" | "month" | "months"}:
                     start = start.start_of("month").subtract(months=int(value) - 1)
-                    end = now.end_of("month")
+                    end = end_of(now, "month")
                 case {  # pragma: no branch
                     "value": value,
                     "unit": "y" | "year" | "years",
                 }:
                     start = start.start_of("year").subtract(years=int(value) - 1)
-                    end = now.end_of("year")
+                    end = end_of(now, "year")
 
         else:
             start = single_time_parse(args, now=now).start_of("day")
     else:
         # we have 2 arguments, but no dash
         # we definitely define a specific time, so we don't change to
         # the start of the day, or the end of the day
```

### Comparing `timeturner-0.2.0/timeturner/rich_output.py` & `timeturner-0.3.0a0/timeturner/rich_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,18 @@
     total_over = []
     w = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
     for segment in segments:
         total_work.append(segment.summary.work_time)
         total_break.append(segment.summary.break_time)
         total_over.append(segment.summary.over_time)
         if segment.summary.start:
-            start_str = f"[bold]{w[segment.day.weekday()]}[/] {segment.day} {segment.summary.start.format('HH:mm')}"
+            start_str = (
+                f"[bold]{w[segment.day.weekday()]}[/] {segment.day} "
+                f"{segment.summary.start.format('HH:mm')}"
+            )
         else:
             start_str = f"[bold]{w[segment.day.weekday()]}[/] {segment.day}"
         table.add_row(
             start_str,
             segment.summary.end.format("HH:mm") if segment.summary.end else "",
             str(segment.summary.day_type.value),
             pretty_duration(segment.summary.work_time),
```

### Comparing `timeturner-0.2.0/timeturner/run.py` & `timeturner-0.3.0a0/timeturner/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,29 @@
 
 
 @app.callback(no_args_is_help=True)
 def callback(
     output: Optional[Output] = None,
 ):
     global settings
-    additional_settings_args = dict()
     if output is not None:
-        additional_settings_args["output"] = output
-    if additional_settings_args:
-        settings = TimeTurnerSettings(**additional_settings_args)
+        if output not in ("json", "rich"):
+            raise typer.BadParameter("Output must be either 'json' or 'rich'")
+        settings.report.output = output
 
 
 @app.command("l", hidden=True)
 @app.command("list")
 def _list(time: Optional[list[str]] = typer.Argument(None)):
-    data = timeturner.list_(time, db=settings.database.connection)
-    if settings.output == "json":
+    data = timeturner.list_(
+        time,
+        report_settings=settings.report,
+        db=settings.database.connection,
+    )
+    if settings.report.output == "json":
         console.print_json(data=data, default=pydantic_encoder)
     else:
         rich_output.segments_by_day(data)
 
 
 @app.command("a", hidden=True)
 @app.command()
@@ -52,35 +55,47 @@
     # passive: bool | None = False,
     # tags: str | None = None,
     # description: str | None = None,
 ):
     data = timeturner.add(
         time,
         holiday=holiday,
+        report_settings=settings.report,
         db=settings.database.connection,
     )
-    if settings.output == "json":
+    if settings.report.output == "json":
         console.print_json(data=data, default=pydantic_encoder)
     else:
-        rich_output.print_pretty_record(data)
+        for segment in data:
+            rich_output.print_pretty_record(segment)
 
 
 @app.command("e", hidden=True)
 @app.command("end")
 def end(
     time: Optional[list[str]] = typer.Argument(None),
 ):
-    data = timeturner.end(time, db=settings.database.connection)
+    data = timeturner.end(
+        time,
+        report_settings=settings.report,
+        db=settings.database.connection,
+    )
     console.print_json(data=data, default=pydantic_encoder)
 
 
 @app.command("i", hidden=True)
 @app.command(name="import")
 def import_(text_file: Path):
-    data = list(timeturner.import_json(text_file, db=settings.database.connection))
+    data = list(
+        timeturner.import_json(
+            text_file,
+            report_settings=settings.report,
+            db=settings.database.connection,
+        )
+    )
     console.print_json(data=data, default=pydantic_encoder)
 
 
 @app.command("c", hidden=True)
 @app.command(name="config")
 def config():
     console.print_json(data=settings, default=pydantic_encoder)
```

### Comparing `timeturner-0.2.0/timeturner/tools/boltons_iterutils.py` & `timeturner-0.3.0a0/timeturner/tools/boltons_iterutils.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.2.0/setup.py` & `timeturner-0.3.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 entry_points = \
 {'console_scripts': ['timeturner = timeturner.run:entrypoint',
                      'tt = timeturner.run:entrypoint']}
 
 setup_kwargs = {
     'name': 'timeturner',
-    'version': '0.2.0',
+    'version': '0.3.0a0',
     'description': '',
-    'long_description': 'Time Turner\n===========\n\n## A Minimalistic Time Tracker.\n\nThis is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.\n\nIn the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.\n\n**Warning, this is still an alpha release, the API is not stable yet.**\n\n## Usage\n\n### Starting an Activity\n\nTo start tracking an activity, run the following command:\n\n\n![`timeturner add`](img/add.svg)\n\nThis will record the current time as the start of your activity.\n\nIf you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)\n\n### Stopping an Activity\n\nTo stop tracking the current activity, run the following command:\n\n\n![`timeturner end`](img/end.svg)\n\n\nThis will record the current time as the end of your activity and calculate the total duration.\n\n### Adding a Past Activity\n\nIf you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`\n\n![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)\n\n### Adding a public holiday\n\n> **Warning:**\n> This is not final yet.\n\nIf you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after\nthe activity times when adding a new event.\n\n\n## Configuration\n\n| Environment Variable       | Default Value                    | Description                                  |\n| -------------------------- | -------------------------------- | -------------------------------------------- |\n| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |\n| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |\n| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |\n| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |\n| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |\n\n## Examples\n\n### Examples for times\n\n<start_time> or <end_time> could be one of the following Examples:\n\n| Example         | Description                               |\n| --------------- | ----------------------------------------- |\n|                 | now                                       |\n| 9:00            | 9:00 today                                |\n| -1m             | 1 minute ago                              |\n| -1h             | 1 hour ago                                |\n| -1d             | 1 day ago, you will be asked for the time |\n| -1d@9:00        | 1 day ago 9:00                            |\n| +1m             | 1 minute from now                         |\n| +1h             | 1 hour from now                           |\n| 12 7:00         | 7:00 on the 12th of the current month     |\n| 02-28 9:00      | 9:00 on February 28 of the current year   |\n| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |\n\n\n\n### Automatic Rest Periods\n\nIf you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.\n\n\n\nTODOs:\n- [ ] Add Configuration\n  - [ ] ignore seconds\n  - [ ] freeze time, to generate useful images\n  - [ ] automatic rest periods\n- [ ] show and generate tui output\n- [ ] Add section about contributions\n- [ ] Add precommit hook to ensure code is formatted\n- [ ] Generate docstrings for DB methods\n- [ ] Remove import command (it contains assumptions that will not be true for everyone)\n  - [ ] Document how to import data from other time trackers\n  - [ ] Add mode to convert hamster output to jsonl file.\n  - [ ] Add mode to import jsonl file\n- [ ] Add logging\n  - [ ] allow different log levels for database and application\n- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app\n- [ ] README\n  - [ ] auto generate config options\n- [ ] db\n  - [ ] add table for tags\n\n\nTODOS by command:\n\n- [ ] add\n  - [ ] allow passive activities\n  - [ ] allow sick days\n  - [ ] allow vacation days\n  - [x] allow for public holidays\n- [ ] end\n  - [ ] add tests\n\n- [ ] configure\n  - [ ] modify and write configfile\n  - [ ] allow to add aliases for commands\n    - [ ] e.g. new new add alias with setting passive to true\n- [ ] list\n  - [ ] split up multiday activities\n  - [x] holidays should not count as work time\n    - [x] it should also not count as missing work time\n  - [ ] group by year, month, week, day\n  - [ ] add option to show only open activities\n  - [ ] add tests\n- [ ] import holidays\n- [ ] export\n  - [ ] probably like list --format jsonl\n\n- [ ] undo (revert the last change)\n- [ ] confirm changes that would modify other entries\n### Design Goals\n\n- minimalistic, little to type\n- enforce as little as possible\n- be clear\n- be extensible\n  - TODO: support plugins (maybe a later version)\n  - be able to use it programmatically\n  - be able to use it as a library\n\n\n### Open Questions\n\n- [ ] should the get_latest_segment return segments from the future (start_time in the future)?\n\n### Nice to have:\n- [ ] Build a minimal Docker image (maybe)\n- [ ] https://github.com/ines/termynal\n',
+    'long_description': 'Time Turner\n===========\n\n## A Minimalistic Time Tracker.\n\nThis is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.\n\nIn the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.\n\n**Warning, this is still an alpha release, the API is not stable yet.**\n\n## Usage\n\n### Starting an Activity\n\nTo start tracking an activity, run the following command:\n\n\n![`timeturner add`](img/add.svg)\n\nThis will record the current time as the start of your activity.\n\nIf you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)\n\n### Stopping an Activity\n\nTo stop tracking the current activity, run the following command:\n\n\n![`timeturner end`](img/end.svg)\n\n\nThis will record the current time as the end of your activity and calculate the total duration.\n\n### Adding a Past Activity\n\nIf you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`\n\n![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)\n\n### Adding a public holiday\n\nTo add May 1st as a public holiday, run the following command:\n\n![`timeturner add 05-01 @holiday`](img/add_holiday.svg)\n\n### Adding your vacation\n\nTo add your vacation, run the following command:\n\n![`timeturner add 04-25 - 05-14 @vacation`](img/add_vacation.svg)\n\nAdding your vacation will add a segments that are not part of holidays, it will also split\nweekends and only add working days as vacation.\n\n\n\n\n## Configuration\n\n| Environment Variable       | Default Value                    | Description                                  |\n| -------------------------- | -------------------------------- | -------------------------------------------- |\n| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |\n| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |\n| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |\n| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |\n| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |\n\n## Examples\n\n### Examples for times\n\n<start_time> or <end_time> could be one of the following Examples:\n\n| Example         | Description                               |\n| --------------- | ----------------------------------------- |\n|                 | now                                       |\n| 9:00            | 9:00 today                                |\n| -1m             | 1 minute ago                              |\n| -1h             | 1 hour ago                                |\n| -1d             | 1 day ago, you will be asked for the time |\n| -1d@9:00        | 1 day ago 9:00                            |\n| +1m             | 1 minute from now                         |\n| +1h             | 1 hour from now                           |\n| 12 7:00         | 7:00 on the 12th of the current month     |\n| 02-28 9:00      | 9:00 on February 28 of the current year   |\n| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |\n\n\n\n### Automatic Rest Periods\n\nIf you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.\n\n\n\nTODOs:\n- [ ] Add Configuration\n  - [ ] ignore seconds\n  - [ ] freeze time, to generate useful and pretty images for docs\n  - [ ] automatic rest periods\n  - [ ] default work time\n  - [ ] default work week days\n- [ ] allow full day activities to coexist with other activities\n  - [ ] travel time and holiday could happen\n- [ ] DB migrations\n- [ ] show and generate tui output\n- [ ] Add section about contributions\n- [ ] Add precommit hook to ensure code is formatted\n- [ ] Generate docstrings for DB methods\n- [ ] Remove import command (it contains assumptions that will not be true for everyone)\n  - [ ] Document how to import data from other time trackers\n  - [ ] Add mode to convert hamster output to jsonl file.\n  - [ ] Add mode to import jsonl file\n- [ ] Add logging\n  - [ ] allow different log levels for database and application\n- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app\n- [ ] README\n  - [ ] auto generate config options\n\n\nTODOS by command:\n\n- [x] add\n\n- [ ] end\n  - [ ] add tests\n\n- [ ] configure\n  - [ ] modify and write configfile\n  - [ ] allow to add aliases for commands\n    - [ ] e.g. new new add alias with setting passive to true\n  - [ ] add test when holiday tag name is changed in settings\n\n- [ ] list\n  - [ ] split up multiday activities\n  - [ ] summaries full day tags differently\n  - [x] holidays should not count as work time\n    - [x] it should also not count as missing work time\n  - [ ] group by year, month, week, daysplit up multiday activities\n  - [ ] add option to show only open activities\n  - [ ] add tests\n\n- [ ] import holidays\n\n- [ ] export\n  - [ ] probably like list --format jsonl\n\n- [ ] undo (revert the last change)\n- [ ] confirm changes that would modify other entries\n\n### Design Goals\n\n- minimalistic, little to type\n- enforce as little as possible\n- be clear\n- be extensible\n  - TODO: support plugins (maybe a later version)\n  - be able to use it programmatically\n  - be able to use it as a library\n\n\n### Open Questions\n\n- [ ] should the get_latest_segment return segments from the future (start_time in the future)?\n\n### Nice to have:\n- [ ] Build a minimal Docker image (maybe)\n- [ ] https://github.com/ines/termynal\n',
     'author': 'Olaf Gladis',
     'author_email': 'olaf@gladis.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `timeturner-0.2.0/PKG-INFO` & `timeturner-0.3.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeturner
-Version: 0.2.0
+Version: 0.3.0a0
 Summary: 
 Author: Olaf Gladis
 Author-email: olaf@gladis.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -53,19 +53,28 @@
 
 If you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`
 
 ![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)
 
 ### Adding a public holiday
 
-> **Warning:**
-> This is not final yet.
+To add May 1st as a public holiday, run the following command:
+
+![`timeturner add 05-01 @holiday`](img/add_holiday.svg)
+
+### Adding your vacation
+
+To add your vacation, run the following command:
+
+![`timeturner add 04-25 - 05-14 @vacation`](img/add_vacation.svg)
+
+Adding your vacation will add a segments that are not part of holidays, it will also split
+weekends and only add working days as vacation.
+
 
-If you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after
-the activity times when adding a new event.
 
 
 ## Configuration
 
 | Environment Variable       | Default Value                    | Description                                  |
 | -------------------------- | -------------------------------- | -------------------------------------------- |
 | TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |
@@ -101,60 +110,66 @@
 If you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.
 
 
 
 TODOs:
 - [ ] Add Configuration
   - [ ] ignore seconds
-  - [ ] freeze time, to generate useful images
+  - [ ] freeze time, to generate useful and pretty images for docs
   - [ ] automatic rest periods
+  - [ ] default work time
+  - [ ] default work week days
+- [ ] allow full day activities to coexist with other activities
+  - [ ] travel time and holiday could happen
+- [ ] DB migrations
 - [ ] show and generate tui output
 - [ ] Add section about contributions
 - [ ] Add precommit hook to ensure code is formatted
 - [ ] Generate docstrings for DB methods
 - [ ] Remove import command (it contains assumptions that will not be true for everyone)
   - [ ] Document how to import data from other time trackers
   - [ ] Add mode to convert hamster output to jsonl file.
   - [ ] Add mode to import jsonl file
 - [ ] Add logging
   - [ ] allow different log levels for database and application
 - [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app
 - [ ] README
   - [ ] auto generate config options
-- [ ] db
-  - [ ] add table for tags
 
 
 TODOS by command:
 
-- [ ] add
-  - [ ] allow passive activities
-  - [ ] allow sick days
-  - [ ] allow vacation days
-  - [x] allow for public holidays
+- [x] add
+
 - [ ] end
   - [ ] add tests
 
 - [ ] configure
   - [ ] modify and write configfile
   - [ ] allow to add aliases for commands
     - [ ] e.g. new new add alias with setting passive to true
+  - [ ] add test when holiday tag name is changed in settings
+
 - [ ] list
   - [ ] split up multiday activities
+  - [ ] summaries full day tags differently
   - [x] holidays should not count as work time
     - [x] it should also not count as missing work time
-  - [ ] group by year, month, week, day
+  - [ ] group by year, month, week, daysplit up multiday activities
   - [ ] add option to show only open activities
   - [ ] add tests
+
 - [ ] import holidays
+
 - [ ] export
   - [ ] probably like list --format jsonl
 
 - [ ] undo (revert the last change)
 - [ ] confirm changes that would modify other entries
+
 ### Design Goals
 
 - minimalistic, little to type
 - enforce as little as possible
 - be clear
 - be extensible
   - TODO: support plugins (maybe a later version)
```

