# Comparing `tmp/culturalconformity-0.0.6.tar.gz` & `tmp/culturalconformity-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culturalconformity-0.0.6.tar", last modified: Wed Apr 26 22:39:41 2023, max compression
+gzip compressed data, was "culturalconformity-0.0.7.tar", last modified: Wed Apr 26 23:01:29 2023, max compression
```

## Comparing `culturalconformity-0.0.6.tar` & `culturalconformity-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.013348 culturalconformity-0.0.6/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 22:39:41.013082 culturalconformity-0.0.6/PKG-INFO
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.012306 culturalconformity-0.0.6/culturalconformity/
--rw-r--r--   0 kaledadenton   (501) staff       (20)       80 2023-04-26 22:39:28.000000 culturalconformity-0.0.6/culturalconformity/__init__.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)     3922 2023-04-26 22:38:29.000000 culturalconformity-0.0.6/culturalconformity/frq_over_time.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)     7139 2023-04-26 22:39:28.000000 culturalconformity-0.0.6/culturalconformity/interactive.py
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 22:39:41.012876 culturalconformity-0.0.6/culturalconformity.egg-info/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/PKG-INFO
--rw-r--r--   0 kaledadenton   (501) staff       (20)      277 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/SOURCES.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/dependency_links.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-26 22:39:41.000000 culturalconformity-0.0.6/culturalconformity.egg-info/top_level.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 22:39:41.013428 culturalconformity-0.0.6/setup.cfg
--rw-r--r--   0 kaledadenton   (501) staff       (20)      976 2023-04-26 22:36:54.000000 culturalconformity-0.0.6/setup.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:01:29.741329 culturalconformity-0.0.7/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 23:01:29.741175 culturalconformity-0.0.7/PKG-INFO
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:01:29.740145 culturalconformity-0.0.7/culturalconformity/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       80 2023-04-26 22:39:28.000000 culturalconformity-0.0.7/culturalconformity/__init__.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     3922 2023-04-26 22:38:29.000000 culturalconformity-0.0.7/culturalconformity/frq_over_time.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     6807 2023-04-26 23:00:22.000000 culturalconformity-0.0.7/culturalconformity/interactive.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:01:29.740998 culturalconformity-0.0.7/culturalconformity.egg-info/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 23:01:29.000000 culturalconformity-0.0.7/culturalconformity.egg-info/PKG-INFO
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      277 2023-04-26 23:01:29.000000 culturalconformity-0.0.7/culturalconformity.egg-info/SOURCES.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 23:01:29.000000 culturalconformity-0.0.7/culturalconformity.egg-info/dependency_links.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-26 23:01:29.000000 culturalconformity-0.0.7/culturalconformity.egg-info/top_level.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 23:01:29.741384 culturalconformity-0.0.7/setup.cfg
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      976 2023-04-26 23:00:39.000000 culturalconformity-0.0.7/setup.py
```

### Comparing `culturalconformity-0.0.6/culturalconformity/frq_over_time.py` & `culturalconformity-0.0.7/culturalconformity/frq_over_time.py`

 * *Files identical despite different names*

### Comparing `culturalconformity-0.0.6/culturalconformity/interactive.py` & `culturalconformity-0.0.7/culturalconformity/interactive.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,88 +8,80 @@
     if m == 1:
         yield (n,)
     else:
         for elem in range(n + 1):
             for state in get_states(n - elem, m - 1):
                 yield (elem,) + state
 
-
 def choose_n():
-    msg = "How many role models do you have? n ="
+    msg = "Number of role models n = "
     n = float(input(msg))
     while not n.is_integer() or n < 3:
-        n = float(input("Sorry, that was not valid; n must be an integer bigger than 2. " + msg))
+        n = float(input("That is not valid; n must be an integer bigger than 2. " + msg))
 
     ack = '0'
     if n > 50:
-        msg = ("Note that your number of role models is very large, and the code might be slow.\n"
-               + "Enter 0 to choose a different n or any other key to move forward with your previous choice.")
+        msg = "This number is large, and the code might be slow.\n Enter 0 to change n or any other key to proceed."
         ack = input(msg)
         if ack == '0':
             n = choose_n()
         else:
             return int(n)
     return int(n)
 
-
 def choose_m():
-    msg = "How many cultural variants do you have? m ="
+    msg = "How many cultural variants do you have? m = "
     m = float(input(msg))
     while not m.is_integer() or m < 2:
-        m = float(input("Sorry, that was not valid; m must be an integer bigger than 1. " + msg))
+        m = float(input("That is not valid; m must be an integer bigger than 1. " + msg))
 
     ack = '0'
     if m > 50:
-        msg = ("Note that your number of cultural variants is very large, and the code might be slow.\n"
-               + "Enter 0 to choose a different m or any other key to move forward with your previous choice.")
+        msg = "This number is large, and the code might be slow.\n Enter 0 to change m or any other key to proceed."
         ack = input(msg)
         if ack == '0':
             m = choose_m()
         else:
             return int(m)
     return int(m)
 
-
 def choose_d(d_min, d_max, denom_high, denom_low, x_vec, n):
     pr = 9  # Precision for rounding
     # Redo this because need it again
     x_subset = [j for j in x_vec if j != 0]
     x_avg = n / len(x_subset)
 
-    msg = ('For the state x = ' + str(x_vec) + ' please choose a value of d(x) between '
-           + str(d_min) + ' and ' + str(d_max) + '. For more information on how '
-           + 'to choose, enter a question mark.')
+    msg = 'For the state x = ' + str(x_vec) + ' choose a value of d(x) \nbetween ' + str(d_min) + ' and ' + str(d_max) + '. \nFor more information, enter a question mark.'
 
     d = input(msg)
     if d == '?':
         # Find g_i(x)*d(x) for each element
         g_values = []
         for l in range(len(x_vec)):
             x_l = x_vec[l]
             if (round(x_l, pr) == 0) or (round(x_l, pr) == n) or (round(x_l, pr) == round(x_avg, pr)):
                 g_values.append(0)
             elif x_l > x_avg:
                 g_values.append(x_l / denom_high)
             elif x_l < x_avg:
                 g_values.append(- (1 / x_l) * (1 / denom_low))
 
-        g_msg = ('For a given xi in x = ' + str(x_vec) + ', the value of d(x) that you choose '
-                 + 'will be divided by the number of role models, ' + str(n) + ', and multiplied '
-                 + 'by gi where g = ' + str(g_values) + '. Remember that this d(x) must be '
+        g_msg = ('For a given xi in x = ' + str(x_vec) + ', the value of d(x) that you choose \n'
+                 + 'will be divided by the number of role models, ' + str(n) + ', and multiplied \n'
+                 + 'by gi where g = ' + str(g_values) + '. Remember that this d(x) must be \n'
                  + 'between ' + str(d_min) + ' and ' + str(d_max) + '. Please enter your choice: ')
         d = input(g_msg)
 
     d = float(d)
     while d > d_max or d < d_min:
-        d = input('Sorry, d(x) is invalid or out of bounds; try again. Enter any key to acknowledge and continue.')
+        d = input('Sorry, d(x) is invalid or out of bounds; try again.')
         d = choose_d(d_min, d_max, denom_high, denom_low, x_vec, n)
 
     return float(d)
 
-
 def choose_conform_coeffs(n, m):
     pr = 9  # Precision used for rounding
     states = list(get_states(n, m))  # Get all possible role model states
     previous_states = {}  # This dictionary will store previous, symmetrical role model states
 
     for x_vec in states:  # For each role model state
         # Make a unique string for each symmetrical role model configuration (to be used later)
@@ -133,45 +125,42 @@
                 d_max = round(d_max, pr)
                 d = choose_d(d_min, d_max, denom_high, denom_low, x_vec, n)
 
             previous_states[x_str] = float(d)
 
     return previous_states
 
-
 def choose_p_vec(m):
     p_vec = []
     for i in range(1, m):
         msg = " frequency of cultural variant " + str(i)
         pi = float(input("Enter the" + msg))
         while sum(p_vec) + pi > 1:
-            pi = float(input("Sorry, the sum of all variant frequencies must not exceed 1. Choose a different" + msg))
+            pi = float(input("The sum of all frequencies cannot exceed 1. \nChoose a different" + msg))
         p_vec.append(pi)
 
     last_pi = 1 - sum(p_vec)
     p_vec.append(last_pi)
 
     return p_vec
 
-
 def interactive():
-    intro = input('Press ? for a detailed description of this function or any key to continue.')
+    intro = input('Press ? for a detailed description of this function or any key to continue. ')
     if intro == '?':
-        print("This function will allow you to specify conformity coefficients, initial variant frequencies, "
-              + "and more, but only one option at a time. Make sure to store your results in a variable, e.g., "
-              + "do not write interactive() all by itself but rather, say, x = interactive() so that "
-              + "your results will go into the variable called x. They will be in the appropriate format "
-              + "for input into future functions. See github.com/kaleda/culturalconformity for how to use "
+        print("This function will allow you to specify conformity coefficients, initial variant frequencies, \n"
+              + "and more, but only one option at a time. Make sure to store your results in a variable, e.g., \n"
+              + "do not write interactive() all by itself but rather, say, x = interactive() so that \n"
+              + "your results will go into the variable called x. They will be in the appropriate format \n"
+              + "for input into future functions. See github.com/kaleda/culturalconformity for how to use \n"
               + "the output of the interactive() function in the other functions. Let's get started!")
 
     msg = ("Enter 1 to make your dictionary of conformity coefficients. \n "
-           + "Enter 2 to make your list of initial frequencies. \n "
-           + "Enter 9 to quit.")
+           + "Enter 2 to make your list of initial frequencies. \n Enter 9 to quit. ")
     answer = float(input("What would you like to do? \n " + msg))
-    while not answer.is_integer() or answer < 1 or answer > 10:
+    while not answer.is_integer() or answer < 1 or answer > 9:
         answer = float(input("Sorry, that was not a valid number. \n " + msg))
 
     if answer == 1 or answer == 2:
         m = choose_m()
     if answer == 1:  # Make your dictionary of conformity coefficients
         n = choose_n()
         coeff_dict = choose_conform_coeffs(n, m)
```

### Comparing `culturalconformity-0.0.6/setup.py` & `culturalconformity-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Simulations of conformity, anti-conformity, and unbiased frequency-dependent transmission'
 # LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     name="culturalconformity",
     version=VERSION,
```

