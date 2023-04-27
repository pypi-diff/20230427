# Comparing `tmp/zha-quirks-0.0.97.tar.gz` & `tmp/zha-quirks-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-quirks-0.0.97.tar", last modified: Wed Apr 12 01:26:30 2023, max compression
+gzip compressed data, was "zha-quirks-0.0.98.tar", last modified: Thu Apr 27 19:00:20 2023, max compression
```

## Comparing `zha-quirks-0.0.97.tar` & `zha-quirks-0.0.98.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32824 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zha_quirks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/adeo/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/adeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/adeo/color_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/aduro/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aduro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aduro/adurolightncc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/aurora/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aurora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aurora/aurora_dimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/bitron/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bitron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bitron/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/bosch/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/isw_zdl1_wp11g.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/centralite/
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3130.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3157100.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3134 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3300S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3643 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3305S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3310S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3457 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3321S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3460L.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5941 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/ias.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/motionandtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/danfoss/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/danfoss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/danfoss/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/develco/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/heat_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/open_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/smoke_alarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/echostar/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/echostar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/echostar/bell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/ecolink/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ecolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ecolink/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/edpwithus/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/edpwithus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/edpwithus/redy_plug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/elko/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/elko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/elko/smart_super_thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/eurotronic/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/eurotronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/eurotronic/spzb0001.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/feibit/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/feibit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/feibit/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/gledopto/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glc009.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glc009p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/gls007z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glsd001.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/soposhgu10.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/heiman/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/heiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/heiman/smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/hivehome/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/mot003V0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/mot003V6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/ikea/
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/cctlightzha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/fivebtnremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/fourbtnremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/motionzha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/opencloseremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/shortcutbtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/starkvind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/symfonisk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/symfonisk2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/tradfriplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/twobtnremote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/iluminize/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/dim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/imagic/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/gs1117s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/im1116s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/innr/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/innr_sp120_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/innr_sp234_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/rs228t.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/inovelli/
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/VZM31SN.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/insta/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/insta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/insta/nexentro_pushbutton_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/keenhome/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/sv02612mp13.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/kof/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/kof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/kof/kof_mr101z.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/konke/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/temp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lds/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lds/cctswitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/ledvance/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/a19rgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/flexrgbw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/legrand/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/legrand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/legrand/dimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lidl/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/TS0501A.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/rgbcct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/ts011f_plug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/linkind/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/a001082.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lixee/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lixee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lixee/zlinky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lutron/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lutron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lutron/lzl4bwhl01remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/mli/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/tint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/tintE14rgbcct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/netvox/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/netvox/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/netvox/z308e3ed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/nodon/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nodon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nodon/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/nue/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nue/auwz02000.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/orvibo/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/osram/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/a19rgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/cla60tw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/flexrgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/gardenpolesrgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/lightifyx4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/osramplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/smartplusac05347.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/switchmini.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/tunablewhite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/paulmann/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/paulmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/paulmann/fourbtnremote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/philio/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philio/pst03a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/philips/
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rdm001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rom001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rwl022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rwlfirstgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/plaid/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/plaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/plaid/soil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/salus/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/salus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/salus/sp600.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/samjin/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/button2.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/multi2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sengled/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sengled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sengled/e1e_g7f.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sercomm/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sercomm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sercomm/szwtd02n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/siglis/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/siglis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/siglis/zigfred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sinope/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    15193 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/smartthings/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2165 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/moisturev4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/multi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/multiv4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/pgc313.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/pgc314.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3337 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/tag_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/smartwings/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartwings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartwings/wm25lz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/sonoff/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sonoff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sonoff/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/smart_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/terncy/
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/pp01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/sd01.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/texasinstruments/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/texasinstruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/texasinstruments/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/thirdreality/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/button.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/trust/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/trust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/trust/zpir8000.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/
--rw-r--r--   0 runner    (1001) docker     (123)    56166 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/air/
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/air/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/air/ts0601_air_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/mcu/
--rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/mcu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/sm0202_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    32600 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts000x.py
--rw-r--r--   0 runner    (1001) docker     (123)    40283 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts001x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0041.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0042.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0043.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0044.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0046.py
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts004f.py
--rw-r--r--   0 runner    (1001) docker     (123)    43413 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts011f_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts011f_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0121_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0201.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0210.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0211.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501_fan_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501b.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_co.py
--rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_din_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_electric_heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_garage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_haozee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_rcbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    70494 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv_sas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_valve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts110e.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts130f.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/universalelectronics/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/universalelectronics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/universalelectronics/contact_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/visonic/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/visonic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/visonic/mct340e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/waxman/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/waxman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/waxman/leaksmart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/xbee/
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/xbee3_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/xbee_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/xiaomi/
--rw-r--r--   0 runner    (1001) docker     (123)    26618 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_ln.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_neutral.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube_aqgl01.py
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/feeder_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/illumination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/light_aqcn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl04.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2b.py
--rw-r--r--   0 runner    (1001) docker     (123)    57638 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_eu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_maus01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/relay_c2acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b186acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b286acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_e1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_h1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/roller_curtain_e1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/switch_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/thermostat_agl001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/tvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/vibration_aq1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/water_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/wleak_aq1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_ht.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/yale/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/yale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/yale/realliving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/zhaquirks/zen/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zen/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/zhaquirks/zhongxing/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zhongxing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zhongxing/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32824 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.355028 zha-quirks-0.0.98/zha_quirks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-27 19:00:20.000000 zha-quirks-0.0.98/zha_quirks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-27 19:00:20.000000 zha-quirks-0.0.98/zha_quirks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:00:20.000000 zha-quirks-0.0.98/zha_quirks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 19:00:20.000000 zha-quirks-0.0.98/zha_quirks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 19:00:20.000000 zha-quirks-0.0.98/zha_quirks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.355028 zha-quirks-0.0.98/zhaquirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.355028 zha-quirks-0.0.98/zhaquirks/adeo/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/adeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/adeo/color_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.355028 zha-quirks-0.0.98/zhaquirks/aduro/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/aduro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/aduro/adurolightncc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.355028 zha-quirks-0.0.98/zhaquirks/aurora/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/aurora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/aurora/aurora_dimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/bitron/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/bitron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/bitron/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/bosch/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/bosch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/bosch/isw_zdl1_wp11g.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/bosch/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/centralite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3130.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3157100.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3134 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3300S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3643 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3305S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3310S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3457 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3321S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/cl_3460L.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5941 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/ias.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/centralite/motionandtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/danfoss/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/danfoss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/danfoss/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/develco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/heat_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/develco/smoke_alarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/echostar/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/echostar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/echostar/bell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/ecolink/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ecolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ecolink/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/edpwithus/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/edpwithus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/edpwithus/redy_plug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/elko/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/elko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/elko/smart_super_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/eurotronic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/eurotronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/eurotronic/spzb0001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/feibit/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/feibit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/feibit/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/gledopto/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/glc009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/glc009p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/gls007z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/glsd001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/gledopto/soposhgu10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.359028 zha-quirks-0.0.98/zhaquirks/heiman/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/heiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/heiman/smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/hivehome/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/hivehome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/hivehome/mot003V0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/hivehome/mot003V6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/ikea/
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/cctlightzha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/fivebtnremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/fourbtnremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/motionzha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/opencloseremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/shortcutbtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/starkvind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/symfonisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/symfonisk2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/tradfriplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ikea/twobtnremote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/iluminize/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/iluminize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/iluminize/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/iluminize/dim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/imagic/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/imagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/imagic/gs1117s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/imagic/im1116s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/innr/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/innr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/innr/innr_sp120_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/innr/innr_sp234_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/innr/rs228t.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/inovelli/
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/inovelli/VZM31SN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/inovelli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/inovelli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/insta/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/insta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/insta/nexentro_pushbutton_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/keenhome/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/keenhome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/keenhome/sv02612mp13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/keenhome/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/kof/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/kof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/kof/kof_mr101z.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.363029 zha-quirks-0.0.98/zhaquirks/konke/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/konke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/konke/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/konke/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/konke/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/konke/temp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/lds/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lds/cctswitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/ledvance/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ledvance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ledvance/a19rgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/ledvance/flexrgbw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/legrand/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/legrand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/legrand/dimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/lidl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lidl/TS0501A.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lidl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lidl/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lidl/rgbcct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lidl/ts011f_plug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/linkind/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/linkind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/linkind/a001082.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/linkind/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/lixee/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lixee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lixee/zlinky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/lutron/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lutron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/lutron/lzl4bwhl01remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/mli/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/mli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/mli/tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/mli/tintE14rgbcct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/netvox/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/netvox/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/netvox/z308e3ed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/nodon/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/nodon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/nodon/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/nue/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/nue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/nue/auwz02000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/orvibo/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/orvibo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/orvibo/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/orvibo/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/osram/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/a19rgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/cla60tw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/flexrgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/gardenpolesrgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/lightifyx4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/osramplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/smartplusac05347.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/switchmini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/osram/tunablewhite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.367029 zha-quirks-0.0.98/zhaquirks/paulmann/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/paulmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/paulmann/fourbtnremote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/philio/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philio/pst03a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/philips/
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/rdm001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/rom001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/rwl022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/philips/rwlfirstgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/plaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/plaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/plaid/soil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/salus/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/salus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/salus/sp600.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/samjin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/samjin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/samjin/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/samjin/button2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/samjin/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/samjin/multi2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/sengled/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sengled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sengled/e1e_g7f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/sercomm/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sercomm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sercomm/szwtd02n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/siglis/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/siglis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/siglis/zigfred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/sinope/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sinope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sinope/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sinope/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sinope/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15193 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sinope/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/smartthings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2165 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/moisturev4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/multi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/multiv4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/pgc313.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/pgc314.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3337 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartthings/tag_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/smartwings/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartwings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/smartwings/wm25lz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/sonoff/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sonoff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sonoff/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/sourcingandcreation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sourcingandcreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/sourcingandcreation/smart_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/terncy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/terncy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/terncy/pp01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/terncy/sd01.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.371029 zha-quirks-0.0.98/zhaquirks/texasinstruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/texasinstruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/texasinstruments/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.375029 zha-quirks-0.0.98/zhaquirks/thirdreality/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/thirdreality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/thirdreality/button.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/thirdreality/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.375029 zha-quirks-0.0.98/zhaquirks/trust/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/trust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/trust/zpir8000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/tuya/
+-rw-r--r--   0 runner    (1001) docker     (123)    56166 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/tuya/air/
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/air/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/air/ts0601_air_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/tuya/mcu/
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/mcu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/sm0202_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32600 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts000x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40283 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts001x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0041.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0042.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0043.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0046.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts004f.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46779 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts011f_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts011f_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0121_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0210.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0211.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0501_fan_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0501b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0501bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_din_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_electric_heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_garage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_haozee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_rcbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70494 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_trv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_trv_sas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts0601_valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts110e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/tuya/ts130f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/universalelectronics/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/universalelectronics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/universalelectronics/contact_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/visonic/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/visonic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/visonic/mct340e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/waxman/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/waxman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/waxman/leaksmart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/xbee/
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xbee/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xbee/xbee3_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xbee/xbee_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.379029 zha-quirks-0.0.98/zhaquirks/xiaomi/
+-rw-r--r--   0 runner    (1001) docker     (123)    26618 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/ctrl_ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/ctrl_neutral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/cube_aqgl01.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/feeder_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/illumination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/light_aqcn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/magnet_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/magnet_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_ac01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_ac02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_agl02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_agl04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_aq2b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57638 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/opple_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/opple_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug_eu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug_maus01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/relay_c2acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_b186acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_b286acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_e1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_h1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/roller_curtain_e1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/switch_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/thermostat_agl001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/tvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/vibration_aq1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/water_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/wleak_aq1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/xiaomi/mija/smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/zhaquirks/yale/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/yale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/yale/realliving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/zhaquirks/zen/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/zen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/zen/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:00:20.383029 zha-quirks-0.0.98/zhaquirks/zhongxing/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/zhongxing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-27 19:00:18.000000 zha-quirks-0.0.98/zhaquirks/zhongxing/motion.py
```

### Comparing `zha-quirks-0.0.97/LICENSE.md` & `zha-quirks-0.0.98/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/PKG-INFO` & `zha-quirks-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha-quirks
-Version: 0.0.97
+Version: 0.0.98
 Summary: Library implementing Zigpy quirks for ZHA in Home Assistant
 Home-page: https://github.com/dmulcahey/zha-device-handlers
 Author: David F. Mulcahey
 Author-email: david.mulcahey@icloud.com
 License: Apache License Version 2.0
 Keywords: zha quirks homeassistant hass
 Platform: UNKNOWN
```

### Comparing `zha-quirks-0.0.97/README.md` & `zha-quirks-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/setup.cfg` & `zha-quirks-0.0.98/setup.cfg`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/setup.py` & `zha-quirks-0.0.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for ZHAQuirks."""
 
 import pathlib
 
 from setuptools import find_packages, setup
 
-VERSION = "0.0.97"
+VERSION = "0.0.98"
 
 
 setup(
     name="zha-quirks",
     version=VERSION,
     description="Library implementing Zigpy quirks for ZHA in Home Assistant",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
```

### Comparing `zha-quirks-0.0.97/zha_quirks.egg-info/PKG-INFO` & `zha-quirks-0.0.98/zha_quirks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha-quirks
-Version: 0.0.97
+Version: 0.0.98
 Summary: Library implementing Zigpy quirks for ZHA in Home Assistant
 Home-page: https://github.com/dmulcahey/zha-device-handlers
 Author: David F. Mulcahey
 Author-email: david.mulcahey@icloud.com
 License: Apache License Version 2.0
 Keywords: zha quirks homeassistant hass
 Platform: UNKNOWN
```

### Comparing `zha-quirks-0.0.97/zha_quirks.egg-info/SOURCES.txt` & `zha-quirks-0.0.98/zha_quirks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/__init__.py` & `zha-quirks-0.0.98/zhaquirks/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/adeo/color_controller.py` & `zha-quirks-0.0.98/zhaquirks/adeo/color_controller.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/aduro/adurolightncc.py` & `zha-quirks-0.0.98/zhaquirks/aduro/adurolightncc.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/aurora/aurora_dimmer.py` & `zha-quirks-0.0.98/zhaquirks/aurora/aurora_dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/bitron/thermostat.py` & `zha-quirks-0.0.98/zhaquirks/bitron/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/bosch/isw_zdl1_wp11g.py` & `zha-quirks-0.0.98/zhaquirks/bosch/isw_zdl1_wp11g.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/bosch/motion.py` & `zha-quirks-0.0.98/zhaquirks/bosch/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/__init__.py` & `zha-quirks-0.0.98/zhaquirks/centralite/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3130.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3130.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3157100.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3157100.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3300S.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3300S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3305S.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3305S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3310S.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3310S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3321S.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3321S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/cl_3460L.py` & `zha-quirks-0.0.98/zhaquirks/centralite/cl_3460L.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/ias.py` & `zha-quirks-0.0.98/zhaquirks/centralite/ias.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/motion.py` & `zha-quirks-0.0.98/zhaquirks/centralite/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/centralite/motionandtemp.py` & `zha-quirks-0.0.98/zhaquirks/centralite/motionandtemp.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/const.py` & `zha-quirks-0.0.98/zhaquirks/const.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/danfoss/thermostat.py` & `zha-quirks-0.0.98/zhaquirks/danfoss/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/__init__.py` & `zha-quirks-0.0.98/zhaquirks/develco/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/air_quality.py` & `zha-quirks-0.0.98/zhaquirks/develco/air_quality.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/heat_alarm.py` & `zha-quirks-0.0.98/zhaquirks/develco/heat_alarm.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/motion.py` & `zha-quirks-0.0.98/zhaquirks/develco/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/open_close.py` & `zha-quirks-0.0.98/zhaquirks/develco/open_close.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/develco/smoke_alarm.py` & `zha-quirks-0.0.98/zhaquirks/develco/smoke_alarm.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/echostar/bell.py` & `zha-quirks-0.0.98/zhaquirks/echostar/bell.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ecolink/contact.py` & `zha-quirks-0.0.98/zhaquirks/ecolink/contact.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/edpwithus/redy_plug.py` & `zha-quirks-0.0.98/zhaquirks/edpwithus/redy_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/elko/__init__.py` & `zha-quirks-0.0.98/zhaquirks/elko/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/elko/smart_super_thermostat.py` & `zha-quirks-0.0.98/zhaquirks/elko/smart_super_thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/eurotronic/__init__.py` & `zha-quirks-0.0.98/zhaquirks/eurotronic/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/eurotronic/spzb0001.py` & `zha-quirks-0.0.98/zhaquirks/eurotronic/spzb0001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/feibit/switch.py` & `zha-quirks-0.0.98/zhaquirks/feibit/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/gledopto/glc009.py` & `zha-quirks-0.0.98/zhaquirks/gledopto/glc009.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/gledopto/glc009p.py` & `zha-quirks-0.0.98/zhaquirks/gledopto/glc009p.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/gledopto/gls007z.py` & `zha-quirks-0.0.98/zhaquirks/gledopto/gls007z.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/gledopto/glsd001.py` & `zha-quirks-0.0.98/zhaquirks/gledopto/glsd001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/gledopto/soposhgu10.py` & `zha-quirks-0.0.98/zhaquirks/gledopto/soposhgu10.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/heiman/smoke.py` & `zha-quirks-0.0.98/zhaquirks/heiman/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/hivehome/mot003V0.py` & `zha-quirks-0.0.98/zhaquirks/hivehome/mot003V0.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/hivehome/mot003V6.py` & `zha-quirks-0.0.98/zhaquirks/hivehome/mot003V6.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/__init__.py` & `zha-quirks-0.0.98/zhaquirks/ikea/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/blinds.py` & `zha-quirks-0.0.98/zhaquirks/ikea/blinds.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/cctlightzha.py` & `zha-quirks-0.0.98/zhaquirks/ikea/cctlightzha.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/dimmer.py` & `zha-quirks-0.0.98/zhaquirks/ikea/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/fivebtnremote.py` & `zha-quirks-0.0.98/zhaquirks/ikea/fivebtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/fourbtnremote.py` & `zha-quirks-0.0.98/zhaquirks/ikea/fourbtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/motion.py` & `zha-quirks-0.0.98/zhaquirks/ikea/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/motionzha.py` & `zha-quirks-0.0.98/zhaquirks/ikea/motionzha.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/opencloseremote.py` & `zha-quirks-0.0.98/zhaquirks/ikea/opencloseremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/shortcutbtn.py` & `zha-quirks-0.0.98/zhaquirks/ikea/shortcutbtn.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/starkvind.py` & `zha-quirks-0.0.98/zhaquirks/ikea/starkvind.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/symfonisk.py` & `zha-quirks-0.0.98/zhaquirks/ikea/symfonisk.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/symfonisk2.py` & `zha-quirks-0.0.98/zhaquirks/ikea/symfonisk2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/tradfriplug.py` & `zha-quirks-0.0.98/zhaquirks/ikea/tradfriplug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ikea/twobtnremote.py` & `zha-quirks-0.0.98/zhaquirks/ikea/twobtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/iluminize/cct.py` & `zha-quirks-0.0.98/zhaquirks/iluminize/cct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/iluminize/dim.py` & `zha-quirks-0.0.98/zhaquirks/iluminize/dim.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/imagic/gs1117s.py` & `zha-quirks-0.0.98/zhaquirks/imagic/gs1117s.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/imagic/im1116s.py` & `zha-quirks-0.0.98/zhaquirks/imagic/im1116s.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/innr/innr_sp120_plug.py` & `zha-quirks-0.0.98/zhaquirks/innr/innr_sp120_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/innr/innr_sp234_plug.py` & `zha-quirks-0.0.98/zhaquirks/innr/innr_sp234_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/innr/rs228t.py` & `zha-quirks-0.0.98/zhaquirks/innr/rs228t.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/inovelli/VZM31SN.py` & `zha-quirks-0.0.98/zhaquirks/inovelli/VZM31SN.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/inovelli/__init__.py` & `zha-quirks-0.0.98/zhaquirks/inovelli/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/inovelli/types.py` & `zha-quirks-0.0.98/zhaquirks/inovelli/types.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/insta/nexentro_pushbutton_interface.py` & `zha-quirks-0.0.98/zhaquirks/insta/nexentro_pushbutton_interface.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/keenhome/sv02612mp13.py` & `zha-quirks-0.0.98/zhaquirks/keenhome/sv02612mp13.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/keenhome/weather.py` & `zha-quirks-0.0.98/zhaquirks/keenhome/weather.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/kof/kof_mr101z.py` & `zha-quirks-0.0.98/zhaquirks/kof/kof_mr101z.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/konke/button.py` & `zha-quirks-0.0.98/zhaquirks/konke/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/konke/magnet.py` & `zha-quirks-0.0.98/zhaquirks/konke/magnet.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/konke/motion.py` & `zha-quirks-0.0.98/zhaquirks/konke/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/konke/temp.py` & `zha-quirks-0.0.98/zhaquirks/konke/temp.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lds/cctswitch.py` & `zha-quirks-0.0.98/zhaquirks/lds/cctswitch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ledvance/a19rgbw.py` & `zha-quirks-0.0.98/zhaquirks/ledvance/a19rgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/ledvance/flexrgbw.py` & `zha-quirks-0.0.98/zhaquirks/ledvance/flexrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/legrand/dimmer.py` & `zha-quirks-0.0.98/zhaquirks/legrand/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lidl/TS0501A.py` & `zha-quirks-0.0.98/zhaquirks/lidl/TS0501A.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lidl/cct.py` & `zha-quirks-0.0.98/zhaquirks/lidl/cct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lidl/rgbcct.py` & `zha-quirks-0.0.98/zhaquirks/lidl/rgbcct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lidl/ts011f_plug.py` & `zha-quirks-0.0.98/zhaquirks/lidl/ts011f_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/linkind/a001082.py` & `zha-quirks-0.0.98/zhaquirks/linkind/a001082.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/linkind/motion.py` & `zha-quirks-0.0.98/zhaquirks/linkind/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lixee/zlinky.py` & `zha-quirks-0.0.98/zhaquirks/lixee/zlinky.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/lutron/lzl4bwhl01remote.py` & `zha-quirks-0.0.98/zhaquirks/lutron/lzl4bwhl01remote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/mli/tint.py` & `zha-quirks-0.0.98/zhaquirks/mli/tint.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/mli/tintE14rgbcct.py` & `zha-quirks-0.0.98/zhaquirks/mli/tintE14rgbcct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/netvox/z308e3ed.py` & `zha-quirks-0.0.98/zhaquirks/netvox/z308e3ed.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/nodon/switch.py` & `zha-quirks-0.0.98/zhaquirks/nodon/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/nue/auwz02000.py` & `zha-quirks-0.0.98/zhaquirks/nue/auwz02000.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/orvibo/dimmer.py` & `zha-quirks-0.0.98/zhaquirks/orvibo/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/orvibo/motion.py` & `zha-quirks-0.0.98/zhaquirks/orvibo/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/a19rgbw.py` & `zha-quirks-0.0.98/zhaquirks/osram/a19rgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/cla60tw.py` & `zha-quirks-0.0.98/zhaquirks/osram/cla60tw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/flexrgbw.py` & `zha-quirks-0.0.98/zhaquirks/osram/flexrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/gardenpolesrgbw.py` & `zha-quirks-0.0.98/zhaquirks/osram/gardenpolesrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/lightifyx4.py` & `zha-quirks-0.0.98/zhaquirks/osram/lightifyx4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/osramplug.py` & `zha-quirks-0.0.98/zhaquirks/osram/osramplug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/smartplusac05347.py` & `zha-quirks-0.0.98/zhaquirks/osram/smartplusac05347.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/switchmini.py` & `zha-quirks-0.0.98/zhaquirks/osram/switchmini.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/osram/tunablewhite.py` & `zha-quirks-0.0.98/zhaquirks/osram/tunablewhite.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/paulmann/fourbtnremote.py` & `zha-quirks-0.0.98/zhaquirks/paulmann/fourbtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/philio/pst03a.py` & `zha-quirks-0.0.98/zhaquirks/philio/pst03a.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/__init__.py` & `zha-quirks-0.0.98/zhaquirks/philips/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,21 +67,27 @@
     (LONG_RELEASE, TURN_ON): {COMMAND: "on_long_release"},
     (LONG_RELEASE, TURN_OFF): {COMMAND: "off_long_release"},
     (LONG_RELEASE, DIM_UP): {COMMAND: "up_long_release"},
     (LONG_RELEASE, DIM_DOWN): {COMMAND: "down_long_release"},
 }
 
 
-class OccupancyCluster(CustomCluster, OccupancySensing):
+class PhilipsOccupancySensing(CustomCluster):
     """Philips occupancy cluster."""
 
+    cluster_id = OccupancySensing.cluster_id
+    ep_attribute = "philips_occupancy"
+
     attributes = OccupancySensing.attributes.copy()
     attributes[0x0030] = ("sensitivity", t.uint8_t, True)
     attributes[0x0031] = ("sensitivity_max", t.uint8_t, True)
 
+    server_commands = OccupancySensing.server_commands.copy()
+    client_commands = OccupancySensing.client_commands.copy()
+
 
 class PhilipsBasicCluster(CustomCluster, Basic):
     """Philips Basic cluster."""
 
     attributes = Basic.attributes.copy()
     attributes[0x0031] = ("philips", t.bitmap16, True)
```

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/motion.py` & `zha-quirks-0.0.98/zhaquirks/philips/motion.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     DEVICE_TYPE,
     ENDPOINTS,
     INPUT_CLUSTERS,
     MODELS_INFO,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
 )
-from zhaquirks.philips import PHILIPS, SIGNIFY, OccupancyCluster
+from zhaquirks.philips import PHILIPS, SIGNIFY, PhilipsOccupancySensing
 
 
 class BasicCluster(CustomCluster, Basic):
     """Hue Motion Basic cluster."""
 
     attributes = Basic.attributes.copy()
     attributes[0x0033] = ("trigger_indicator", t.Bool, True)
@@ -102,15 +102,15 @@
                 DEVICE_TYPE: zha.DeviceType.OCCUPANCY_SENSOR,
                 INPUT_CLUSTERS: [
                     BasicCluster,
                     PowerConfiguration.cluster_id,
                     Identify.cluster_id,
                     IlluminanceMeasurement.cluster_id,
                     TemperatureMeasurement.cluster_id,
-                    OccupancyCluster,
+                    PhilipsOccupancySensing,
                 ],
                 OUTPUT_CLUSTERS: [Ota.cluster_id],
             },
         }
     }
 
 
@@ -148,15 +148,15 @@
                 DEVICE_TYPE: zha.DeviceType.OCCUPANCY_SENSOR,
                 INPUT_CLUSTERS: [
                     BasicCluster,
                     PowerConfiguration.cluster_id,
                     Identify.cluster_id,
                     IlluminanceMeasurement.cluster_id,
                     TemperatureMeasurement.cluster_id,
-                    OccupancyCluster,
+                    PhilipsOccupancySensing,
                 ],
                 OUTPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
                     OnOff.cluster_id,
                     Ota.cluster_id,
                 ],
```

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/rdm001.py` & `zha-quirks-0.0.98/zhaquirks/philips/rdm001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/rom001.py` & `zha-quirks-0.0.98/zhaquirks/philips/rom001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/rwl022.py` & `zha-quirks-0.0.98/zhaquirks/philips/rwl022.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/philips/rwlfirstgen.py` & `zha-quirks-0.0.98/zhaquirks/philips/rwlfirstgen.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/plaid/soil.py` & `zha-quirks-0.0.98/zhaquirks/plaid/soil.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/salus/sp600.py` & `zha-quirks-0.0.98/zhaquirks/salus/sp600.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/samjin/__init__.py` & `zha-quirks-0.0.98/zhaquirks/samjin/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/samjin/button.py` & `zha-quirks-0.0.98/zhaquirks/samjin/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/samjin/button2.py` & `zha-quirks-0.0.98/zhaquirks/samjin/button2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/samjin/multi2.py` & `zha-quirks-0.0.98/zhaquirks/samjin/multi2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sengled/e1e_g7f.py` & `zha-quirks-0.0.98/zhaquirks/sengled/e1e_g7f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sercomm/szwtd02n.py` & `zha-quirks-0.0.98/zhaquirks/sercomm/szwtd02n.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/siglis/zigfred.py` & `zha-quirks-0.0.98/zhaquirks/siglis/zigfred.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sinope/__init__.py` & `zha-quirks-0.0.98/zhaquirks/sinope/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sinope/light.py` & `zha-quirks-0.0.98/zhaquirks/sinope/light.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sinope/sensor.py` & `zha-quirks-0.0.98/zhaquirks/sinope/sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sinope/switch.py` & `zha-quirks-0.0.98/zhaquirks/sinope/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sinope/thermostat.py` & `zha-quirks-0.0.98/zhaquirks/sinope/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/__init__.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/moisturev4.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/moisturev4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/motion.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/multi.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/multi.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/multiv4.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/multiv4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/pgc313.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/pgc313.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/pgc314.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/pgc314.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartthings/tag_v4.py` & `zha-quirks-0.0.98/zhaquirks/smartthings/tag_v4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/smartwings/wm25lz.py` & `zha-quirks-0.0.98/zhaquirks/smartwings/wm25lz.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sonoff/button.py` & `zha-quirks-0.0.98/zhaquirks/sonoff/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/sourcingandcreation/smart_button.py` & `zha-quirks-0.0.98/zhaquirks/sourcingandcreation/smart_button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/terncy/__init__.py` & `zha-quirks-0.0.98/zhaquirks/terncy/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/terncy/pp01.py` & `zha-quirks-0.0.98/zhaquirks/terncy/pp01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/terncy/sd01.py` & `zha-quirks-0.0.98/zhaquirks/terncy/sd01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/texasinstruments/router.py` & `zha-quirks-0.0.98/zhaquirks/texasinstruments/router.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/thirdreality/button.py` & `zha-quirks-0.0.98/zhaquirks/thirdreality/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/thirdreality/switch.py` & `zha-quirks-0.0.98/zhaquirks/thirdreality/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/trust/zpir8000.py` & `zha-quirks-0.0.98/zhaquirks/trust/zpir8000.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/__init__.py` & `zha-quirks-0.0.98/zhaquirks/tuya/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/air/__init__.py` & `zha-quirks-0.0.98/zhaquirks/tuya/air/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/air/ts0601_air_quality.py` & `zha-quirks-0.0.98/zhaquirks/tuya/air/ts0601_air_quality.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/mcu/__init__.py` & `zha-quirks-0.0.98/zhaquirks/tuya/mcu/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/sm0202_motion.py` & `zha-quirks-0.0.98/zhaquirks/tuya/sm0202_motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts000x.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts000x.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts001x.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts001x.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0041.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0041.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0042.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0042.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0043.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0043.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0044.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0044.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0046.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0046.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts004f.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts004f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts011f_plug.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts011f_plug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1206,7 +1206,99 @@
                 PROFILE_ID: 41440,
                 DEVICE_TYPE: 97,
                 INPUT_CLUSTERS: [],
                 OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
             },
         },
     }
+
+
+class Plug_2AC_var05(EnchantedDevice):
+    """Immax TS0011F 2 outlet plug."""
+
+    signature = {
+        MODEL: "TS011F",
+        ENDPOINTS: {
+            1: {
+                # "profile_id": 260,
+                # "device_type": "0x010a",
+                # "in_clusters": ["0x0000","0x0003","0x0004","0x0005","0x0006","0x0702","0x0b04","0xe000","0xe001"],
+                # "out_clusters": ["0x000a","0x0019"]
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
+                    Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    OnOff.cluster_id,
+                    Metering.cluster_id,
+                    ElectricalMeasurement.cluster_id,
+                    TuyaZBE000Cluster.cluster_id,
+                    TuyaZBExternalSwitchTypeCluster.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
+            },
+            2: {
+                # "profile_id": 260,
+                # "device_type": "0x010a",
+                # "in_clusters": ["0x0004","0x0005","0x0006","0xe001"],
+                # "out_clusters": []
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                INPUT_CLUSTERS: [
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    OnOff.cluster_id,
+                    TuyaZBExternalSwitchTypeCluster.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [],
+            },
+            242: {
+                # "profile_id": 41440,
+                # "device_type": "0x0061",
+                # "in_clusters": [],
+                # "out_clusters": ["0x0021"]
+                PROFILE_ID: 41440,
+                DEVICE_TYPE: 97,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+            },
+        },
+    }
+    replacement = {
+        ENDPOINTS: {
+            1: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
+                    Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    TuyaZBOnOffAttributeCluster,
+                    TuyaZBMeteringCluster,
+                    TuyaZBElectricalMeasurement,
+                    TuyaZBE000Cluster,
+                    TuyaZBExternalSwitchTypeCluster,
+                ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
+            },
+            2: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                INPUT_CLUSTERS: [
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    TuyaZBOnOffAttributeCluster,
+                    TuyaZBExternalSwitchTypeCluster,
+                ],
+                OUTPUT_CLUSTERS: [],
+            },
+            242: {
+                PROFILE_ID: 41440,
+                DEVICE_TYPE: 97,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+            },
+        },
+    }
```

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts011f_switch.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts011f_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0121_plug.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0121_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0201.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0201.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0210.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0210.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0211.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0211.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0501_fan_switch.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0501_fan_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0501b.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0501b.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0501bs.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0501bs.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_co.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_co.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_cover.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_cover.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_dimmer.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_din_power.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_din_power.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_electric_heating.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_electric_heating.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_garage.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_garage.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_gas.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_gas.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_haozee.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_haozee.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_illuminance.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_illuminance.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_motion.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_rcbo.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_rcbo.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_sensor.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_siren.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_siren.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_smoke.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_switch.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_trv.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv_sas.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_trv_sas.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_valve.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts0601_valve.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts110e.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts110e.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/tuya/ts130f.py` & `zha-quirks-0.0.98/zhaquirks/tuya/ts130f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/universalelectronics/contact_sensor.py` & `zha-quirks-0.0.98/zhaquirks/universalelectronics/contact_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/visonic/mct340e.py` & `zha-quirks-0.0.98/zhaquirks/visonic/mct340e.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/waxman/leaksmart.py` & `zha-quirks-0.0.98/zhaquirks/waxman/leaksmart.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xbee/__init__.py` & `zha-quirks-0.0.98/zhaquirks/xbee/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xbee/types.py` & `zha-quirks-0.0.98/zhaquirks/xbee/types.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xbee/xbee3_io.py` & `zha-quirks-0.0.98/zhaquirks/xbee/xbee3_io.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xbee/xbee_io.py` & `zha-quirks-0.0.98/zhaquirks/xbee/xbee_io.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/__init__.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_ln.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/ctrl_ln.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_neutral.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/ctrl_neutral.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/cube.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube_aqgl01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/cube_aqgl01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/feeder_acn001.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/feeder_acn001.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         elif attribute == FEEDING_REPORT:
             attr_str = attribute_value.decode("utf-8")
             feeding_source = attr_str[0:2]
             feeding_size = attr_str[3:4]
             self._update_attribute(
                 ZCL_LAST_FEEDING_SOURCE, OppleCluster.FeedingSource(feeding_source)
             )
-            self._update_attribute(ZCL_LAST_FEEDING_SIZE, int(feeding_size))
+            self._update_attribute(ZCL_LAST_FEEDING_SIZE, int(feeding_size, base=16))
         elif attribute == PORTIONS_DISPENSED:
             portions_per_day, _ = types.uint16_t_be.deserialize(attribute_value)
             self._update_attribute(ZCL_PORTIONS_DISPENSED, portions_per_day)
         elif attribute == WEIGHT_DISPENSED:
             weight_per_day, _ = types.uint32_t_be.deserialize(attribute_value)
             self._update_attribute(ZCL_WEIGHT_DISPENSED, weight_per_day)
         elif attribute == SCHEDULING_STRING:
```

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/illumination.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/illumination.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/light_aqcn2.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/light_aqcn2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_acn001.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/magnet_acn001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_aq2.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/magnet_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_ac01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac02.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_ac02.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl02.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_agl02.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl04.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_agl04.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2b.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/motion_aq2b.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_remote.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/opple_remote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_switch.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/opple_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_eu.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug_eu.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_maus01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/plug_maus01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/relay_c2acn01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/relay_c2acn01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b186acn01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_b186acn01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b286acn01.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_b286acn01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_e1.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_e1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_h1.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/remote_h1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/roller_curtain_e1.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/roller_curtain_e1.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,7 +296,53 @@
                 INPUT_CLUSTERS: [],
                 OUTPUT_CLUSTERS: [
                     GreenPowerProxy.cluster_id,
                 ],
             },
         },
     }
+
+
+class RollerE1AQ_3(RollerE1AQ):
+    """Aqara Roller Shade Driver E1 (version 3) device."""
+
+    signature = {
+        MODELS_INFO: [(LUMI, "lumi.curtain.acn002")],
+        ENDPOINTS: {
+            # <SizePrefixedSimpleDescriptor endpoint=1 profile=260 device_type=514
+            # device_version=1
+            # input_clusters=[0, 2, 3, 4, 5, 6, 9, 13, 19, 258]
+            # output_clusters=[10, 25]>
+            1: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.WINDOW_COVERING_DEVICE,
+                INPUT_CLUSTERS: [
+                    Alarms.cluster_id,
+                    AnalogOutput.cluster_id,
+                    Basic.cluster_id,
+                    DeviceTemperature.cluster_id,
+                    Groups.cluster_id,
+                    Identify.cluster_id,
+                    MultistateOutput.cluster_id,
+                    OnOff.cluster_id,
+                    Scenes.cluster_id,
+                    WindowCovering.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [
+                    Ota.cluster_id,
+                    Time.cluster_id,
+                ],
+            },
+            # <SizePrefixedSimpleDescriptor endpoint=242 profile=41440 device_type=97
+            # device_version=0,
+            # input_clusters=[]
+            # output_clusters=[33]>
+            242: {
+                PROFILE_ID: 41440,
+                DEVICE_TYPE: 0x0061,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [
+                    GreenPowerProxy.cluster_id,
+                ],
+            },
+        },
+    }
```

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/smoke.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/switch_aq2.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/switch_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/thermostat_agl001.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/thermostat_agl001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/tvoc.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/tvoc.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/vibration_aq1.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/vibration_aq1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/water_acn001.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/water_acn001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/weather.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/weather.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/wleak_aq1.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/aqara/wleak_aq1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/motion.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/mija/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_ht.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_ht.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_magnet.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_magnet.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_switch.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/mija/sensor_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/smoke.py` & `zha-quirks-0.0.98/zhaquirks/xiaomi/mija/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/yale/realliving.py` & `zha-quirks-0.0.98/zhaquirks/yale/realliving.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/zen/thermostat.py` & `zha-quirks-0.0.98/zhaquirks/zen/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.97/zhaquirks/zhongxing/motion.py` & `zha-quirks-0.0.98/zhaquirks/zhongxing/motion.py`

 * *Files identical despite different names*

