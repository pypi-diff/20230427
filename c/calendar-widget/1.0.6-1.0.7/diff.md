# Comparing `tmp/calendar_widget-1.0.6.tar.gz` & `tmp/calendar_widget-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.6.tar", last modified: Tue Apr 25 22:45:42 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.7.tar", last modified: Thu Apr 27 17:16:31 2023, max compression
```

## Comparing `calendar_widget-1.0.6.tar` & `calendar_widget-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     9419 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8530 2023-04-25 22:44:21.000000 calendar_widget-1.0.6/README.md
--rw-rw-rw-   0        0        0      763 2023-04-25 22:44:34.000000 calendar_widget-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.700430 calendar_widget-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.778563 calendar_widget-1.0.6/src/calendar_widget/
--rw-rw-rw-   0        0        0   127902 2023-04-25 22:28:54.000000 calendar_widget-1.0.6/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.6/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.794188 calendar_widget-1.0.6/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     9419 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.809814 calendar_widget-1.0.6/tests/
--rw-rw-rw-   0        0        0      628 2023-04-25 22:29:34.000000 calendar_widget-1.0.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0    14037 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13144 2023-04-27 17:15:12.000000 calendar_widget-1.0.7/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-27 17:15:39.000000 calendar_widget-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.119794 calendar_widget-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.213553 calendar_widget-1.0.7/src/calendar_widget/
+-rw-rw-rw-   0        0        0   129221 2023-04-27 16:34:52.000000 calendar_widget-1.0.7/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.7/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.244803 calendar_widget-1.0.7/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0    14037 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.244803 calendar_widget-1.0.7/tests/
+-rw-rw-rw-   0        0        0      821 2023-04-27 16:36:43.000000 calendar_widget-1.0.7/tests/test.py
```

### Comparing `calendar_widget-1.0.6/LICENSE.md` & `calendar_widget-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.6/pyproject.toml` & `calendar_widget-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.6/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.7/src/calendar_widget/Calendar_Widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,53 +37,59 @@
             trail_text_fill="black",
             date_highlight="orange",
             text_highlight_fill="black",
             weekday_font_family="Algerian",
             weekday_font_weight='normal',
             weekday_font_slant='roman',
             weekday_font_underline=False,
+            weekday_font_size=None,
             date_heading_font_family="Garamond",
             date_heading_font_weight='normal',
             date_heading_font_slant='roman',
             date_heading_font_underline=False,
+            date_heading_font_size=None,
             date_text_font_family="Arial CE",
             date_text_font_weight='normal',
             date_text_font_slant='roman',
             date_text_font_underline=False,
+            date_text_font_size=None,
             user_highlight_colour="gray75",
             user_highlight_text="black",
             img_pos_x=0,
             img_pos_y=0,
-            img_anchor='nw'):
+            img_anchor='nw',
+            current_date_highlight=True):
 
         self.command = command   # create global instance of user command for use within the click binding
 
         # styling options that need to be utilized outside of the init function are given global assignment in the block below
         self.calendar_date_title = calendar_date_title       # colour of the calendar title (ex: Aug 2020)
         self.date_text_fill = date_text_fill                 # colour of the text numbers associated with the month dates
         self.date_boxes_outline = date_boxes_outline         # colour of the box outline that make up the month grid
         self.trail_box_fill = trail_box_fill                 # colour of the background of the date boxes that trail into the previous and following months
         self.trail_text_fill = trail_text_fill               # colour of the text numbers associated with the trailing date boxes
         self.date_highlight = date_highlight                 # colour of the permanent date highlight associated with the current date retrieved from the OS
         self.text_highlight_fill = text_highlight_fill       # colour of the text associated with the permanent date highlight
         self.user_highlight_colour = user_highlight_colour   # colour of the highlight that is displayed when the user clicks on a month date
         self.user_highlight_text = user_highlight_text       # colour of the text associated with the user highlight
         self.date_box_width = date_box_width                 # width of the lines that make up the date boxes
+        self.current_date_highlight = current_date_highlight # toggles the current date highlight on/off, using True/False values
+        self.date_box_fill = date_box_fill                   # colour of the background of the date boxes associated with the current month
 
         # The following condition describes the preset styling options for the "Dark" style variation. Note: if the preset
         # is not specified, the calendar defaults to the options defined within the __init__ parameters. The default styling
         # is considered to be the "Light" preset. To manually style the calendar, the default arguments within the __init__
         # function are overridden by the options specified when and instance of the calendar object is created.
         if style == "Dark":
             background = "gray7"                     # colour of the calendar background
             calendar_relief = "flat"                 # relief style options associated with the canvas on which the calendar is created
             arrow_box_border = "gray25"              # colour of the box outline that contains the arrows for selecting previous and following months
             arrow_box_fill = "gray7"                 # colour inside the box that contains the arrows
             arrow_box_width = 1                      # width of the line used to create the box that contains the arrows
-            date_box_fill = "gray7"                  # colour inside the boxes that make up the monthly calendar grid
+            self.date_box_fill = "gray7"                  # colour inside the boxes that make up the monthly calendar grid
             date_box_width = 2                       # width of the line used to create the grid for the monthly calendar
             self.date_boxes_outline = "gray50"       # colour of the box outline for the boxes that make up the monthly claendar grid
             arrow_outline = "gray25"                 # colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows
             arrow_fill = "black"                     # colour of the calendar arrows
             arrow_thickness = 1                      # thickness of the calendar arrows
             arrow_active = "lime"                    # colour for the activefill associated with the calendar arrows
             weekday_border = "gray25"                # colour for the outline of the boxes that hold the weekday headings
@@ -189,15 +195,18 @@
                                            weekday_bot_y,
                                            outline=weekday_border,
                                            fill=weekday_fill,
                                            width=weekday_width,
                                            tags=weekdays[heading_inc])
             heading_inc = heading_inc + 1
 
-        font_size = int((box_depth * 0.75) * 0.75)
+        if weekday_font_size != None:
+            font_size = weekday_font_size
+        else:
+            font_size = int((box_depth * 0.75) * 0.75)
         weekday_font = font.Font(family=weekday_font_family, size=font_size, 
             weight=weekday_font_weight, slant=weekday_font_slant, underline=weekday_font_underline)
         for day in weekdays:
             weekday_coords = self.Calendar.coords(day)
             letter_x = (weekday_coords[0] + weekday_coords[2]) / 2
             letter_y = (weekday_coords[1] + weekday_coords[3]) / 2
             letter = day[0]
@@ -223,15 +232,18 @@
         # Initialize global date holder for selected days
         self.day_num = None
 
         # create calendar date heading (ex: Aug 2022)
         arrow_box_coords = self.Calendar.coords("arrow_box")
         self.arrow_date_x = (arrow_box_coords[0] + arrow_box_coords[2]) / 2
         self.arrow_date_y = (arrow_box_coords[1] + arrow_box_coords[3]) / 2
-        font_size = int((self.arrow_date_y * 0.75) * 0.5)
+        if date_heading_font_size != None:
+            font_size = date_heading_font_size
+        else:
+            font_size = int((self.arrow_date_y * 0.75) * 0.5)
         self.date_heading_font = font.Font(family=date_heading_font_family, size=font_size, 
             weight=date_heading_font_weight, slant=date_heading_font_slant, underline=date_heading_font_underline)
         self.Calendar.create_text(self.arrow_date_x, self.arrow_date_y, text=self.date_today, anchor="center",
                                   font=self.date_heading_font,
                                   fill=self.calendar_date_title, tags="arrow_box_date")
 
         # create date boxes for days of the month
@@ -239,26 +251,29 @@
         # boxes are globally stored and are used to define the position of the text on the grid.
         box_width = ((size - (padding * 2)) * 0.144)
         box_depth = ((depth - padding) - (padding + (depth * 0.25))) * 0.1428
         box_y_start = (padding + (depth * 0.25)) + box_depth
         width_inc = 0
         depth_inc = 0
         box_count = 0
-        self.date_box_font_size = int(((box_depth) * 0.75) * 0.6)
+        if date_text_font_size != None:
+            self.date_box_font_size = date_text_font_size
+        else:
+            self.date_box_font_size = int(((box_depth) * 0.75) * 0.6)
         self.date_text_font = font.Font(family=date_text_font_family, size=self.date_box_font_size, 
             weight=date_text_font_weight, slant=date_text_font_slant, underline=date_text_font_underline)
         self.date_box_tags = []
         while box_count != 42:
             box_tag = "date_box_" + str(box_count)
             self.Calendar.create_rectangle((padding + (box_width * width_inc)),
                                            (box_y_start + (box_depth * depth_inc)),
                                            (padding + (box_width * (width_inc + 1))),
                                            (box_y_start + (box_depth * (depth_inc + 1))),
                                            outline=self.date_boxes_outline, tags=box_tag,
-                                           fill=date_box_fill, width=date_box_width)
+                                           fill=None, width=date_box_width)
             self.date_box_tags.append(box_tag)
             width_inc = width_inc + 1
             box_count = box_count + 1
             if (box_count / 7).is_integer():
                 width_inc = 0
                 depth_inc = depth_inc + 1
 
@@ -364,34 +379,42 @@
                                   font=self.date_heading_font, fill=self.calendar_date_title, tags="arrow_box_date")
 
 
         # create date text on the calendar
         if len(self.date_tags[0]) > 0:
             for date in self.date_tags[0]:
                 self.Calendar.delete(date)
+            for coll in self.date_colour:
+                self.Calendar.delete(coll)
             if (self.date_store[0] != self.year) or (self.date_store[1] != self.month):
                 self.Calendar.delete("date_highlight")
                 self.Calendar.delete("date_highlight_text")
         day_count = 1
         self.date_tags = [[], []]
+        self.date_colour = []
         monthrange = calendar.monthrange(self.year, self.month)
         month_length = monthrange[1]
         start_box = (calendar.weekday(self.year, self.month, 1)) + 1
         self.prev_box = start_box - 1
         self.foll_box = start_box + int(month_length)
         while month_length != 0:
             date_tag = "day_" + str(day_count)
+            date_colour_tag = "day_colour" + str(day_count)
             date_box_coords = self.Calendar.coords(self.date_box_tags[start_box])
             x_coords = (date_box_coords[0] + date_box_coords[2]) / 2
             y_coords = (date_box_coords[1] + date_box_coords[3]) / 2
+            self.Calendar.create_rectangle(date_box_coords[0], date_box_coords[1],
+                date_box_coords[2], date_box_coords[3], fill=self.date_box_fill, 
+                outline=self.date_boxes_outline, width=self.date_box_width, tags=date_colour_tag)
             self.Calendar.create_text(x_coords, y_coords, text=str(day_count), anchor="center",
                                       font=self.date_text_font, fill=self.date_text_fill, activefill=self.date_highlight,
                                       tags=date_tag)
             self.date_tags[0].append(date_tag)
             self.date_tags[1].append(date_box_coords)
+            self.date_colour.append(date_colour_tag)
             day_count = day_count + 1
             start_box = start_box + 1
             month_length = month_length - 1
 
         # create trailing month dates
         def trail_boxes(previous=False, following=False):
             if previous:
@@ -458,25 +481,26 @@
                 self.Calendar.delete(trail_text)
             self.foll_tags = [[], []]
 
         trail_boxes(previous=True)
         trail_boxes(following=True)
 
         # create date highlight
-        if (self.date_store[0] == self.year) and (self.date_store[1] == self.month):
-            highlight_coords = self.Calendar.coords("day_" + str(self.date_store[2]))
-            hx_1 = highlight_coords[0] - self.date_box_font_size
-            hy_1 = highlight_coords[1] - self.date_box_font_size
-            hx_2 = highlight_coords[0] + self.date_box_font_size
-            hy_2 = highlight_coords[1] + self.date_box_font_size
-            self.Calendar.create_oval(hx_1, hy_1, hx_2, hy_2, fill=self.date_highlight, outline=self.date_highlight,
-                                      tags="date_highlight")
-            self.Calendar.create_text(highlight_coords[0], highlight_coords[1], text=str(self.date_store[2]),
-                                      anchor="center", font=self.date_text_font, fill=self.text_highlight_fill,
-                                      tags="date_highlight_text")
+        if self.current_date_highlight:
+            if (self.date_store[0] == self.year) and (self.date_store[1] == self.month):
+                highlight_coords = self.Calendar.coords("day_" + str(self.date_store[2]))
+                hx_1 = highlight_coords[0] - self.date_box_font_size
+                hy_1 = highlight_coords[1] - self.date_box_font_size
+                hx_2 = highlight_coords[0] + self.date_box_font_size
+                hy_2 = highlight_coords[1] + self.date_box_font_size
+                self.Calendar.create_oval(hx_1, hy_1, hx_2, hy_2, fill=self.date_highlight, outline=self.date_highlight,
+                                          tags="date_highlight")
+                self.Calendar.create_text(highlight_coords[0], highlight_coords[1], text=str(self.date_store[2]),
+                                          anchor="center", font=self.date_text_font, fill=self.text_highlight_fill,
+                                          tags="date_highlight_text")
 
         # delete checkboxes if they exist
         if len(self.checkbox_tags) != 0:
             for cbox in self.checkbox_tags:
                 self.Calendar.delete(cbox)
 
         # create checkboxes
```

