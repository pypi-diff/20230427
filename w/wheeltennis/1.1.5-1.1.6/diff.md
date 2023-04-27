# Comparing `tmp/wheeltennis-1.1.5.tar.gz` & `tmp/wheeltennis-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheeltennis-1.1.5.tar", last modified: Fri Dec 16 11:15:54 2022, max compression
+gzip compressed data, was "wheeltennis-1.1.6.tar", last modified: Thu Apr 27 14:24:11 2023, max compression
```

## Comparing `wheeltennis-1.1.5.tar` & `wheeltennis-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-16 11:15:54.634308 wheeltennis-1.1.5/
--rw-rw-rw-   0        0        0     1091 2022-11-09 09:24:51.000000 wheeltennis-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     1317 2022-12-16 11:15:54.635306 wheeltennis-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      799 2022-11-15 16:11:43.000000 wheeltennis-1.1.5/README.md
--rw-rw-rw-   0        0        0       86 2022-12-16 11:15:54.641081 wheeltennis-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      996 2022-12-16 11:13:55.000000 wheeltennis-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-16 11:15:54.608766 wheeltennis-1.1.5/wheeltennis/
--rw-rw-rw-   0        0        0      184 2022-12-16 11:13:55.000000 wheeltennis-1.1.5/wheeltennis/__init__.py
--rw-rw-rw-   0        0        0    16023 2022-11-23 14:46:47.000000 wheeltennis-1.1.5/wheeltennis/match.py
--rw-rw-rw-   0        0        0    36533 2022-12-16 11:13:03.000000 wheeltennis-1.1.5/wheeltennis/plots.py
--rw-rw-rw-   0        0        0    13924 2022-12-15 15:23:15.000000 wheeltennis-1.1.5/wheeltennis/testing.py
-drwxrwxrwx   0        0        0        0 2022-12-16 11:15:54.630637 wheeltennis-1.1.5/wheeltennis.egg-info/
--rw-rw-rw-   0        0        0     1317 2022-12-16 11:15:54.000000 wheeltennis-1.1.5/wheeltennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-12-16 11:15:54.000000 wheeltennis-1.1.5/wheeltennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-16 11:15:54.000000 wheeltennis-1.1.5/wheeltennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-12-16 11:15:54.000000 wheeltennis-1.1.5/wheeltennis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-16 11:15:54.000000 wheeltennis-1.1.5/wheeltennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 14:24:11.708999 wheeltennis-1.1.6/
+-rw-rw-rw-   0        0        0     1091 2022-11-09 09:24:51.000000 wheeltennis-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1317 2023-04-27 14:24:11.708999 wheeltennis-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2022-11-15 16:11:43.000000 wheeltennis-1.1.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-27 14:24:11.715014 wheeltennis-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-04-27 14:17:00.000000 wheeltennis-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:24:11.689295 wheeltennis-1.1.6/wheeltennis/
+-rw-rw-rw-   0        0        0      184 2023-04-27 14:20:41.000000 wheeltennis-1.1.6/wheeltennis/__init__.py
+-rw-rw-rw-   0        0        0    18202 2023-04-27 14:12:19.000000 wheeltennis-1.1.6/wheeltennis/match.py
+-rw-rw-rw-   0        0        0    32259 2023-04-27 14:17:00.000000 wheeltennis-1.1.6/wheeltennis/plots.py
+-rw-rw-rw-   0        0        0    17736 2023-04-27 14:20:41.000000 wheeltennis-1.1.6/wheeltennis/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 14:24:11.706695 wheeltennis-1.1.6/wheeltennis.egg-info/
+-rw-rw-rw-   0        0        0     1317 2023-04-27 14:24:11.000000 wheeltennis-1.1.6/wheeltennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-27 14:24:11.000000 wheeltennis-1.1.6/wheeltennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 14:24:11.000000 wheeltennis-1.1.6/wheeltennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-27 14:24:11.000000 wheeltennis-1.1.6/wheeltennis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 14:24:11.000000 wheeltennis-1.1.6/wheeltennis.egg-info/top_level.txt
```

### Comparing `wheeltennis-1.1.5/LICENSE` & `wheeltennis-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wheeltennis-1.1.5/PKG-INFO` & `wheeltennis-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeltennis
-Version: 1.1.5
+Version: 1.1.6
 Summary: Basic scripts for wheelchair tennis analysis
 Home-page: https://gitlab.com/Thomas2016/wheeltennis
 Download-URL: https://gitlab.com/Thomas2016/wheeltennis
 Author: Thomas Rietveld
 Author-email: t.rietveld@lboro.ac.uk
 License: GNU GPLv3
 Keywords: wheelchair tennis,sensor,IMUs
```

### Comparing `wheeltennis-1.1.5/README.md` & `wheeltennis-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wheeltennis-1.1.5/setup.py` & `wheeltennis-1.1.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
 	name             		= 'wheeltennis',
-	version          		= '1.1.5',
+	version          		= '1.1.6',
 	description      		= 'Basic scripts for wheelchair tennis analysis',
 	author           		= 'Thomas Rietveld',
 	author_email     		= 't.rietveld@lboro.ac.uk',
 	url              		= 'https://gitlab.com/Thomas2016/wheeltennis',
 	download_url     		= 'https://gitlab.com/Thomas2016/wheeltennis',
 	packages         		= ['wheeltennis'],
 	package_data     		= {},
 	include_package_data 	= True,
 	long_description 		= read("README.md"),
 	license 				= 'GNU GPLv3',
 	keywords         		= ['wheelchair tennis', 'sensor', 'IMUs'],
 	classifiers      		= ["Programming Language :: Python",
 							   "Intended Audience :: Science/Research",
 							   "Operating System :: OS Independent"],
-	install_requires 		= ["numpy", "scipy>=1.2.0", "pandas", "matplotlib", "worklab"]
+	install_requires 		= ["numpy", "seaborn", "scipy>=1.2.0", "pandas", "matplotlib", "worklab"]
 )
```

### Comparing `wheeltennis-1.1.5/wheeltennis/match.py` & `wheeltennis-1.1.6/wheeltennis/match.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,42 +22,35 @@
     # Cut the dataset in forward and reverse velocity
     forward = sessiondata['frame'][(sessiondata['frame']['vel']) > 0.1].reset_index(drop=True)
     reverse = sessiondata['frame'][(sessiondata['frame']['vel']) < -0.1].reset_index(drop=True)
 
     mean_vel = np.mean(forward['vel'])
     peak_vel = np.max(forward['vel'])
 
-    lsa = forward[forward['vel'] < 1]
-    lsa_per = len(lsa) / len(forward) * 100
-    msa = forward[(forward['vel'] > 1) & (forward['vel'] < 2)]
-    msa_per = len(msa) / len(forward) * 100
     hsa = forward[forward['vel'] > 2]
-    hsa_per = len(hsa) / len(forward) * 100
-
     n_hsa = (hsa['time'].diff() > 2).sum()
     n_hsa_pm = (n_hsa / ((len(forward) + len(reverse)) / 100)) * 60
 
     peaks, _ = find_peaks(forward['vel'], prominence=0.5, distance=50, width=50, height=2)
     vel_peaks = forward['vel'][peaks]
     vel_peaks = vel_peaks.sort_values(ascending=False)
     mean_vel_best5 = np.mean(vel_peaks.head(5))
 
-    mean_rev_vel = -np.mean(reverse['vel'])
-    peak_rev_vel = -np.min(reverse['vel'])
+    mean_rev_vel = np.mean(reverse['vel'])
+    peak_rev_vel = np.min(reverse['vel'])
 
     outcomes_vel = pd.DataFrame([])
-    outcomes_vel = outcomes_vel.append([{'vel_mean': mean_vel,
-                                         'vel_peak': peak_vel,
-                                         'rev_vel_mean': mean_rev_vel,
-                                         'rev_vel_peak': peak_rev_vel,
-                                         'per_low_speed_zone': lsa_per,
-                                         'per_mid_speed_zone': msa_per,
-                                         'per_high_speed_zone': hsa_per,
-                                         'num_high_speed_activations_pm': n_hsa_pm,
-                                         'mean_best_5_vel': mean_vel_best5}], ignore_index=True)
+    outcomes_vel['vel_mean'] = [mean_vel]
+    outcomes_vel['vel_peak'] = peak_vel
+    outcomes_vel['rev_vel_mean'] = mean_rev_vel
+    outcomes_vel['rev_vel_peak'] = peak_rev_vel
+    outcomes_vel['num_high_speed_activations_pm'] = n_hsa_pm
+    outcomes_vel['mean_best_5_vel'] = mean_vel_best5
+    outcomes_vel = round(outcomes_vel, 2)
+
     return outcomes_vel
 
 
 def acc_var(sessiondata):
     """
     Calculate acceleration variables of a wheelchair tennis match
 
@@ -70,44 +63,63 @@
     -------
     outcomes_acc : pd.Series
         pd.Series with all acceleration variables
 
     """
     # Cut the dataset in forward, reverse velocity and positive accelerations
     forward = sessiondata['frame'][(sessiondata['frame']['vel']) > 0.1].reset_index(drop=True)
+    forward['acc'] = forward['acc_wheel']
     forward_acc = forward[(forward['acc']) > 0.1].reset_index(drop=True)
+    forward_dec = forward[(forward['acc']) < -0.1].reset_index(drop=True)
 
     mean_acc = np.mean(forward_acc['acc'])
+    mean_dec = np.mean(forward_dec['acc'])
+
+    peak_acc = np.max(forward_acc['acc'])
+    peak_dec = np.min(forward_dec['acc'])
 
     laa = forward_acc[forward_acc['acc'] < 0.75]
     laa_per = len(laa) / len(forward_acc) * 100
     maa = forward_acc[(forward_acc['acc'] > 0.75) & (forward_acc['acc'] < 1.5)]
     maa_per = len(maa) / len(forward_acc) * 100
     haa = forward_acc[forward_acc['acc'] > 1.5]
     haa_per = len(haa) / len(forward_acc) * 100
 
     outcomes_acc = pd.DataFrame([])
-    outcomes_acc = outcomes_acc.append([{'acc_mean': mean_acc,
-                                         'per_low_acc_zone': laa_per,
-                                         'per_mid_acc_zone': maa_per,
-                                         'per_high_acc_zone': haa_per}], ignore_index=True)
+    outcomes_acc['acc_mean'] = [mean_acc]
+    outcomes_acc['dec_mean'] = mean_dec
+    # outcomes_acc['acc_peak'] = peak_acc
+    # outcomes_acc['dec_peak'] = peak_dec
+    # outcomes_acc['per_low_acc_zone'] = laa_per
+    # outcomes_acc['per_mid_acc_zone'] = maa_per
+    # outcomes_acc['per_high_acc_zone'] = haa_per
+
+    outcomes_acc = round(outcomes_acc, 2)
+
     return outcomes_acc
 
 
-def rot_vel_var(sessiondata, side: bool = True):
+def rot_vel_var(sessiondata, side: bool = True, subsets: bool = True):
     """
     Calculate rotational velocity variables of a wheelchair tennis match
 
     Parameters
     ----------
     sessiondata : dict
         processed sessiondata structure
     side : bool
         if set to True left side is analysed
         if set to False right side is analysed
+    subsets : bool
+        if set to True subsets are analysed (curve 1-2 and turns 1-2)
+            turn 1: velocities -0.5 - 0.5 m/s
+            turn 2: velocities -1.5 - 1.5 m/s
+            curve 1: velocities 1 - 2 m/s
+            curve 2: velocities > 1.5 m/s
+        if set to False no subsets are analysed
 
     Returns
     -------
     outcomes_rot_vel : pd.Series
         pd.Series with all rotational velocity variables
 
     """
@@ -125,44 +137,54 @@
 
     turn1 = rotate[(rotate['vel'] > -0.5) & (rotate['vel'] < 0.5)].reset_index(drop=True)
     turn2 = rotate[(rotate['vel'] > -1.5) & (rotate['vel'] < 1.5)].reset_index(drop=True)
     curve1 = rotate[(rotate['vel'] > 1) & (rotate['vel'] < 2)].reset_index(drop=True)
     curve2 = rotate[rotate['vel'] > 1.5].reset_index(drop=True)
 
     moves = [rotate, turn1, turn2, curve1, curve2]
-    moves_keys = ['all', 'turn1', 'turn2', 'curve1', 'curve2']
+    if subsets is True:
+        moves_keys = ['all', 'turn1', 'turn2', 'curve1', 'curve2']
+    else:
+        moves_keys = ['all']
     outcomes_rot_vel = pd.DataFrame([])
 
     for movement, keys in zip(moves, moves_keys):
         if keys == 'all':
             peaks, _ = find_peaks(movement['rot_vel'], prominence=50, height=90, width=20, distance=50)
         else:
             peaks, _ = find_peaks(movement['rot_vel'], prominence=50, height=90, width=20, distance=50)
         rot_vel_peaks = movement['rot_vel'][peaks]
         rot_vel_peaks = rot_vel_peaks.sort_values(ascending=False)
         mean_rot_vel = np.mean(movement['rot_vel'])
         mean_rot_vel_best5 = np.mean(rot_vel_peaks.head(5))
         outcomes_rot_vel[keys + '_mean_rot_vel_' + side] = [mean_rot_vel]
         outcomes_rot_vel[keys + '_mean_best5_rot_vel_' + side] = [mean_rot_vel_best5]
+    outcomes_rot_vel = round(outcomes_rot_vel, 2)
 
     return outcomes_rot_vel
 
 
-def rot_acc_var(sessiondata, side: bool = True):
+def rot_acc_var(sessiondata, side: bool = True, subsets: bool = True):
     """
     Calculate rotational acceleration variables of a wheelchair tennis match
 
     Parameters
     ----------
     sessiondata : dict
         processed sessiondata structure
     side : bool
         if set to True left side is analysed
         if set to False right side is analysed
-
+    subsets : bool
+        if set to True subsets are analysed (curve 1-2 and turns 1-2)
+            turn 1: velocities -0.5 - 0.5 m/s
+            turn 2: velocities -1.5 - 1.5 m/s
+            curve 1: velocities 1 - 2 m/s
+            curve 2: velocities > 1.5 m/s
+        if set to False no subsets are analysed
     Returns
     -------
     outcomes_rot_acc : pd.Series
         pd.Series with all rotational acceleration variables
 
     """
     # Cut the dataset in part where there was movement
@@ -180,45 +202,45 @@
 
     turn1 = rotate_acc[(rotate_acc['vel'] > -0.5) & (rotate_acc['vel'] < 0.5)].reset_index(drop=True)
     turn2 = rotate_acc[(rotate_acc['vel'] > -1.5) & (rotate_acc['vel'] < 1.5)].reset_index(drop=True)
     curve1 = rotate_acc[(rotate_acc['vel'] > 1) & (rotate_acc['vel'] < 2)].reset_index(drop=True)
     curve2 = rotate_acc[rotate_acc['vel'] > 1.5].reset_index(drop=True)
 
     moves = [rotate_acc, turn1, turn2, curve1, curve2]
-    moves_keys = ['all', 'turn1', 'turn2', 'curve1', 'curve2']
+    if subsets is True:
+        moves_keys = ['all', 'turn1', 'turn2', 'curve1', 'curve2']
+    else:
+        moves_keys = ['all']
     outcomes_rot_acc = pd.DataFrame([])
 
     for movement, keys in zip(moves, moves_keys):
         mean_rot_acc = np.mean(movement['rot_acc'])
         outcomes_rot_acc[keys + '_mean_rot_acc_' + side] = [mean_rot_acc]
+    outcomes_rot_acc = round(outcomes_rot_acc, 2)
 
     return outcomes_rot_acc
 
 
-def gen_var(sessiondata, side: bool = True, sfreq: float = 400.):
+def gen_var(sessiondata):
     """
     Calculate general variables of a wheelchair tennis match
 
     Parameters
     ----------
     sessiondata : dict
         processed sessiondata structure
-    side: bool = True
-        if set to True (right-handed)
-        if set to False (left-handed)
-    sfreq : float
-        sampling frequency
 
     Returns
     -------
     outcomes_gen : pd.Series
-        pd.Series with all general variables (time, distance, turns)
+        pd.Series with all general variables (time, distance, ratios)
 
     """
     # Cut the dataset in forward and reverse velocity and the resting part
+    sfreq = 1 / sessiondata['frame']['time'].diff().mean()
     forward = sessiondata['frame'][(sessiondata['frame']['vel']) > 0.1].reset_index(drop=True)
     reverse = sessiondata['frame'][(sessiondata['frame']['vel']) < -0.1].reset_index(drop=True)
     rest = sessiondata['frame'][(sessiondata['frame']['vel'] < 0.1) & (sessiondata['frame']['vel'] > -0.1)].reset_index(
         drop=True)
 
     work = len(forward['time']) + len(reverse['time'])
     rest = len(rest['time'])
@@ -228,116 +250,163 @@
     ratio_reverse = len(reverse['time']) / work * 100
     for_rev = ratio_forward / ratio_reverse
 
     ratio_work = work / total * 100
     ratio_rest = rest / total * 100
     work_rest = ratio_work / ratio_rest
 
-    if side is True:
-        noracket_rotate = forward[forward['rot_vel'] > 160]
-        racket_rotate = forward[forward['rot_vel'] < -160]
-    else:
-        noracket_rotate = forward[forward['rot_vel'] < -160]
-        racket_rotate = forward[forward['rot_vel'] > 160]
-
-    n_noracket_turns = (noracket_rotate['time'].diff() > 2).sum()
-    n_noracket_turns_pm = (n_noracket_turns / ((len(forward) + len(reverse)) / 100)) * 60
-    n_racket_turns = (racket_rotate['time'].diff() > 2).sum()
-    n_racket_turns_pm = (n_racket_turns / ((len(forward) + len(reverse)) / 100)) * 60
-
     tot_duration_min = total / (sfreq * 60)
+    tot_duration_active = work / (sfreq * 60)
     tot_distance = max(sessiondata['frame']['dist'])
 
-    distance_pm = tot_distance / tot_duration_min
+    distance_pm = tot_distance / tot_duration_active
 
     outcomes_gen = pd.DataFrame([])
-    outcomes_gen = outcomes_gen.append([{'ratio_forward': ratio_forward,
-                                         'ratio_reverse': ratio_reverse,
-                                         'forward_reverse': for_rev,
-                                         'n_noracket_turns_pm': n_noracket_turns_pm,
-                                         'n_racket_turns_pm': n_racket_turns_pm,
-                                         'ratio_work': ratio_work,
-                                         'ratio_rest': ratio_rest,
-                                         'work_rest': work_rest,
-                                         'tot_duration_m': tot_duration_min,
-                                         'tot_distance': tot_distance,
-                                         'distance_pm': distance_pm}], ignore_index=True)
+    outcomes_gen['ratio_forward'] = [ratio_forward]
+    outcomes_gen['ratio_reverse'] = ratio_reverse
+    outcomes_gen['forward_reverse'] = for_rev
+    outcomes_gen['ratio_work'] = ratio_work
+    outcomes_gen['ratio_rest'] = ratio_rest
+    outcomes_gen['work_rest'] = work_rest
+    outcomes_gen['tot_duration_active_min'] = tot_duration_active
+    outcomes_gen['tot_duration'] = tot_duration_min
+    outcomes_gen['tot_distance'] = tot_distance
+    outcomes_gen['distance_per_min'] = distance_pm
+    outcomes_gen = round(outcomes_gen, 2)
+
     return outcomes_gen
 
 
-def speed_zones(sessiondata):
-    speed_zone_outcomes = pd.DataFrame([])
-    movement = sessiondata['frame'][
-        (sessiondata['frame']['vel_filt'] > 0.1) | (sessiondata['frame']['vel_filt'] < -0.1)]
-    zones = [-10, 0, 5, 7.5, 10, 12.5, 15]
-    zones2 = [0, 5, 7.5, 10, 12.5, 15, 99]
-    zones_ms = [x / 3.6 for x in zones]
-    zones_ms2 = [x / 3.6 for x in zones2]
-
-    for zone, zone2 in zip(zones_ms, zones_ms2):
-        zone_ind = ((movement['vel_filt'] >= zone) & (movement['vel_filt'] < zone2))
-        movement_zone = movement[zone_ind]
+def speed_zones(sessiondata, percentage=False, top_speed=0):
+    speed_zone_outcomes_all = pd.DataFrame([])
+    speed_zone_outcomes_disp = pd.DataFrame([])
+    speed_zone_outcomes_per = pd.DataFrame([])
+    move = sessiondata['frame'][
+        (sessiondata['frame']['vel'] > 0.1) | (sessiondata['frame']['vel'] < -0.1)]
+
+    if percentage is True:  # and math.isnan(top_speed) is False
+        zones = [-np.inf, 0, 0.2 * top_speed, 0.5 * top_speed, 0.8 * top_speed,
+                 0.95 * top_speed]
+        zones2 = [0, 0.2 * top_speed, 0.5 * top_speed, 0.8 * top_speed, 0.95 * top_speed,
+                  np.inf]
+        zone_names = ['-inf', '0', '20%', '50%', '80%', '95%']
+        zone_names2 = ['0', '20%', '50%', '80%', '95%', 'inf']
+    else:
+        zones = [-np.inf, 0, 1, 2, 3, 4, 5]
+        zones2 = [0, 1, 2, 3, 4, 5, np.inf]
+        zone_names = ['-inf', '0', '1', '2', '3', '4', '5']
+        zone_names2 = ['0', '1', '2', '3', '4', '5', 'inf']
+
+    for zone, zone2, zone_name, zone_name2 in zip(zones, zones2, zone_names, zone_names2):
+        zone_ind = ((move['vel'] >= zone) & (move['vel'] < zone2))
+        move_zone = move[zone_ind]
         if zone_ind is not None:
-            per_speed_zone = (len(movement_zone) / len(movement) * 100)
-            frame_dist = cumtrapz(movement_zone['vel_filt'], initial=0.0) / 52
+            per_speed_zone = (len(move_zone) / len(move) * 100)
+            frame_dist = cumtrapz(move_zone['vel'], initial=0.0) / 52
             disp_speed_zone = (max(abs(frame_dist)))
-            freq_speed_zone = ((movement_zone['time'].diff() > 0.5).sum())
+            freq_speed_zone = ((move_zone['time'].diff() > 0.5).sum())
         else:
             per_speed_zone = 0
             disp_speed_zone = 0
             freq_speed_zone = 0
-
         outcomes = pd.DataFrame([[per_speed_zone, disp_speed_zone, freq_speed_zone]],
                                 columns=['per_speed_zone', 'disp_speed_zone', 'freq_speed_zone'],
-                                index=[str(round(zone, 2)) + ' - ' + str(round(zone2, 2))])
-        speed_zone_outcomes = pd.concat([speed_zone_outcomes, outcomes])
+                                index=[zone_name + ' - ' + zone_name2])
+        outcomes_per = pd.DataFrame([per_speed_zone], columns=['per_speed_zone_' + zone_name + '-' + zone_name2])
+        outcomes_disp = pd.DataFrame([disp_speed_zone], columns=['disp_speed_zone_' + zone_name + '-' + zone_name2])
+
+        speed_zone_outcomes_all = pd.concat([speed_zone_outcomes_all, outcomes])
+        speed_zone_outcomes_disp = pd.concat([speed_zone_outcomes_disp, outcomes_disp], axis=1)
+        speed_zone_outcomes_per = pd.concat([speed_zone_outcomes_per, outcomes_per], axis=1)
+
+    speed_zone_outcomes_table = round(speed_zone_outcomes_all, 2)
+    speed_zone_outcomes_row = pd.concat([speed_zone_outcomes_disp, speed_zone_outcomes_per], axis=1)
+    speed_zone_outcomes_row = round(speed_zone_outcomes_row, 2)
 
-    return speed_zone_outcomes
+    return speed_zone_outcomes_row
 
 
 def acc_zones(sessiondata):
     acc_zone_outcomes = pd.DataFrame([])
-    movement = sessiondata['frame'][
-        (sessiondata['frame']['vel_filt'] > 0.1) | (sessiondata['frame']['vel_filt'] < -0.1)]
-    zones = [-99, 0, 1, 1.5, 2, 2.5, 5]
-    zones2 = [0, 1, 1.5, 2, 2.5, 5, 99]
+    move = sessiondata['frame'][
+        (sessiondata['frame']['vel'] > 0.1) | (sessiondata['frame']['vel'] < -0.1)]
+    zones = [-np.inf, 0, 1, 1.5, 2, 2.5, 5]
+    zones2 = [0, 1, 1.5, 2, 2.5, 5, np.inf]
 
     for zone, zone2 in zip(zones, zones2):
-        zone_ind = ((movement['acc'] >= zone) & (movement['acc'] < zone2))
-        movement_zone = movement[zone_ind]
+        zone_ind = ((move['acc'] >= zone) & (move['acc'] < zone2))
+        move_zone = move[zone_ind]
         if zone_ind is not None:
-            per_acc_zone = (len(movement_zone) / len(movement) * 100)
-            frame_dist = cumtrapz(movement_zone['vel_filt'], initial=0.0) / 52
+            per_acc_zone = (len(move_zone) / len(move) * 100)
+            frame_dist = cumtrapz(move_zone['vel'], initial=0.0) / 52
             disp_acc_zone = (max(abs(frame_dist)))
-            freq_acc_zone = ((movement_zone['time'].diff() > 0.1).sum())
+            freq_acc_zone = ((move_zone['time'].diff() > 0.1).sum())
         else:
             per_acc_zone = 0
             disp_acc_zone = 0
             freq_acc_zone = 0
 
         outcomes = pd.DataFrame([[per_acc_zone, disp_acc_zone, freq_acc_zone]],
                                 columns=['per_acc_zone', 'disp_acc_zone', 'freq_acc_zone'],
                                 index=[str(round(zone, 2)) + ' - ' + str(round(zone2, 2))])
         acc_zone_outcomes = pd.concat([acc_zone_outcomes, outcomes])
+    acc_zone_outcomes = round(acc_zone_outcomes, 2)
 
     return acc_zone_outcomes
 
-# def turns(sessiondata):
 
-#     movement = sessiondata['frame'][(sessiondata['frame']['vel_filt']>0.1) | (sessiondata['frame']['vel_filt']<-0.1)]
-#     left_rotate = movement[movement['rot_vel_filt'] > 120]
-#     right_rotate = movement[movement['rot_vel_filt'] < -120]
+def turns(sessiondata):  # Rotations are based on rotational velocity now, not on actual rotations
+    sfreq = 1 / sessiondata['frame']['time'].diff().mean()
+    move = sessiondata['frame'][(sessiondata['frame']['vel'] > 0.1) | (sessiondata['frame']['vel'] < -0.1)]
+    left_rotate = move[move['rot_vel'] > 160]
+    right_rotate = move[move['rot_vel'] < -160]
+
+    left_turns = (left_rotate['time'].diff() > 0.5).sum()
+    left_turns_pm = (left_turns / (len(move) / sfreq)) * 60
+    right_turns = (right_rotate['time'].diff() > 0.5).sum()
+    right_turns_pm = (right_turns / (len(move) / sfreq)) * 60
+
+    turns = pd.DataFrame([])
+    turns['left_turns'] = [left_turns]
+    turns['right_turns'] = right_turns
+    turns['left_turns_pm'] = left_turns_pm
+    turns['right_turns_pm'] = right_turns_pm
+
+    return turns
+
+
+def rot_vel_zones(sessiondata):
+    rot_vel_zone_outcomes = pd.DataFrame([])
+    move = sessiondata['frame'][
+        (sessiondata['frame']['vel'] > 0.1) | (sessiondata['frame']['vel'] < -0.1)]
+    rotate = move[abs(move['rot_vel']) > 10].reset_index(drop=True)
 
+    zones = [-np.inf, -180, -135, -90, -45, 0, 45, 90, 135, 180]
+    zones2 = [-180, -135, -90, -45, 0, 45, 90, 135, 180, np.inf]
 
-#     left_turns = (left_rotate['time'].diff() > 0.5).sum()
-#     left_turns_pm = (left_turns / (len(movement) / 100)) * 60
-#     right_turns = (right_rotate['time'].diff() > 0.5).sum()
-#     right_turns_pm = (right_turns / (len(movement) / 100)) * 60
+    for zone, zone2 in zip(zones, zones2):
+        zone_ind = ((rotate['rot_vel'] >= zone) & (rotate['rot_vel'] < zone2))
+        move_zone = rotate[zone_ind]
+        if zone_ind is not None:
+            per_rot_vel_zone = (len(move_zone) / len(move) * 100)
+            frame_dist = cumtrapz(move_zone['vel'], initial=0.0) / 52
+            disp_rot_vel_zone = (max(abs(frame_dist)))
+            freq_rot_vel_zone = ((move_zone['time'].diff() > 0.1).sum())
+        else:
+            per_rot_vel_zone = 0
+            disp_rot_vel_zone = 0
+            freq_rot_vel_zone = 0
+
+        outcomes = pd.DataFrame([[per_rot_vel_zone, disp_rot_vel_zone, freq_rot_vel_zone]],
+                                columns=['per_rot_vel_zone', 'disp_rot_vel_zone', 'freq_rot_vel_zone'],
+                                index=[str(round(zone, 2)) + ' - ' + str(round(zone2, 2))])
+        rot_vel_zone_outcomes = pd.concat([rot_vel_zone_outcomes, outcomes])
+    rot_vel_zone_outcomes = round(rot_vel_zone_outcomes, 2)
 
-#     return left_turns, right_turns
+    return rot_vel_zone_outcomes
 
 # def key_var(sessiondata):
 #     """
 #     Calculate key variables of a wheelchair tennis match, based on study:
 #     ...
 #
 #     Parameters
@@ -354,21 +423,14 @@
 #     # Cut the dataset in forward and reverse velocity
 #     forward = sessiondata['frame'][(sessiondata['frame']['vel']) > 0.1].reset_index(drop=True)
 #     reverse = sessiondata['frame'][(sessiondata['frame']['vel']) < -0.1].reset_index(drop=True)
 #
 #     mean_vel = np.mean(forward['vel'])
 #     peak_vel = np.max(forward['vel'])
 #
-#     lsa = forward[forward['vel'] < 1]
-#     lsa_per = len(lsa) / len(forward) * 100
-#     msa = forward[(forward['vel'] > 1) & (forward['vel'] < 2)]
-#     msa_per = len(msa) / len(forward) * 100
-#     hsa = forward[forward['vel'] > 2]
-#     hsa_per = len(hsa) / len(forward) * 100
-#
 #     n_hsa = (hsa['time'].diff() > 2).sum()
 #     n_hsa_pm = (n_hsa / ((len(forward) + len(reverse)) / 100)) * 60
 #
 #     peaks, _ = find_peaks(forward['vel'], height=2.5, width=100, distance=100)
 #     vel_peaks = forward['vel'][peaks]
 #     vel_peaks = vel_peaks.sort_values(ascending=False)
 #     mean_vel_best5 = np.mean(vel_peaks.head(5))
@@ -377,15 +439,11 @@
 #     peak_rev_vel = -np.min(reverse['vel'])
 #
 #     outcomes_vel = pd.DataFrame([])
 #     outcomes_vel = outcomes_vel.append([{'rot_vel_curve': mean_vel,
 #                                          'mean_best_5_vel': mean_vel_best5,
 #                                          'rot_vel_turn': mean_rev_vel,
 #                                          'num_high_speed_activations_pm': n_hsa_pm,
-#
 #                                          'rev_vel_peak': peak_rev_vel,
-#                                          'per_low_speed_zone': lsa_per,
-#                                          'per_mid_speed_zone': msa_per,
-#                                          'per_high_speed_zone': hsa_per,
 #                                          'num_high_speed_activations_pm': n_hsa_pm,
 #                                          }], ignore_index=True)
 #     return outcomes_vel
```

### Comparing `wheeltennis-1.1.5/wheeltennis/plots.py` & `wheeltennis-1.1.6/wheeltennis/plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,157 +1,145 @@
 import numpy as np
-from scipy.integrate import cumtrapz
-from worklab.utils import lowpass_butter
 from worklab.imu import push_imu
 import matplotlib.pyplot as plt
 from scipy.signal import find_peaks
+import seaborn as sns
 
 
 def peaks_plot(sessiondata, name=''):
     """
-    Plot peaks  plot
+    Plot peaks velocity and rotational velocity
 
     Parameters
     ----------
     sessiondata : str
         processed sessiondata structure
     name : str
         name of a session
 
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
 
-    move = sessiondata['frame'][(sessiondata['frame'][vel] < -0.1) | (sessiondata['frame'][vel] > 0.1)].reset_index(
-        drop=True)
+    move = sessiondata['frame'][(sessiondata['frame']["vel"] < -0.1) | (sessiondata['frame']["vel"] > 0.1)].reset_index(drop=True)
     rotate = move[abs(move['rot_vel']) > 10].reset_index(drop=True)
-    forward = sessiondata['frame'][(sessiondata['frame'][vel]) > 0.1].reset_index(drop=True)
+    forward = sessiondata['frame'][(sessiondata['frame']["vel"]) > 0.1].reset_index(drop=True)
 
     fig, [ax1, ax2] = plt.subplots(2, 1, figsize=[14, 10])
-    ax1.plot(forward['time'], forward[vel])
-    peaks, properties = find_peaks(forward[vel], prominence=0.5, distance=50, width=50, height=2)
-    ax1.plot(forward['time'][peaks], forward[vel][peaks], 'k.')
+    ax1.plot(forward['time'], forward["vel"])
+    peaks, properties = find_peaks(forward["vel"], prominence=0.5, distance=50,
+                                   width=50, height=2)
+    ax1.plot(forward['time'][peaks], forward["vel"][peaks], 'k.')
     ax1.set_ylabel("Velocity [m/s]", fontsize=10)
     ax1.tick_params(axis='y', labelsize=10)
     ax1.tick_params(axis='x', labelsize=10)
     ax1.set_title(f"{name} Velocity with peaks")
 
     ax2.plot(rotate['time'], rotate['rot_vel'])
-    peaks2, _ = find_peaks(rotate['rot_vel'], prominence=50, height=90, width=20, distance=50)
-    peaks3, _ = find_peaks(-rotate['rot_vel'], prominence=50, height=90, width=20, distance=50)
+    peaks2, _ = find_peaks(rotate['rot_vel'], prominence=50, height=90,
+                           width=20, distance=50)
+    peaks3, _ = find_peaks(-rotate['rot_vel'], prominence=50, height=90,
+                           width=20, distance=50)
     ax2.plot(rotate['time'][peaks2], rotate['rot_vel'][peaks2], 'k.')
     ax2.plot(rotate['time'][peaks3], rotate['rot_vel'][peaks3], 'k.')
     ax2.set_xlabel("Time [s]", fontsize=10)
     ax2.set_ylabel("Rotational velocity [deg/s]", fontsize=10)
     ax2.tick_params(axis='y', labelsize=10)
     ax2.tick_params(axis='x', labelsize=10)
     ax2.set_title(f"{name} Rotational velocity with peaks")
 
     return fig, ax1, ax2
 
 
 def peaks_rot_vel_plot(sessiondata, side: bool = True):
     """
-    Plot peaks  plot
+    Plot peaks rotational velocity
 
     Parameters
     ----------
     sessiondata : str
         processed sessiondata structure
     side : bool
         if set to True left side is analysed
         if set to False right side is analysed
 
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
     # Cut the dataset in part where there was movement
-    move = sessiondata['frame'][(sessiondata['frame'][vel] < -0.1) | (sessiondata['frame'][vel] > 0.1)].reset_index(
+    move = sessiondata['frame'][(sessiondata['frame']["vel"] < -0.1) | (sessiondata['frame']["vel"] > 0.1)].reset_index(
         drop=True)
 
     if side is True:  # left
         rotate = move[move['rot_vel'] > 10].reset_index(drop=True)
     else:  # right
         rotate = move[move['rot_vel'] < -10].reset_index(drop=True)
         rotate['rot_vel'] = -rotate['rot_vel']
 
-    turn1 = rotate[(rotate[vel] > -0.5) & (rotate[vel] < 0.5)].reset_index(drop=True)
-    turn2 = rotate[(rotate[vel] > -1.5) & (rotate[vel] < 1.5)].reset_index(drop=True)
-    curve1 = rotate[(rotate[vel] > 1) & (rotate[vel] < 2)].reset_index(drop=True)
-    curve2 = rotate[rotate[vel] > 1.5].reset_index(drop=True)
+    turn1 = rotate[(rotate["vel"] > -0.5) & (rotate["vel"] < 0.5)].reset_index(drop=True)
+    turn2 = rotate[(rotate["vel"] > -1.5) & (rotate["vel"] < 1.5)].reset_index(drop=True)
+    curve1 = rotate[(rotate["vel"] > 1) & (rotate["vel"] < 2)].reset_index(drop=True)
+    curve2 = rotate[rotate["vel"] > 1.5].reset_index(drop=True)
 
     moves = [turn1, turn2, curve1, curve2]
     moves_keys = ['turn1', 'turn2', 'curve1', 'curve2']
     fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(2, 2, figsize=[14, 10])
     axes = [ax1, ax2, ax3, ax4]
     for movement, keys, axi in zip(moves, moves_keys, axes):
-        peaks, _ = find_peaks(movement['rot_vel'], prominence=50, height=90, width=20, distance=50)
+        peaks, _ = find_peaks(movement['rot_vel'], prominence=50, height=90,
+                              width=20, distance=50)
         axi.plot(movement['time'], movement['rot_vel'])
         axi.plot(movement['time'][peaks], movement['rot_vel'][peaks], 'k.')
         axi.set_ylabel("Rotational velocity [deg/s]", fontsize=10)
         axi.set_title(keys)
 
     return fig, ax1, ax2, ax3, ax4
 
 
 def straight_sprint_plot(data, name=''):
     """
-    Plot straight sprint plot
+    Plot straight sprint
 
     Parameters
     ----------
     data : pd.Series
         processed sprint pd.Series
     name : str
         name of a session
 
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
 
-    vel = data[vel]
-    time = data['time']
-    dist = data['dist']
-    rot_vel = data['rot_vel']
-
-    sfreq = 1 / time.diff().mean()
-
-    # Determine distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
+    vel = data["vel"]
+    dist_x = data['dist_x']
+    dist_y = data['dist_y']
 
     # Calculate vel_peak and position of vel_peak
     y_max_vel = vel.idxmax()
     y_max_vel_value = np.max(vel)
 
     # Define vel zones
     vel_sin_2 = dist_y[vel > 2]
     vel_cos_2 = dist_x[vel > 2]
     vel_sin_3 = dist_y[vel > 3]
     vel_cos_3 = dist_x[vel > 3]
     vel_sin_4 = dist_y[vel > 4]
     vel_cos_4 = dist_x[vel > 4]
 
     # Create straight sprint figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, ax = plt.subplots(1, 1, figsize=[10, 6])
-    ax.set_xlim(-10, 10)
+    ax.set_xlim(-6, 6)
     ax.set_ylim(0, max(dist_x) + 1)
     ax.plot(-dist_y, dist_x)
     ax.plot(-vel_sin_2, vel_cos_2, 'y.', markersize=5,
             label='vel > 2 m/s')
     ax.plot(-vel_sin_3, vel_cos_3, 'g.', markersize=8,
             label='vel > 3 m/s')
     ax.plot(-vel_sin_4, vel_cos_4, 'r.', markersize=14,
@@ -159,77 +147,66 @@
     ax.plot(-dist_y[y_max_vel],
             dist_x[y_max_vel], 'ko', markersize=10,
             label='$vel_{peak}$: ' + str(round(y_max_vel_value, 2)) + ' m/s')
     ax.set_xlabel("Distance [m]", fontsize=12)
     ax.set_ylabel("Distance [m]", fontsize=12)
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
-    ax.set_title(f"{name} Sprint test")
-    ax.legend()
+    ax.set_title(f"{name}")
+    ax.legend(loc='upper left', prop={'size': 10})
 
     return ax
 
 
 def overview_sprint_plot(data, name=''):
     """
-    Plot overview straight sprint test
+    Plot overview straight sprint
 
     Parameters
     ----------
     data : pd.Series
         processed sprint pd.Series
     name : str
         name of a session
 
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
 
-    vel = data[vel]
+    vel = data["vel"]
+    acc = data['acc']
     time = data['time']
     dist = data['dist']
-    rot_vel = data['rot_vel']
+    dist_x = data['dist_x']
+    dist_y = data['dist_y']
 
     sfreq = 1 / time.diff().mean()
 
-    # Calculate processed acceleration from velocity
-    acc_raw = data['accelerometer_x']
-    acc = lowpass_butter(data['accelerometer_x'], sfreq=sfreq, cutoff=20)
-
     # Calculate push detection with function
-    push_idx, acc_filt, n_pushes, cycle_time, push_freq = push_imu(acc_raw, sfreq)
-
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
+    push_idx, acc_filt, n_pushes, cycle_time, push_freq = push_imu(acc, sfreq)
 
     # Calculate vel zones, vel_peak and acc_peak
     y_max_vel = vel.idxmax()
     y_max_acc = acc.argmax()
     y_max_vel_value = np.max(vel)
     y_max_acc_value = np.max(acc)
     vel_sin_2 = dist_y[vel > 2]
     vel_cos_2 = dist_x[vel > 2]
     vel_sin_3 = dist_y[vel > 3]
     vel_cos_3 = dist_x[vel > 3]
     vel_sin_4 = dist_y[vel > 4]
     vel_cos_4 = dist_x[vel > 4]
 
     # Create time vs. velocity with push detection figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(2, 2, figsize=[14, 10])
     fig.subplots_adjust(hspace=0.3, wspace=0.3)
-    fig.suptitle(f"{name} Overview Sprint test")
+    fig.suptitle(f"{name} Overview")
     ax1.set_ylim(-6, 6)
     ax1.plot(time, vel, 'r')
     ax1.plot(time[push_idx], vel[push_idx], 'k.')
     ax1.set_xlabel("Time [s]", fontsize=10)
     ax1.set_ylabel("Velocity [m/s]", fontsize=10)
     ax1.tick_params(axis='y', colors='r', labelsize=10)
     ax1.tick_params(axis='x', labelsize=10)
@@ -253,15 +230,15 @@
     ax2.plot(time[y_max_vel], vel[y_max_vel], 'k.',
              label='Vel$_{peak}$: ' + str(round(y_max_vel_value, 2)) + ' m/s')
     ax2.set_xlabel("Time [s]", fontsize=10)
     ax2.set_ylabel("Velocity [m/s]", fontsize=10)
     ax2.tick_params(axis='y', colors='r', labelsize=10)
     ax2.tick_params(axis='x', labelsize=10)
     ax2.yaxis.label.set_color('r')
-    ax2.legend(loc='lower right', prop={'size': 10})
+    ax2.legend(loc='lower right', prop={'size': 8})
     ax2.autoscale(axis='x', tight=True)
 
     # Create time vs. distance figure
     ax6 = ax2.twinx()
     ax6.set_ylim(0, max(dist) + 1)
     ax6.plot(time, dist)
     ax6.plot(time[y_max_vel], dist[y_max_vel], 'k.')
@@ -276,15 +253,15 @@
     ax3.plot(time[y_max_acc], acc[y_max_acc], 'k.',
              label='Acc$_{peak}$: ' + str(round(y_max_acc_value, 2)) + ' m/$s^2$')
     ax3.set_xlabel("Time [s]", fontsize=10)
     ax3.set_ylabel("Acceleration [m/$s^2$]", fontsize=10)
     ax3.tick_params(axis='y', colors='g', labelsize=10)
     ax3.tick_params(axis='x', labelsize=10)
     ax3.yaxis.label.set_color('g')
-    ax3.legend(loc='lower center', prop={'size': 10})
+    ax3.legend(loc='lower center', prop={'size': 8})
     ax3.autoscale(axis='x', tight=True)
 
     # Create time vs. distance figure
     ax7 = ax3.twinx()
     ax7.set_ylim(0, max(dist) + 1)
     ax7.plot(time, dist)
     ax7.plot(time[y_max_acc], dist[y_max_acc], 'k.')
@@ -292,16 +269,16 @@
     ax7.tick_params(axis='y', colors='b', labelsize=10)
     ax7.yaxis.label.set_color('b')
     ax3.autoscale(axis='x', tight=True)
 
     # Create Straight sprint figure with vel zones and vel_peak
     ax4.set_xlim(-10, 10)
     ax4.set_ylim(0, max(dist_x) + 1)
-    # ax4.text(3, max(dist)-2, 'Endtime: ' + str(round(len(time) / sfreq, 2)) +'s',
-    #          bbox=dict(facecolor='green', alpha=0.5))
+    ax4.text(3, max(dist) - 2, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
+             bbox=dict(facecolor='green', alpha=0.5))
     ax4.plot(-dist_y, dist_x)
     ax4.plot(-vel_sin_2, vel_cos_2, 'y.', markersize=5,
              label='Vel > 2 m/s')
     ax4.plot(-vel_sin_3, vel_cos_3, 'g.', markersize=8,
              label='Vel > 3 m/s')
     ax4.plot(-vel_sin_4, vel_cos_4, 'r.', markersize=14,
              label='Vel > 4 m/s')
@@ -313,66 +290,53 @@
     ax4.tick_params(axis='y', labelsize=10)
     ax4.tick_params(axis='x', labelsize=10)
     ax4.legend(loc='upper left', prop={'size': 8})
 
     return ax1, ax2, ax3, ax4, ax5, ax6, ax7
 
 
-def butterfly_plot(data, name='', mirror=False):
+def butterfly_plot(data, name=''):
     """
     Plot butterfly sprint test
 
     Parameters
     ----------
     data : pd.Series
         processed butterfly pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
 
     Returns
     -------
     ax: axis object
 
     """
     time = data['time']
-    dist = data['dist']
     rot_vel = data['rot_vel']
+    dist_y = data['dist_y']
+    dist_x = data['dist_x']
 
     sfreq = 1 / time.diff().mean()
-    # Determine distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_y = -dist_y
-        dist_x = -dist_x
 
-    # Caculate rotational vel zones and rot_vel_peak, rot_acc_peak
+    # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
 
     # Create butterfly sprint figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, ax = plt.subplots(1, 1, figsize=[10, 6])
     ax.text(2, 7, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
             bbox=dict(facecolor='green', alpha=0.5))
     ax.plot(dist_x, dist_y)
     ax.plot(rot_vel_x_45, rot_vel_y_45, 'y.', markersize=5,
             label='Rot vel > 45 deg/s')
     ax.plot(rot_vel_x_90, rot_vel_y_90, 'g.', markersize=8,
@@ -385,85 +349,69 @@
     ax.plot(dist_x[y_max_rot_acc],
             dist_y[y_max_rot_acc], 'k*', markersize=10,
             label='Rot acc$_{peak}:$ ' + str(int(y_max_rot_acc_value)) + ' deg/$s^2$')
     ax.set_xlabel("Distance [m]", fontsize=12)
     ax.set_ylabel("Distance [m]", fontsize=12)
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
-    ax.set_title(f"{name} Butterfly test")
+    ax.set_title(f"{name}")
     ax.legend(loc='upper left', prop={'size': 10})
 
     return ax
 
 
-def overview_butterfly_plot(data, name='', mirror=False):
+def overview_butterfly_plot(data, name=''):
     """
     Plot butterfly sprint test overview
 
     Parameters
     ----------
     data : pd.Series
         processed butterfly pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
+
     Returns
     -------
     ax: axis object
 
     """
     vel = "vel"
 
     vel = data[vel]
     time = data['time']
-    dist = data['dist']
     rot_vel = data['rot_vel']
-
+    dist_x = data['dist_x']
+    dist_y = data['dist_y']
+    acc = data['acc']
     sfreq = 1 / time.diff().mean()
 
-    # Calculate processed acceleration from velocity
-    acc = lowpass_butter(np.gradient(vel) * sfreq, sfreq=sfreq, cutoff=10)
-
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_y = -dist_y
-        dist_x = -dist_x
-
-    # Caculate rotational vel zones and rot_vel_peak, rot_acc_peak
+    # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
     y_max_vel = vel.idxmax()
     y_max_acc = acc.argmax()
     y_max_vel_value = np.max(vel)
     y_max_acc_value = np.max(acc)
 
     # Create time vs. rotational velocity figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(2, 2, figsize=[14, 10])
     fig.subplots_adjust(hspace=0.3, wspace=0.3)
-    fig.suptitle(f"{name} Overview Butterfly test")
+    fig.suptitle(f"{name} Overview")
     ax1.set_ylim(np.min(rot_vel) - 10, np.max(rot_vel) + 10)
     ax1.plot(time, rot_vel, 'b')
     ax1.set_xlabel("Time [s]", fontsize=10)
     ax1.set_ylabel("Rotational velocity [deg/s]", fontsize=10)
     ax1.tick_params(axis='y', colors='b', labelsize=10)
     ax1.tick_params(axis='x', labelsize=10)
     ax1.yaxis.label.set_color('b')
@@ -475,28 +423,29 @@
     ax2.plot(time[y_max_vel], vel[y_max_vel], 'k.',
              label='Vel$_{peak}$: ' + str(round(y_max_vel_value, 2)) + ' m/s')
     ax2.set_xlabel("Time [s]", fontsize=10)
     ax2.set_ylabel("Velocity [m/s]", fontsize=10)
     ax2.tick_params(axis='y', colors='r', labelsize=10)
     ax2.tick_params(axis='x', labelsize=10)
     ax2.yaxis.label.set_color('r')
-    ax2.legend()
+    ax2.legend(loc='lower right', prop={'size': 8})
     ax2.autoscale(axis='x', tight=True)
 
     # Create time vs. acceleration figure with acc_peak
     ax3.set_ylim(np.min(acc) - 1, y_max_acc_value + 1)
     ax3.plot(time, acc, 'g')
     ax3.plot(time[y_max_acc], acc[y_max_acc], 'k.',
              label='Acc$_{peak}$: ' + str(round(y_max_acc_value, 2)) + ' m/$s^2$')
     ax3.set_xlabel("Time [s]", fontsize=10)
     ax3.set_ylabel("Acceleration [m/$s^2$]", fontsize=10)
     ax3.tick_params(axis='y', colors='g', labelsize=10)
     ax3.tick_params(axis='x', labelsize=10)
     ax3.yaxis.label.set_color('g')
-    ax3.legend()
+    ax3.legend(loc='lower center', prop={'size': 8})
+    ax3.autoscale(axis='x', tight=True)
 
     # Create butterfly sprint figure
     ax4.plot(dist_x, dist_y)
     ax4.text(2, 7, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
              bbox=dict(facecolor='green', alpha=0.5))
     ax4.plot(rot_vel_x_45, rot_vel_y_45, 'y.', markersize=6,
              label='Rot vel > 45 deg/s')
@@ -515,74 +464,56 @@
     ax4.tick_params(axis='y', labelsize=10)
     ax4.tick_params(axis='x', labelsize=10)
     ax4.legend(loc='upper left', prop={'size': 8})
 
     return ax1, ax2, ax3, ax4
 
 
-def spider_plot(data, name='', mirror=False):
+def spider_plot(data, name=''):
     """
     Plot spider test
 
     Parameters
     ----------
     data : pd.Series
         processed spider pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
 
     Returns
     -------
     ax: axis object
 
     """
     time = data['time']
-    dist = data['dist']
     rot_vel = data['rot_vel']
+    dist_y = data['dist_y']
+    dist_x = data['dist_x']
 
     sfreq = 1 / time.diff().mean()
 
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_x = -dist_x
-        dist_y = -dist_y
-
-    # Caculate rotational vel zones and rot_vel_peak, rot_acc_peak
+    # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
 
     # Create Spider figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, ax = plt.subplots(1, 1, figsize=[10, 6])
-    if mirror is True:
-        ax.text(0.8, 3.1, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
-                bbox=dict(facecolor='green', alpha=0.5))
-    else:
-        ax.text(2.7, 3.1, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
-                bbox=dict(facecolor='green', alpha=0.5))
+    ax.text(-min(dist_x)-0.8, -min(dist_y)+0.5, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
+            bbox=dict(facecolor='green', alpha=0.5))
     ax.plot(-dist_x, -dist_y)
     ax.plot(-rot_vel_x_45, -rot_vel_y_45, 'y.', markersize=5,
             label='Rot vel > 45 deg/s')
     ax.plot(-rot_vel_x_90, -rot_vel_y_90, 'g.', markersize=8,
             label='Rot vel > 90 deg/s')
     ax.plot(-rot_vel_x_180, -rot_vel_y_180, 'r.', markersize=14,
             label='Rot vel > 180 deg/s')
@@ -592,85 +523,69 @@
     ax.plot(-dist_x[y_max_rot_acc],
             -dist_y[y_max_rot_acc], 'k*', markersize=10,
             label='Rot acc$_{peak}:$ ' + str(int(y_max_rot_acc_value)) + ' deg/s$^{2}$')
     ax.set_xlabel("Distance [m]", fontsize=12)
     ax.set_ylabel("Distance [m]", fontsize=12)
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
-    ax.set_title(f"{name} Spider test")
+    ax.set_title(f"{name}")
     ax.legend(loc='upper left', prop={'size': 10})
 
     return ax
 
 
-def overview_spider_plot(data, name='', mirror=False):
+def overview_spider_plot(data, name=''):
     """
-    Plot spider test
+    Plot overview spider test
 
     Parameters
     ----------
     data : pd.Series
         processed spider pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
+
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
 
-    vel = data[vel]
+    vel = data["vel"]
+    acc = data["acc"]
     time = data['time']
-    dist = data['dist']
     rot_vel = data['rot_vel']
+    dist_y = data['dist_y']
+    dist_x = data['dist_x']
 
     sfreq = 1 / time.diff().mean()
 
-    # Calculate processed acceleration from velocity
-    acc = lowpass_butter(np.gradient(vel) * sfreq, sfreq=sfreq, cutoff=10)
-
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_x = -dist_x
-        dist_y = -dist_y
-
     # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
     y_max_vel = vel.idxmax()
     y_max_acc = acc.argmax()
     y_max_vel_value = np.max(vel)
     y_max_acc_value = np.max(acc)
 
     # Create time vs. rotational velocity figure
-    plt.style.use("seaborn-whitegrid")
+    sns.set_style('darkgrid')
     fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(2, 2, figsize=[14, 10])
     fig.subplots_adjust(hspace=0.3, wspace=0.3)
-    fig.suptitle(f"{name} Overview Spider test")
+    fig.suptitle(f"{name} Overview")
     ax1.set_ylim(np.min(rot_vel) - 10, np.max(rot_vel) + 10)
     ax1.plot(time, rot_vel, 'b')
     ax1.set_xlabel("Time [s]", fontsize=10)
     ax1.set_ylabel("Rotational velocity [deg/s]", fontsize=10)
     ax1.tick_params(axis='y', colors='b', labelsize=10)
     ax1.tick_params(axis='x', labelsize=10)
     ax1.yaxis.label.set_color('b')
@@ -695,21 +610,19 @@
     ax3.plot(time[y_max_acc], acc[y_max_acc], 'k.',
              label='Acc$_{peak}$: ' + str(round(y_max_acc_value, 2)) + ' m/$s^2$')
     ax3.set_xlabel("Time [s]", fontsize=10)
     ax3.set_ylabel("Acceleration [m/$s^2$]", fontsize=10)
     ax3.tick_params(axis='y', colors='g', labelsize=10)
     ax3.tick_params(axis='x', labelsize=10)
     ax3.yaxis.label.set_color('g')
-    ax3.legend(loc='lower center', prop={'size': 10})
+    ax3.legend(loc='lower center', prop={'size': 8})
     ax3.autoscale(axis='x', tight=True)
 
     # Create Spider figure
-    ax4.set_ylim(-0.5, 3)
-    ax4.set_xlim(-3, 2)
-    ax4.text(1, 3, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
+    ax4.text(-min(dist_x)-0.8, -min(dist_y)+0.5, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
              bbox=dict(facecolor='green', alpha=0.5))
     ax4.plot(-dist_x, -dist_y)
     ax4.plot(-rot_vel_x_45, -rot_vel_y_45, 'y.', markersize=5,
              label='rot_vel > 45 deg/s')
     ax4.plot(-rot_vel_x_90, -rot_vel_y_90, 'g.', markersize=8,
              label='rot_vel > 90 deg/s')
     ax4.plot(-rot_vel_x_180, -rot_vel_y_180, 'r.', markersize=14,
@@ -725,74 +638,57 @@
     ax4.tick_params(axis='y', labelsize=10)
     ax4.tick_params(axis='x', labelsize=10)
     ax4.legend(loc='upper left', prop={'size': 8})
 
     return ax1, ax2, ax3, ax4
 
 
-def illinois_plot(data, name='', mirror=False):
+def illinois_plot(data, name=''):
     """
     Plot illinois test
 
     Parameters
     ----------
     data : pd.Series
         processed illinois pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
 
     Returns
     -------
     ax: axis object
 
     """
     time = data['time']
-    dist = data['dist']
     rot_vel = data['rot_vel']
 
     sfreq = 1 / time.diff().mean()
 
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_x = -dist_x
-        dist_y = -dist_y
+    dist_x = data['dist_x']
+    dist_y = data['dist_y']
 
-    # Caculate rotational vel zones and rot_vel_peak, rot_acc_peak
+    # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
 
-    # Create Spider figure
-    plt.style.use("seaborn-darkgrid")
+    # Create Illinois figure
+    sns.set_style('darkgrid')
     fig, ax = plt.subplots(1, 1, figsize=[10, 6])
-    if mirror is True:
-        ax.text(0.8, 3.1, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
-                bbox=dict(facecolor='green', alpha=0.5))
-    else:
-        ax.text(2.7, 6, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
-                bbox=dict(facecolor='green', alpha=0.5))
+    ax.text(-min(dist_y)-1.2, max(dist_x)+1, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
+            bbox=dict(facecolor='green', alpha=0.5))
     ax.plot(-dist_y, dist_x)
     ax.plot(-rot_vel_y_45, rot_vel_x_45, 'y.', markersize=5,
             label='Rot vel > 45 deg/s')
     ax.plot(-rot_vel_y_90, rot_vel_x_90, 'g.', markersize=8,
             label='Rot vel > 90 deg/s')
     ax.plot(-rot_vel_y_180, rot_vel_x_180, 'r.', markersize=14,
             label='Rot vel > 180 deg/s')
@@ -802,85 +698,69 @@
     ax.plot(-dist_y[y_max_rot_acc],
             dist_x[y_max_rot_acc], 'k*', markersize=10,
             label='Rot acc$_{peak}:$ ' + str(int(y_max_rot_acc_value)) + ' deg/s$^{2}$')
     ax.set_xlabel("Distance [m]", fontsize=12)
     ax.set_ylabel("Distance [m]", fontsize=12)
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
-    ax.set_title(f"{name} Illinois test")
+    ax.set_title(f"{name}")
     ax.legend(loc='lower right', prop={'size': 10})
 
     return ax
 
 
-def overview_illinois_plot(data, name='', mirror=False):
+def overview_illinois_plot(data, name=''):
     """
-    Plot spider test
+    Plot overview illinois test
 
     Parameters
     ----------
     data : pd.Series
         processed illinois pd.Series
     name : str
         name of a session
-    mirror : bool
-        make true if test is executed in reversed order
+
     Returns
     -------
     ax: axis object
 
     """
-    vel = "vel"
 
-    vel = data[vel]
+    vel = data["vel"]
     time = data['time']
-    dist = data['dist']
+    acc = data['acc']
     rot_vel = data['rot_vel']
+    dist_x = data['dist_x']
+    dist_y = data['dist_y']
 
     sfreq = 1 / time.diff().mean()
 
-    # Calculate processed acceleration from velocity
-    acc = lowpass_butter(np.gradient(vel) * sfreq, sfreq=sfreq, cutoff=10)
-
-    # Calculate distance in x and y direction
-    dist_y = cumtrapz(
-        np.gradient(dist) * np.sin(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-    dist_x = cumtrapz(
-        np.gradient(dist) * np.cos(np.deg2rad(cumtrapz(rot_vel / sfreq, initial=0.0))),
-        initial=0.0)
-
-    # Change signal if test was executed in reversed order
-    if mirror is True:
-        dist_x = -dist_x
-        dist_y = -dist_y
-
     # Calculate rotational vel zones and rot_vel_peak, rot_acc_peak
     rot_vel.reset_index(inplace=True, drop=True)
     rot_vel_y_45 = dist_y[rot_vel.abs() > 45]
     rot_vel_x_45 = dist_x[rot_vel.abs() > 45]
     rot_vel_y_90 = dist_y[rot_vel.abs() > 90]
     rot_vel_x_90 = dist_x[rot_vel.abs() > 90]
     rot_vel_y_180 = dist_y[rot_vel.abs() > 180]
     rot_vel_x_180 = dist_x[rot_vel.abs() > 180]
     rot_acc = np.gradient(rot_vel) * sfreq
-    y_max_rot_vel = abs(rot_vel).idxmax()
+    y_max_rot_vel = rot_vel.idxmax()
     y_max_rot_acc = np.argmax(rot_acc)
-    y_max_rot_vel_value = np.max(abs(rot_vel))
+    y_max_rot_vel_value = np.max(rot_vel)
     y_max_rot_acc_value = np.max(rot_acc)
     y_max_vel = vel.idxmax()
     y_max_acc = acc.argmax()
     y_max_vel_value = np.max(vel)
     y_max_acc_value = np.max(acc)
 
     # Create time vs. rotational velocity figure
-    plt.style.use("seaborn-whitegrid")
+    sns.set_style('darkgrid')
     fig, [[ax1, ax2], [ax3, ax4]] = plt.subplots(2, 2, figsize=[14, 10])
     fig.subplots_adjust(hspace=0.3, wspace=0.3)
-    fig.suptitle(f"{name} Overview Illinois test")
+    fig.suptitle(f"{name}")
     ax1.set_ylim(np.min(rot_vel) - 10, np.max(rot_vel) + 10)
     ax1.plot(time, rot_vel, 'b')
     ax1.set_xlabel("Time [s]", fontsize=10)
     ax1.set_ylabel("Rotational velocity [deg/s]", fontsize=10)
     ax1.tick_params(axis='y', colors='b', labelsize=10)
     ax1.tick_params(axis='x', labelsize=10)
     ax1.yaxis.label.set_color('b')
@@ -905,19 +785,19 @@
     ax3.plot(time[y_max_acc], acc[y_max_acc], 'k.',
              label='Acc$_{peak}$: ' + str(round(y_max_acc_value, 2)) + ' m/$s^2$')
     ax3.set_xlabel("Time [s]", fontsize=10)
     ax3.set_ylabel("Acceleration [m/$s^2$]", fontsize=10)
     ax3.tick_params(axis='y', colors='g', labelsize=10)
     ax3.tick_params(axis='x', labelsize=10)
     ax3.yaxis.label.set_color('g')
-    ax3.legend(loc='lower center', prop={'size': 10})
+    ax3.legend(loc='lower center', prop={'size': 8})
     ax3.autoscale(axis='x', tight=True)
 
-    # Create Spider figure
-    ax4.text(2.7, 6, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
+    # Create Illinois figure
+    ax4.text(-min(dist_y)-1.2, max(dist_x)+1, 'Endtime: ' + str(round(len(time) / sfreq, 2)) + 's',
              bbox=dict(facecolor='green', alpha=0.5))
     ax4.plot(-dist_y, dist_x)
     ax4.plot(-rot_vel_y_45, rot_vel_x_45, 'y.', markersize=5,
              label='rot_vel > 45 deg/s')
     ax4.plot(-rot_vel_y_90, rot_vel_x_90, 'g.', markersize=8,
              label='rot_vel > 90 deg/s')
     ax4.plot(-rot_vel_y_180, rot_vel_x_180, 'r.', markersize=14,
@@ -933,63 +813,72 @@
     ax4.tick_params(axis='y', labelsize=10)
     ax4.tick_params(axis='x', labelsize=10)
     ax4.legend(loc='lower right', prop={'size': 8})
 
     return ax1, ax2, ax3, ax4
 
 
-def imu_push_plot(time, vel, acc_raw, name='', dec=False):
+def imu_push_plot(data, name='', dec=False, acc_frame=True):
     """
     Plot push detection with IMUs
 
     Parameters
     ----------
-    time : dict
-        time structure
-    vel : dict
-        velocity structure
-    acc_raw : dict
-        raw acceleration structure
+    data : dict or pd.Series
+        processed sessiondata structure or pd.Series with frame data
     name : str
         name of a session
     dec : boolean
         set to True if main deceleration should be found
+    acc_frame: boolean
+        default is True, acceleration from frame used
+        if changed to False, acceleration from velocity wheels is used
 
     Returns
     -------
     ax: axis object
 
     """
-    # Calculate push detection with function
+    if type(data) == dict:
+        data = data["frame"]
+    if acc_frame is False:
+        data['acc'] = data['acc_wheel']
+    time = data['time']
+    vel = data['vel']
+
     sfreq = 1 / time.diff().mean()
-    acc_raw = lowpass_butter(acc_raw, sfreq=sfreq, cutoff=20)
-    push_idx, acc_filt, n_pushes, cycle_time, push_freq = push_imu(acc_raw, sfreq)
+
+    # Calculate push detection with function
+    push_idx, acc_filt, n_pushes, cycle_time, push_freq = push_imu(data['acc'],
+                                                                   sfreq)
 
     # Change signal if the main deceleration values should be found
     if dec is True:
         acc_filt = -acc_filt
 
     # Create time vs. velocity with push detection figure
-    plt.style.use("seaborn-darkgrid")
+    sns.set_style('darkgrid')
     fig, ax1 = plt.subplots(1, 1, figsize=[10, 6])
     ax1.set_ylim(-6, 6)
     ax1.plot(time, vel, 'r')
     ax1.plot(time[push_idx], vel[push_idx], 'k.', markersize=10)
     ax1.set_xlabel("Time [s]", fontsize=12)
     ax1.set_ylabel("Velocity [m/s]", fontsize=12)
     ax1.tick_params(axis='y', colors='r', labelsize=12)
     ax1.tick_params(axis='x', labelsize=12)
     ax1.yaxis.label.set_color('r')
     ax1.set_title(f"{name} Push detection Sprint test")
 
     # Create time vs. acceleration with push detection figure
     ax2 = ax1.twinx()
     ax2.set_ylim(-30, 30)
-    ax2.plot(time, acc_raw, 'C7', alpha=0.5)
+    ax2.plot(time, data['acc'], 'C7', alpha=0.5)
     ax2.plot(time, acc_filt, 'b')
-    ax2.plot(time[push_idx], acc_filt[push_idx], 'k.', markersize=10, label="Detected push")
+    ax2.plot(time[push_idx], acc_filt[push_idx], 'k.', markersize=10,
+             label="Detected push")
     ax2.set_ylabel("Acceleration [m/$s^2$]", fontsize=12)
     ax2.tick_params(axis='y', colors='b', labelsize=12)
     ax2.yaxis.label.set_color('b')
     ax2.legend(frameon=True, loc='lower right')
 
     return ax1, ax2
+
```

### Comparing `wheeltennis-1.1.5/wheeltennis.egg-info/PKG-INFO` & `wheeltennis-1.1.6/wheeltennis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeltennis
-Version: 1.1.5
+Version: 1.1.6
 Summary: Basic scripts for wheelchair tennis analysis
 Home-page: https://gitlab.com/Thomas2016/wheeltennis
 Download-URL: https://gitlab.com/Thomas2016/wheeltennis
 Author: Thomas Rietveld
 Author-email: t.rietveld@lboro.ac.uk
 License: GNU GPLv3
 Keywords: wheelchair tennis,sensor,IMUs
```

