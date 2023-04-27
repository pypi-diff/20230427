# Comparing `tmp/pose2sim-0.3.5.tar.gz` & `tmp/pose2sim-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pose2sim-0.3.5.tar", last modified: Thu Apr  6 11:52:34 2023, max compression
+gzip compressed data, was "pose2sim-0.3.6.tar", last modified: Thu Apr 27 09:08:25 2023, max compression
```

## Comparing `pose2sim-0.3.5.tar` & `pose2sim-0.3.6.tar`

### file list

```diff
@@ -1,698 +1,702 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.414062 pose2sim-0.3.5/
--rw-rw-rw-   0        0        0     1550 2023-02-05 04:03:13.000000 pose2sim-0.3.5/LICENSE
--rw-rw-rw-   0        0        0    33171 2023-04-06 11:52:34.414062 pose2sim-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.884736 pose2sim-0.3.5/Pose2Sim/
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.884736 pose2sim-0.3.5/Pose2Sim/Demo/
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.900363 pose2sim-0.3.5/Pose2Sim/Demo/User/
--rw-rw-rw-   0        0        0     2979 2023-02-05 10:45:27.000000 pose2sim-0.3.5/Pose2Sim/Demo/User/Config.toml
--rw-rw-rw-   0        0        0    14037 2023-04-06 11:13:02.000000 pose2sim-0.3.5/Pose2Sim/Demo/User/logs.txt
--rw-rw-rw-   0        0        0     2866 2023-04-06 11:51:08.000000 pose2sim-0.3.5/Pose2Sim/Demo/User/test.toml
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.900363 pose2sim-0.3.5/Pose2Sim/Demo/__pycache__/
--rw-rw-rw-   0        0        0      467 2023-04-06 11:06:55.000000 pose2sim-0.3.5/Pose2Sim/Demo/__pycache__/test.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.900363 pose2sim-0.3.5/Pose2Sim/Demo/calib-2d/
--rw-rw-rw-   0        0        0     4881 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/calib-2d/Calib.qca.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.900363 pose2sim-0.3.5/Pose2Sim/Demo/opensim/
--rw-rw-rw-   0        0        0   127394 2023-04-06 10:53:50.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Balancing_for_IK.trc
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.978486 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/
--rw-rw-rw-   0        0        0    90719 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp
--rw-rw-rw-   0        0        0    10273 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp
--rw-rw-rw-   0        0        0    10274 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp
--rw-rw-rw-   0        0        0    30752 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp
--rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp
--rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp
--rw-rw-rw-   0        0        0    13858 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp
--rw-rw-rw-   0        0        0    13861 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp
--rw-rw-rw-   0        0        0   100947 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/foot.vtp
--rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp
--rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp
--rw-rw-rw-   0        0        0   142705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp
--rw-rw-rw-   0        0        0   749317 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp
--rw-rw-rw-   0        0        0   326089 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp
--rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp
--rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp
--rw-rw-rw-   0        0        0    14416 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp
--rw-rw-rw-   0        0        0    14419 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp
--rw-rw-rw-   0        0        0    15215 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp
--rw-rw-rw-   0        0        0    15214 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp
--rw-rw-rw-   0        0        0    13148 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    13149 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    91325 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp
--rw-rw-rw-   0        0        0   100995 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp
--rw-rw-rw-   0        0        0     7066 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp
--rw-rw-rw-   0        0        0    13913 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp
--rw-rw-rw-   0        0        0    18108 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp
--rw-rw-rw-   0        0        0    18114 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp
--rw-rw-rw-   0        0        0    13625 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp
--rw-rw-rw-   0        0        0    13621 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp
--rw-rw-rw-   0        0        0    15563 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    15562 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp
--rw-rw-rw-   0        0        0     7900 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp
--rw-rw-rw-   0        0        0     7897 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp
--rw-rw-rw-   0        0        0    33931 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp
--rw-rw-rw-   0        0        0    33928 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp
--rw-rw-rw-   0        0        0    25886 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp
--rw-rw-rw-   0        0        0    25890 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp
--rw-rw-rw-   0        0        0    36718 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp
--rw-rw-rw-   0        0        0    36716 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp
--rw-rw-rw-   0        0        0    39943 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp
--rw-rw-rw-   0        0        0    39937 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp
--rw-rw-rw-   0        0        0    44236 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp
--rw-rw-rw-   0        0        0    44228 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp
--rw-rw-rw-   0        0        0    16127 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp
--rw-rw-rw-   0        0        0    16128 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp
--rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp
--rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp
--rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp
--rw-rw-rw-   0        0        0     4228 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp
--rw-rw-rw-   0        0        0     4229 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp
--rw-rw-rw-   0        0        0     7324 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp
--rw-rw-rw-   0        0        0    14125 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp
--rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp
--rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp
--rw-rw-rw-   0        0        0    14184 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp
--rw-rw-rw-   0        0        0    14187 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp
--rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp
--rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp
--rw-rw-rw-   0        0        0    14990 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    14991 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    18621 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp
--rw-rw-rw-   0        0        0     8432 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp
--rw-rw-rw-   0        0        0     8434 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp
--rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp
--rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp
--rw-rw-rw-   0        0        0    19781 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp
--rw-rw-rw-   0        0        0    19782 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp
--rw-rw-rw-   0        0        0    16243 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    16246 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    16483 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp
--rw-rw-rw-   0        0        0    16479 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp
--rw-rw-rw-   0        0        0    11920 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp
--rw-rw-rw-   0        0        0    11919 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp
--rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp
--rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp
--rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp
--rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp
--rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp
--rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp
--rw-rw-rw-   0        0        0     9630 2023-04-06 10:53:50.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml
--rw-rw-rw-   0        0        0   460246 2023-02-05 10:45:27.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim
--rw-rw-rw-   0        0        0    31130 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
--rw-rw-rw-   0        0        0    32363 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.853523 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.040990 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/
--rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json
--rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json
--rw-rw-rw-   0        0        0     1648 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json
--rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json
--rw-rw-rw-   0        0        0     1648 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json
--rw-rw-rw-   0        0        0     1677 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json
--rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json
--rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json
--rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json
--rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json
--rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json
--rw-rw-rw-   0        0        0     1629 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json
--rw-rw-rw-   0        0        0     1657 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json
--rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json
--rw-rw-rw-   0        0        0     1661 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json
--rw-rw-rw-   0        0        0     1647 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json
--rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json
--rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json
--rw-rw-rw-   0        0        0     1650 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json
--rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json
--rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json
--rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json
--rw-rw-rw-   0        0        0     1645 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json
--rw-rw-rw-   0        0        0     1658 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json
--rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json
--rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json
--rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json
--rw-rw-rw-   0        0        0     1655 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json
--rw-rw-rw-   0        0        0     2046 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json
--rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json
--rw-rw-rw-   0        0        0     1645 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json
--rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json
--rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json
--rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json
--rw-rw-rw-   0        0        0     1608 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json
--rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json
--rw-rw-rw-   0        0        0     1640 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json
--rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json
--rw-rw-rw-   0        0        0     1626 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json
--rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json
--rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json
--rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json
--rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json
--rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json
--rw-rw-rw-   0        0        0     1620 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json
--rw-rw-rw-   0        0        0     1619 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json
--rw-rw-rw-   0        0        0     1637 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json
--rw-rw-rw-   0        0        0     1627 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json
--rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json
--rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json
--rw-rw-rw-   0        0        0     1627 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json
--rw-rw-rw-   0        0        0     1621 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json
--rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json
--rw-rw-rw-   0        0        0     1639 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json
--rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json
--rw-rw-rw-   0        0        0     1608 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json
--rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json
--rw-rw-rw-   0        0        0     1629 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json
--rw-rw-rw-   0        0        0     1655 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json
--rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json
--rw-rw-rw-   0        0        0     1613 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json
--rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json
--rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json
--rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json
--rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json
--rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.119112 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/
--rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json
--rw-rw-rw-   0        0        0     1702 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json
--rw-rw-rw-   0        0        0     1710 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json
--rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json
--rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json
--rw-rw-rw-   0        0        0     1701 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json
--rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json
--rw-rw-rw-   0        0        0     1704 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json
--rw-rw-rw-   0        0        0     1698 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json
--rw-rw-rw-   0        0        0     1702 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json
--rw-rw-rw-   0        0        0     1714 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json
--rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json
--rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json
--rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json
--rw-rw-rw-   0        0        0     1701 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json
--rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json
--rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json
--rw-rw-rw-   0        0        0     1704 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json
--rw-rw-rw-   0        0        0     1711 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json
--rw-rw-rw-   0        0        0     1711 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json
--rw-rw-rw-   0        0        0     1710 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json
--rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json
--rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json
--rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json
--rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json
--rw-rw-rw-   0        0        0     1695 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json
--rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json
--rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json
--rw-rw-rw-   0        0        0     1639 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json
--rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json
--rw-rw-rw-   0        0        0     1671 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json
--rw-rw-rw-   0        0        0     1668 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json
--rw-rw-rw-   0        0        0     1670 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json
--rw-rw-rw-   0        0        0     1646 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json
--rw-rw-rw-   0        0        0     1673 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json
--rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json
--rw-rw-rw-   0        0        0     1665 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json
--rw-rw-rw-   0        0        0     1673 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json
--rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json
--rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json
--rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json
--rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json
--rw-rw-rw-   0        0        0     1646 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json
--rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json
--rw-rw-rw-   0        0        0     1662 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json
--rw-rw-rw-   0        0        0     1676 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json
--rw-rw-rw-   0        0        0     1677 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json
--rw-rw-rw-   0        0        0     1684 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json
--rw-rw-rw-   0        0        0     1687 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json
--rw-rw-rw-   0        0        0     1695 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json
--rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json
--rw-rw-rw-   0        0        0     1682 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json
--rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json
--rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json
--rw-rw-rw-   0        0        0     1694 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json
--rw-rw-rw-   0        0        0     1669 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json
--rw-rw-rw-   0        0        0     1671 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json
--rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json
--rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json
--rw-rw-rw-   0        0        0     1713 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json
--rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json
--rw-rw-rw-   0        0        0     1700 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json
--rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json
--rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json
--rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json
--rw-rw-rw-   0        0        0     1713 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json
--rw-rw-rw-   0        0        0     1672 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json
--rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json
--rw-rw-rw-   0        0        0     1672 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json
--rw-rw-rw-   0        0        0     1650 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json
--rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json
--rw-rw-rw-   0        0        0     1669 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json
--rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json
--rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json
--rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json
--rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json
--rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json
--rw-rw-rw-   0        0        0     1693 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json
--rw-rw-rw-   0        0        0     1683 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json
--rw-rw-rw-   0        0        0     1682 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json
--rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json
--rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json
--rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json
--rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json
--rw-rw-rw-   0        0        0     1677 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json
--rw-rw-rw-   0        0        0     1670 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.181612 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json
--rw-rw-rw-   0        0        0      841 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json
--rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json
--rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json
--rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json
--rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json
--rw-rw-rw-   0        0        0      831 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json
--rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json
--rw-rw-rw-   0        0        0      833 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json
--rw-rw-rw-   0        0        0      839 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json
--rw-rw-rw-   0        0        0      826 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json
--rw-rw-rw-   0        0        0      835 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json
--rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json
--rw-rw-rw-   0        0        0      828 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json
--rw-rw-rw-   0        0        0      856 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json
--rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json
--rw-rw-rw-   0        0        0      830 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json
--rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json
--rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json
--rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json
--rw-rw-rw-   0        0        0      855 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json
--rw-rw-rw-   0        0        0      856 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json
--rw-rw-rw-   0        0        0      825 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json
--rw-rw-rw-   0        0        0      839 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.259736 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json
--rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json
--rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json
--rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json
--rw-rw-rw-   0        0        0      827 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json
--rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json
--rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json
--rw-rw-rw-   0        0        0      808 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json
--rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json
--rw-rw-rw-   0        0        0      808 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json
--rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json
--rw-rw-rw-   0        0        0      790 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json
--rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json
--rw-rw-rw-   0        0        0      803 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json
--rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json
--rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json
--rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json
--rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json
--rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json
--rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json
--rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json
--rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json
--rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json
--rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json
--rw-rw-rw-   0        0        0      803 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json
--rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json
--rw-rw-rw-   0        0        0      833 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json
--rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json
--rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json
--rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json
--rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json
--rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json
--rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json
--rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json
--rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json
--rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json
--rw-rw-rw-   0        0        0      834 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json
--rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json
--rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json
--rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json
--rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json
--rw-rw-rw-   0        0        0      301 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Demo/test.py
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:33.869111 pose2sim-0.3.5/Pose2Sim/Empty_project/
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.259736 pose2sim-0.3.5/Pose2Sim/Empty_project/User/
--rw-rw-rw-   0        0        0     2987 2023-03-06 13:10:05.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/User/Config.toml
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.275361 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.353486 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/
--rw-rw-rw-   0        0        0    90719 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp
--rw-rw-rw-   0        0        0    10273 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp
--rw-rw-rw-   0        0        0    10274 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp
--rw-rw-rw-   0        0        0    30752 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp
--rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp
--rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp
--rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp
--rw-rw-rw-   0        0        0    13858 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp
--rw-rw-rw-   0        0        0    13861 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp
--rw-rw-rw-   0        0        0   100947 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp
--rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp
--rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp
--rw-rw-rw-   0        0        0   142705 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp
--rw-rw-rw-   0        0        0   749317 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp
--rw-rw-rw-   0        0        0   326089 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp
--rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp
--rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp
--rw-rw-rw-   0        0        0    14416 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp
--rw-rw-rw-   0        0        0    14419 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp
--rw-rw-rw-   0        0        0    15215 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp
--rw-rw-rw-   0        0        0    15214 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp
--rw-rw-rw-   0        0        0    13148 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    13149 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    91325 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp
--rw-rw-rw-   0        0        0   100995 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp
--rw-rw-rw-   0        0        0     7066 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp
--rw-rw-rw-   0        0        0    13913 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp
--rw-rw-rw-   0        0        0    18108 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp
--rw-rw-rw-   0        0        0    18114 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp
--rw-rw-rw-   0        0        0    13625 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp
--rw-rw-rw-   0        0        0    13621 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp
--rw-rw-rw-   0        0        0    15563 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    15562 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp
--rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp
--rw-rw-rw-   0        0        0     7900 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp
--rw-rw-rw-   0        0        0     7897 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp
--rw-rw-rw-   0        0        0    33931 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp
--rw-rw-rw-   0        0        0    33928 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp
--rw-rw-rw-   0        0        0    25886 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp
--rw-rw-rw-   0        0        0    25890 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp
--rw-rw-rw-   0        0        0    36718 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp
--rw-rw-rw-   0        0        0    36716 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp
--rw-rw-rw-   0        0        0    39943 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp
--rw-rw-rw-   0        0        0    39937 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp
--rw-rw-rw-   0        0        0    44236 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp
--rw-rw-rw-   0        0        0    44228 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp
--rw-rw-rw-   0        0        0    16127 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp
--rw-rw-rw-   0        0        0    16128 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp
--rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp
--rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp
--rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp
--rw-rw-rw-   0        0        0     4228 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp
--rw-rw-rw-   0        0        0     4229 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp
--rw-rw-rw-   0        0        0     7324 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp
--rw-rw-rw-   0        0        0    14125 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp
--rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp
--rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp
--rw-rw-rw-   0        0        0    14184 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp
--rw-rw-rw-   0        0        0    14187 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp
--rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp
--rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp
--rw-rw-rw-   0        0        0    14990 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    14991 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    18621 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp
--rw-rw-rw-   0        0        0     8432 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp
--rw-rw-rw-   0        0        0     8434 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp
--rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp
--rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp
--rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp
--rw-rw-rw-   0        0        0    19781 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp
--rw-rw-rw-   0        0        0    19782 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp
--rw-rw-rw-   0        0        0    16243 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp
--rw-rw-rw-   0        0        0    16246 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp
--rw-rw-rw-   0        0        0    16483 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp
--rw-rw-rw-   0        0        0    16479 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp
--rw-rw-rw-   0        0        0    11920 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp
--rw-rw-rw-   0        0        0    11919 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp
--rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp
--rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp
--rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp
--rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp
--rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp
--rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp
--rw-rw-rw-   0        0        0    10935 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml
--rw-rw-rw-   0        0        0    11547 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml
--rw-rw-rw-   0        0        0     9626 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml
--rw-rw-rw-   0        0        0     9620 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml
--rw-rw-rw-   0        0        0    11547 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml
--rw-rw-rw-   0        0        0     9931 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml
--rw-rw-rw-   0        0        0    11849 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml
--rw-rw-rw-   0        0        0   461565 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim
--rw-rw-rw-   0        0        0   463111 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim
--rw-rw-rw-   0        0        0   465487 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim
--rw-rw-rw-   0        0        0   460280 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim
--rw-rw-rw-   0        0        0   463094 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim
--rw-rw-rw-   0        0        0   460710 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim
--rw-rw-rw-   0        0        0   463517 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim
--rw-rw-rw-   0        0        0    24491 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml
--rw-rw-rw-   0        0        0    31035 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml
--rw-rw-rw-   0        0        0    30816 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml
--rw-rw-rw-   0        0        0    31106 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
--rw-rw-rw-   0        0        0    31035 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml
--rw-rw-rw-   0        0        0    31339 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml
--rw-rw-rw-   0        0        0    31339 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml
--rw-rw-rw-   0        0        0     5586 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Pose2Sim.py
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.398439 pose2sim-0.3.5/Pose2Sim/Utilities/
--rw-rw-rw-   0        0        0     5101 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py
--rw-rw-rw-   0        0        0    10169 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/Utilities/Blazepose_runsave.py
--rw-rw-rw-   0        0        0     3655 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/DLC_to_OpenPose.py
--rw-rw-rw-   0        0        0      108 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/__init__.py
--rw-rw-rw-   0        0        0     4846 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/c3d_to_trc.py
--rw-rw-rw-   0        0        0    12642 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/calib_from_checkerboard.py
--rw-rw-rw-   0        0        0     8657 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/calib_qca_to_toml.py
--rw-rw-rw-   0        0        0     8057 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/calib_toml_to_qca.py
--rw-rw-rw-   0        0        0     5324 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/calib_toml_to_yml.py
--rw-rw-rw-   0        0        0     6115 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/calib_yml_to_toml.py
--rw-rw-rw-   0        0        0     5008 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/json_display_with_img.py
--rw-rw-rw-   0        0        0     6024 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/json_display_without_img.py
--rw-rw-rw-   0        0        0     2780 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_Zup_to_Yup.py
--rw-rw-rw-   0        0        0     6104 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_combine.py
--rw-rw-rw-   0        0        0     3069 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_desample.py
--rw-rw-rw-   0        0        0    12931 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_filter.py
--rw-rw-rw-   0        0        0     6640 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_gaitevents.py
--rw-rw-rw-   0        0        0     4914 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/Utilities/trc_plot.py
--rw-rw-rw-   0        0        0      110 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/__init__.py
--rw-rw-rw-   0        0        0    16591 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/calibrate_cams.py
--rw-rw-rw-   0        0        0     7100 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/common.py
--rw-rw-rw-   0        0        0    12122 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/filter_3d.py
--rw-rw-rw-   0        0        0    15387 2023-03-06 13:10:05.000000 pose2sim-0.3.5/Pose2Sim/skeletons.py
--rw-rw-rw-   0        0        0    13776 2023-02-05 04:03:13.000000 pose2sim-0.3.5/Pose2Sim/track_2d.py
--rw-rw-rw-   0        0        0    21093 2023-04-06 11:41:35.000000 pose2sim-0.3.5/Pose2Sim/triangulate_3d.py
--rw-rw-rw-   0        0        0    30383 2023-03-06 13:10:05.000000 pose2sim-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 11:52:34.414062 pose2sim-0.3.5/pose2sim.egg-info/
--rw-rw-rw-   0        0        0    33171 2023-04-06 11:52:33.000000 pose2sim-0.3.5/pose2sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    33010 2023-04-06 11:52:33.000000 pose2sim-0.3.5/pose2sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 11:52:33.000000 pose2sim-0.3.5/pose2sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-05 04:05:05.000000 pose2sim-0.3.5/pose2sim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      101 2023-04-06 11:52:33.000000 pose2sim-0.3.5/pose2sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 11:52:33.000000 pose2sim-0.3.5/pose2sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      113 2023-02-05 04:03:13.000000 pose2sim-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0     1518 2023-04-06 11:52:34.414062 pose2sim-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-05 04:03:13.000000 pose2sim-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:25.251766 pose2sim-0.3.6/
+-rw-rw-rw-   0        0        0     1550 2023-02-05 04:03:13.000000 pose2sim-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0    33171 2023-04-27 09:08:25.251766 pose2sim-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.331435 pose2sim-0.3.6/Pose2Sim/
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.337007 pose2sim-0.3.6/Pose2Sim/Demo/
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.345977 pose2sim-0.3.6/Pose2Sim/Demo/User/
+-rw-rw-rw-   0        0        0     3048 2023-04-27 08:53:08.000000 pose2sim-0.3.6/Pose2Sim/Demo/User/Config.toml
+-rw-rw-rw-   0        0        0    15459 2023-04-27 09:01:34.000000 pose2sim-0.3.6/Pose2Sim/Demo/User/logs.txt
+-rw-rw-rw-   0        0        0    23055 2023-04-06 11:56:12.000000 pose2sim-0.3.6/Pose2Sim/Demo/User/logs.txt.2023-04-06
+-rw-rw-rw-   0        0        0     3052 2023-04-27 08:53:51.000000 pose2sim-0.3.6/Pose2Sim/Demo/User/test.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.347972 pose2sim-0.3.6/Pose2Sim/Demo/__pycache__/
+-rw-rw-rw-   0        0        0      467 2023-04-06 11:06:55.000000 pose2sim-0.3.6/Pose2Sim/Demo/__pycache__/test.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.348977 pose2sim-0.3.6/Pose2Sim/Demo/calib-2d/
+-rw-rw-rw-   0        0        0     4881 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/calib-2d/Calib.qca.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.393746 pose2sim-0.3.6/Pose2Sim/Demo/opensim/
+-rw-rw-rw-   0        0        0   127394 2023-04-06 10:53:50.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Balancing_for_IK.trc
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.037315 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/
+-rw-rw-rw-   0        0        0    90719 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp
+-rw-rw-rw-   0        0        0    10273 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp
+-rw-rw-rw-   0        0        0    10274 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp
+-rw-rw-rw-   0        0        0    30752 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp
+-rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp
+-rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp
+-rw-rw-rw-   0        0        0    13858 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp
+-rw-rw-rw-   0        0        0    13861 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp
+-rw-rw-rw-   0        0        0   100947 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/foot.vtp
+-rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp
+-rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp
+-rw-rw-rw-   0        0        0   142705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp
+-rw-rw-rw-   0        0        0   749317 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp
+-rw-rw-rw-   0        0        0   326089 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp
+-rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp
+-rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp
+-rw-rw-rw-   0        0        0    14416 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    14419 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    15215 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    15214 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    13148 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    13149 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    91325 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp
+-rw-rw-rw-   0        0        0   100995 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp
+-rw-rw-rw-   0        0        0     7066 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp
+-rw-rw-rw-   0        0        0    13913 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp
+-rw-rw-rw-   0        0        0    18108 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    18114 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    13625 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    13621 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    15563 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    15562 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp
+-rw-rw-rw-   0        0        0     7900 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp
+-rw-rw-rw-   0        0        0     7897 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp
+-rw-rw-rw-   0        0        0    33931 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp
+-rw-rw-rw-   0        0        0    33928 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp
+-rw-rw-rw-   0        0        0    25886 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp
+-rw-rw-rw-   0        0        0    25890 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp
+-rw-rw-rw-   0        0        0    36718 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp
+-rw-rw-rw-   0        0        0    36716 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp
+-rw-rw-rw-   0        0        0    39943 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp
+-rw-rw-rw-   0        0        0    39937 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp
+-rw-rw-rw-   0        0        0    44236 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp
+-rw-rw-rw-   0        0        0    44228 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp
+-rw-rw-rw-   0        0        0    16127 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    16128 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0     4228 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp
+-rw-rw-rw-   0        0        0     4229 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp
+-rw-rw-rw-   0        0        0     7324 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp
+-rw-rw-rw-   0        0        0    14125 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp
+-rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp
+-rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp
+-rw-rw-rw-   0        0        0    14184 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    14187 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    14990 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    14991 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    18621 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp
+-rw-rw-rw-   0        0        0     8432 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp
+-rw-rw-rw-   0        0        0     8434 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp
+-rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp
+-rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp
+-rw-rw-rw-   0        0        0    19781 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    19782 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    16243 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    16246 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    16483 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp
+-rw-rw-rw-   0        0        0    16479 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp
+-rw-rw-rw-   0        0        0    11920 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp
+-rw-rw-rw-   0        0        0    11919 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp
+-rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp
+-rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp
+-rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp
+-rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp
+-rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp
+-rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp
+-rw-rw-rw-   0        0        0     9630 2023-04-06 10:53:50.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml
+-rw-rw-rw-   0        0        0   460246 2023-02-05 10:45:27.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim
+-rw-rw-rw-   0        0        0    31130 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
+-rw-rw-rw-   0        0        0    32363 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.278352 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.115449 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/
+-rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json
+-rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json
+-rw-rw-rw-   0        0        0     1648 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json
+-rw-rw-rw-   0        0        0     1648 2023-04-26 11:31:40.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json
+-rw-rw-rw-   0        0        0     1642 2023-04-26 11:31:35.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json
+-rw-rw-rw-   0        0        0     1671 2023-04-26 11:31:30.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json
+-rw-rw-rw-   0        0        0     1650 2023-04-26 11:31:24.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json
+-rw-rw-rw-   0        0        0     1648 2023-04-26 11:31:20.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json
+-rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json
+-rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json
+-rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json
+-rw-rw-rw-   0        0        0     1629 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json
+-rw-rw-rw-   0        0        0     1657 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json
+-rw-rw-rw-   0        0        0     1643 2023-04-26 20:54:11.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json
+-rw-rw-rw-   0        0        0     1661 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json
+-rw-rw-rw-   0        0        0     1647 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json
+-rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json
+-rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json
+-rw-rw-rw-   0        0        0     1650 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json
+-rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json
+-rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json
+-rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json
+-rw-rw-rw-   0        0        0     1645 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json
+-rw-rw-rw-   0        0        0     1658 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json
+-rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json
+-rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json
+-rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json
+-rw-rw-rw-   0        0        0     1655 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json
+-rw-rw-rw-   0        0        0     2046 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json
+-rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json
+-rw-rw-rw-   0        0        0     1645 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json
+-rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json
+-rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json
+-rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json
+-rw-rw-rw-   0        0        0     1608 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json
+-rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json
+-rw-rw-rw-   0        0        0     1640 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json
+-rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json
+-rw-rw-rw-   0        0        0     1626 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json
+-rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json
+-rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json
+-rw-rw-rw-   0        0        0     1636 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json
+-rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json
+-rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json
+-rw-rw-rw-   0        0        0     1620 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json
+-rw-rw-rw-   0        0        0     1619 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json
+-rw-rw-rw-   0        0        0     1637 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json
+-rw-rw-rw-   0        0        0     1627 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json
+-rw-rw-rw-   0        0        0     1628 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json
+-rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json
+-rw-rw-rw-   0        0        0     1627 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json
+-rw-rw-rw-   0        0        0     1621 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json
+-rw-rw-rw-   0        0        0     1641 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json
+-rw-rw-rw-   0        0        0     1639 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json
+-rw-rw-rw-   0        0        0     1633 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json
+-rw-rw-rw-   0        0        0     1608 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json
+-rw-rw-rw-   0        0        0     1632 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json
+-rw-rw-rw-   0        0        0     1629 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json
+-rw-rw-rw-   0        0        0     1655 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json
+-rw-rw-rw-   0        0        0     1630 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json
+-rw-rw-rw-   0        0        0     1613 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json
+-rw-rw-rw-   0        0        0     1635 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json
+-rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json
+-rw-rw-rw-   0        0        0     1631 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json
+-rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json
+-rw-rw-rw-   0        0        0     1638 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.193982 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/
+-rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json
+-rw-rw-rw-   0        0        0     1702 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json
+-rw-rw-rw-   0        0        0     1710 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json
+-rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json
+-rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json
+-rw-rw-rw-   0        0        0     1701 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json
+-rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json
+-rw-rw-rw-   0        0        0     1704 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json
+-rw-rw-rw-   0        0        0     1698 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json
+-rw-rw-rw-   0        0        0     1702 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json
+-rw-rw-rw-   0        0        0     1714 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json
+-rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json
+-rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json
+-rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json
+-rw-rw-rw-   0        0        0     1701 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json
+-rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json
+-rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json
+-rw-rw-rw-   0        0        0     1704 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json
+-rw-rw-rw-   0        0        0     1711 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json
+-rw-rw-rw-   0        0        0     1711 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json
+-rw-rw-rw-   0        0        0     1710 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json
+-rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json
+-rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json
+-rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json
+-rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json
+-rw-rw-rw-   0        0        0     1695 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json
+-rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json
+-rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json
+-rw-rw-rw-   0        0        0     1639 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json
+-rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json
+-rw-rw-rw-   0        0        0     1671 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json
+-rw-rw-rw-   0        0        0     1668 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json
+-rw-rw-rw-   0        0        0     1670 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json
+-rw-rw-rw-   0        0        0     1646 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json
+-rw-rw-rw-   0        0        0     1673 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json
+-rw-rw-rw-   0        0        0     1651 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json
+-rw-rw-rw-   0        0        0     1665 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json
+-rw-rw-rw-   0        0        0     1673 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json
+-rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json
+-rw-rw-rw-   0        0        0     1634 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json
+-rw-rw-rw-   0        0        0     1653 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json
+-rw-rw-rw-   0        0        0     1654 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json
+-rw-rw-rw-   0        0        0     1646 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json
+-rw-rw-rw-   0        0        0     1649 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json
+-rw-rw-rw-   0        0        0     1662 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json
+-rw-rw-rw-   0        0        0     1676 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json
+-rw-rw-rw-   0        0        0     1677 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json
+-rw-rw-rw-   0        0        0     1684 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json
+-rw-rw-rw-   0        0        0     1687 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json
+-rw-rw-rw-   0        0        0     1695 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json
+-rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json
+-rw-rw-rw-   0        0        0     1682 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json
+-rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json
+-rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json
+-rw-rw-rw-   0        0        0     1694 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json
+-rw-rw-rw-   0        0        0     1669 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json
+-rw-rw-rw-   0        0        0     1671 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json
+-rw-rw-rw-   0        0        0     1707 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json
+-rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json
+-rw-rw-rw-   0        0        0     1713 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json
+-rw-rw-rw-   0        0        0     1706 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json
+-rw-rw-rw-   0        0        0     1700 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json
+-rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json
+-rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json
+-rw-rw-rw-   0        0        0     1705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json
+-rw-rw-rw-   0        0        0     1713 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json
+-rw-rw-rw-   0        0        0     1672 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json
+-rw-rw-rw-   0        0        0     1652 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json
+-rw-rw-rw-   0        0        0     1672 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json
+-rw-rw-rw-   0        0        0     1650 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json
+-rw-rw-rw-   0        0        0     1656 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json
+-rw-rw-rw-   0        0        0     1669 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json
+-rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json
+-rw-rw-rw-   0        0        0     1708 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json
+-rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json
+-rw-rw-rw-   0        0        0     1709 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json
+-rw-rw-rw-   0        0        0     1692 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json
+-rw-rw-rw-   0        0        0     1693 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json
+-rw-rw-rw-   0        0        0     1683 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json
+-rw-rw-rw-   0        0        0     1682 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json
+-rw-rw-rw-   0        0        0     1712 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json
+-rw-rw-rw-   0        0        0     1688 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json
+-rw-rw-rw-   0        0        0     1686 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json
+-rw-rw-rw-   0        0        0     1690 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json
+-rw-rw-rw-   0        0        0     1677 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json
+-rw-rw-rw-   0        0        0     1670 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.272509 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json
+-rw-rw-rw-   0        0        0      841 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json
+-rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json
+-rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json
+-rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json
+-rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json
+-rw-rw-rw-   0        0        0      831 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json
+-rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json
+-rw-rw-rw-   0        0        0      833 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json
+-rw-rw-rw-   0        0        0      839 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json
+-rw-rw-rw-   0        0        0      826 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json
+-rw-rw-rw-   0        0        0      835 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json
+-rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json
+-rw-rw-rw-   0        0        0      828 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json
+-rw-rw-rw-   0        0        0      856 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json
+-rw-rw-rw-   0        0        0      832 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json
+-rw-rw-rw-   0        0        0      830 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json
+-rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json
+-rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json
+-rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json
+-rw-rw-rw-   0        0        0      855 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json
+-rw-rw-rw-   0        0        0      856 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json
+-rw-rw-rw-   0        0        0      825 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json
+-rw-rw-rw-   0        0        0      839 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.351044 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json
+-rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json
+-rw-rw-rw-   0        0        0      854 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json
+-rw-rw-rw-   0        0        0      852 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json
+-rw-rw-rw-   0        0        0      827 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json
+-rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json
+-rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json
+-rw-rw-rw-   0        0        0      808 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json
+-rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json
+-rw-rw-rw-   0        0        0      808 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json
+-rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json
+-rw-rw-rw-   0        0        0      790 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json
+-rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json
+-rw-rw-rw-   0        0        0      803 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json
+-rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json
+-rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json
+-rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json
+-rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json
+-rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json
+-rw-rw-rw-   0        0        0      814 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json
+-rw-rw-rw-   0        0        0      815 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json
+-rw-rw-rw-   0        0        0      812 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json
+-rw-rw-rw-   0        0        0      809 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json
+-rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json
+-rw-rw-rw-   0        0        0      803 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json
+-rw-rw-rw-   0        0        0      811 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json
+-rw-rw-rw-   0        0        0      833 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json
+-rw-rw-rw-   0        0        0      813 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json
+-rw-rw-rw-   0        0        0      807 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json
+-rw-rw-rw-   0        0        0      850 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json
+-rw-rw-rw-   0        0        0      848 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json
+-rw-rw-rw-   0        0        0      849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json
+-rw-rw-rw-   0        0        0      847 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json
+-rw-rw-rw-   0        0        0      851 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json
+-rw-rw-rw-   0        0        0      846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json
+-rw-rw-rw-   0        0        0      810 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json
+-rw-rw-rw-   0        0        0      834 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json
+-rw-rw-rw-   0        0        0      853 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json
+-rw-rw-rw-   0        0        0      843 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json
+-rw-rw-rw-   0        0        0      844 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json
+-rw-rw-rw-   0        0        0      845 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json
+-rw-rw-rw-   0        0        0      301 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Demo/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:23.278352 pose2sim-0.3.6/Pose2Sim/Empty_project/
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.351044 pose2sim-0.3.6/Pose2Sim/Empty_project/User/
+-rw-rw-rw-   0        0        0     3048 2023-04-27 08:52:49.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/User/Config.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:24.554957 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:25.126470 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/
+-rw-rw-rw-   0        0        0    90719 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp
+-rw-rw-rw-   0        0        0    10273 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp
+-rw-rw-rw-   0        0        0    10274 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp
+-rw-rw-rw-   0        0        0    30752 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp
+-rw-rw-rw-   0        0        0    15032 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp
+-rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp
+-rw-rw-rw-   0        0        0    52511 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp
+-rw-rw-rw-   0        0        0    13858 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp
+-rw-rw-rw-   0        0        0    13861 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp
+-rw-rw-rw-   0        0        0   100947 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp
+-rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp
+-rw-rw-rw-   0        0        0     8763 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp
+-rw-rw-rw-   0        0        0   142705 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp
+-rw-rw-rw-   0        0        0   749317 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp
+-rw-rw-rw-   0        0        0   326089 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp
+-rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp
+-rw-rw-rw-   0        0        0    39017 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp
+-rw-rw-rw-   0        0        0    14416 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    14419 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    15215 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    15214 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    13148 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    13149 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    91325 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp
+-rw-rw-rw-   0        0        0   100995 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp
+-rw-rw-rw-   0        0        0     7066 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp
+-rw-rw-rw-   0        0        0    13913 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp
+-rw-rw-rw-   0        0        0    18108 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    18114 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    13625 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    13621 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    15563 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    15562 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp
+-rw-rw-rw-   0        0        0    24266 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp
+-rw-rw-rw-   0        0        0     7900 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp
+-rw-rw-rw-   0        0        0     7897 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp
+-rw-rw-rw-   0        0        0    33931 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp
+-rw-rw-rw-   0        0        0    33928 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp
+-rw-rw-rw-   0        0        0    25886 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp
+-rw-rw-rw-   0        0        0    25890 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp
+-rw-rw-rw-   0        0        0    36718 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp
+-rw-rw-rw-   0        0        0    36716 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp
+-rw-rw-rw-   0        0        0    39943 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp
+-rw-rw-rw-   0        0        0    39937 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp
+-rw-rw-rw-   0        0        0    44236 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp
+-rw-rw-rw-   0        0        0    44228 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp
+-rw-rw-rw-   0        0        0    16127 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    16128 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    18866 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    15103 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0     4228 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp
+-rw-rw-rw-   0        0        0     4229 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp
+-rw-rw-rw-   0        0        0     7324 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp
+-rw-rw-rw-   0        0        0    14125 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp
+-rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp
+-rw-rw-rw-   0        0        0    22104 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp
+-rw-rw-rw-   0        0        0    14184 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    14187 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp
+-rw-rw-rw-   0        0        0    19793 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp
+-rw-rw-rw-   0        0        0    14990 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    14991 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    18621 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp
+-rw-rw-rw-   0        0        0     8432 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp
+-rw-rw-rw-   0        0        0     8434 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp
+-rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp
+-rw-rw-rw-   0        0        0    52941 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp
+-rw-rw-rw-   0        0        0    24270 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp
+-rw-rw-rw-   0        0        0    19781 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp
+-rw-rw-rw-   0        0        0    19782 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp
+-rw-rw-rw-   0        0        0    16243 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp
+-rw-rw-rw-   0        0        0    16246 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp
+-rw-rw-rw-   0        0        0    16483 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp
+-rw-rw-rw-   0        0        0    16479 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp
+-rw-rw-rw-   0        0        0    11920 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp
+-rw-rw-rw-   0        0        0    11919 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp
+-rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp
+-rw-rw-rw-   0        0        0     7575 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp
+-rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp
+-rw-rw-rw-   0        0        0     9516 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp
+-rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp
+-rw-rw-rw-   0        0        0    22572 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp
+-rw-rw-rw-   0        0        0    10935 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml
+-rw-rw-rw-   0        0        0    11547 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml
+-rw-rw-rw-   0        0        0     9626 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml
+-rw-rw-rw-   0        0        0     9620 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml
+-rw-rw-rw-   0        0        0    11547 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml
+-rw-rw-rw-   0        0        0     7507 2023-04-16 10:21:12.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml
+-rw-rw-rw-   0        0        0     9931 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml
+-rw-rw-rw-   0        0        0    11849 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml
+-rw-rw-rw-   0        0        0   461565 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim
+-rw-rw-rw-   0        0        0   463111 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim
+-rw-rw-rw-   0        0        0   465487 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim
+-rw-rw-rw-   0        0        0   460280 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim
+-rw-rw-rw-   0        0        0   463094 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim
+-rw-rw-rw-   0        0        0   460615 2023-04-16 10:12:57.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim
+-rw-rw-rw-   0        0        0   460710 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim
+-rw-rw-rw-   0        0        0   463517 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim
+-rw-rw-rw-   0        0        0    24491 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml
+-rw-rw-rw-   0        0        0    31035 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml
+-rw-rw-rw-   0        0        0    30816 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml
+-rw-rw-rw-   0        0        0    31106 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
+-rw-rw-rw-   0        0        0    31035 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml
+-rw-rw-rw-   0        0        0    26368 2023-04-16 10:19:34.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml
+-rw-rw-rw-   0        0        0    31339 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml
+-rw-rw-rw-   0        0        0    31339 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml
+-rw-rw-rw-   0        0        0     5575 2023-04-27 08:50:19.000000 pose2sim-0.3.6/Pose2Sim/Pose2Sim.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:25.236132 pose2sim-0.3.6/Pose2Sim/Utilities/
+-rw-rw-rw-   0        0        0     5101 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py
+-rw-rw-rw-   0        0        0    10169 2023-04-06 11:41:35.000000 pose2sim-0.3.6/Pose2Sim/Utilities/Blazepose_runsave.py
+-rw-rw-rw-   0        0        0     3655 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/DLC_to_OpenPose.py
+-rw-rw-rw-   0        0        0      108 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/__init__.py
+-rw-rw-rw-   0        0        0     4846 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/c3d_to_trc.py
+-rw-rw-rw-   0        0        0    12642 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/calib_from_checkerboard.py
+-rw-rw-rw-   0        0        0     8657 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/calib_qca_to_toml.py
+-rw-rw-rw-   0        0        0     8057 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/calib_toml_to_qca.py
+-rw-rw-rw-   0        0        0     5324 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/calib_toml_to_yml.py
+-rw-rw-rw-   0        0        0     6115 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/calib_yml_to_toml.py
+-rw-rw-rw-   0        0        0     5008 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/json_display_with_img.py
+-rw-rw-rw-   0        0        0     6024 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/json_display_without_img.py
+-rw-rw-rw-   0        0        0     2780 2023-04-06 11:41:35.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_Zup_to_Yup.py
+-rw-rw-rw-   0        0        0     6104 2023-04-06 11:41:35.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_combine.py
+-rw-rw-rw-   0        0        0     3069 2023-04-06 11:41:35.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_desample.py
+-rw-rw-rw-   0        0        0    12931 2023-04-06 11:41:35.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_filter.py
+-rw-rw-rw-   0        0        0     6640 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_gaitevents.py
+-rw-rw-rw-   0        0        0     4914 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/Utilities/trc_plot.py
+-rw-rw-rw-   0        0        0      110 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/__init__.py
+-rw-rw-rw-   0        0        0    16591 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/calibrate_cams.py
+-rw-rw-rw-   0        0        0     7100 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/common.py
+-rw-rw-rw-   0        0        0    13554 2023-04-27 08:54:35.000000 pose2sim-0.3.6/Pose2Sim/filter_3d.py
+-rw-rw-rw-   0        0        0    15387 2023-03-06 13:10:05.000000 pose2sim-0.3.6/Pose2Sim/skeletons.py
+-rw-rw-rw-   0        0        0    13776 2023-02-05 04:03:13.000000 pose2sim-0.3.6/Pose2Sim/track_2d.py
+-rw-rw-rw-   0        0        0    22634 2023-04-27 09:00:37.000000 pose2sim-0.3.6/Pose2Sim/triangulate_3d.py
+-rw-rw-rw-   0        0        0    30383 2023-03-06 13:10:05.000000 pose2sim-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 09:08:25.251766 pose2sim-0.3.6/pose2sim.egg-info/
+-rw-rw-rw-   0        0        0    33171 2023-04-27 09:08:23.000000 pose2sim-0.3.6/pose2sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    33232 2023-04-27 09:08:23.000000 pose2sim-0.3.6/pose2sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:08:23.000000 pose2sim-0.3.6/pose2sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 09:08:22.000000 pose2sim-0.3.6/pose2sim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      101 2023-04-27 09:08:23.000000 pose2sim-0.3.6/pose2sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 09:08:23.000000 pose2sim-0.3.6/pose2sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      113 2023-02-05 04:03:13.000000 pose2sim-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1518 2023-04-27 09:08:25.267391 pose2sim-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-05 04:03:13.000000 pose2sim-0.3.6/setup.py
```

### Comparing `pose2sim-0.3.5/LICENSE` & `pose2sim-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/PKG-INFO` & `pose2sim-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose2sim
-Version: 0.3.5
+Version: 0.3.6
 Summary: Perform a markerless kinematic analysis from multiple calibrated views as a unified workflow from an OpenPose input to an OpenSim result.
 Home-page: https://github.com/perfanalytics/pose2sim
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/perfanalytics/pose2sim/issues
 Keywords: markerless,kinematics,OpenPose,OpenSim,3D human pose,biomechanics
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/User/Config.toml` & `pose2sim-0.3.6/Pose2Sim/Demo/User/Config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 pose_json_folder_extension = 'json'
 pose_img_folder_extension = 'img'
 poseTracked_folder_name = 'pose-2d-tracked'
 pose3d_folder_name = 'pose-3d'
 opensim_folder_name = 'opensim'
 
 [pose-2d]
-pose_model = 'BODY_25B' #CUSTOM, BODY_25B, BODY_25, BODY_135, BLAZEPOSE, HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
+pose_model = 'BODY_25B' #CUSTOM, BODY_25B, BODY_25, BODY_135, BLAZEPOSE, 
+# HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
 # from DeepLabCut, OpenPose, MediaPipe BlazePose, and AlphaPose
 # See Pose2Sim\skeleton.py for their skeleton hierarchy
 
 [calibration]
 type = 'qca' # 'qca', 'checkerboard', 'arucoboard', or 'charucoboard'
    [calibration.qca]
    binning_factor = 1 # Usually 1
@@ -47,15 +48,16 @@
 
 [3d-triangulation]
 error_threshold_triangulation = 15 # px
 likelihood_threshold = 0.3
 min_cameras_for_triangulation = 2
 interpolation = 'cubic' #linear, slinear, quadratic, cubic, or none
 # 'none' if you don't want to interpolate missing points
-show_interp_indices = false # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
+interp_if_gap_smaller_than = 10 # do not interpolate bigger gaps
+show_interp_indices = true # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
 
 [3d-filtering]
 type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median
 display_figures = true # true or false (lowercase)
 
    [3d-filtering.butterworth]
    type = 'low'
@@ -64,13 +66,13 @@
    [3d-filtering.butterworth_on_speed]
    type = 'low'
    order = 4 
    cut_off_frequency = 10 # Hz
    [3d-filtering.gaussian]
    sigma_kernel = 2 #px
    [3d-filtering.LOESS]
-   nb_values_used = 30 # = fraction of data used * nb frames
+   nb_values_used = 15 # = fraction of data used * nb frames
    [3d-filtering.median]
    kernel_size = 9
 
 [opensim]
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/User/logs.txt` & `pose2sim-0.3.6/Pose2Sim/Demo/User/logs.txt`

 * *Files 23% similar despite different names*

```diff
@@ -5,232 +5,278 @@
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
 --> Residual (RMS) calibration errors for each camera are respectively [0.221, 0.235, 0.171, 0.191] px, which corresponds to [0.402, 0.445, 0.45, 0.505] mm.
 
 Calibration file is stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\calib-2d\Calib_qca.toml.
-Calibration took 0.01 s.
+Calibration took 0.02 s.
 
 
 ---------------------------------------------------------------------
-Tracking of the person of interest for Demo, for frames 0 to 20.
+Tracking of the person of interest for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
---> Mean reprojection error for Neck point on all frames is 10.5 px, which roughly corresponds to 19.1 mm. 
---> In average, 0.0 cameras had to be excluded to reach the demanded 20 px error threshold.
+--> Mean reprojection error for Neck point on all frames is 12.3 px, which roughly corresponds to 22.4 mm. 
+--> In average, 0.01 cameras had to be excluded to reach the demanded 20 px error threshold.
 
 Tracked json files are stored in D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-2d-tracked.
-Tracking took 0.32 s.
+Tracking took 1.46 s.
 Note: NumExpr detected 12 cores but "NUMEXPR_MAX_THREADS" not set, so enforcing safe limit of 8.
 NumExpr defaulting to 8 threads.
 
 
 ---------------------------------------------------------------------
-Triangulation of 2D points for Demo, for frames 0 to 20.
+Triangulation of 2D points for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
-Mean reprojection error for RHip is 9.0 px (~ 0.016 m), reached with 1.0 excluded cameras. 
-Mean reprojection error for RKnee is 10.1 px (~ 0.018 m), reached with 0.65 excluded cameras. 
-Mean reprojection error for RAnkle is 9.6 px (~ 0.017 m), reached with 0.1 excluded cameras. 
-Mean reprojection error for RBigToe is 6.9 px (~ 0.013 m), reached with 0.1 excluded cameras. 
-Mean reprojection error for RSmallToe is 8.6 px (~ 0.016 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for RHeel is 12.2 px (~ 0.022 m), reached with 0.3 excluded cameras. 
-Mean reprojection error for LHip is 8.2 px (~ 0.015 m), reached with 0.95 excluded cameras. 
-Mean reprojection error for LKnee is 12.6 px (~ 0.023 m), reached with 1.05 excluded cameras. 
-Mean reprojection error for LAnkle is 12.8 px (~ 0.023 m), reached with 0.15 excluded cameras. 
-Mean reprojection error for LBigToe is 12.1 px (~ 0.022 m), reached with 0.7 excluded cameras. 
-Mean reprojection error for LSmallToe is 11.4 px (~ 0.021 m), reached with 0.9 excluded cameras. 
-Mean reprojection error for LHeel is 10.4 px (~ 0.019 m), reached with 0.75 excluded cameras. 
-Mean reprojection error for Neck is 10.5 px (~ 0.019 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for Head is 11.1 px (~ 0.02 m), reached with 0.2 excluded cameras. 
-Mean reprojection error for Nose is 9.4 px (~ 0.017 m), reached with 2.0 excluded cameras. 
-Mean reprojection error for RShoulder is 8.4 px (~ 0.015 m), reached with 0.6 excluded cameras. 
-Mean reprojection error for RElbow is 9.5 px (~ 0.017 m), reached with 1.0 excluded cameras. 
-Mean reprojection error for RWrist is 11.0 px (~ 0.02 m), reached with 0.55 excluded cameras. 
-Mean reprojection error for LShoulder is 10.4 px (~ 0.019 m), reached with 0.3 excluded cameras. 
-Mean reprojection error for LElbow is 12.7 px (~ 0.023 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for LWrist is 11.8 px (~ 0.021 m), reached with 0.4 excluded cameras. 
+Mean reprojection error for RHip is 8.0 px (~ 0.015 m), reached with 0.99 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RKnee is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RAnkle is 10.8 px (~ 0.02 m), reached with 0.1 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RBigToe is 10.9 px (~ 0.02 m), reached with 0.57 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RSmallToe is 10.6 px (~ 0.019 m), reached with 0.44 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RHeel is 11.1 px (~ 0.02 m), reached with 0.31 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHip is 8.8 px (~ 0.016 m), reached with 0.83 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LKnee is 10.6 px (~ 0.019 m), reached with 0.8 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LAnkle is 12.3 px (~ 0.022 m), reached with 0.15 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LBigToe is 10.2 px (~ 0.019 m), reached with 0.33 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LSmallToe is 11.2 px (~ 0.02 m), reached with 0.46 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHeel is 10.6 px (~ 0.019 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Neck is 11.1 px (~ 0.02 m), reached with 0.17 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Head is 9.8 px (~ 0.018 m), reached with 0.56 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Nose is 8.2 px (~ 0.015 m), reached with 1.96 excluded cameras. 
+Frames ['4:9', '15:16'] were interpolated.
+Mean reprojection error for RShoulder is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RElbow is 9.0 px (~ 0.016 m), reached with 0.63 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RWrist is 9.7 px (~ 0.018 m), reached with 0.49 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LShoulder is 10.2 px (~ 0.019 m), reached with 0.5 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LElbow is 12.1 px (~ 0.022 m), reached with 0.39 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LWrist is 11.6 px (~ 0.021 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
 
---> Mean reprojection error for all points on all frames is 10.4 px, which roughly corresponds to 18.9 mm. 
+--> Mean reprojection error for all points on all frames is 10.3 px, which roughly corresponds to 18.8 mm. 
 Cameras were excluded if likelihood was below 0.3 and if the reprojection error was above 15 px.
 In average, 0.56 cameras had to be excluded to reach these thresholds.
-Camera cam03 was excluded 28% of the time, Camera cam01: 13%, Camera cam04: 4%, and Camera cam02: 4%.
+Camera cam03 was excluded 30% of the time, Camera cam01: 11%, Camera cam04: 6%, and Camera cam02: 3%.
 
-3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_0-20.trc.
-Triangulation took 0.59 s.
+3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_0-100.trc.
+Triangulation took 2.61 s.
 
 
 ---------------------------------------------------------------------
-Filtering 3D coordinates for Demo, for frames 0 to 20.
+Filtering 3D coordinates for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 --> Filter type: Butterworth low-pass. Order 4, Cut-off frequency 6 Hz.
-Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_0-20.trc.
+Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_0-100.trc.
 
 
 ---------------------------------------------------------------------
 Camera calibration
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
 --> Residual (RMS) calibration errors for each camera are respectively [0.221, 0.235, 0.171, 0.191] px, which corresponds to [0.402, 0.445, 0.45, 0.505] mm.
 
 Calibration file is stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\calib-2d\Calib_qca.toml.
-Calibration took 0.00 s.
+Calibration took 0.02 s.
 
 
 ---------------------------------------------------------------------
-Tracking of the person of interest for Demo, for frames 1 to 20.
+Tracking of the person of interest for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
---> Mean reprojection error for Neck point on all frames is 10.4 px, which roughly corresponds to 18.9 mm. 
---> In average, 0.0 cameras had to be excluded to reach the demanded 20 px error threshold.
+--> Mean reprojection error for Neck point on all frames is 12.3 px, which roughly corresponds to 22.4 mm. 
+--> In average, 0.01 cameras had to be excluded to reach the demanded 20 px error threshold.
 
 Tracked json files are stored in D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-2d-tracked.
-Tracking took 0.08 s.
+Tracking took 0.29 s.
+Note: NumExpr detected 12 cores but "NUMEXPR_MAX_THREADS" not set, so enforcing safe limit of 8.
+NumExpr defaulting to 8 threads.
 
 
 ---------------------------------------------------------------------
-Triangulation of 2D points for Demo, for frames 1 to 20.
+Triangulation of 2D points for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
-Mean reprojection error for RHip is 8.9 px (~ 0.016 m), reached with 1.0 excluded cameras. 
-Mean reprojection error for RKnee is 10.0 px (~ 0.018 m), reached with 0.68 excluded cameras. 
-Mean reprojection error for RAnkle is 9.6 px (~ 0.017 m), reached with 0.11 excluded cameras. 
-Mean reprojection error for RBigToe is 7.0 px (~ 0.013 m), reached with 0.11 excluded cameras. 
-Mean reprojection error for RSmallToe is 8.7 px (~ 0.016 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for RHeel is 12.3 px (~ 0.022 m), reached with 0.32 excluded cameras. 
-Mean reprojection error for LHip is 8.2 px (~ 0.015 m), reached with 0.95 excluded cameras. 
-Mean reprojection error for LKnee is 12.7 px (~ 0.023 m), reached with 1.05 excluded cameras. 
-Mean reprojection error for LAnkle is 13.1 px (~ 0.024 m), reached with 0.11 excluded cameras. 
-Mean reprojection error for LBigToe is 12.0 px (~ 0.022 m), reached with 0.74 excluded cameras. 
-Mean reprojection error for LSmallToe is 11.4 px (~ 0.021 m), reached with 0.89 excluded cameras. 
-Mean reprojection error for LHeel is 10.3 px (~ 0.019 m), reached with 0.79 excluded cameras. 
-Mean reprojection error for Neck is 10.4 px (~ 0.019 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for Head is 10.9 px (~ 0.02 m), reached with 0.21 excluded cameras. 
-Mean reprojection error for Nose is 9.1 px (~ 0.017 m), reached with 2.0 excluded cameras. 
-Mean reprojection error for RShoulder is 8.5 px (~ 0.015 m), reached with 0.58 excluded cameras. 
-Mean reprojection error for RElbow is 9.6 px (~ 0.017 m), reached with 1.0 excluded cameras. 
-Mean reprojection error for RWrist is 10.9 px (~ 0.02 m), reached with 0.58 excluded cameras. 
-Mean reprojection error for LShoulder is 10.3 px (~ 0.019 m), reached with 0.32 excluded cameras. 
-Mean reprojection error for LElbow is 12.7 px (~ 0.023 m), reached with 0.0 excluded cameras. 
-Mean reprojection error for LWrist is 11.8 px (~ 0.021 m), reached with 0.37 excluded cameras. 
+Mean reprojection error for RHip is 8.0 px (~ 0.015 m), reached with 0.99 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RKnee is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RAnkle is 10.8 px (~ 0.02 m), reached with 0.1 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RBigToe is 10.9 px (~ 0.02 m), reached with 0.57 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RSmallToe is 10.6 px (~ 0.019 m), reached with 0.44 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RHeel is 11.1 px (~ 0.02 m), reached with 0.31 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHip is 8.8 px (~ 0.016 m), reached with 0.83 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LKnee is 10.6 px (~ 0.019 m), reached with 0.8 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LAnkle is 12.3 px (~ 0.022 m), reached with 0.15 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LBigToe is 10.2 px (~ 0.019 m), reached with 0.33 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LSmallToe is 11.2 px (~ 0.02 m), reached with 0.46 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHeel is 10.6 px (~ 0.019 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Neck is 11.1 px (~ 0.02 m), reached with 0.17 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Head is 9.8 px (~ 0.018 m), reached with 0.56 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Nose is 8.2 px (~ 0.015 m), reached with 1.96 excluded cameras. 
+Frames ['4:9', '15:16'] were interpolated.
+Mean reprojection error for RShoulder is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RElbow is 9.0 px (~ 0.016 m), reached with 0.63 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RWrist is 9.7 px (~ 0.018 m), reached with 0.49 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LShoulder is 10.2 px (~ 0.019 m), reached with 0.5 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LElbow is 12.1 px (~ 0.022 m), reached with 0.39 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LWrist is 11.6 px (~ 0.021 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
 
---> Mean reprojection error for all points on all frames is 10.4 px, which roughly corresponds to 18.9 mm. 
+--> Mean reprojection error for all points on all frames is 10.3 px, which roughly corresponds to 18.8 mm. 
 Cameras were excluded if likelihood was below 0.3 and if the reprojection error was above 15 px.
 In average, 0.56 cameras had to be excluded to reach these thresholds.
-Camera cam03 was excluded 29% of the time, Camera cam01: 13%, Camera cam04: 5%, and Camera cam02: 4%.
+Camera cam03 was excluded 30% of the time, Camera cam01: 11%, Camera cam04: 6%, and Camera cam02: 3%.
 
-3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_1-20.trc.
-Triangulation took 0.42 s.
+3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_0-100.trc.
+Triangulation took 2.24 s.
 
 
 ---------------------------------------------------------------------
-Filtering 3D coordinates for Demo, for frames 1 to 20.
+Filtering 3D coordinates for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 --> Filter type: Butterworth low-pass. Order 4, Cut-off frequency 6 Hz.
-Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_1-20.trc.
+Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_0-100.trc.
 
 
 ---------------------------------------------------------------------
 Camera calibration
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
 --> Residual (RMS) calibration errors for each camera are respectively [0.221, 0.235, 0.171, 0.191] px, which corresponds to [0.402, 0.445, 0.45, 0.505] mm.
 
 Calibration file is stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\calib-2d\Calib_qca.toml.
-Calibration took 0.00 s.
+Calibration took 0.02 s.
 
 
 ---------------------------------------------------------------------
-Tracking of the person of interest for Demo, for frames 1 to 20.
+Tracking of the person of interest for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
---> Mean reprojection error for Neck point on all frames is 10.4 px, which roughly corresponds to 18.9 mm. 
---> In average, 0.0 cameras had to be excluded to reach the demanded 20 px error threshold.
+--> Mean reprojection error for Neck point on all frames is 12.3 px, which roughly corresponds to 22.4 mm. 
+--> In average, 0.01 cameras had to be excluded to reach the demanded 20 px error threshold.
 
 Tracked json files are stored in D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-2d-tracked.
-Tracking took 0.06 s.
+Tracking took 0.28 s.
+Note: NumExpr detected 12 cores but "NUMEXPR_MAX_THREADS" not set, so enforcing safe limit of 8.
+NumExpr defaulting to 8 threads.
 
 
 ---------------------------------------------------------------------
-Triangulation of 2D points for Demo, for frames 1 to 20.
+Triangulation of 2D points for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 
-Mean reprojection error for RHip is 8.9 px (~ 0.016 m), reached with 1.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RKnee is 10.0 px (~ 0.018 m), reached with 0.68 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RAnkle is 9.6 px (~ 0.017 m), reached with 0.11 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RBigToe is 7.0 px (~ 0.013 m), reached with 0.11 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RSmallToe is 8.7 px (~ 0.016 m), reached with 0.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RHeel is 12.3 px (~ 0.022 m), reached with 0.32 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LHip is 8.2 px (~ 0.015 m), reached with 0.95 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LKnee is 12.7 px (~ 0.023 m), reached with 1.05 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LAnkle is 13.1 px (~ 0.024 m), reached with 0.11 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LBigToe is 12.0 px (~ 0.022 m), reached with 0.74 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LSmallToe is 11.4 px (~ 0.021 m), reached with 0.89 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LHeel is 10.3 px (~ 0.019 m), reached with 0.79 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for Neck is 10.4 px (~ 0.019 m), reached with 0.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for Head is 10.9 px (~ 0.02 m), reached with 0.21 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for Nose is 9.1 px (~ 0.017 m), reached with 2.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RShoulder is 8.5 px (~ 0.015 m), reached with 0.58 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RElbow is 9.6 px (~ 0.017 m), reached with 1.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for RWrist is 10.9 px (~ 0.02 m), reached with 0.58 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LShoulder is 10.3 px (~ 0.019 m), reached with 0.32 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LElbow is 12.7 px (~ 0.023 m), reached with 0.0 excluded cameras. 
-Frames [] had to be interpolated. 
-Mean reprojection error for LWrist is 11.8 px (~ 0.021 m), reached with 0.37 excluded cameras. 
-Frames [] had to be interpolated. 
+Mean reprojection error for RHip is 8.0 px (~ 0.015 m), reached with 0.99 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RKnee is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RAnkle is 10.8 px (~ 0.02 m), reached with 0.1 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RBigToe is 10.9 px (~ 0.02 m), reached with 0.57 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RSmallToe is 10.6 px (~ 0.019 m), reached with 0.44 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RHeel is 11.1 px (~ 0.02 m), reached with 0.31 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHip is 8.8 px (~ 0.016 m), reached with 0.83 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LKnee is 10.6 px (~ 0.019 m), reached with 0.8 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LAnkle is 12.3 px (~ 0.022 m), reached with 0.15 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LBigToe is 10.2 px (~ 0.019 m), reached with 0.33 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LSmallToe is 11.2 px (~ 0.02 m), reached with 0.46 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LHeel is 10.6 px (~ 0.019 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Neck is 11.1 px (~ 0.02 m), reached with 0.17 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Head is 9.8 px (~ 0.018 m), reached with 0.56 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for Nose is 8.2 px (~ 0.015 m), reached with 1.96 excluded cameras. 
+Frames ['4:8', '15:15'] were interpolated.
+Mean reprojection error for RShoulder is 9.4 px (~ 0.017 m), reached with 0.61 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RElbow is 9.0 px (~ 0.016 m), reached with 0.63 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for RWrist is 9.7 px (~ 0.018 m), reached with 0.49 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LShoulder is 10.2 px (~ 0.019 m), reached with 0.5 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LElbow is 12.1 px (~ 0.022 m), reached with 0.39 excluded cameras. 
+Frames [] were interpolated.
+Mean reprojection error for LWrist is 11.6 px (~ 0.021 m), reached with 0.38 excluded cameras. 
+Frames [] were interpolated.
 
---> Mean reprojection error for all points on all frames is 10.4 px, which roughly corresponds to 18.9 mm. 
+--> Mean reprojection error for all points on all frames is 10.3 px, which roughly corresponds to 18.8 mm. 
 Cameras were excluded if likelihood was below 0.3 and if the reprojection error was above 15 px.
 In average, 0.56 cameras had to be excluded to reach these thresholds.
-Camera cam03 was excluded 29% of the time, Camera cam01: 13%, Camera cam04: 5%, and Camera cam02: 4%.
+Camera cam03 was excluded 30% of the time, Camera cam01: 11%, Camera cam04: 6%, and Camera cam02: 3%.
 
-3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_1-20.trc.
-Triangulation took 0.44 s.
+3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_0-100.trc.
+Triangulation took 2.24 s.
 
 
 ---------------------------------------------------------------------
-Filtering 3D coordinates for Demo, for frames 1 to 20.
+Filtering 3D coordinates for Demo, for all frames.
 ---------------------------------------------------------------------
 
 Project directory: D:\softs\github_david\pose2sim\Pose2Sim\Demo
 --> Filter type: Butterworth low-pass. Order 4, Cut-off frequency 6 Hz.
-Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_1-20.trc.
+Filtered 3D coordinates are stored at D:\softs\github_david\pose2sim\Pose2Sim\Demo\pose-3d\Demo_filt_0-100.trc.
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/User/test.toml` & `pose2sim-0.3.6/Pose2Sim/Demo/User/test.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 ## PROJECT PARAMETERS                                                        ##
 ###############################################################################
 
 # Configure your project parameters here
 
 [project]
 project_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
-frame_range = [0,20] #For example [10,300], or [] if all frames.
+frame_range = [0,10] #For example [10,300], or [] for all frames
 frame_rate = 60 #Hz
 
 rawImg_folder_name = 'raw-2d'
 calib_folder_name = 'calib-2d'
 pose_folder_name = 'pose-2d'
 pose_json_folder_extension = 'json'
 pose_img_folder_extension = 'img'
 poseTracked_folder_name = 'pose-2d-tracked'
 pose3d_folder_name = 'pose-3d'
 opensim_folder_name = 'opensim'
 
 [pose-2d]
-pose_model = 'BODY_25B' #BODY_25B, BODY_25, BLAZEPOSE, COCO, MPI are available.
-# set your own model in skeleton.py if you don't use openpose.
+pose_model = 'BODY_25B' #CUSTOM, BODY_25B, BODY_25, BODY_135, BLAZEPOSE, 
+# HALPE_26, HALPE_68, HALPE_136, COCO_133, COCO, MPII are available,
+# from DeepLabCut, OpenPose, MediaPipe BlazePose, and AlphaPose
+# See Pose2Sim\skeleton.py for their skeleton hierarchy
 
 [calibration]
 type = 'qca' # 'qca', 'checkerboard', 'arucoboard', or 'charucoboard'
    [calibration.qca]
    binning_factor = 1 # Usually 1
 
    [calibration.checkerboard]
    corners_nb = [7,12] # [H,W] rather than [w,h]
    square_size = 80 # mm # [h,w] if square is actually a rectangle
-   frame_for_origin = -1 # starting from zero. -1 if board is at origin on last frame.
+   frame_for_origin = -1 # starting from zero. -1 if board is at origin on last frame
    # /!\ Beware that corners must be detected on all view at frame_for_origin, or else 
    # extrinsic parameters will be wrong. Set show_corner_detection to true to check it.
    show_corner_detection = false # true or false (lowercase)
    from_vid_or_img = 'img' # 'vid' or 'img'
    vid_snapshot_every_N_frames = 20
    vid_extension = 'mp4'
    img_extension = 'jpg' # 'png', 'jpg', etc
@@ -46,29 +48,31 @@
 
 [3d-triangulation]
 error_threshold_triangulation = 15 # px
 likelihood_threshold = 0.3
 min_cameras_for_triangulation = 2
 interpolation = 'cubic' #linear, slinear, quadratic, cubic, or none
 # 'none' if you don't want to interpolate missing points
-show_interp_indices = false # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
+interp_if_gap_smaller_than = 10 # do not interpolate bigger gaps
+show_interp_indices = true # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
 
 [3d-filtering]
-type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median.
-display_figures = false # true or false (lowercase)
+type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median
+display_figures = true # true or false (lowercase)
 
    [3d-filtering.butterworth]
    type = 'low'
    order = 4 
    cut_off_frequency = 6 # Hz
    [3d-filtering.butterworth_on_speed]
    type = 'low'
    order = 4 
    cut_off_frequency = 10 # Hz
    [3d-filtering.gaussian]
    sigma_kernel = 2 #px
    [3d-filtering.LOESS]
-   nb_values_used = 30 # = fraction of data used * nb frames
+   nb_values_used = 15 # = fraction of data used * nb frames
    [3d-filtering.median]
    kernel_size = 9
 
 [opensim]
+
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/calib-2d/Calib.qca.txt` & `pose2sim-0.3.6/Pose2Sim/Demo/calib-2d/Calib.qca.txt`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Balancing_for_IK.trc` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Balancing_for_IK.trc`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/capitate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/capitate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv1sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv2sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv3sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv4sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv5sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv6sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/cerv7.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/femur_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/femur_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/fibula_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/fibula_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/foot.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hamate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hamate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_jaw.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_ribs_scap.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/hat_skull.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/humerus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/humerus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/index_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/l_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/little_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar1.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar2.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar3.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar4.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lumbar5.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lunate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/lunate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal1_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal1_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal2_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal2_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal3_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal3_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal4_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal4_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal5_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/metacarpal5_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/middle_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/pisiform_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/pisiform_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/r_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/r_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/radius_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/radius_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ring_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/sacrum.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/scaphoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/scaphoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/talus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/talus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic10_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic11_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic12_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic1_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic2_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic3_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic4_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic5_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic6_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic7_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic8_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thoracic9_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/thumb_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/tibia_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/tibia_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezium_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezium_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/trapezoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/triquetrum_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/triquetrum_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ulna_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Geometry/ulna_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc` & `pose2sim-0.3.6/Pose2Sim/Demo/opensim/Standing_for_Scaling.trc`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0004.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                526.168,
+                0,
                 436.77,
                 0.682186,
                 541.991,
                 415.893,
                 0.591759,
                 520.854,
                 405.396,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0005.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                531.513,
+                0,
                 436.877,
                 0.64958,
                 557.716,
                 421.114,
                 0.559619,
                 521.11,
                 405.455,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0006.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                547.259,
+                0,
                 442.086,
                 0.647621,
                 563.122,
                 431.595,
                 0.627625,
                 531.454,
                 415.896,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0007.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                562.954,
+                0,
                 442.085,
                 0.668835,
                 568.449,
                 431.569,
                 0.630959,
                 547.322,
                 415.913,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0008.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                568.27,
+                0,
                 442.15,
                 0.692068,
                 578.784,
                 431.627,
                 0.647805,
                 562.955,
                 421.132,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0015.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998172514619883%*

 * *Differences: {"'people'": "{0: {'pose_keypoints_2d': {insert: [(0, 0)], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "hand_left_keypoints_3d": [],
             "hand_right_keypoints_2d": [],
             "hand_right_keypoints_3d": [],
             "person_id": [
                 -1
             ],
             "pose_keypoints_2d": [
-                620.875,
+                0,
                 473.616,
                 0.65484,
                 641.833,
                 457.999,
                 0.619575,
                 615.574,
                 447.359,
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam1_json/cam01.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam2_json/cam02.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam3_json/cam03.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0000.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0001.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0002.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0003.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0004.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0005.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0006.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0007.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0008.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0009.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0010.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0011.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0012.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0013.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0014.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0015.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0016.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0017.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0018.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0019.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0020.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0021.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0022.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0023.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0024.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0025.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0026.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0027.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0028.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0029.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0030.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0031.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0032.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0033.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0034.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0035.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0036.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0037.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0038.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0039.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0040.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0041.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0042.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0043.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0044.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0045.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0046.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0047.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0048.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0049.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0050.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0051.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0052.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0053.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0054.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0055.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0056.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0057.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0058.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0059.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0060.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0061.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0062.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0063.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0064.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0065.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0066.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0067.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0068.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0069.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0070.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0071.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0072.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0073.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0074.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0075.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0076.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0077.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0078.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0079.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0080.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0081.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0082.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0083.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0084.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0085.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0086.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0087.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0088.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0089.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0090.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0091.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0092.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0093.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0094.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0095.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0096.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0097.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0098.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json` & `pose2sim-0.3.6/Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/User/Config.toml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/User/Config.toml`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
 [3d-triangulation]
 error_threshold_triangulation = 15 # px
 likelihood_threshold = 0.3
 min_cameras_for_triangulation = 2
 interpolation = 'cubic' #linear, slinear, quadratic, cubic, or none
 # 'none' if you don't want to interpolate missing points
-show_interp_indices = false # true or false (lowercase). 
-# For each keypoint, return the frames that need to be interpolated
+interp_if_gap_smaller_than = 10 # do not interpolate bigger gaps
+show_interp_indices = true # true or false (lowercase). For each keypoint, return the frames that need to be interpolated
 
 [3d-filtering]
 type = 'butterworth' # butterworth, butterworth_on_speed, gaussian, LOESS, median
 display_figures = true # true or false (lowercase)
 
    [3d-filtering.butterworth]
    type = 'low'
@@ -66,13 +66,13 @@
    [3d-filtering.butterworth_on_speed]
    type = 'low'
    order = 4 
    cut_off_frequency = 10 # Hz
    [3d-filtering.gaussian]
    sigma_kernel = 2 #px
    [3d-filtering.LOESS]
-   nb_values_used = 30 # = fraction of data used * nb frames
+   nb_values_used = 15 # = fraction of data used * nb frames
    [3d-filtering.median]
    kernel_size = 9
 
 [opensim]
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv3sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv4sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv5sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv6sm.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/cerv7.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/femur_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/femur_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/fibula_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/fibula_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hamate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hamate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_jaw.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_ribs_scap.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/hat_skull.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/humerus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/humerus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/index_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_bofoot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_foot.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/l_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/little_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar1.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar2.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar3.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar4.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lumbar5.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lunate_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/lunate_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal1_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal2_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal3_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal4_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/metacarpal5_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/middle_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/pisiform_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/pisiform_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/r_patella.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/r_pelvis.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/radius_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/radius_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_medial_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ring_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/sacrum.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/scaphoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/talus_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/talus_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic10_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic11_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic12_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic1_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic2_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic3_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic4_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic5_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic6_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic7_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic8_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thoracic9_s.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_distal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/thumb_proximal_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/tibia_l.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/tibia_r.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezium_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezium_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/trapezoid_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_lvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/triquetrum_rvs.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ulna_lv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Geometry/ulna_rv.vtp`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml` & `pose2sim-0.3.6/Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Pose2Sim.py` & `pose2sim-0.3.6/Pose2Sim/Pose2Sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     - Cameras calibration,
     - Tracking the person of interest,
     - Robust triangulation,
     - Filtration.
 
     It has been tested on Windows 10 but should work similarly on Linux.
     Please subscribe to this issue if you wish to be notified of the code release. 
-    See https://github.com/davidpagnon/Openpose-to-Opensim  
+    See https://github.com/perfanalytics/pose2sim
     
     Installation: 
     # Open Anaconda prompt. Type:
     # - conda create -n Pose2Sim python=3.7 tensorflow-gpu=1.13.1
     # - conda activate Pose2Sim
     # - conda install Pose2Sim
```

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/AlphaPose_to_OpenPose.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/Blazepose_runsave.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/DLC_to_OpenPose.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/DLC_to_OpenPose.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/c3d_to_trc.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/c3d_to_trc.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/calib_from_checkerboard.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/calib_from_checkerboard.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/calib_qca_to_toml.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/calib_qca_to_toml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/calib_toml_to_qca.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/calib_toml_to_qca.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/calib_toml_to_yml.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/calib_toml_to_yml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/calib_yml_to_toml.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/calib_yml_to_toml.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/json_display_with_img.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/json_display_with_img.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/json_display_without_img.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/json_display_without_img.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_Zup_to_Yup.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_Zup_to_Yup.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_combine.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_combine.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_desample.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_desample.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_filter.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_filter.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_gaitevents.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_gaitevents.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/Utilities/trc_plot.py` & `pose2sim-0.3.6/Pose2Sim/Utilities/trc_plot.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/calibrate_cams.py` & `pose2sim-0.3.6/Pose2Sim/calibrate_cams.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/common.py` & `pose2sim-0.3.6/Pose2Sim/common.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/filter_3d.py` & `pose2sim-0.3.6/Pose2Sim/filter_3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     
 '''
 
 
 ## INIT
 import os
 import fnmatch
+import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import logging
 
 from scipy import signal
 from scipy.ndimage import gaussian_filter1d
 from statsmodels.nonparametric.smoothers_lowess import lowess
@@ -46,57 +47,87 @@
 __status__ = "Development"
 
 
 ## FUNCTIONS
 def butterworth_filter_1d(config, col):
     '''
     1D Zero-phase Butterworth filter (dual pass)
+    Deals with nans
 
     INPUT:
-    - col: Pandas dataframe column
-    - frame rate, order, cut-off frequency, type (from Config.toml)
+    - col: numpy array
+    - order: int
+    - cutoff: int
+    - framerate: int
 
     OUTPUT
     - col_filtered: Filtered pandas dataframe column
     '''
 
-    butterworth_filter_type = config.get('3d-filtering').get('butterworth').get('type')
-    butterworth_filter_order = int(config.get('3d-filtering').get('butterworth').get('order'))
-    butterworth_filter_cutoff = int(config.get('3d-filtering').get('butterworth').get('cut_off_frequency'))    
-    frame_rate = config.get('project').get('frame_rate')
-
-    b, a = signal.butter(butterworth_filter_order/2, butterworth_filter_cutoff/(frame_rate/2), butterworth_filter_type, analog = False) 
-    col_filtered = signal.filtfilt(b, a, col)
+    type = config.get('3d-filtering').get('butterworth').get('type')
+    order = int(config.get('3d-filtering').get('butterworth').get('order'))
+    cutoff = int(config.get('3d-filtering').get('butterworth').get('cut_off_frequency'))    
+    framerate = config.get('project').get('frame_rate')
+
+    b, a = signal.butter(order/2, cutoff/(framerate/2), type, analog = False) 
+    padlen = 3 * max(len(a), len(b))
+    
+    # split into sequences of not nans
+    col_filtered = col.copy()
+    mask = np.isnan(col_filtered)  | col_filtered.eq(0)
+    falsemask_indices = np.where(~mask)[0]
+    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
+    idx_sequences = np.split(falsemask_indices, gaps)
+    if idx_sequences[0].size > 0:
+        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > padlen]
+    
+    # Filter each of the selected sequences
+    for seq_f in idx_sequences_to_filter:
+        col_filtered[seq_f] = signal.filtfilt(b, a, col_filtered[seq_f])
     
     return col_filtered
-
+    
 
 def butterworth_on_speed_filter_1d(config, col):
     '''
     1D zero-phase Butterworth filter (dual pass) on derivative
 
     INPUT:
     - col: Pandas dataframe column
     - frame rate, order, cut-off frequency, type (from Config.toml)
 
     OUTPUT
     - col_filtered: Filtered pandas dataframe column
     '''
 
-    butter_speed_filter_type = config.get('3d-filtering').get('butterworth_on_speed').get('type')
-    butter_speed_filter_order = int(config.get('3d-filtering').get('butterworth_on_speed').get('order'))
-    butter_speed_filter_cutoff = int(config.get('3d-filtering').get('butterworth_on_speed').get('cut_off_frequency'))
-    frame_rate = config.get('project').get('frame_rate')
-
-    b, a = signal.butter(butter_speed_filter_order/2, butter_speed_filter_cutoff/(frame_rate/2), butter_speed_filter_type, analog = False)
-    
-    col_diff = col.diff()   # derivative
-    col_diff = col_diff.fillna(col_diff.iloc[1]/2) # set first value correctly instead of nan
-    col_diff_filt = signal.filtfilt(b, a, col_diff) # filter derivative
-    col_filtered = col_diff_filt.cumsum() + col.iloc[0] # integrate filtered derivative
+    type = config.get('3d-filtering').get('butterworth_on_speed').get('type')
+    order = int(config.get('3d-filtering').get('butterworth_on_speed').get('order'))
+    cutoff = int(config.get('3d-filtering').get('butterworth_on_speed').get('cut_off_frequency'))
+    framerate = config.get('project').get('frame_rate')
+
+    b, a = signal.butter(order/2, cutoff/(framerate/2), type, analog = False)
+    padlen = 3 * max(len(a), len(b))
+    
+    # derivative
+    col_filtered = col.copy()
+    col_filtered_diff = col_filtered.diff()   # derivative
+    col_filtered_diff = col_filtered_diff.fillna(col_filtered_diff.iloc[1]/2) # set first value correctly instead of nan
+    
+    # split into sequences of not nans
+    mask = np.isnan(col_filtered_diff)  | col_filtered_diff.eq(0)
+    falsemask_indices = np.where(~mask)[0]
+    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
+    idx_sequences = np.split(falsemask_indices, gaps)
+    if idx_sequences[0].size > 0:
+        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > padlen]
+    
+    # Filter each of the selected sequences
+    for seq_f in idx_sequences_to_filter:
+        col_filtered_diff[seq_f] = signal.filtfilt(b, a, col_filtered_diff[seq_f])
+    col_filtered = col_filtered_diff.cumsum() + col.iloc[0] # integrate filtered derivative
     
     return col_filtered
 
 
 def gaussian_filter_1d(config, col):
     '''
     1D Gaussian filter
@@ -125,17 +156,27 @@
     - loess_filter_nb_values: window used for smoothing from Config.toml
     frac = loess_filter_nb_values * frames_number
 
     OUTPUT
     - col_filtered: Filtered pandas dataframe column
     '''
 
-    loess_filter_nb_values = config.get('3d-filtering').get('LOESS').get('nb_values_used')
+    kernel = config.get('3d-filtering').get('LOESS').get('nb_values_used')
 
-    col_filtered = lowess(col, col.index, is_sorted=True, frac=loess_filter_nb_values/len(col), it=0)[:,1]
+    col_filtered = col.copy()
+    mask = np.isnan(col_filtered) 
+    falsemask_indices = np.where(~mask)[0]
+    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
+    idx_sequences = np.split(falsemask_indices, gaps)
+    if idx_sequences[0].size > 0:
+        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > kernel]
+    
+    # Filter each of the selected sequences
+    for seq_f in idx_sequences_to_filter:
+        col_filtered[seq_f] = lowess(col_filtered[seq_f], seq_f, is_sorted=True, frac=kernel/len(seq_f), it=0)[:,1]
 
     return col_filtered
     
 
 def median_filter_1d(config, col):
     '''
     1D median filter
```

### Comparing `pose2sim-0.3.5/Pose2Sim/skeletons.py` & `pose2sim-0.3.6/Pose2Sim/skeletons.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/track_2d.py` & `pose2sim-0.3.6/Pose2Sim/track_2d.py`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/Pose2Sim/triangulate_3d.py` & `pose2sim-0.3.6/Pose2Sim/triangulate_3d.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,39 +77,55 @@
     cols = list(Q.columns)
     cols = np.array([[cols[i*3+1],cols[i*3+2],cols[i*3]] for i in range(int(len(cols)/3))]).flatten()
     Q = Q[cols]
 
     return Q
 
 
-def interpolate_nans(col, *kind):
+def interpolate_zeros_nans(col, *args):
     '''
-    Interpolate missing points (of value nan)
+    Interpolate missing points (of value zero),
+    unless more than N contiguous values are missing.
 
     INPUTS:
     - col: pandas column of coordinates
-    - kind: 'linear', 'slinear', 'quadratic', 'cubic'. Default: 'cubic'
+    - args[0] = N: max number of contiguous bad values, above which they won't be interpolated
+    - args[1] = kind: 'linear', 'slinear', 'quadratic', 'cubic'. Default: 'cubic'
 
     OUTPUT:
     - col_interp: interpolated pandas column
     '''
 
-    idx = col.index
-    idx_good = np.where(np.isfinite(col))[0] #index of non zeros
-    if len(idx_good) <= 10: return col
-    # idx_notgood = np.delete(np.arange(len(col)), idx_good)
-
-    if not kind: # 'linear', 'slinear', 'quadratic', 'cubic'
-        f_interp = interpolate.interp1d(idx_good, col[idx_good], kind="cubic", bounds_error=False)
+    if len(args)==2:
+        N, kind = args
+    if len(args)==1:
+        N = np.inf
+        kind = args[0]
+    if not args:
+        N = np.inf
+    
+    # Interpolate nans
+    mask = ~(np.isnan(col) | col.eq(0)) # true where nans or zeros
+    idx_good = np.where(mask)[0]
+    if 'kind' not in locals(): # 'linear', 'slinear', 'quadratic', 'cubic'
+        f_interp = interpolate.interp1d(idx_good, col[idx_good], kind="linear", bounds_error=False)
     else:
-        f_interp = interpolate.interp1d(idx_good, col[idx_good], kind=kind[0], bounds_error=False)
-    col_interp = np.where(np.isfinite(col), col, f_interp(idx)) #replace nans with interpolated values
-    col_interp = np.where(np.isfinite(col_interp), col_interp, np.nanmean(col_interp)) #replace remaining nans
-
-    return col_interp #, idx_notgood
+        f_interp = interpolate.interp1d(idx_good, col[idx_good], kind=kind, fill_value='extrapolate', bounds_error=False)
+    col_interp = np.where(mask, col, f_interp(col.index)) #replace at false index with interpolated values
+    
+    # Reintroduce nans if lenght of sequence > N
+    idx_notgood = np.where(~mask)[0]
+    gaps = np.where(np.diff(idx_notgood) > 1)[0] + 1 # where the indices of true are not contiguous
+    sequences = np.split(idx_notgood, gaps)
+    if sequences[0].size>0:
+        for seq in sequences:
+            if len(seq) > N: # values to exclude from interpolation are set to false when they are too long 
+                col_interp[seq] = np.nan
+    
+    return col_interp
 
 
 def make_trc(config, Q, keypoints_names, f_range):
     '''
     Make Opensim compatible trc file from a dataframe with 3D coordinates
 
     INPUT:
@@ -155,15 +171,15 @@
     with open(trc_path, 'w') as trc_o:
         [trc_o.write(line+'\n') for line in header_trc]
         Q.to_csv(trc_o, sep='\t', index=True, header=None, line_terminator='\n')
 
     return trc_path
 
 
-def recap_triangulate(config, error, nb_cams_excluded, keypoints_names, cam_excluded_count, interp_frames, trc_path):
+def recap_triangulate(config, error, nb_cams_excluded, keypoints_names, cam_excluded_count, interp_frames, non_interp_frames, trc_path):
     '''
     Print a message giving statistics on reprojection errors (in pixel and in m)
     as well as the number of cameras that had to be excluded to reach threshold 
     conditions. Also stored in User/logs.txt.
 
     INPUT:
     - a Config.toml file
@@ -197,19 +213,20 @@
     logging.info('')
     for idx, name in enumerate(keypoints_names):
         mean_error_keypoint_px = np.around(error.iloc[:,idx].mean(), decimals=1) # RMS à la place?
         mean_error_keypoint_m = np.around(mean_error_keypoint_px * Dm / fm, decimals=3)
         mean_cam_excluded_keypoint = np.around(nb_cams_excluded.iloc[:,idx].mean(), decimals=2)
         logging.info(f'Mean reprojection error for {name} is {mean_error_keypoint_px} px (~ {mean_error_keypoint_m} m), reached with {mean_cam_excluded_keypoint} excluded cameras. ')
         if show_interp_indices:
-            interp_frames_keypoint = interp_frames[1][np.where(interp_frames[0]==idx)[0]]
             if interpolation_kind != 'none':
-                logging.info(f'Frames {list(interp_frames_keypoint)} had to be interpolated. ')
+                logging.info(f'Frames {list(interp_frames[idx])} were interpolated.')
+                if len(list(non_interp_frames[idx]))>0:
+                    logging.info(f'Frames {list(non_interp_frames[idx])} could not be interpolated: consider adjusting thresholds.')
             else:
-                logging.info(f'Frames {list(interp_frames_keypoint)} need to be interpolated, or thresholds need to be adjusted. ')
+                logging.info(f'No frames were interpolated because \'interpolation_kind\' was set to none. ')
     
     mean_error_px = np.around(error['mean'].mean(), decimals=1)
     mean_error_mm = np.around(mean_error_px * Dm / fm *1000, decimals=1)
     mean_cam_excluded = np.around(nb_cams_excluded['mean'].mean(), decimals=2)
 
     logging.info(f'\n--> Mean reprojection error for all points on all frames is {mean_error_px} px, which roughly corresponds to {mean_error_mm} mm. ')
     logging.info(f'Cameras were excluded if likelihood was below {likelihood_threshold} and if the reprojection error was above {error_threshold_triangulation} px.')
@@ -386,14 +403,15 @@
     calib_folder_name = config.get('project').get('calib_folder_name')
     pose_model = config.get('pose-2d').get('pose_model')
     pose_folder_name = config.get('project').get('pose_folder_name')
     json_folder_extension =  config.get('project').get('pose_json_folder_extension')
     frame_range = config.get('project').get('frame_range')
     likelihood_threshold = config.get('3d-triangulation').get('likelihood_threshold')
     interpolation_kind = config.get('3d-triangulation').get('interpolation')
+    interp_gap_smaller_than = config.get('3d-triangulation').get('interp_if_gap_smaller_than')
     show_interp_indices = config.get('3d-triangulation').get('show_interp_indices')
     pose_dir = os.path.join(project_dir, pose_folder_name)
     poseTracked_folder_name = config.get('project').get('poseTracked_folder_name')
     calib_dir = os.path.join(project_dir, calib_folder_name)
     calib_file = glob.glob(os.path.join(calib_dir, '*.toml'))[0]
     poseTracked_dir = os.path.join(project_dir, poseTracked_folder_name)
     
@@ -462,20 +480,26 @@
     cam_excluded_count.update((x, y/keypoints_nb/frames_nb) for x, y in cam_excluded_count.items())
     
     error_tot['mean'] = error_tot.mean(axis = 1)
     nb_cams_excluded_tot['mean'] = nb_cams_excluded_tot.mean(axis = 1)
 
     # Optionally, for each keypoint, show indices of frames that should be interpolated
     if show_interp_indices:
-        interp_frames = np.where(~np.isfinite(Q_tot.iloc[:,::3].T))
+        zero_nan_frames = np.where( Q_tot.iloc[:,::3].T.eq(0) | ~np.isfinite(Q_tot.iloc[:,::3].T) )
+        zero_nan_frames_per_kpt = [zero_nan_frames[1][np.where(zero_nan_frames[0]==k)[0]] for k in range(keypoints_nb)]
+        gaps = [np.where(np.diff(zero_nan_frames_per_kpt[k]) > 1)[0] + 1 for k in range(keypoints_nb)]
+        sequences = [np.split(zero_nan_frames_per_kpt[k], gaps[k]) for k in range(keypoints_nb)]
+        interp_frames = [[f'{seq[0]}:{seq[-1]}' for seq in seq_kpt if len(seq)<=interp_gap_smaller_than and len(seq)>0] for seq_kpt in sequences]
+        non_interp_frames = [[f'{seq[0]}:{seq[-1]}' for seq in seq_kpt if len(seq)>interp_gap_smaller_than] for seq_kpt in sequences]
     else:
         interp_frames = None
-    
+
     # Interpolate missing values
     if interpolation_kind != 'none':
-        Q_tot = Q_tot.apply(interpolate_nans, axis=0, args = [interpolation_kind])
+        Q_tot = Q_tot.apply(interpolate_zeros_nans, axis=0, args = [interp_gap_smaller_than, interpolation_kind])
+    Q_tot.replace(np.nan, 0, inplace=True)
     
     # Create TRC file
     trc_path = make_trc(config, Q_tot, keypoints_names, f_range)
     
     # Recap message
-    recap_triangulate(config, error_tot, nb_cams_excluded_tot, keypoints_names, cam_excluded_count, interp_frames, trc_path)
+    recap_triangulate(config, error_tot, nb_cams_excluded_tot, keypoints_names, cam_excluded_count, interp_frames, non_interp_frames, trc_path)
```

### Comparing `pose2sim-0.3.5/README.md` & `pose2sim-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pose2sim-0.3.5/pose2sim.egg-info/PKG-INFO` & `pose2sim-0.3.6/pose2sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pose2sim
-Version: 0.3.5
+Version: 0.3.6
 Summary: Perform a markerless kinematic analysis from multiple calibrated views as a unified workflow from an OpenPose input to an OpenSim result.
 Home-page: https://github.com/perfanalytics/pose2sim
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/perfanalytics/pose2sim/issues
 Keywords: markerless,kinematics,OpenPose,OpenSim,3D human pose,biomechanics
```

### Comparing `pose2sim-0.3.5/pose2sim.egg-info/SOURCES.txt` & `pose2sim-0.3.6/pose2sim.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Pose2Sim/filter_3d.py
 Pose2Sim/skeletons.py
 Pose2Sim/track_2d.py
 Pose2Sim/triangulate_3d.py
 Pose2Sim/Demo/test.py
 Pose2Sim/Demo/User/Config.toml
 Pose2Sim/Demo/User/logs.txt
+Pose2Sim/Demo/User/logs.txt.2023-04-06
 Pose2Sim/Demo/User/test.toml
 Pose2Sim/Demo/__pycache__/test.cpython-38.pyc
 Pose2Sim/Demo/calib-2d/Calib.qca.txt
 Pose2Sim/Demo/opensim/Balancing_for_IK.trc
 Pose2Sim/Demo/opensim/IK_Setup_Pose2Sim_Body25b.xml
 Pose2Sim/Demo/opensim/Model_Pose2Sim_Body25b.osim
 Pose2Sim/Demo/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
@@ -528,28 +529,31 @@
 Pose2Sim/Demo/pose-2d/cam4_json/cam04.0099.json
 Pose2Sim/Empty_project/User/Config.toml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Blazepose.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body135.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Body25b.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco133.xml
+Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Coco18.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe26.xml
 Pose2Sim/Empty_project/opensim/IK_Setup_Pose2Sim_Halpe68_136.xml
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_BlazePose.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body135.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Body25b.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco133.osim
+Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Coco18.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe26.osim
 Pose2Sim/Empty_project/opensim/Model_Pose2Sim_Halpe68_136.osim
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Blazepose.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body135.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Body25b.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco133.xml
+Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Coco18.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe26.xml
 Pose2Sim/Empty_project/opensim/Scaling_Setup_Pose2Sim_Halpe68_136.xml
 Pose2Sim/Empty_project/opensim/Geometry/bofoot.vtp
 Pose2Sim/Empty_project/opensim/Geometry/capitate_lvs.vtp
 Pose2Sim/Empty_project/opensim/Geometry/capitate_rvs.vtp
 Pose2Sim/Empty_project/opensim/Geometry/cerv1sm.vtp
 Pose2Sim/Empty_project/opensim/Geometry/cerv2sm.vtp
```

### Comparing `pose2sim-0.3.5/setup.cfg` & `pose2sim-0.3.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f73 6532 7369 6d0d 0a76 6572   = pose2sim..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e35 0d0a 6175  sion = 0.3.5..au
+00000020: 7369 6f6e 203d 2030 2e33 2e36 0d0a 6175  sion = 0.3.6..au
 00000030: 7468 6f72 203d 2044 6176 6964 2050 6167  thor = David Pag
 00000040: 6e6f 6e0d 0a61 7574 686f 725f 656d 6169  non..author_emai
 00000050: 6c20 3d20 636f 6e74 6163 7440 6461 7669  l = contact@davi
 00000060: 642d 7061 676e 6f6e 2e63 6f6d 0d0a 6465  d-pagnon.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 5065 7266  scription = Perf
 00000080: 6f72 6d20 6120 6d61 726b 6572 6c65 7373  orm a markerless
 00000090: 206b 696e 656d 6174 6963 2061 6e61 6c79   kinematic analy
```

