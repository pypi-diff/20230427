# Comparing `tmp/pyboxen-1.1.2.tar.gz` & `tmp/pyboxen-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboxen-1.1.2.tar", max compression
+gzip compressed data, was "pyboxen-1.2.0.tar", max compression
```

## Comparing `pyboxen-1.1.2.tar` & `pyboxen-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-09-30 13:12:13.571211 pyboxen-1.1.2/LICENSE
--rw-r--r--   0        0        0      235 2023-04-01 08:13:03.356372 pyboxen-1.1.2/pyboxen/__init__.py
--rw-r--r--   0        0        0     7506 2023-04-01 08:12:29.041654 pyboxen-1.1.2/pyboxen/main.py
--rw-r--r--   0        0        0      496 2023-04-01 08:13:06.493682 pyboxen-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5478 2023-04-01 08:12:29.040655 pyboxen-1.1.2/README.md
--rw-r--r--   0        0        0     6389 2023-04-01 08:13:32.663470 pyboxen-1.1.2/setup.py
--rw-r--r--   0        0        0     6144 2023-04-01 08:13:32.665507 pyboxen-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-09-30 13:12:13.571211 pyboxen-1.2.0/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-27 13:44:36.005660 pyboxen-1.2.0/pyboxen/__init__.py
+-rw-r--r--   0        0        0     7506 2023-04-01 08:12:29.041654 pyboxen-1.2.0/pyboxen/main.py
+-rw-r--r--   0        0        0      497 2023-04-27 13:44:18.374193 pyboxen-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6105 2023-04-27 13:41:15.801246 pyboxen-1.2.0/README.md
+-rw-r--r--   0        0        0     7014 2023-04-27 13:45:28.082426 pyboxen-1.2.0/setup.py
+-rw-r--r--   0        0        0     6763 2023-04-27 13:45:28.083443 pyboxen-1.2.0/PKG-INFO
```

### Comparing `pyboxen-1.1.2/LICENSE` & `pyboxen-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboxen-1.1.2/pyboxen/main.py` & `pyboxen-1.2.0/pyboxen/main.py`

 * *Files identical despite different names*

### Comparing `pyboxen-1.1.2/README.md` & `pyboxen-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # pyboxen
 <!-- markdownlint-disable MD010 MD033 MD001 MD003 -->
 
 > **Create beautiful boxes in the terminal using Python**
 
+[![release](https://badge.fury.io/py/pyboxen.svg)](https://pypi.org/project/pyboxen)
+[![downloads](https://img.shields.io/pypi/dm/pyboxen.svg)](https://pypistats.org/packages/pyboxen)
+[![github](https://img.shields.io/github/license/savioxavier/pyboxen.svg)](https://github.com/savioxavier/pyboxen/blob/master/LICENSE)
+[![total downloads](https://static.pepy.tech/personalized-badge/pyboxen?period=total&units=none&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/pyboxen)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 This package is a Python "port" of the popular NPM package [boxen](https://github.com/sindresorhus/boxen/).
 
 It's built on top of [Rich](https://github.com/Textualize/rich/), and features an API that would be familiar to the users of the NPM boxen package.
 
 ## 🛠️ Install
 
 Using [pip](https://pypi.org/)
```

### Comparing `pyboxen-1.1.2/setup.py` & `pyboxen-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['pyboxen']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['rich>=12.5.1,<13.0.0']
+['rich>=12.5.1']
 
 setup_kwargs = {
     'name': 'pyboxen',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'Beautiful, customizable boxes in your terminal using Python',
-    'long_description': '# pyboxen\n<!-- markdownlint-disable MD010 MD033 MD001 MD003 -->\n\n> **Create beautiful boxes in the terminal using Python**\n\nThis package is a Python "port" of the popular NPM package [boxen](https://github.com/sindresorhus/boxen/).\n\nIt\'s built on top of [Rich](https://github.com/Textualize/rich/), and features an API that would be familiar to the users of the NPM boxen package.\n\n## 🛠️ Install\n\nUsing [pip](https://pypi.org/)\n\n```text\npip install pyboxen\n```\n\n---\n\n## 🔗 Usage\n\n- Simplest of simple boxes\n\n```py\nfrom pyboxen import boxen\n\nprint(boxen("Python is cool!"))\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198232802-e41575c6-abd6-416d-9ba6-d1b1c31a2660.png)\n\n- Define options\n\n```py\nfrom pyboxen import boxen\n\nprint(\n    boxen(\n        "Python is cool!",\n        padding=1,\n        margin=1,\n        color="cyan",\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198233490-52feeeba-efd3-4fe4-93cf-641d0f58fbf4.png)\n\n- Multiple texts and [Rich Renderables](https://github.com/Textualize/rich#rich-library)\n\n> You can even use Rich\'s special color style syntax for the text, title and subtitle as well\n>\n> Example: `[red]Hello[/red] [bold italic]World[/]`\n\n```py\nfrom pyboxen import boxen\n\n# Multiple texts\n\nprint(\n    boxen(\n        "Python is cool!",\n        "Yeah it totally is!",\n        "I [red]:heart:[/red]  [yellow bold]Python[/]!",  # You can even use Rich syntax here too!\n        padding=1,\n        margin=1,\n        color="cyan",\n    )\n)\n\n# Rich renderables, with a mix of strings and renderables\n\nfrom rich.table import Table\n\ntable = Table(show_header=True, header_style="bold magenta")\n\ntable.add_column("Date", style="dim", width=12)\ntable.add_column("Title")\ntable.add_column("Production Budget", justify="right")\ntable.add_column("Box Office", justify="right")\ntable.add_row(\n    "Dec 20, 2019", "Star Wars: The Rise of Skywalker", "$275,000,000", "$375,126,118"\n)\ntable.add_row(\n    "May 25, 2018",\n    "[red]Solo[/red]: A Star Wars Story",\n    "$275,000,000",\n    "$393,151,347",\n)\ntable.add_row(\n    "Dec 15, 2017",\n    "Star Wars Ep. VIII: The Last Jedi",\n    "$262,000,000",\n    "[bold]$1,332,539,889[/bold]",\n)\n\nprint(\n    boxen(\n        "Python is cool!",\n        table\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198234218-0a4ccfd8-a858-4f84-a99d-f804b926f684.png)\n\n- Title and subtitles\n\n```py\nfrom pyboxen import boxen\n\nprint(\n    boxen(\n        "Titles and subtitles!",\n        title="Hello, [black on cyan] World [/]",\n        subtitle="Cool subtitle goes here",\n        subtitle_alignment="center",\n        color="yellow",\n        padding=1,\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198237935-d01857b8-f61a-42de-b7e5-9fdff59a9739.png)\n---\n\n## 🔮 API\n\n### `boxen(*text, **kwargs)`\n\n#### text\n\nA variable (infinite) amount of text strings or [Rich Renderables](https://github.com/Textualize/rich#rich-library), or a mix of both.\n\n#### kwargs\n\nCustomize options for the box\n\nAvailable options include:\n\n```py\ncolor: str = "white",\nstyle: Literal["ascii", "ascii2", "ascii_double_head", "square", "square_double_head", "minimal", "horizontals", "rounded", "heavy", "double"] = "rounded"\npadding: Union[int, tuple[int]] = 0,\nmargin: Union[int, tuple[int]] = 0,\ntext_alignment: Literal["left", "center", "right"] = "center",\nbox_alignment: Literal["left", "center", "right"] = "left",\ntitle: str = None,\ntitle_alignment: Literal["left", "center", "right"] = "left",\nsubtitle: str = None,\nsubtitle_alignment: Literal["left", "center", "right"] = "left",\nfullwidth: bool = False,\n```\n\n#### color\n\nThe color of the box in color or hex code starting with #, defaults to white\n\n#### style\n\nThe style of the box, defaults to rounded\n\n#### padding\n\nThe padding between the text and the box in int or tuple of ints, defaults to 0\n\n#### margin\n\nThe margin around the box in int or tuple of ints, defaults to 0\n\n#### text_alignment\n\nThe alignment of the text inside the box, defaults to center\n\n#### box_alignment\n\nThe alignment of the box in the terminal, defaults to left\n\n#### title\n\nThe title of the box, displayed on the top of the box, if provided\n\n#### title_alignment\n\nThe alignment of the title, defaults to left\n\n#### subtitle\n\nThe subtitle of the box, displayed on the bottom of the box, if provided\n\n#### subtitle_alignment\n\nThe alignment of the subtitle, defaults to left\n\n#### fullwidth\n\nIf True, the box will expand to fill the entire terminal width, defaults to False\n\n> **Note**\n> `padding` and `margin` attributes can be either an int, a tuple of ints (with a total of either 2 elements or 4 elements)\n> Example:\n>\n> `2` - all of top, right, bottom, left\n>\n> `(2, 4)` - (top = bottom, right = left)\n>\n> `(2, 4, 6, 8)` - (top, right, bottom, left)\n\n---\n\n## ❤️ Support\n\nYou can support further development of this project by **giving it a 🌟** and help me make even better stuff in the future by **buying me a ☕**\n\n<a href="https://www.buymeacoffee.com/savioxavier">\n<img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" height="50px">\n</a>\n\n<br>\n\n**Also, if you liked this repo, consider checking out my other projects, that would be real cool!**\n\n---\n\n## 💫 Attributions and special thanks\n\n- [boxen](https://github.com/sindresorhus/boxen/) - the NPM package I was inspired from\n- [rich](https://github.com/Textualize/rich) - for making such an incredibly powerful text customization tool\n',
+    'long_description': '# pyboxen\n<!-- markdownlint-disable MD010 MD033 MD001 MD003 -->\n\n> **Create beautiful boxes in the terminal using Python**\n\n[![release](https://badge.fury.io/py/pyboxen.svg)](https://pypi.org/project/pyboxen)\n[![downloads](https://img.shields.io/pypi/dm/pyboxen.svg)](https://pypistats.org/packages/pyboxen)\n[![github](https://img.shields.io/github/license/savioxavier/pyboxen.svg)](https://github.com/savioxavier/pyboxen/blob/master/LICENSE)\n[![total downloads](https://static.pepy.tech/personalized-badge/pyboxen?period=total&units=none&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/pyboxen)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nThis package is a Python "port" of the popular NPM package [boxen](https://github.com/sindresorhus/boxen/).\n\nIt\'s built on top of [Rich](https://github.com/Textualize/rich/), and features an API that would be familiar to the users of the NPM boxen package.\n\n## 🛠️ Install\n\nUsing [pip](https://pypi.org/)\n\n```text\npip install pyboxen\n```\n\n---\n\n## 🔗 Usage\n\n- Simplest of simple boxes\n\n```py\nfrom pyboxen import boxen\n\nprint(boxen("Python is cool!"))\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198232802-e41575c6-abd6-416d-9ba6-d1b1c31a2660.png)\n\n- Define options\n\n```py\nfrom pyboxen import boxen\n\nprint(\n    boxen(\n        "Python is cool!",\n        padding=1,\n        margin=1,\n        color="cyan",\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198233490-52feeeba-efd3-4fe4-93cf-641d0f58fbf4.png)\n\n- Multiple texts and [Rich Renderables](https://github.com/Textualize/rich#rich-library)\n\n> You can even use Rich\'s special color style syntax for the text, title and subtitle as well\n>\n> Example: `[red]Hello[/red] [bold italic]World[/]`\n\n```py\nfrom pyboxen import boxen\n\n# Multiple texts\n\nprint(\n    boxen(\n        "Python is cool!",\n        "Yeah it totally is!",\n        "I [red]:heart:[/red]  [yellow bold]Python[/]!",  # You can even use Rich syntax here too!\n        padding=1,\n        margin=1,\n        color="cyan",\n    )\n)\n\n# Rich renderables, with a mix of strings and renderables\n\nfrom rich.table import Table\n\ntable = Table(show_header=True, header_style="bold magenta")\n\ntable.add_column("Date", style="dim", width=12)\ntable.add_column("Title")\ntable.add_column("Production Budget", justify="right")\ntable.add_column("Box Office", justify="right")\ntable.add_row(\n    "Dec 20, 2019", "Star Wars: The Rise of Skywalker", "$275,000,000", "$375,126,118"\n)\ntable.add_row(\n    "May 25, 2018",\n    "[red]Solo[/red]: A Star Wars Story",\n    "$275,000,000",\n    "$393,151,347",\n)\ntable.add_row(\n    "Dec 15, 2017",\n    "Star Wars Ep. VIII: The Last Jedi",\n    "$262,000,000",\n    "[bold]$1,332,539,889[/bold]",\n)\n\nprint(\n    boxen(\n        "Python is cool!",\n        table\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198234218-0a4ccfd8-a858-4f84-a99d-f804b926f684.png)\n\n- Title and subtitles\n\n```py\nfrom pyboxen import boxen\n\nprint(\n    boxen(\n        "Titles and subtitles!",\n        title="Hello, [black on cyan] World [/]",\n        subtitle="Cool subtitle goes here",\n        subtitle_alignment="center",\n        color="yellow",\n        padding=1,\n    )\n)\n```\n\n> ![image](https://user-images.githubusercontent.com/38729705/198237935-d01857b8-f61a-42de-b7e5-9fdff59a9739.png)\n---\n\n## 🔮 API\n\n### `boxen(*text, **kwargs)`\n\n#### text\n\nA variable (infinite) amount of text strings or [Rich Renderables](https://github.com/Textualize/rich#rich-library), or a mix of both.\n\n#### kwargs\n\nCustomize options for the box\n\nAvailable options include:\n\n```py\ncolor: str = "white",\nstyle: Literal["ascii", "ascii2", "ascii_double_head", "square", "square_double_head", "minimal", "horizontals", "rounded", "heavy", "double"] = "rounded"\npadding: Union[int, tuple[int]] = 0,\nmargin: Union[int, tuple[int]] = 0,\ntext_alignment: Literal["left", "center", "right"] = "center",\nbox_alignment: Literal["left", "center", "right"] = "left",\ntitle: str = None,\ntitle_alignment: Literal["left", "center", "right"] = "left",\nsubtitle: str = None,\nsubtitle_alignment: Literal["left", "center", "right"] = "left",\nfullwidth: bool = False,\n```\n\n#### color\n\nThe color of the box in color or hex code starting with #, defaults to white\n\n#### style\n\nThe style of the box, defaults to rounded\n\n#### padding\n\nThe padding between the text and the box in int or tuple of ints, defaults to 0\n\n#### margin\n\nThe margin around the box in int or tuple of ints, defaults to 0\n\n#### text_alignment\n\nThe alignment of the text inside the box, defaults to center\n\n#### box_alignment\n\nThe alignment of the box in the terminal, defaults to left\n\n#### title\n\nThe title of the box, displayed on the top of the box, if provided\n\n#### title_alignment\n\nThe alignment of the title, defaults to left\n\n#### subtitle\n\nThe subtitle of the box, displayed on the bottom of the box, if provided\n\n#### subtitle_alignment\n\nThe alignment of the subtitle, defaults to left\n\n#### fullwidth\n\nIf True, the box will expand to fill the entire terminal width, defaults to False\n\n> **Note**\n> `padding` and `margin` attributes can be either an int, a tuple of ints (with a total of either 2 elements or 4 elements)\n> Example:\n>\n> `2` - all of top, right, bottom, left\n>\n> `(2, 4)` - (top = bottom, right = left)\n>\n> `(2, 4, 6, 8)` - (top, right, bottom, left)\n\n---\n\n## ❤️ Support\n\nYou can support further development of this project by **giving it a 🌟** and help me make even better stuff in the future by **buying me a ☕**\n\n<a href="https://www.buymeacoffee.com/savioxavier">\n<img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" height="50px">\n</a>\n\n<br>\n\n**Also, if you liked this repo, consider checking out my other projects, that would be real cool!**\n\n---\n\n## 💫 Attributions and special thanks\n\n- [boxen](https://github.com/sindresorhus/boxen/) - the NPM package I was inspired from\n- [rich](https://github.com/Textualize/rich) - for making such an incredibly powerful text customization tool\n',
     'author': 'Skyascii',
     'author_email': 'savioxavier112@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/savioxavier/pyboxen',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyboxen-1.1.2/PKG-INFO` & `pyboxen-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: pyboxen
-Version: 1.1.2
+Version: 1.2.0
 Summary: Beautiful, customizable boxes in your terminal using Python
 Home-page: https://github.com/savioxavier/pyboxen
 License: MIT
 Author: Skyascii
 Author-email: savioxavier112@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: rich (>=12.5.1)
 Project-URL: Repository, https://github.com/savioxavier/pyboxen
 Description-Content-Type: text/markdown
 
 # pyboxen
 <!-- markdownlint-disable MD010 MD033 MD001 MD003 -->
 
 > **Create beautiful boxes in the terminal using Python**
 
+[![release](https://badge.fury.io/py/pyboxen.svg)](https://pypi.org/project/pyboxen)
+[![downloads](https://img.shields.io/pypi/dm/pyboxen.svg)](https://pypistats.org/packages/pyboxen)
+[![github](https://img.shields.io/github/license/savioxavier/pyboxen.svg)](https://github.com/savioxavier/pyboxen/blob/master/LICENSE)
+[![total downloads](https://static.pepy.tech/personalized-badge/pyboxen?period=total&units=none&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/pyboxen)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 This package is a Python "port" of the popular NPM package [boxen](https://github.com/sindresorhus/boxen/).
 
 It's built on top of [Rich](https://github.com/Textualize/rich/), and features an API that would be familiar to the users of the NPM boxen package.
 
 ## 🛠️ Install
 
 Using [pip](https://pypi.org/)
```

