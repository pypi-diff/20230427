# Comparing `tmp/mell-2.0.2.tar.gz` & `tmp/mell-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.2.tar", last modified: Mon Apr 24 00:31:38 2023, max compression
+gzip compressed data, was "mell-2.0.3.tar", last modified: Wed Apr 26 22:11:15 2023, max compression
```

## Comparing `mell-2.0.2.tar` & `mell-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.185941 mell-2.0.2/
--rw-rw-r--   0 diego     (1000) diego     (1000)    14237 2023-04-24 00:31:38.185941 mell-2.0.2/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)    13785 2023-04-24 00:03:39.000000 mell-2.0.2/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.181941 mell-2.0.2/mell/
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-22 21:31:52.000000 mell-2.0.2/mell/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      238 2023-04-24 00:31:32.000000 mell-2.0.2/mell/consts.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    21618 2023-04-24 00:30:51.000000 mell-2.0.2/mell/main.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-24 00:31:38.181941 mell-2.0.2/mell.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)    14237 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      233 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-24 00:31:38.000000 mell-2.0.2/mell.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-24 00:31:38.185941 mell-2.0.2/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-23 13:44:11.000000 mell-2.0.2/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.371753 mell-2.0.3/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-26 22:11:15.371753 mell-2.0.3/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15314 2023-04-26 21:22:17.000000 mell-2.0.3/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.367753 mell-2.0.3/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.3/mell/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-04-26 15:39:46.000000 mell-2.0.3/mell/consts.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    25505 2023-04-26 22:09:09.000000 mell-2.0.3/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.367753 mell-2.0.3/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      233 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-26 22:11:15.371753 mell-2.0.3/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.3/setup.py
```

### Comparing `mell-2.0.2/PKG-INFO` & `mell-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.2
-Summary: A Metaprogramming Logic Layer designed to generate anything from template files
-Home-page: https://github.com/diegofps/pywup
+Version: 2.0.3
+Summary: Generate anything from template files and metadata files!
+Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: full
 
 # Mell
 
 Mell is a Metaprogramming Logic Layer designed to generate anything from template files. 
 
 # Why do I need this?
 
-There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that you may want to use mell. So far, I have used it in the following situations:
+Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
@@ -34,48 +34,56 @@
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
 # Concepts
 
 To use this library you must understand a few concepts. These are:
 
-* `metadata:` These is data describing what we want to generate. We use json format for it.
-* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, plugins, and logic rules.
-* `generated folder:` This is where the rendered files will be saved and you must never change these files. However, you may want to execute or compile them if you are generating a webserver or a latex template, for instance. 
+* `metadata:` The data describing what we want to generate. It is written using the json format.
+* `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
+* `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
-A style is composed of the following concepts:
+A style is composed of the following items:
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
-* `plugin:` Scripts that will be executed by mell. These usually access the files in the asset folder.
-* `logic:` Scripts that will be executed in order by mell. These are used to validate and extend the metadata.
+* `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
+* `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
 # Basic folder structure
 
 The following table describes the folders used by mell.
 
 | Folder  | Description | 
 |-------------|-------------|
-| \<root\> | The base folder that contains all folders described here |
+| \<root\> | Base folder containing the folders meta, style, and the generated folder |
 | \<root\>/style | The base folder for template, static, plugin, and asset |
 | \<root\>/generate | this will hold the generated data, never edit this folder |
 | \<root\>/meta | holds all metadata as json files |
-| \<root\>/style/template | holds the template files that will be automatically rendered and written to the generated folder |
-| \<root\>/style/static | contains static files that will be copied as they are to the generate folder |
-| \<root\>/style/plugin | contains scripts that will be executed by mell. Use these to render multiple files from templates in the asset folder |
-| \<root\>/style/asset | contains template and other files that are not automatically used by mell. They may be used by plugins or other tools |
-| \<root\>/style/logic | contains scripts used automatically executed by mell to transform the metadata |
+| \<root\>/style/template | template files that will be automatically rendered and written to the generated folder |
+| \<root\>/style/static | static files that will be copied as they are to the output folder |
+| \<root\>/style/plugin | scripts that will be automatically executed by mell to render multiple output files |
+| \<root\>/style/asset | extra files that are not automatically used by mell. They may be used inside plugin and logic scripts |
+| \<root\>/style/logic | scripts automatically executed by mell to transform or extend the metadata |
 
-If you want to create a new project using this structure with the root folder named testing_mell, you can use the following command.
+To create a new project using the structure above, use the following command.
 
 ```shell
-mell --new testing_mell
+mell --new <name_of_root_folder>
 ```
 
+# Context variables
+
+These are important variables available troughout mell. They help to interact with templates, metadata, and command arguments.
+
+* `meta: ` an object of type Meta that encapsulates the metadata allowing easy navigation through its fields. Use `.` to access attributes and `[]` to access array elements. Navigation always returns an object with its same type, a Meta object. To access the object it references you must use the attribute `value`. You can also iterate over this object, if it references a json object the iteration will return a tuple of type `(str, Meta)`. If you iterate over an array it will always return a `Meta` object.
+* `inflater: ` an object used to inflate templates in the asset folder. Use the method `inflate` to inflate a template. You may call this method from a template inside the template folder or from a template in the asset folder to render a partial template in the template being generated. You may also call it from a plugin script, in this case it makes sense to use the optional parameter `to_file`. This will save the rendered template to the corresponding file in the output folder.
+* `args: ` an object holding all the program parameters. `Program parameters` are attributes that control the program executing, like the folders it reads and writes data to, and so on. You should never change any of these values during the program execution.
+
 # How to install / uninstall it?
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
@@ -83,15 +91,15 @@
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your $PATH variable includes the local bin directory that pip uses; (2) install it in a virtual environment, like virtualenv; or (3) try to install it at the system level, running pip as root;
 
-# Generating Hello Worlds
+# Generating Programs
 
 This will demonstrate how to use mell in a simple use case, changing the language for a static interface. You may be thinking now, "what a naive example, most web frameworks have much more powerful internationalization tools and I would never use it for that". Indeed, me neither. I used this in my resumes in latex, though. By doing this I had a different metadata for each place I would apply, some in portuguese, some in english, some specific for each position. Another benefit is that I could update the resume by changing only a single file. I could generate old ones again, they had their own metadata, and so on.
 
 ## Step 1. Create a new mell project
 
 Execute the following command to create the standard structure.
 
@@ -244,51 +252,51 @@
         ├── asset
         ├── plugin
         ├── static
         └── template
             └── main.py
 ```
 
-# The Pipeline
+# Understanding the Pipeline
 
-Sometimes it is important to understand the order in which the operations are executed. The list below describe these operations in their standard order.
+It is important that you understand the order that operations are executed, as these may impact the availability of data throughout the execution. The list below shows the standard order.
 
 1. Load metadata
-1. Execute logic scripts
-1. Actions to generate the output:
+1. Run logic scripts
+1. Execute actions to generate the output:
 >4. Clean output folder [clean]
 >1. Copy static files [static]
 >1. Render templates and copy them to output [template]
->1. Execute plugin scripts [plugin]
+>1. Run plugin scripts [plugin]
 
-Loading the metadata and executing the logic scripts is always executed first and can't be changed. The list of actions to generate the output, though, can be modified or canceled. To modify the list of actions we use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
+Loading the metadata and running the logic scripts is always executed first. You can't modify this behaviour. The list of actions to generate the output, though, can be modified or supressed. To modify it we must use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
 
 ```shell
 # These two calls are the same
 mell --do clean --do static --do template --do plugin data
 mell data
 
 # This will only generate output files based on the template folder
 mell --do template data
 
 # This will only clean the generated folder
-mell --do clean data
+mell --do clean
 
 # The word 'nothing' is a special keyword. It will not do any action but will still load the metadata and execute logic scripts. This is useful when used with -v (verose mode) or --show-metadata (display the metadata after executing the logic scripts).
 mell --do nothing data
 mell --do nothing -v data
 mell --do nothing --show-metadata data
 ```
 
 # Tutorials
 
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
-* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend extend the input metadata, generating more metadata and preventing complex rules in template files.
+* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend the input metadata, generating more metadata and preventing complex rules in template files.
 
 # List of useful command options
 
 These are a few examples of common operations.
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
@@ -302,14 +310,19 @@
 
 # Create a new logic file as <root>/style/logic/<timestamp>.logic_name.py
 mell --new-logic logic_name
 
 # Display the version number and exit
 mell --version
 
+# Use --set to customize the metadata from command line - useful when an external scripts needs to change something
+mell --set message 'Hello World!' en
+mell --set company.name 'Wespa' en
+mell --set users[2].name 'Diego Souza' en
+
 # Display more info during execution (verbose mode)
 mell -v en
 
 # Display less info during execution (quiet mode)
 mell -q en
 
 # Specify what we want to generate
@@ -332,9 +345,9 @@
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
 # Source Code
 
-The source code is available [here](https://github.com/diegofps/mell)
+The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.2/README.md` & `mell-2.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Mell
 
 Mell is a Metaprogramming Logic Layer designed to generate anything from template files. 
 
 # Why do I need this?
 
-There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that you may want to use mell. So far, I have used it in the following situations:
+Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
@@ -21,48 +21,56 @@
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
 # Concepts
 
 To use this library you must understand a few concepts. These are:
 
-* `metadata:` These is data describing what we want to generate. We use json format for it.
-* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, plugins, and logic rules.
-* `generated folder:` This is where the rendered files will be saved and you must never change these files. However, you may want to execute or compile them if you are generating a webserver or a latex template, for instance. 
+* `metadata:` The data describing what we want to generate. It is written using the json format.
+* `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
+* `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
-A style is composed of the following concepts:
+A style is composed of the following items:
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
-* `plugin:` Scripts that will be executed by mell. These usually access the files in the asset folder.
-* `logic:` Scripts that will be executed in order by mell. These are used to validate and extend the metadata.
+* `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
+* `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
 # Basic folder structure
 
 The following table describes the folders used by mell.
 
 | Folder  | Description | 
 |-------------|-------------|
-| \<root\> | The base folder that contains all folders described here |
+| \<root\> | Base folder containing the folders meta, style, and the generated folder |
 | \<root\>/style | The base folder for template, static, plugin, and asset |
 | \<root\>/generate | this will hold the generated data, never edit this folder |
 | \<root\>/meta | holds all metadata as json files |
-| \<root\>/style/template | holds the template files that will be automatically rendered and written to the generated folder |
-| \<root\>/style/static | contains static files that will be copied as they are to the generate folder |
-| \<root\>/style/plugin | contains scripts that will be executed by mell. Use these to render multiple files from templates in the asset folder |
-| \<root\>/style/asset | contains template and other files that are not automatically used by mell. They may be used by plugins or other tools |
-| \<root\>/style/logic | contains scripts used automatically executed by mell to transform the metadata |
+| \<root\>/style/template | template files that will be automatically rendered and written to the generated folder |
+| \<root\>/style/static | static files that will be copied as they are to the output folder |
+| \<root\>/style/plugin | scripts that will be automatically executed by mell to render multiple output files |
+| \<root\>/style/asset | extra files that are not automatically used by mell. They may be used inside plugin and logic scripts |
+| \<root\>/style/logic | scripts automatically executed by mell to transform or extend the metadata |
 
-If you want to create a new project using this structure with the root folder named testing_mell, you can use the following command.
+To create a new project using the structure above, use the following command.
 
 ```shell
-mell --new testing_mell
+mell --new <name_of_root_folder>
 ```
 
+# Context variables
+
+These are important variables available troughout mell. They help to interact with templates, metadata, and command arguments.
+
+* `meta: ` an object of type Meta that encapsulates the metadata allowing easy navigation through its fields. Use `.` to access attributes and `[]` to access array elements. Navigation always returns an object with its same type, a Meta object. To access the object it references you must use the attribute `value`. You can also iterate over this object, if it references a json object the iteration will return a tuple of type `(str, Meta)`. If you iterate over an array it will always return a `Meta` object.
+* `inflater: ` an object used to inflate templates in the asset folder. Use the method `inflate` to inflate a template. You may call this method from a template inside the template folder or from a template in the asset folder to render a partial template in the template being generated. You may also call it from a plugin script, in this case it makes sense to use the optional parameter `to_file`. This will save the rendered template to the corresponding file in the output folder.
+* `args: ` an object holding all the program parameters. `Program parameters` are attributes that control the program executing, like the folders it reads and writes data to, and so on. You should never change any of these values during the program execution.
+
 # How to install / uninstall it?
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
@@ -70,15 +78,15 @@
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your $PATH variable includes the local bin directory that pip uses; (2) install it in a virtual environment, like virtualenv; or (3) try to install it at the system level, running pip as root;
 
-# Generating Hello Worlds
+# Generating Programs
 
 This will demonstrate how to use mell in a simple use case, changing the language for a static interface. You may be thinking now, "what a naive example, most web frameworks have much more powerful internationalization tools and I would never use it for that". Indeed, me neither. I used this in my resumes in latex, though. By doing this I had a different metadata for each place I would apply, some in portuguese, some in english, some specific for each position. Another benefit is that I could update the resume by changing only a single file. I could generate old ones again, they had their own metadata, and so on.
 
 ## Step 1. Create a new mell project
 
 Execute the following command to create the standard structure.
 
@@ -231,51 +239,51 @@
         ├── asset
         ├── plugin
         ├── static
         └── template
             └── main.py
 ```
 
-# The Pipeline
+# Understanding the Pipeline
 
-Sometimes it is important to understand the order in which the operations are executed. The list below describe these operations in their standard order.
+It is important that you understand the order that operations are executed, as these may impact the availability of data throughout the execution. The list below shows the standard order.
 
 1. Load metadata
-1. Execute logic scripts
-1. Actions to generate the output:
+1. Run logic scripts
+1. Execute actions to generate the output:
 >4. Clean output folder [clean]
 >1. Copy static files [static]
 >1. Render templates and copy them to output [template]
->1. Execute plugin scripts [plugin]
+>1. Run plugin scripts [plugin]
 
-Loading the metadata and executing the logic scripts is always executed first and can't be changed. The list of actions to generate the output, though, can be modified or canceled. To modify the list of actions we use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
+Loading the metadata and running the logic scripts is always executed first. You can't modify this behaviour. The list of actions to generate the output, though, can be modified or supressed. To modify it we must use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
 
 ```shell
 # These two calls are the same
 mell --do clean --do static --do template --do plugin data
 mell data
 
 # This will only generate output files based on the template folder
 mell --do template data
 
 # This will only clean the generated folder
-mell --do clean data
+mell --do clean
 
 # The word 'nothing' is a special keyword. It will not do any action but will still load the metadata and execute logic scripts. This is useful when used with -v (verose mode) or --show-metadata (display the metadata after executing the logic scripts).
 mell --do nothing data
 mell --do nothing -v data
 mell --do nothing --show-metadata data
 ```
 
 # Tutorials
 
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
-* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend extend the input metadata, generating more metadata and preventing complex rules in template files.
+* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend the input metadata, generating more metadata and preventing complex rules in template files.
 
 # List of useful command options
 
 These are a few examples of common operations.
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
@@ -289,14 +297,19 @@
 
 # Create a new logic file as <root>/style/logic/<timestamp>.logic_name.py
 mell --new-logic logic_name
 
 # Display the version number and exit
 mell --version
 
+# Use --set to customize the metadata from command line - useful when an external scripts needs to change something
+mell --set message 'Hello World!' en
+mell --set company.name 'Wespa' en
+mell --set users[2].name 'Diego Souza' en
+
 # Display more info during execution (verbose mode)
 mell -v en
 
 # Display less info during execution (quiet mode)
 mell -q en
 
 # Specify what we want to generate
@@ -319,9 +332,9 @@
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
 # Source Code
 
-The source code is available [here](https://github.com/diegofps/mell)
+The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.2/mell/main.py` & `mell-2.0.3/mell/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import shutil
 import json
 import glob
 import time
 import sys
 import os
-
+import re
 
 LOG_LEVEL = 2
 
 def debug(*args):
     if LOG_LEVEL <= 0:
         print("DEBUG:", *args)
 
@@ -73,15 +73,15 @@
         error("Can't create the plugin. A plugin with this name already exists at", filepath)
     
     info(f"  {filepath}")
     dirname = os.path.dirname(filepath)
     os.makedirs(dirname, exist_ok=True)
 
     with open(filepath, 'w') as fout:
-        fout.write("def plugin(meta, inflator):\n    pass\n\n")
+        fout.write("def plugin(args, meta, inflator):\n    pass\n\n")
     
     sys.exit(0)
 
 def run_new_logic(args):
 
     info("Creating a new logic script")
     
@@ -92,44 +92,51 @@
         error("Can't create the plugin. A plugin with this name already exists at", filepath)
     
     info(f"  {filepath}")
     dirname = os.path.dirname(filepath)
     os.makedirs(dirname, exist_ok=True)
 
     with open(filepath, 'w') as fout:
-        fout.write("def logic(meta):\n    pass\n\n")
+        fout.write("def logic(args, meta):\n    pass\n\n")
     
     sys.exit(0)
 
 def parse_args():
 
     parser = argparse.ArgumentParser(
                         prog='mell',
                         description='Metaprogramming layer designed to generates anything from template files.',
                         epilog="Check the README.md to learn more tips on how to use this application: https://github.com/diegofps/mell/blob/main/README.md",
                         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     parser.add_argument('metadata',
                         type=str,
                         metavar='METADATA',
-                        nargs='?',
+                        nargs='*',
                         help="name of file(s) located inside the meta folder. If multiple names are provided, separated by comma, a merge will be performed.")
 
     parser.add_argument('-v', '--verbose',
                         default=None,
                         dest='verbose',
                         help="allow debug log messages to be displayed",
                         action='store_true')
 
     parser.add_argument('-q', '--quiet',
                         default=None,
                         dest='quiet',
                         help="display only warning messages and above",
                         action='store_true')
 
+    parser.add_argument('--set',
+                        default=[],
+                        nargs=2,
+                        dest='set',
+                        help="customize the value of individual properties in the metadata",
+                        action='append')
+
     parser.add_argument('--do',
                         type=str,
                         metavar='NAME',
                         default=None,
                         choices=['nothing', 'clean', 'static', 'template', 'plugin'],
                         dest='do',
                         help="define one or more action to be executed [nothing, clean, static, template, plugin]",
@@ -361,29 +368,33 @@
     if args.metadata is None:
         parser.print_help()
         sys.exit(0)
     
     return args
 
 
-def load_metadata(args, meta_filenames):
+def load_metadata(args, meta_parameters):
 
     meta = {}
 
-    for filename in meta_filenames.split(','):
-        filepath = os.path.join(args.meta, filename) + ".json"
-        
-        with open(filepath, "r") as fin:
-            meta_parent = json.loads(fin.read())
-            
-            if "__parent__" in meta_parent:
-                meta_parent_2 = load_metadata(args, meta_parent["__parent__"])
-                meta_parent = update_dict_recursively(meta_parent_2, meta_parent)
+    for metadata_names in meta_parameters:
+        for metadata_name in metadata_names.split(','):
+            if not metadata_name:
+                continue
+
+            filepath = os.path.join(args.meta, metadata_name) + ".json"
             
-            meta = update_dict_recursively(meta, meta_parent)
+            with open(filepath, "r") as fin:
+                meta_parent = json.loads(fin.read())
+                
+                if "__parent__" in meta_parent:
+                    meta_parent_2 = load_metadata(args, meta_parent["__parent__"].split())
+                    meta_parent = update_dict_recursively(meta_parent_2, meta_parent)
+                
+                meta = update_dict_recursively(meta, meta_parent)
     
     return meta
 
 def update_dict_recursively(dst, src):
 
     if isinstance(dst, dict):
         for key, value in src.items():
@@ -524,89 +535,82 @@
 
             loader=FileSystemLoader(folderpath),
             autoescape=select_autoescape(),
             trim_blocks=True, 
             lstrip_blocks=True
         )
     
-    def inflateTemplate(self, relpath, meta, to_file=None):
+    def inflate(self, relpath, meta, to_file=None, from_asset=True):
         
-        if self.template_env is None:
-            raise IOError("Missing template folder")
+        if from_asset:
+            if self.asset_env is None:
+                raise IOError("Missing asset folder")
+            template = self.asset_env.get_template(relpath)
         
-        template = self.template_env.get_template(relpath)
-        text = template.render(meta=meta, inflater=self)
-
-        if to_file is not None:
-            self._save_as_generated_file(text, to_file)
-        
-        return text
-    
-    def inflateAsset(self, relpath, meta, to_file=None):
-        
-        if self.asset_env is None:
-            raise IOError("Missing asset folder")
+        else:
+            if self.template_env is None:
+                raise IOError("Missing template folder")
+            template = self.template_env.get_template(relpath)
         
-        template = self.asset_env.get_template(relpath)
-        text = template.render(meta=meta, inflater=self)
+        text = template.render(args=self.args, meta=meta, inflater=self)
 
         if to_file is not None:
-            self._save_as_generated_file(text, to_file)
-        
-        return text
-    
-    def _save_as_generated_file(self, text, relpath):
 
-        filepath_out = os.path.join(self.args.generate, relpath)
-        folderpath_out = os.path.dirname(filepath_out)
-        
-        os.makedirs(folderpath_out, exist_ok=True)
-        
-        with open(filepath_out, "w") as fout:
-            fout.write(text)
+            filepath_out = os.path.join(self.args.generate, to_file)
+            folderpath_out = os.path.dirname(filepath_out)
+            
+            os.makedirs(folderpath_out, exist_ok=True)
+            
+            with open(filepath_out, "w") as fout:
+                fout.write(text)
+
+        return text
         
 def do_nothing(args, inflater, meta):
     pass
 
 def do_clean(args, inflater, meta):
 
     info("Cleaning generate directory")
 
     if os.path.exists(args.generate):
         if os.path.isdir(args.generate):
-            shutil.rmtree(args.generate)
+            for filepath in glob.glob(os.path.join(args.generate, '*')):
+                debug("  Removing:", filepath)
+                if os.path.isdir(filepath):
+                    shutil.rmtree(filepath)
+                else:
+                    os.remove(filepath)
         else:
             os.remove(args.generate)
     
-    os.makedirs(args.generate, exist_ok=True)
-
 def do_static(args, inflater, meta):
 
     info("Copying static data")
 
     for filepath in glob.glob(os.path.join(args.static, '**'), recursive=True):
         if os.path.isfile(filepath):
             relpath = os.path.relpath(filepath, args.static)
             filepath_out = os.path.join(args.generate, relpath)
             debug(f"{filepath} -> {filepath_out}")
 
             folderpath_out = os.path.dirname(filepath_out)
             os.makedirs(folderpath_out, exist_ok=True)
             shutil.copy2(filepath, filepath_out)
 
-def do_template(args, inflater, meta):
+def do_template(args, inflater:Inflater, meta:Meta):
 
     info("Generating template based files")
 
     for filepath in glob.glob(os.path.join(args.template, "**"), recursive=True):
         if os.path.isfile(filepath):
             relpath = os.path.relpath(filepath, args.template)
             debug("  ", relpath)
 
-            inflater.inflateTemplate(relpath, meta, to_file=relpath)
+            inflater.inflate(relpath, meta, to_file=relpath, from_asset=False)
 
 
 def do_plugin(args, inflater, meta):
     
     info("Executing plugin files")
 
     rootpath = os.path.dirname(args.plugin)
@@ -615,15 +619,15 @@
         if os.path.isfile(filepath):
             plugin_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
             debug("  ", filepath)
             
             plugin_spec = importlib.util.spec_from_file_location(plugin_name, filepath)
             plugin = importlib.util.module_from_spec(plugin_spec)
             plugin_spec.loader.exec_module(plugin)
-            plugin.plugin(meta, inflater)
+            plugin.plugin(args, meta, inflater)
 
 def get_logic_files(args):
 
     filepaths = []
 
     for filepath in glob.glob(os.path.join(args.logic, '**', '*.py'), recursive=True):
         if os.path.isfile(filepath):
@@ -635,59 +639,146 @@
                     filepaths.append((timestamp, filepath))
                 except ValueError:
                     pass
     
     filepaths.sort()
     return filepaths
 
-def apply_logic_scripts(args, meta):
+def do_logic_scripts(args, meta):
     
     info("Executing logic files")
     
     rootpath = os.path.dirname(args.logic)
     filepaths = get_logic_files(args)
     
     for _, filepath in filepaths:
         logic_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
         debug("  ", filepath)
         
         plugin_spec = importlib.util.spec_from_file_location(logic_name, filepath)
         plugin = importlib.util.module_from_spec(plugin_spec)
         plugin_spec.loader.exec_module(plugin)
-        plugin.logic(meta)
+        plugin.logic(args, meta)
 
-def main(*params):
+def do_set_values(args, meta):
+
+    info("Applying set")
     
-    args = parse_args()
+    r = re.compile('\[(\d+)\]')
 
-    info("Loading the metadata")
-    if os.path.exists(args.meta):
-        meta = Meta(load_metadata(args, args.metadata))
+    for address, value in args.set:
+        property_names = address.split('.')
+        property_names = [re.split(r, x) for x in property_names]
+        property_names = [x if i % 2 == 0 else int(x) for y in property_names for i,x in enumerate(y) if x]
+
+        current = meta.value
+
+        try:
+            for i, idx in enumerate(property_names[:-1]):
+                if isinstance(idx, str):
+                    if isinstance(current, dict):
+                        if not idx in current:
+                            next_idx = property_names[i+1]
+                            current[idx] = [] if isinstance(next_idx, int) else {}
+                    elif isinstance(current, list):
+                        raise ValueError(f"expected an address, got the property name `.{idx}'")
+                    else:
+                        raise ValueError(f"expected nothing, got the property name `.{idx}'")
+                else:
+                    if isinstance(current, list):
+                        if idx >= len(current):
+                            next_idx = property_names[i+1]
+                            if isinstance(next_idx, int):
+                                current += [[] for _ in range(idx + 1 - len(current))]
+                                current[idx] = []
+                            else:
+                                current += [{} for _ in range(idx + 1 - len(current))]
+                                current[idx] = {}
+                    elif isinstance(current, dict):
+                        raise ValueError(f"expected a property name, got the address [{idx}]")
+                    else:
+                        raise ValueError(f"expected nothing, got the address [{idx}]")
+                    
+                current = current[idx]
+            
+            idx = property_names[-1]
+
+            if isinstance(idx, str):
+                if isinstance(current, dict):
+                    current[idx] = value
+                elif isinstance(current, list):
+                    raise ValueError(f"expected an address, got the property name `.{idx}'")
+                else:
+                    raise ValueError(f"expected nothing, got the property name `.{idx}'")
+            else:
+                if isinstance(current, list):
+                    if idx >= len(current):
+                        current += [None for _ in range(idx + 1 - len(current))]
+                    current[idx] = value
+                elif isinstance(current, dict):
+                    raise ValueError(f"expected a property name, got the address [{idx}]")
+                else:
+                    raise ValueError(f"expected nothing, got the address [{idx}]")
+            
+        except ValueError as e:
+            msg = str(e)
+            if msg:
+                warn(f"Invalid property '{address}' - {msg}")
+            else:
+                warn(f"Invalid property '{address}'")
+        except IndexError:
+            warn(f"Invalid property '{address}', index {idx} is out of range")
+
+def do_show_metadata(args, meta):
 
-    else:
-        warn(f"Folder meta does not exists - {args.meta}")
-        meta = Meta({})
-    
-    apply_logic_scripts(args, meta)
-    
     if args.show_metadata:
-        print("METADATA:")
+        print("Metadata:")
         print(json.dumps(meta.value, indent=2))
-    
+
+def do_show_parameters(args):
+
     if args.show_parameters:
         print("Parameters:")
         print(json.dumps(args.__dict__, indent=2))
 
+def do_action(name, args, inflater, meta):
+
+    globals()['do_' + name](args, inflater, meta)
+
+def do_load_meta(args):
+    if os.path.exists(args.meta):
+        return Meta(load_metadata(args, args.metadata))
+
+    if args.metadata:
+        error(f"Folder meta does not exist - {args.meta}")
+    
+    return Meta({})
+    
+def do_load_inflater(args):
+    return Inflater(args)
+
+def main(*params):
+    
+    args = parse_args()
+
+    info("Loading the metadata")
+    meta = do_load_meta(args)
+    
+    do_set_values(args, meta)
+    do_logic_scripts(args, meta)
+
+    do_show_metadata(args, meta)
+    do_show_parameters(args)
+
     info("Loading the inflater")
-    inflater = Inflater(args)
+    inflater = do_load_inflater(args)
 
     info("Executing actions")
     for name in args.do:
-        globals()['do_' + name](args, inflater, meta)
-
+        do_action(name, args, inflater, meta)
 
     info("Bye!")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mell-2.0.2/mell.egg-info/PKG-INFO` & `mell-2.0.3/mell.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.2
-Summary: A Metaprogramming Logic Layer designed to generate anything from template files
-Home-page: https://github.com/diegofps/pywup
+Version: 2.0.3
+Summary: Generate anything from template files and metadata files!
+Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: full
 
 # Mell
 
 Mell is a Metaprogramming Logic Layer designed to generate anything from template files. 
 
 # Why do I need this?
 
-There are moments in life that you may find yourself needing to customize an entire project, not only an e-mail or a single webpage in a backend response. These are the moments that you may want to use mell. So far, I have used it in the following situations:
+Sometimes it is useful to render an entire project, not only an e-mail or a single webpage, like in a webserver response. This is when mell comes to help. So far, I have used it in the following situations:
 
 * Generating VHDL code for a static neural network, variating a few parameters. Mell is much more flexible than the generic atributes available in the language.
 * Generating model classes for an ORM. I defined the model classes and relations as metadata and asked mell to generate them for me in C#.
 * Generating resumes to send to job applications. I use latex to generate my resume. Instead of changing multiple configuration files in my latex project I change only a single metadata file, customizing the letter, company name, color, and so on. Mell generates a latex source that I compile to PDF.
 
 Conceptually, you may use mell in two directions. A metadata used with multiple styles, representing different projections of the same thing, or a single style used by multiple metadata, creating different things with the same look. 
 
@@ -34,48 +34,56 @@
 
 You may constantly find that mell may be replaced by reflection or similar concepts on your programming language of choice. This is true and the answer to "which of them is better?" depends on your requirements. Mell may be more efficient as many logic rules are evaluated during rendering time, whereas reflection adds more complexity during the program execution. However, reflection is also simpler and more flexible during runtime. Mell is also more suitable to generate configuration files based on global parameters, like a kubernetes' configuration file or a django's settings.
 
 # Concepts
 
 To use this library you must understand a few concepts. These are:
 
-* `metadata:` These is data describing what we want to generate. We use json format for it.
-* `style:` This is the set of features that are necessary to transform the metadata into something. It is composed by templates, assets, static files, plugins, and logic rules.
-* `generated folder:` This is where the rendered files will be saved and you must never change these files. However, you may want to execute or compile them if you are generating a webserver or a latex template, for instance. 
+* `metadata:` The data describing what we want to generate. It is written using the json format.
+* `style:` Set of scripts, templates, and assets that will transform the metadata into something else.
+* `generated folder:` This is where the rendered files will be saved. You must never change these files as they will be overwritten the next time you execute mell. 
 
-A style is composed of the following concepts:
+A style is composed of the following items:
 
 * `template:` file snippets with a few missing parts. Mell will fill these parts with metadata when it generates the files and copy them to the generated folder, keeping the original path structure.
 * `static:` files that will not be modified. Mell will copy them directly to the generated folder, keeping the original path structure.
 * `asset:` files used by your style that are not automatically used by mell.
-* `plugin:` Scripts that will be executed by mell. These usually access the files in the asset folder.
-* `logic:` Scripts that will be executed in order by mell. These are used to validate and extend the metadata.
+* `plugin:` Scripts that will be automatically executed by mell. These scripts will usually interact with the `inflater` variable to generate multiple output files. It may load template files from the asset folder.
+* `logic:` Scripts that will be automatically executed, in order, by mell. These are used to validate and extend the metadata.
 
 # Basic folder structure
 
 The following table describes the folders used by mell.
 
 | Folder  | Description | 
 |-------------|-------------|
-| \<root\> | The base folder that contains all folders described here |
+| \<root\> | Base folder containing the folders meta, style, and the generated folder |
 | \<root\>/style | The base folder for template, static, plugin, and asset |
 | \<root\>/generate | this will hold the generated data, never edit this folder |
 | \<root\>/meta | holds all metadata as json files |
-| \<root\>/style/template | holds the template files that will be automatically rendered and written to the generated folder |
-| \<root\>/style/static | contains static files that will be copied as they are to the generate folder |
-| \<root\>/style/plugin | contains scripts that will be executed by mell. Use these to render multiple files from templates in the asset folder |
-| \<root\>/style/asset | contains template and other files that are not automatically used by mell. They may be used by plugins or other tools |
-| \<root\>/style/logic | contains scripts used automatically executed by mell to transform the metadata |
+| \<root\>/style/template | template files that will be automatically rendered and written to the generated folder |
+| \<root\>/style/static | static files that will be copied as they are to the output folder |
+| \<root\>/style/plugin | scripts that will be automatically executed by mell to render multiple output files |
+| \<root\>/style/asset | extra files that are not automatically used by mell. They may be used inside plugin and logic scripts |
+| \<root\>/style/logic | scripts automatically executed by mell to transform or extend the metadata |
 
-If you want to create a new project using this structure with the root folder named testing_mell, you can use the following command.
+To create a new project using the structure above, use the following command.
 
 ```shell
-mell --new testing_mell
+mell --new <name_of_root_folder>
 ```
 
+# Context variables
+
+These are important variables available troughout mell. They help to interact with templates, metadata, and command arguments.
+
+* `meta: ` an object of type Meta that encapsulates the metadata allowing easy navigation through its fields. Use `.` to access attributes and `[]` to access array elements. Navigation always returns an object with its same type, a Meta object. To access the object it references you must use the attribute `value`. You can also iterate over this object, if it references a json object the iteration will return a tuple of type `(str, Meta)`. If you iterate over an array it will always return a `Meta` object.
+* `inflater: ` an object used to inflate templates in the asset folder. Use the method `inflate` to inflate a template. You may call this method from a template inside the template folder or from a template in the asset folder to render a partial template in the template being generated. You may also call it from a plugin script, in this case it makes sense to use the optional parameter `to_file`. This will save the rendered template to the corresponding file in the output folder.
+* `args: ` an object holding all the program parameters. `Program parameters` are attributes that control the program executing, like the folders it reads and writes data to, and so on. You should never change any of these values during the program execution.
+
 # How to install / uninstall it?
 
 ```shell
 # To install
 pip install mell
 
 # To upgrade
@@ -83,15 +91,15 @@
 
 # To uninstall
 pip uninstall mell
 ```
 
 After installing the module you should be able to access the command `mell` via terminal. If it doesn't, you may try the following options: (1) check that your $PATH variable includes the local bin directory that pip uses; (2) install it in a virtual environment, like virtualenv; or (3) try to install it at the system level, running pip as root;
 
-# Generating Hello Worlds
+# Generating Programs
 
 This will demonstrate how to use mell in a simple use case, changing the language for a static interface. You may be thinking now, "what a naive example, most web frameworks have much more powerful internationalization tools and I would never use it for that". Indeed, me neither. I used this in my resumes in latex, though. By doing this I had a different metadata for each place I would apply, some in portuguese, some in english, some specific for each position. Another benefit is that I could update the resume by changing only a single file. I could generate old ones again, they had their own metadata, and so on.
 
 ## Step 1. Create a new mell project
 
 Execute the following command to create the standard structure.
 
@@ -244,51 +252,51 @@
         ├── asset
         ├── plugin
         ├── static
         └── template
             └── main.py
 ```
 
-# The Pipeline
+# Understanding the Pipeline
 
-Sometimes it is important to understand the order in which the operations are executed. The list below describe these operations in their standard order.
+It is important that you understand the order that operations are executed, as these may impact the availability of data throughout the execution. The list below shows the standard order.
 
 1. Load metadata
-1. Execute logic scripts
-1. Actions to generate the output:
+1. Run logic scripts
+1. Execute actions to generate the output:
 >4. Clean output folder [clean]
 >1. Copy static files [static]
 >1. Render templates and copy them to output [template]
->1. Execute plugin scripts [plugin]
+>1. Run plugin scripts [plugin]
 
-Loading the metadata and executing the logic scripts is always executed first and can't be changed. The list of actions to generate the output, though, can be modified or canceled. To modify the list of actions we use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
+Loading the metadata and running the logic scripts is always executed first. You can't modify this behaviour. The list of actions to generate the output, though, can be modified or supressed. To modify it we must use the command `--do <action_name>`. By default, mell will execute all of them but if we use the parameter `--do` it will execute only the tasks it received. A few examples are listed bellow.
 
 ```shell
 # These two calls are the same
 mell --do clean --do static --do template --do plugin data
 mell data
 
 # This will only generate output files based on the template folder
 mell --do template data
 
 # This will only clean the generated folder
-mell --do clean data
+mell --do clean
 
 # The word 'nothing' is a special keyword. It will not do any action but will still load the metadata and execute logic scripts. This is useful when used with -v (verose mode) or --show-metadata (display the metadata after executing the logic scripts).
 mell --do nothing data
 mell --do nothing -v data
 mell --do nothing --show-metadata data
 ```
 
 # Tutorials
 
 * [Metadata](https://github.com/diegofps/mell/blob/main/docs/metadata.md) - Explains how the metadata work and how to inherit and extend from existing metadata;
 * [Template](https://github.com/diegofps/mell/blob/main/docs/template.md) - Explains the template syntax and how to customize it;
 * [Plugin and Asset](https://github.com/diegofps/mell/blob/main/docs/plugin_and_asset.md) - Shows how to use a plugin script to generate multiple output files from a single template;
-* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend extend the input metadata, generating more metadata and preventing complex rules in template files.
+* [Logic](https://github.com/diegofps/mell/blob/main/docs/logic.md) - Shows how to extend the input metadata, generating more metadata and preventing complex rules in template files.
 
 # List of useful command options
 
 These are a few examples of common operations.
 
 ```shell
 # This will create a folder named project_name with the recommended root folder structure
@@ -302,14 +310,19 @@
 
 # Create a new logic file as <root>/style/logic/<timestamp>.logic_name.py
 mell --new-logic logic_name
 
 # Display the version number and exit
 mell --version
 
+# Use --set to customize the metadata from command line - useful when an external scripts needs to change something
+mell --set message 'Hello World!' en
+mell --set company.name 'Wespa' en
+mell --set users[2].name 'Diego Souza' en
+
 # Display more info during execution (verbose mode)
 mell -v en
 
 # Display less info during execution (quiet mode)
 mell -q en
 
 # Specify what we want to generate
@@ -332,9 +345,9 @@
 mell --style styles/python --generate generates/python/pt pt
 mell --style styles/cpp --generate generates/cpp/en en
 mell --style styles/cpp --generate generates/cpp/pt pt
 ```
 
 # Source Code
 
-The source code is available [here](https://github.com/diegofps/mell)
+The source code is available in the project's [repository](https://github.com/diegofps/mell).
```

### Comparing `mell-2.0.2/setup.py` & `mell-2.0.3/setup.py`

 * *Files identical despite different names*

