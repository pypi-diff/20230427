# Comparing `tmp/fast2q-2.5.1.tar.gz` & `tmp/fast2q-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast2q-2.5.1.tar", last modified: Mon Dec 12 13:22:29 2022, max compression
+gzip compressed data, was "dist\fast2q-2.5.2.tar", last modified: Thu Apr 27 13:11:37 2023, max compression
```

## Comparing `fast2q-2.5.1.tar` & `fast2q-2.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 13:22:29.000000 fast2q-2.5.1/
--rw-rw-rw-   0        0        0    13168 2022-12-12 13:22:29.000000 fast2q-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      492 2021-11-17 10:01:50.000000 fast2q-2.5.1/README.txt
-drwxrwxrwx   0        0        0        0 2022-12-12 13:22:29.000000 fast2q-2.5.1/fast2q/
--rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.1/fast2q/__init__.py
--rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.1/fast2q/__main__.py
--rw-rw-rw-   0        0        0    49468 2022-12-12 13:08:32.000000 fast2q-2.5.1/fast2q/fast2q.py
-drwxrwxrwx   0        0        0        0 2022-12-12 13:22:29.000000 fast2q-2.5.1/fast2q.egg-info/
--rw-rw-rw-   0        0        0    13168 2022-12-12 13:22:28.000000 fast2q-2.5.1/fast2q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2022-12-12 13:22:28.000000 fast2q-2.5.1/fast2q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 13:22:28.000000 fast2q-2.5.1/fast2q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2022-12-12 13:22:28.000000 fast2q-2.5.1/fast2q.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-12 13:22:28.000000 fast2q-2.5.1/fast2q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 13:22:29.000000 fast2q-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1525 2022-12-12 13:16:17.000000 fast2q-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/
+-rw-rw-rw-   0        0        0    13645 2023-04-27 13:11:37.000000 fast2q-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2021-11-17 10:01:50.000000 fast2q-2.5.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/fast2q/
+-rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.2/fast2q/__init__.py
+-rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.2/fast2q/__main__.py
+-rw-rw-rw-   0        0        0    49523 2023-04-27 13:00:29.000000 fast2q-2.5.2/fast2q/fast2q.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:11:37.000000 fast2q-2.5.2/fast2q.egg-info/
+-rw-rw-rw-   0        0        0    13645 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 13:11:36.000000 fast2q-2.5.2/fast2q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:11:37.000000 fast2q-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-04-27 13:09:14.000000 fast2q-2.5.2/setup.py
```

### Comparing `fast2q-2.5.1/PKG-INFO` & `fast2q-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.1
+Version: 2.5.2
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -30,14 +30,20 @@
         `python -m fast2q`
         
         
         For the non-graphical interface (the graphical interface can be buggy, or not work in some OS), type:
         
         `python -m fast2q -c`
         
+        
+        Make sure you have the latest version, type:
+        
+        `python -m fast2q -v`
+        
+        
         When running without specified parameters, 2FAST2Q will assume the current running directory has all the required files:
         
         	one .csv corresponding to features file (not required in 'Extract and Counter' mode)
         	the .FASTQ files
         
         
         
@@ -45,14 +51,16 @@
         
         	`python -m fast2q -h`
         
         	 `-h, --help  show this help message and exit `
         
         	 `-c [C]      cmd line mode`
         
+        	 `-v [V]      prints the current version`
+        
         	 `--s S       The full path to the directory with the sequencing files OR file`
         
         	 `--g G       The full path to the .csv file with the features.`
         
         	 `--o O       The full path to the output directory`
         	 
         	 `--fn FN     Specify an output compiled file name (default is called compiled)`
@@ -156,18 +164,19 @@
         
         Upon completion, several files should be seen in the indicated output folder (when running in default mode only b, c, and d will be kept):
         
         a. 	“*_reads.csv” files corresponding to the read counts per feature per inputted sequencing file; 
         
         b.	A “compiled_stats.csv” containing all the relevant input/output information about the 2FAST2Q analysis; 
         
-        c. 	A bar plot "reads_plot.png" representing the total number of reads, and valid reads, per sample; 
+        c.	A “compiled.csv” file with the compilation of all the read counts per feature in all the inputted files. Use this latter in the next steps of the data analysis pipeline. 
         
-        d.	A “compiled.csv” file with the compilation of all the read counts per feature in all the inputted files. Use this latter in the next steps of the data analysis pipeline. 
+        d.	A bar plot "reads_plot.png" with the number of total and quality passed reads (absolute), and in percentage ("reads_plot_percentage.png"), per sample; 
         
+        e. 	2 other violin plots with the distribution of the found features per sample are also presented (normalized for reads per milion, and absolute numbers). The interquartile distribution is also ploted for each sample (25%-75%)
         
         # Short Explanation
         
         2FAST2Q will return the read counts for all the features present in the input file. 
         A read will be aligned to its features if the minimum quality score in each nucleotide is >= the indicated phred-score,
         and if there is less than the indicated allowed mismatches. 
         Like said before, these parameters can be modified by the user.
```

### Comparing `fast2q-2.5.1/fast2q/fast2q.py` & `fast2q-2.5.2/fast2q/fast2q.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-try:
-    import csv
-    import glob
-    import os
-    import gzip
-    import multiprocessing as mp
-    import time
-    import matplotlib.pyplot as plt
-    import numpy as np
-    from numba import njit
-    import psutil
-    import argparse
-    import datetime
-    from tqdm import tqdm
-    from dataclasses import dataclass
-    from pathlib import Path
-    from io import SEEK_END
-    import zlib
-    import tkinter #(imported inside inputs_initializer()). imported here just to assertain
-except ImportError as e:
-    input(f"{e}\nConsider installing it using 'pip install {e.name}', and try again.\nPress enter to exit")
-    raise Exception
+import csv
+import glob
+import os
+import gzip
+import multiprocessing as mp
+import time
+import matplotlib.pyplot as plt
+import numpy as np
+from numba import njit
+import psutil
+import argparse
+import datetime
+from tqdm import tqdm
+from dataclasses import dataclass
+from pathlib import Path
+from io import SEEK_END
+import zlib
 
 #####################
 
 @dataclass
 class Features:
     
     """ Each feature will have its own class instance, where the read counts will be kept.
@@ -150,35 +145,38 @@
             if (start is not None) & (end is not None):
                 qual_up = str(qual[start:start+len(param['upstream'])],"utf-8")
                 qual_down = str(qual[end:end+len(param['downstream'])],"utf-8")
                 
                 if (len(param['quality_set_up'].intersection(qual_up)) == 0) &\
                     (len(param['quality_set_down'].intersection(qual_down)) == 0):
                     start+=len(param['upstream'])
+                    return start,end
 
         elif (param['upstream'] is not None) & (param['downstream'] is None):
             start=border_finder(param['upstream'],read_bin,param['miss_search_up'])
             
             if start is not None:
                 qual_up = str(qual[start:start+len(param['upstream'])],"utf-8")
                 
                 if len(param['quality_set_up'].intersection(qual_up)) == 0:
                     start+=len(param['upstream'])
                     end = start + param['length']
+                    return start,end
             
         elif (param['upstream'] is None) & (param['downstream'] is not None):
             end=border_finder(param['downstream'],read_bin,param['miss_search_down'])
             
             if end is not None:
                 qual_down = str(qual[end:end+len(param['downstream'])],"utf-8")
                 
                 if len(param['quality_set_down'].intersection(qual_down)) == 0:
                     start = end-param['length']
+                    return start,end
 
-        return start,end
+        return None,None
 
     def progress_bar(i,o,raw,cpu):
         
         def getuncompressedsize(raw):
             
             """ Estimates the total size of a .gz compressed 
             file for the progress bars """
@@ -236,15 +234,15 @@
                     if (start is not None) & (end is not None):
                         if end < start: #if the end is not found or found before the start
                             start=None
 
                 if (fixed_start) or (start is not None):
                     seq = str(reading[1][start:end].upper(),"utf-8")
                     quality = str(reading[3][start:end],"utf-8") #convert from bin to str
-    
+
                     if len(param['quality_set'].intersection(quality)) == 0:
                         
                         if param['Running Mode']=='C':
                             if seq in features:
                                 features[seq].counts += 1
                                 perfect_counter += 1
                             
@@ -477,16 +475,16 @@
         parameters["miss"]=int(parameters["miss"])
         parameters["phred"]=int(parameters["phred"])
         parameters["miss_search_up"]=int(parameters["miss_search_up"])
         parameters["miss_search_down"]=int(parameters["miss_search_down"])
         parameters["qual_up"]=int(parameters["qual_up"])
         parameters["qual_down"]=int(parameters["qual_down"])
     except Exception:
-        input("\nPlease confirm you have provided the correct parameters.\nOnly numeric values are accepted in the folowing fields:\n-Feature read starting place;\n-Feature length;\n-mismatch;\n-Phred score.\n\nPlease try again. Press enter to exit")
-        raise Exception    
+        print("\nPlease confirm you have provided the correct parameters.\nOnly numeric values are accepted in the folowing fields:\n-Feature read starting place;\n-Feature length;\n-mismatch;\n-Phred score.\n")
+        exit()
     
     # avoids getting -1 and actually filtering by highest phred score by mistake
     if int(parameters["phred"]) == 0:
         parameters["phred"] = 1
         
     if int(parameters["qual_up"]) == 0:
         parameters["qual_up"] = 1
@@ -513,16 +511,16 @@
     if "Extractor" in parameters['Running Mode']:
         parameters['Running Mode']="EC"
     else:
         parameters['Running Mode']="C"
         
     if parameters['Running Mode']=='C':
         if len(parameters) != 17:
-            input("Please confirm that all the input boxes are filled. Some parameters are missing.\nPress enter to exit")
-            raise Exception
+            print("Please confirm that all the input boxes are filled. Some parameters are missing.\nPress enter to exit")
+            exit()
             
     parameters["cmd"] = False
     parameters['cpu'] = False
 
     return parameters
 
 def inputs_initializer():
@@ -550,27 +548,27 @@
         
     def file(column,row,parameter,frame):
         filename = filedialog.askopenfilename(title = "Select a file", filetypes = \
             (("CSV files","*.csv"),("all files","*.*")) )
         filing_parser(column,row,filename,parameter,frame)
     
     def filing_parser(column,row,filename,parameter,frame):
-        place = Entry(frame,borderwidth=5,width=50)
+        place = Entry(frame,borderwidth=5,width=125)
         place.grid(row=row,column=column+1)
         place.insert(0, filename)
         parameters[parameter] = filename
 
     def browsing(keyword,inputs,placeholder="Use the Browse button to navigate, or paste a link"):
         title1,title2,row,column,function=inputs
         frame=LabelFrame(root,text=title1,padx=5,pady=5)
-        frame.grid(row=row,column=column, columnspan=2)
+        frame.grid(row=row,column=column, columnspan=4)
         button = Button(frame, text = title2,command = lambda: function(column,row,keyword,frame))
         button.grid(column = column, row = row)
-        button_place = Entry(frame,borderwidth=5,width=50)
-        button_place.grid(row=row,column=column+1)
+        button_place = Entry(frame,borderwidth=5,width=125)
+        button_place.grid(row=row,column=column+1, columnspan=4)
         button_place.insert(0, placeholder)
         temporary[keyword]=button_place
         
     def write_menu(keyword,inputs):
         title,row,column,default=inputs
         start = Entry(root,width=25,borderwidth=5)
         start.grid(row=row,column=column+1,padx=20,pady=5)
@@ -594,65 +592,63 @@
     def placeholder(row, column,title,padx,pady):
         placeholder = Label(root, text=title)
         placeholder.grid(row=row,column=column,padx=padx,pady=pady)
         return placeholder
         
     root = Tk()
     root.title("2FAST2Q Input Parameters Window")
-    root.minsize(425, 730)
+    root.minsize(425, 500)
     parameters,temporary = {},{}  
 
     browsing_inputs = {"seq_files":["Path to the .fastq(.gz) files folder","Browse",1,0,directory],
                        "feature":["Path to the features .csv file","Browse",2,0,file],
                        "out":["Path to the output folder","Browse",3,0,directory]}
 
-    default_inputs = {"out_file_name":["Output File Name",6,0,"Compiled"],
-                      "start":["Feature start position in the read",7,0,0],
-                      "length":["Feature length",8,0,20],
-                      "miss":["Allowed mismatches",9,0,1],
-                      "phred":["Minimal feature Phred-score",10,0,30],
-                      "delete":["Delete intermediary files [y/n]",12,0,"y"],
-                      "upstream":["Upstream search sequence",13,0,"None"],
-                      "downstream":["Downstream search sequence",16,0,"None"],
-                      "miss_search_up":["Mismatches in the upstream sequence",14,0,0],
-                      "miss_search_down":["Mismatches in the downstream sequence",17,0,0],
-                      "qual_up":["Minimal upstream sequence Phred-score",15,0,30],
-                      "qual_down":["Minimal downstream sequence Phred-score",18,0,30],}
+    default_inputs = {"out_file_name":["Output File Name",5,0,"Compiled"],
+                      "start":["Feature start position in the read",6,0,0],
+                      "length":["Feature length",7,0,20],
+                      "miss":["Allowed mismatches",8,0,1],
+                      "phred":["Minimal feature Phred-score",9,0,30],
+                      "delete":["Delete intermediary files [y/n]",10,0,"y"],
+                      "upstream":["Upstream search sequence",5,2,"None"],
+                      "downstream":["Downstream search sequence",8,2,"None"],
+                      "miss_search_up":["Mismatches in the upstream sequence",6,2,0],
+                      "miss_search_down":["Mismatches in the downstream sequence",9,2,0],
+                      "qual_up":["Minimal upstream sequence Phred-score",7,2,30],
+                      "qual_down":["Minimal downstream sequence Phred-score",10,2,30],}
     
     dropdown_options = {"Running Mode":["Counter", "Extractor + Counter",4,0],
-                        "Progress bar":["Yes", "No",5,0]}
+                        "Progress bar":["Yes", "No",4,2]}
 
     # Generating the dropdown browsing buttons
     [dropdown(arg,dropdown_options[arg]) for arg in dropdown_options]
     
     # Generating the file/folder browsing buttons
     [browsing(arg,browsing_inputs[arg]) for arg in browsing_inputs]
     
     # Generating the input parameter buttons
     [write_menu(arg,default_inputs[arg]) for arg in default_inputs]
     
     placeholder(0,1,"",0,0)
     #placeholder(19,0,"",0,0)
-    button_click(19, 0, "OK", submit)
-    button_click(19, 1, "Reset", restart)
+    button_click(19, 1, "OK", submit)
+    button_click(19, 2, "Reset", restart)
 
     root.mainloop()
 
     return parameters
 
 def initializer(cmd):
     
     """ Handles the program initialization process.
     Makes sure the path separators, and the input parser function is correct
     for the used OS.
     Creates the output diretory and handles some parameter parsing"""
-    
-    version = "2.5.1"
 
-    print("\nVersion: {}".format(version))
+    print(f"\nVersion: {version}")
 
     param = inputs_handler() if cmd is None else cmd
 
     param["version"] = version
     
     quality_list = '!"#$%&' + "'()*+,-/0123456789:;<=>?@ABCDEFGHI" #Phred score
 
@@ -688,14 +684,17 @@
 
     return param
 
 def input_parser():
     
     """ Handles the cmd line interface, and all the parameter inputs"""
     
+    global version
+    version = "2.5.2"
+    
     def current_dir_path_handling(param):
         if param[0] is None:
             parameters[param[1]]=os.getcwd()
             if param[1] == 'feature':
                 file = path_finder(os.getcwd(), ["*.csv"])
                 if parameters['Running Mode']!="EC":
                     if len(file) > 1:
@@ -705,19 +704,20 @@
                         parameters[param[1]]=file[0][0]
         else:
             parameters[param[1]]=param[0]
         return parameters
     
     parser = argparse.ArgumentParser()
     parser.add_argument("-c",nargs='?',const=True,help="cmd line mode")
+    parser.add_argument("-v",nargs='?',const=True,help="prints the installed version")
     parser.add_argument("--s",help="The full path to the directory with the sequencing files OR file")
     parser.add_argument("--g",help="The full path to the .csv file with the sgRNAs.")
     parser.add_argument("--o",help="The full path to the output directory")
     parser.add_argument("--fn",nargs='?',const="compiled",help="Specify an output compiled file name (default is called compiled)")
-    parser.add_argument("--v",nargs='?',const=False,help="Adds progress bars (default is enabled)")
+    parser.add_argument("--pb",nargs='?',const=False,help="Adds progress bars (default is enabled)")
     parser.add_argument("--m",help="number of allowed mismatches (default=1)")
     parser.add_argument("--ph",help="Minimal Phred-score (default=30)")
     parser.add_argument("--st",help="Feauture start position in the read (default is 0==1st bp)")
     parser.add_argument("--l",help="Feature length (default=20bp)")
     parser.add_argument("--us",help="Upstream search sequence")
     parser.add_argument("--ds",help="Downstream search sequence")
     parser.add_argument("--msu",help="mismatches allowed in the upstream sequence")
@@ -725,14 +725,18 @@
     parser.add_argument("--qsu",help="Minimal Phred-score (default=30) in the upstream search sequence")
     parser.add_argument("--qsd",help="Minimal Phred-score (default=30) in the downstream search sequence")
     parser.add_argument("--mo",help="Running Mode (default=C) [Counter (C) / Extractor + Counter (EC)]")
     parser.add_argument("--cp",help="Number of cpus to be used (default is max(cpu)-2 for >=3 cpus, -1 for >=2 cpus, 1 if 1 cpu")
     parser.add_argument("--k",nargs='?',const=False,help="If enabled, keeps all temporary files (default is disabled)")
     args = parser.parse_args()
     
+    if args.v is not None:
+        print(f"\nVersion: {version}\n")
+        exit()
+    
     #if its not running on command window mode
     if args.c is None:
         return None
     
     parameters = {}
     parameters["cmd"] = True
     paths_param = [[args.s,'seq_files'],
@@ -744,15 +748,15 @@
         parameters['out_file_name'] = args.fn
 
     parameters['length']=20
     if args.l is not None:
         parameters['length']=int(args.l)
         
     parameters['Progress bar']=True
-    if args.v is not None:
+    if args.pb is not None:
         parameters['Progress bar']=False
                  
     parameters['start']=0
     if args.st is not None:
         parameters['start']=int(args.st)
         
     parameters['phred']=30
@@ -1016,19 +1020,23 @@
     
     data = []
     for entry in distributions:
         data.append(distributions[entry])
     violin(data,head)
     
     ## normalized RPM
-    data = np.array(data)
-    data1 = []
-    for i,entry in enumerate(data):
-        data1.append(entry/sum(entry)*1000000) #RPM
-    violin(data1,head,normalized=True)
+    try:
+        data = np.array(data)
+        data1 = []
+        for i,entry in enumerate(data):
+            if sum(entry)>0:
+                data1.append(entry/sum(entry)*1000000) #RPM
+        violin(data1,head,normalized=True)
+    except ValueError:
+        pass
 
 def ram_lock():
 
     """ stops increasing the hash tables (failed and passed reads) 
     size to avoid using RAM that isnt there """
 
     if psutil.virtual_memory().percent >= 95:
@@ -1098,15 +1106,15 @@
 def hash_preprocesser(files,features,param,pool,cpu):
     
     """ For the smallest files, we processe them for the first x amount of reads to
     initialize the failed reads and passed reads hash tables. This will confer some 
     speed advantages, as subsquent files normally share the same reads that dont
     align to anything, or reads with mismatches that indeed align"""
     
-    print("\nInitializing hash tables.")
+    print("\nPlease standby for the initialization procedure.")
     result=[]
     for name in files[:cpu]:
         result.append(pool.apply_async(reads_counter, args=(0,0,name,features,param,cpu,set(),{},True)))
     
     compiled = [x.get() for x in result]
     throw1,throw2,throw3,throw4,failed_reads_compiled,passed_reads_compiled = zip(*compiled)
```

### Comparing `fast2q-2.5.1/fast2q.egg-info/PKG-INFO` & `fast2q-2.5.2/fast2q.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.1
+Version: 2.5.2
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -30,14 +30,20 @@
         `python -m fast2q`
         
         
         For the non-graphical interface (the graphical interface can be buggy, or not work in some OS), type:
         
         `python -m fast2q -c`
         
+        
+        Make sure you have the latest version, type:
+        
+        `python -m fast2q -v`
+        
+        
         When running without specified parameters, 2FAST2Q will assume the current running directory has all the required files:
         
         	one .csv corresponding to features file (not required in 'Extract and Counter' mode)
         	the .FASTQ files
         
         
         
@@ -45,14 +51,16 @@
         
         	`python -m fast2q -h`
         
         	 `-h, --help  show this help message and exit `
         
         	 `-c [C]      cmd line mode`
         
+        	 `-v [V]      prints the current version`
+        
         	 `--s S       The full path to the directory with the sequencing files OR file`
         
         	 `--g G       The full path to the .csv file with the features.`
         
         	 `--o O       The full path to the output directory`
         	 
         	 `--fn FN     Specify an output compiled file name (default is called compiled)`
@@ -156,18 +164,19 @@
         
         Upon completion, several files should be seen in the indicated output folder (when running in default mode only b, c, and d will be kept):
         
         a. 	“*_reads.csv” files corresponding to the read counts per feature per inputted sequencing file; 
         
         b.	A “compiled_stats.csv” containing all the relevant input/output information about the 2FAST2Q analysis; 
         
-        c. 	A bar plot "reads_plot.png" representing the total number of reads, and valid reads, per sample; 
+        c.	A “compiled.csv” file with the compilation of all the read counts per feature in all the inputted files. Use this latter in the next steps of the data analysis pipeline. 
         
-        d.	A “compiled.csv” file with the compilation of all the read counts per feature in all the inputted files. Use this latter in the next steps of the data analysis pipeline. 
+        d.	A bar plot "reads_plot.png" with the number of total and quality passed reads (absolute), and in percentage ("reads_plot_percentage.png"), per sample; 
         
+        e. 	2 other violin plots with the distribution of the found features per sample are also presented (normalized for reads per milion, and absolute numbers). The interquartile distribution is also ploted for each sample (25%-75%)
         
         # Short Explanation
         
         2FAST2Q will return the read counts for all the features present in the input file. 
         A read will be aligned to its features if the minimum quality score in each nucleotide is >= the indicated phred-score,
         and if there is less than the indicated allowed mismatches. 
         Like said before, these parameters can be modified by the user.
```

### Comparing `fast2q-2.5.1/setup.py` & `fast2q-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '2.5.1' 
+VERSION = '2.5.2' 
 DESCRIPTION = """A Python3 program that counts sequence occurences in fastq files."""
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="fast2q", 
         version=VERSION,
```

