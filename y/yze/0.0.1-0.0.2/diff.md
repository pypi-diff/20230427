# Comparing `tmp/yze-0.0.1.tar.gz` & `tmp/yze-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yze-0.0.1.tar", last modified: Sun Apr 23 19:56:45 2023, max compression
+gzip compressed data, was "yze-0.0.2.tar", last modified: Thu Apr 27 12:56:11 2023, max compression
```

## Comparing `yze-0.0.1.tar` & `yze-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-23 19:56:45.611866 yze-0.0.1/
--rw-r--r--   0 nicolas    (501) staff       (20)     2452 2023-04-23 19:56:45.611751 yze-0.0.1/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     1955 2023-04-23 19:47:23.000000 yze-0.0.1/README.md
--rw-r--r--   0 nicolas    (501) staff       (20)      679 2023-04-22 22:18:54.000000 yze-0.0.1/pyproject.toml
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-23 19:56:45.611897 yze-0.0.1/setup.cfg
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-23 19:56:45.609962 yze-0.0.1/src/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-23 19:56:45.610536 yze-0.0.1/src/yze/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-17 19:54:16.000000 yze-0.0.1/src/yze/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3927 2023-04-23 19:43:28.000000 yze-0.0.1/src/yze/benchmark_mutant.py
--rw-r--r--   0 nicolas    (501) staff       (20)     8557 2023-04-22 21:54:05.000000 yze-0.0.1/src/yze/dice.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-23 19:56:45.611483 yze-0.0.1/src/yze.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     2452 2023-04-23 19:56:45.000000 yze-0.0.1/src/yze.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      269 2023-04-23 19:56:45.000000 yze-0.0.1/src/yze.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-23 19:56:45.000000 yze-0.0.1/src/yze.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       63 2023-04-23 19:56:45.000000 yze-0.0.1/src/yze.egg-info/entry_points.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-04-23 19:56:45.000000 yze-0.0.1/src/yze.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-23 19:56:45.611603 yze-0.0.1/tests/
--rw-r--r--   0 nicolas    (501) staff       (20)     1232 2023-04-22 21:56:06.000000 yze-0.0.1/tests/test_yze_dice.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003690 yze-0.0.2/
+-rw-r--r--   0 nicolas    (501) staff       (20)     4123 2023-04-27 12:56:11.003570 yze-0.0.2/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     3625 2023-04-27 12:53:16.000000 yze-0.0.2/README.md
+-rw-r--r--   0 nicolas    (501) staff       (20)      735 2023-04-27 12:53:55.000000 yze-0.0.2/pyproject.toml
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-27 12:56:11.003722 yze-0.0.2/setup.cfg
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.001676 yze-0.0.2/src/
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.002647 yze-0.0.2/src/yze/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-17 19:54:16.000000 yze-0.0.2/src/yze/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     4193 2023-04-24 07:10:59.000000 yze-0.0.2/src/yze/benchmark_mutant.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     9364 2023-04-25 11:31:30.000000 yze-0.0.2/src/yze/dice.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     5162 2023-04-27 12:49:37.000000 yze-0.0.2/src/yze/mutant_odds_of_pushing.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003275 yze-0.0.2/src/yze.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     4123 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      303 2023-04-27 12:56:11.000000 yze-0.0.2/src/yze.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      120 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003394 yze-0.0.2/tests/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1988 2023-04-27 11:06:19.000000 yze-0.0.2/tests/test_yze_dice.py
```

### Comparing `yze-0.0.1/PKG-INFO` & `yze-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yze
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package to handle YZE games mechanics
 Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
 Project-URL: Homepage, https://github.com/nlegrand/yze
 Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # System supported:
 - [X] Mutant: Year Zero
@@ -46,20 +46,70 @@
 >>> alien = AlienDicePool(pool=4, stress=1)
 >>> alien.throw()
 {'pool': [4, 1, 6, 1], 'stress': [2]}
 >>> alien.push()
 {'pool': [1, 3, 6, 2], 'stress': [1, 1]}
 ```
 
+# Odds of pushing
+
+Free League gives very general chances to get a succes when throwing
+and pushing a dice pool according to it’s size. But how can we get
+odds after the first roll is made? `mutant_odds_of_pushing` tries do
+do exactly that. Here is the doc:
+
+```
+$ mutant_odds_of_pushing  --help           
+usage: mutant_odds_of_pushing [-h] [-t THROWS] -a ATTRIBUTE_DICE [-s SKILL_DICE] [-g GEAR_DICE]
+
+Once you get a result, what are your odds when pushing it? feed this command your results and see what is likely or not to happen
+
+options:
+  -h, --help            show this help message and exit
+  -t THROWS, --throws THROWS
+  -a ATTRIBUTE_DICE, --attribute_dice ATTRIBUTE_DICE
+                        List your dice results eg: 253
+  -s SKILL_DICE, --skill_dice SKILL_DICE
+                        List your dice results eg: 45
+  -g GEAR_DICE, --gear_dice GEAR_DICE
+                        List your dice results eg: 32
+
+Experimental probabilities made with pseudo random numbers. Maybie it’s not the best you can get :).
+```
+And here is an example:
+
+
+```
+$ mutant_odds_of_pushing -a 253 -s 45 -g 32
+Throwing dice 100000 times !
+Odds of having:
+    -at least one success: 72.026 %
+    -at least one attr botch: 42.091 %
+    -at least one gear botch: 30.404 %
+    - 1 successes: 39.356 %
+    - 2 successes: 23.168 %
+    - 3 successes: 7.759 %
+    - 4 successes: 1.543 %
+    - 5 successes: 0.192 %
+    - 6 successes: 0.008 %
+    - 1 attribute botchs: 34.628 %
+    - 2 attribute botchs: 6.957 %
+    - 3 attribute botchs: 0.506 %
+    - 1 gear botchs: 27.686 %
+    - 2 gear botchs: 2.718 %
+```
+
+Running multiple times produce different odds, but in the same order.
+
 # Benchmark
 You can also benchmark dice throw to see what are your chances to get
 some successes or damage.
 
 ```
-benchmark_mutant --throw 10000 --attribute 4 --skill 2 --gear 1
+benchmark_mutant --throws 10000 --attribute 4 --skill 2 --gear 1
 Throwing dice 10000 times !
     at least one success : 7243
     at least one pushed success : 9096
     at least one damage to attribute : 7245
     at least one damage to gear : 2767
 {   'atleast_one': 7243,
     'atleast_one_attr_botch': 7245,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yze-0.0.1/src/yze/benchmark_mutant.py` & `yze-0.0.2/src/yze/benchmark_mutant.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,42 +14,32 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from yze.dice import MutantDicePool
 import argparse
 import pprint
 
-def main():
-    parser = argparse.ArgumentParser(
-                        prog='benchmark_mutant',
-                        description='make a lot of YZE rolls so as to have an idea of chances of success',
-                        epilog='')
-    
-    parser.add_argument('-t', '--throw', default=10000)      # option that takes a value
-    parser.add_argument('-a', '--attribute', default=1)
-    parser.add_argument('-s', '--skill', default=0)
-    parser.add_argument('-g', '--gear', default=0)
-    
-    args = parser.parse_args()
-    
-    
+def multiple_throws(throws=10000, attribute=1, skill=0, gear=0):
+    """Throw dice <throws> times, store results in <results>, return
+    results.
+    """
     results = {
         'atleast_one': 0,
         'atleast_one_pushed': 0,
         'atleast_one_attr_botch': 0,
         'atleast_one_gear_botch': 0,
         'successes': {},
         'pushed_successes': {},
         'attribute_botched': {},
         'gear_botched': {},
     }
     
-    print(f'Throwing dice {args.throw} times !')
-    for i in range(int(args.throw)):
-        d = MutantDicePool(attr=int(args.attribute), skill=int(args.skill), gear=int(args.gear))
+    print(f'Throwing dice {throws} times !')
+    for i in range(int(throws)):
+        d = MutantDicePool(attr=int(attribute), skill=int(skill), gear=int(gear))
         res = d.throw()
         pushed_res = d.push()
         successes = [x for x in d.result['attr'] + d.result['skill'] + d.result['gear'] if x == 6]
         if len(successes) > 0:
             results['atleast_one'] += 1
             if len(successes) not in results['successes']:
                 results['successes'][len(successes)] = 1
@@ -72,19 +62,37 @@
         gear_botched = [x for x in d.pushed_res['gear'] if x == 1]
         if len(gear_botched) > 0:
             results['atleast_one_gear_botch'] += 1
             if len(gear_botched) not in results['gear_botched']:
                 results['gear_botched'][len(gear_botched)] = 1
             else:
                 results['gear_botched'][len(gear_botched)] += 1
-    
+    return results
+
+def main():
+    """Fetch args from the commandline and proceed.
+    """
+    parser = argparse.ArgumentParser(
+                        prog='benchmark_mutant',
+                        description='make a lot of YZE rolls so as to have an idea of chances of success',
+                        epilog='')
+
+    parser.add_argument('-t', '--throws', default=10000)      # option that takes a value
+    parser.add_argument('-a', '--attribute', default=1)
+    parser.add_argument('-s', '--skill', default=0)
+    parser.add_argument('-g', '--gear', default=0)
+
+    args = parser.parse_args()
+
+    results = multiple_throws(args.throws, args.attribute, args.skill, args.gear)
+
     print (f'    at least one success : {results["atleast_one"]}')
     print (f'    at least one pushed success : {results["atleast_one_pushed"]}')
     print (f'    at least one damage to attribute : {results["atleast_one_attr_botch"]}')
     print (f'    at least one damage to gear : {results["atleast_one_gear_botch"]}')
-    
-    
+
+
     pp = pprint.PrettyPrinter(indent=4)
     pp.pprint(results)
 
 if __name__ == "__main__":
     main()
```

### Comparing `yze-0.0.1/src/yze/dice.py` & `yze-0.0.2/src/yze/dice.py`

 * *Files 5% similar despite different names*

```diff
@@ -197,22 +197,24 @@
                 self.pushed_res['artefact'] = self.result['artefact']
 
         self.pushed = True
         return self.pushed_res
 
 
 class AlienDicePool:
-    """Emulate the Alien dice pool throw and push. TODO: add multipush"""
+    """Emulate the Alien dice pool throw, push and multipush."""
     def __init__(self, pool=1, stress=0):
         self.pool = pool
         self.stress = stress
         self.thrown = False
         self.pushed = False
+        self.multipushed = False
         self.result = {'pool': [], 'stress': []}
         self.pushed_res = {'pool': [], 'stress': []}
+        self.multipushed_res = {'pool': [], 'stress': []}
 
     def throw(self):
         """Throw the dice and set the thrown state on.
         """    
         if self.thrown:
             return self.result
         dice = SimpleDice()
@@ -238,7 +240,28 @@
             if r == 6:
                 self.pushed_res['stress'].append(r)
             else:
                 self.pushed_res['stress'].append(dice.throw())
 
         self.pushed = True
         return self.pushed_res
+
+    def multipush(self):
+        """Push the dice a second time adding a stress die and set the
+        multipushed state on.
+        """
+        if self.multipushed:
+            return self.multipushed_res
+        dice = SimpleDice()
+        for r in self.pushed_res['pool']:
+            if r == 6:
+                self.multipushed_res['pool'].append(r)
+            else:
+                self.multipushed_res['pool'].append(dice.throw())
+        for r in self.pushed_res['stress'] + [2]:
+            if r == 6:
+                self.multipushed_res['stress'].append(r)
+            else:
+                self.multipushed_res['stress'].append(dice.throw())
+
+        self.multipushed = True
+        return self.multipushed_res
```

### Comparing `yze-0.0.1/src/yze.egg-info/PKG-INFO` & `yze-0.0.2/src/yze.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yze
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package to handle YZE games mechanics
 Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
 Project-URL: Homepage, https://github.com/nlegrand/yze
 Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # System supported:
 - [X] Mutant: Year Zero
@@ -46,20 +46,70 @@
 >>> alien = AlienDicePool(pool=4, stress=1)
 >>> alien.throw()
 {'pool': [4, 1, 6, 1], 'stress': [2]}
 >>> alien.push()
 {'pool': [1, 3, 6, 2], 'stress': [1, 1]}
 ```
 
+# Odds of pushing
+
+Free League gives very general chances to get a succes when throwing
+and pushing a dice pool according to it’s size. But how can we get
+odds after the first roll is made? `mutant_odds_of_pushing` tries do
+do exactly that. Here is the doc:
+
+```
+$ mutant_odds_of_pushing  --help           
+usage: mutant_odds_of_pushing [-h] [-t THROWS] -a ATTRIBUTE_DICE [-s SKILL_DICE] [-g GEAR_DICE]
+
+Once you get a result, what are your odds when pushing it? feed this command your results and see what is likely or not to happen
+
+options:
+  -h, --help            show this help message and exit
+  -t THROWS, --throws THROWS
+  -a ATTRIBUTE_DICE, --attribute_dice ATTRIBUTE_DICE
+                        List your dice results eg: 253
+  -s SKILL_DICE, --skill_dice SKILL_DICE
+                        List your dice results eg: 45
+  -g GEAR_DICE, --gear_dice GEAR_DICE
+                        List your dice results eg: 32
+
+Experimental probabilities made with pseudo random numbers. Maybie it’s not the best you can get :).
+```
+And here is an example:
+
+
+```
+$ mutant_odds_of_pushing -a 253 -s 45 -g 32
+Throwing dice 100000 times !
+Odds of having:
+    -at least one success: 72.026 %
+    -at least one attr botch: 42.091 %
+    -at least one gear botch: 30.404 %
+    - 1 successes: 39.356 %
+    - 2 successes: 23.168 %
+    - 3 successes: 7.759 %
+    - 4 successes: 1.543 %
+    - 5 successes: 0.192 %
+    - 6 successes: 0.008 %
+    - 1 attribute botchs: 34.628 %
+    - 2 attribute botchs: 6.957 %
+    - 3 attribute botchs: 0.506 %
+    - 1 gear botchs: 27.686 %
+    - 2 gear botchs: 2.718 %
+```
+
+Running multiple times produce different odds, but in the same order.
+
 # Benchmark
 You can also benchmark dice throw to see what are your chances to get
 some successes or damage.
 
 ```
-benchmark_mutant --throw 10000 --attribute 4 --skill 2 --gear 1
+benchmark_mutant --throws 10000 --attribute 4 --skill 2 --gear 1
 Throwing dice 10000 times !
     at least one success : 7243
     at least one pushed success : 9096
     at least one damage to attribute : 7245
     at least one damage to gear : 2767
 {   'atleast_one': 7243,
     'atleast_one_attr_botch': 7245,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yze-0.0.1/tests/test_yze_dice.py` & `yze-0.0.2/tests/test_yze_dice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 import unittest
 
 import yze.dice
 
 
 class TestYZEDice(unittest.TestCase):
     def test_is_int(self):
+        """SimpleDice should return an int
+        """
         d = yze.dice.SimpleDice()
         self.assertTrue(isinstance(d.throw(), int))
 
     def test_is_tuple(self):
+        """ArtefactDice and StepDice should return a tuple of two int
+        """
         ad = yze.dice.ArtefactDice()
         res = ad.throw()
         self.assertTrue(isinstance(res, tuple))
         self.assertEqual(len(res), 2)
         self.assertTrue(isinstance(res[0], int))
         self.assertTrue(isinstance(res[1], int))
         sd = yze.dice.StepDice()
         sres = sd.throw()
         self.assertTrue(isinstance(sres, tuple))
         self.assertEqual(len(sres), 2)
         self.assertTrue(isinstance(sres[0], int))
         self.assertTrue(isinstance(sres[1], int))
 
-    def test_state(self):
+    def test_state_mutant(self):
+        """MutantDicePool have state, thrown and pushed.
+        """
         mdp = yze.dice.MutantDicePool()
         self.assertFalse(mdp.thrown)
         self.assertFalse(mdp.pushed)
         mdp.throw()
         self.assertTrue(mdp.thrown)
         mdp.push()
         self.assertTrue(mdp.pushed)
+
+    def test_state_fbl(self):
+        """FBLDicePool have state, thrown and pushed.
+        """
         fbl = yze.dice.FBLDicePool()
         self.assertFalse(fbl.thrown)
         self.assertFalse(fbl.pushed)
         fbl.throw()
         self.assertTrue(fbl.thrown)
         fbl.push()
         self.assertTrue(fbl.pushed)
 
+    def test_state_alien(self):
+        """AlienDicePool have state, thrown, pushed and multipushed.
+        """
+        adp = yze.dice.AlienDicePool()
+        self.assertFalse(adp.thrown)
+        self.assertFalse(adp.pushed)
+        self.assertFalse(adp.multipushed)
+        adp.throw()
+        self.assertTrue(adp.thrown)
+        adp.push()
+        self.assertTrue(adp.pushed)
+        adp.multipush()
+        self.assertTrue(adp.multipushed)
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

