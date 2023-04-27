# Comparing `tmp/networklab-1.5.2.tar.gz` & `tmp/networklab-1.5.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.2.tar", last modified: Thu Apr 27 06:48:13 2023, max compression
+gzip compressed data, was "networklab-1.5.2.dev1.tar", last modified: Sat Apr 15 09:01:42 2023, max compression
```

## Comparing `networklab-1.5.2.tar` & `networklab-1.5.2.dev1.tar`

### file list

```diff
@@ -1,618 +1,606 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.509757 networklab-1.5.2/
--rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.2/LICENSE.md
--rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.2/MANIFEST.in
--rw-r--r--   0 pipi       (501) staff       (20)     4076 2023-04-27 06:48:13.509592 networklab-1.5.2/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)     3367 2023-04-02 11:32:00.000000 networklab-1.5.2/README.md
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.370516 networklab-1.5.2/netsim/
--rwxr-xr-x   0 pipi       (501) staff       (20)       46 2023-04-27 06:46:18.000000 networklab-1.5.2/netsim/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/addressing.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.372184 networklab-1.5.2/netsim/ansible/
--rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     2714 2023-04-08 06:22:10.000000 networklab-1.5.2/netsim/ansible/config.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/create-config.ansible
--rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.2/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     3424 2023-01-25 10:08:09.000000 networklab-1.5.2/netsim/ansible/initial-config.ansible
--rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.2/netsim/ansible/missing.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.372944 networklab-1.5.2/netsim/ansible/tasks/
--rw-r--r--   0 pipi       (501) staff       (20)      684 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.378246 networklab-1.5.2/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-07 18:34:46.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3084 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2142 2023-01-25 10:08:09.000000 networklab-1.5.2/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.384906 networklab-1.5.2/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.2/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.385539 networklab-1.5.2/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.385825 networklab-1.5.2/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.386124 networklab-1.5.2/netsim/ansible/tasks/linux/
--rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.386353 networklab-1.5.2/netsim/ansible/tasks/nxos/
--rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.2/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.387079 networklab-1.5.2/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/tasks/readiness-check/routeros7.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.387407 networklab-1.5.2/netsim/ansible/tasks/vmx/
--rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.2/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.387682 networklab-1.5.2/netsim/ansible/templates/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.389679 networklab-1.5.2/netsim/ansible/templates/bfd/
--rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.2/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.2/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.2/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.2/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.2/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.397325 networklab-1.5.2/netsim/ansible/templates/bgp/
--rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.2/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.2/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.2/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     7934 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3252 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.2/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.2/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.397735 networklab-1.5.2/netsim/ansible/templates/eigrp/
--rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.2/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.400097 networklab-1.5.2/netsim/ansible/templates/evpn/
--rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.2/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1580 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.2/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1708 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      405 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.2/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.402428 networklab-1.5.2/netsim/ansible/templates/gateway/
--rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.2/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.2/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.2/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.411440 networklab-1.5.2/netsim/ansible/templates/initial/
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     5271 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.2/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.2/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.2/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.412250 networklab-1.5.2/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      906 2022-12-22 08:29:57.000000 networklab-1.5.2/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2918 2022-12-22 09:39:24.000000 networklab-1.5.2/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1933 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-01-30 13:30:53.000000 networklab-1.5.2/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3431 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4711 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.2/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.2/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.2/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.2/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.414814 networklab-1.5.2/netsim/ansible/templates/isis/
--rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.2/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.2/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.2/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.2/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.422669 networklab-1.5.2/netsim/ansible/templates/mpls/
--rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      472 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.2/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      732 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.432953 networklab-1.5.2/netsim/ansible/templates/ospf/
--rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.2/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.2/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.2/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.2/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.2/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.2/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.2/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.2/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.2/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.434532 networklab-1.5.2/netsim/ansible/templates/sr/
--rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.2/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.2/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.2/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.2/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.2/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.434820 networklab-1.5.2/netsim/ansible/templates/srv6/
--rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.438578 networklab-1.5.2/netsim/ansible/templates/vlan/
--rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.2/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.2/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.2/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.2/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.2/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.2/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.2/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.447690 networklab-1.5.2/netsim/ansible/templates/vrf/
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.2/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.2/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.2/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      807 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.2/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.453345 networklab-1.5.2/netsim/ansible/templates/vxlan/
--rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1651 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2219 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.2/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/api.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.456513 networklab-1.5.2/netsim/augment/
--rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-08 17:21:52.000000 networklab-1.5.2/netsim/augment/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-10 10:09:55.000000 networklab-1.5.2/netsim/augment/components.py
--rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/augment/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     3343 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/augment/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)    17496 2023-04-27 06:23:42.000000 networklab-1.5.2/netsim/augment/groups.py
--rw-r--r--   0 pipi       (501) staff       (20)    40531 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/augment/links.py
--rw-r--r--   0 pipi       (501) staff       (20)     3179 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/augment/main.py
--rw-r--r--   0 pipi       (501) staff       (20)    12537 2023-04-27 06:20:07.000000 networklab-1.5.2/netsim/augment/nodes.py
--rw-r--r--   0 pipi       (501) staff       (20)     2814 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/augment/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     7489 2023-04-27 06:17:17.000000 networklab-1.5.2/netsim/augment/topology.py
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/callback.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.462138 networklab-1.5.2/netsim/cli/
--rwxr-xr-x   0 pipi       (501) staff       (20)     9700 2023-04-24 09:41:34.000000 networklab-1.5.2/netsim/cli/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.2/netsim/cli/alias.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1758 2022-03-20 09:00:36.000000 networklab-1.5.2/netsim/cli/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     4192 2022-12-11 09:34:30.000000 networklab-1.5.2/netsim/cli/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.2/netsim/cli/collect.py
--rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.2/netsim/cli/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     5556 2023-04-24 10:46:01.000000 networklab-1.5.2/netsim/cli/connect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/cli/create.py
--rw-r--r--   0 pipi       (501) staff       (20)     6747 2023-04-24 10:09:53.000000 networklab-1.5.2/netsim/cli/down.py
--rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.2/netsim/cli/empty.yml
--rw-r--r--   0 pipi       (501) staff       (20)     5528 2023-04-25 07:16:54.000000 networklab-1.5.2/netsim/cli/external_commands.py
--rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/cli/initial.py
--rw-r--r--   0 pipi       (501) staff       (20)     2038 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/cli/install.py
--rw-r--r--   0 pipi       (501) staff       (20)     9143 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/cli/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.2/netsim/cli/read.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/cli/restart.py
--rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-03-06 07:47:06.000000 networklab-1.5.2/netsim/cli/show.py
--rw-r--r--   0 pipi       (501) staff       (20)     4785 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/cli/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     3453 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/cli/test.py
--rw-r--r--   0 pipi       (501) staff       (20)    10689 2023-04-25 07:09:50.000000 networklab-1.5.2/netsim/cli/up.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.2/netsim/cli/usage.py
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/cli/usage.txt
--rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/cli/version.py
--rw-r--r--   0 pipi       (501) staff       (20)     1488 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/common.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.463071 networklab-1.5.2/netsim/data/
--rw-r--r--   0 pipi       (501) staff       (20)     4805 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/data/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/data/filemaps.py
--rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/data/global_vars.py
--rw-r--r--   0 pipi       (501) staff       (20)    20493 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/data/types.py
--rw-r--r--   0 pipi       (501) staff       (20)    19214 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/data/validate.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.464439 networklab-1.5.2/netsim/defaults/
--rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/defaults/addressing.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2318 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/defaults/attributes.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/defaults/automation.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/defaults/hints.yml
--rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/defaults/multilab.yml
--rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/defaults/ports.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.469868 networklab-1.5.2/netsim/devices/
--rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/arubacx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/asav.py
--rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/devices/asav.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1223 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/csr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/eos.py
--rw-r--r--   0 pipi       (501) staff       (20)     1593 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      927 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/iosv.py
--rw-r--r--   0 pipi       (501) staff       (20)     1411 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/iosv.yml
--rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/junos.py
--rw-r--r--   0 pipi       (501) staff       (20)      705 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      858 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1311 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1634 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/vmx.py
--rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/vmx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/devices/vsrx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/vsrx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/devices/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.365857 networklab-1.5.2/netsim/extra/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.470064 networklab-1.5.2/netsim/extra/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.2/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.472299 networklab-1.5.2/netsim/extra/ebgp.utils/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.472705 networklab-1.5.2/netsim/extra/ebgp.utils/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.2/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.2/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.2/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.2/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.472958 networklab-1.5.2/netsim/extra/multilab/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.473503 networklab-1.5.2/netsim/extra/multilab/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.2/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.2/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.2/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.473757 networklab-1.5.2/netsim/extra/none/
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/extra/none/none.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.474306 networklab-1.5.2/netsim/extra/proxy-arp/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.475260 networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.476691 networklab-1.5.2/netsim/install/
--rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.2/netsim/install/ansible.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     3484 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/install/containerlab.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.2/netsim/install/grpc.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.479977 networklab-1.5.2/netsim/install/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.480228 networklab-1.5.2/netsim/install/libvirt/asav/
--rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/install/libvirt/asav.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.2/netsim/install/libvirt/csr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.2/netsim/install/libvirt/eos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/install/libvirt/iosv.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.480407 networklab-1.5.2/netsim/install/libvirt/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.2/netsim/install/libvirt/iosxr/iosxr_config.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.2/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.2/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.480652 networklab-1.5.2/netsim/install/libvirt/vsrx/
--rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.2/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.2/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 pipi       (501) staff       (20)     3179 2023-01-12 13:45:42.000000 networklab-1.5.2/netsim/install/libvirt.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/install/ubuntu.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.488952 networklab-1.5.2/netsim/modules/
--rw-r--r--   0 pipi       (501) staff       (20)    21840 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/_dataplane.py
--rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/_routing.py
--rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.2/netsim/modules/bfd.py
--rw-r--r--   0 pipi       (501) staff       (20)      702 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/bfd.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20495 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/bgp.py
--rw-r--r--   0 pipi       (501) staff       (20)     1470 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/bgp.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.2/netsim/modules/eigrp.py
--rw-r--r--   0 pipi       (501) staff       (20)      324 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/modules/eigrp.yml
--rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/evpn.py
--rw-r--r--   0 pipi       (501) staff       (20)      892 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/evpn.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/gateway.py
--rw-r--r--   0 pipi       (501) staff       (20)      960 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/gateway.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/modules/isis.py
--rw-r--r--   0 pipi       (501) staff       (20)      906 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/modules/isis.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/mpls.py
--rw-r--r--   0 pipi       (501) staff       (20)      879 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/mpls.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3036 2023-01-14 10:57:46.000000 networklab-1.5.2/netsim/modules/ospf.py
--rw-r--r--   0 pipi       (501) staff       (20)     1033 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/ospf.yml
--rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/modules/sr.py
--rw-r--r--   0 pipi       (501) staff       (20)      390 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/modules/sr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.2/netsim/modules/srv6.py
--rw-r--r--   0 pipi       (501) staff       (20)      420 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/modules/srv6.yml
--rw-r--r--   0 pipi       (501) staff       (20)    58619 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vlan.py
--rw-r--r--   0 pipi       (501) staff       (20)     1022 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vlan.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20435 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vrf.py
--rw-r--r--   0 pipi       (501) staff       (20)      431 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vrf.yml
--rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vxlan.py
--rw-r--r--   0 pipi       (501) staff       (20)      564 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/modules/vxlan.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.492759 networklab-1.5.2/netsim/outputs/
--rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/outputs/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     7081 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/outputs/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/outputs/common.py
--rw-r--r--   0 pipi       (501) staff       (20)    10000 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/outputs/d2.py
--rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/outputs/d2.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2754 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/outputs/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2/netsim/outputs/format.py
--rw-r--r--   0 pipi       (501) staff       (20)     7545 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/outputs/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/outputs/graph.yml
--rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-24 10:45:00.000000 networklab-1.5.2/netsim/outputs/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.2/netsim/outputs/json.py
--rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.2/netsim/outputs/none.py
--rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/outputs/provider.py
--rw-r--r--   0 pipi       (501) staff       (20)     2667 2023-04-24 09:30:15.000000 networklab-1.5.2/netsim/outputs/tools.py
--rw-r--r--   0 pipi       (501) staff       (20)     1688 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/outputs/yaml.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.494774 networklab-1.5.2/netsim/providers/
--rw-r--r--   0 pipi       (501) staff       (20)     7919 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/providers/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/providers/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)      517 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/providers/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.2/netsim/providers/external.py
--rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/providers/external.yml
--rw-r--r--   0 pipi       (501) staff       (20)    11356 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/providers/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)      481 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/providers/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.2/netsim/providers/virtualbox.py
--rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/providers/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7799 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/read_topology.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.495025 networklab-1.5.2/netsim/templates/
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.2/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.367159 networklab-1.5.2/netsim/templates/provider/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.495302 networklab-1.5.2/netsim/templates/provider/clab/
--rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.495751 networklab-1.5.2/netsim/templates/provider/clab/frr/
--rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.496116 networklab-1.5.2/netsim/templates/provider/clab/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.2/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.496413 networklab-1.5.2/netsim/templates/provider/external/
--rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.2/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.502704 networklab-1.5.2/netsim/templates/provider/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)      541 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.2/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.2/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.2/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.2/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.2/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.2/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.2/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.2/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.2/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.2/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:30:59.000000 networklab-1.5.2/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.2/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.2/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.2/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.2/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.2/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.2/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.504758 networklab-1.5.2/netsim/templates/provider/virtualbox/
--rw-r--r--   0 pipi       (501) staff       (20)      782 2022-05-02 06:40:29.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.2/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.505656 networklab-1.5.2/netsim/templates/tests/
--rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.2/netsim/templates/tests/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.2/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.2/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.506758 networklab-1.5.2/netsim/tools/
--rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-24 09:07:41.000000 networklab-1.5.2/netsim/tools/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-24 09:03:45.000000 networklab-1.5.2/netsim/tools/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      580 2023-04-25 07:15:19.000000 networklab-1.5.2/netsim/tools/graphite.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.506991 networklab-1.5.2/netsim/tools/suzieq/
--rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-23 17:42:23.000000 networklab-1.5.2/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-25 08:08:07.000000 networklab-1.5.2/netsim/tools/suzieq.yml
--rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/topology-defaults.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.508279 networklab-1.5.2/netsim/utils/
--rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/utils/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     4068 2023-01-28 06:30:20.000000 networklab-1.5.2/netsim/utils/log.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.2/netsim/utils/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-23 09:03:00.000000 networklab-1.5.2/netsim/utils/strings.py
--rw-r--r--   0 pipi       (501) staff       (20)     4906 2023-04-21 16:48:35.000000 networklab-1.5.2/netsim/utils/templates.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.509142 networklab-1.5.2/networklab.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)     4076 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)    20838 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       51 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/entry_points.txt
--rw-r--r--   0 pipi       (501) staff       (20)      120 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        7 2023-04-27 06:48:13.000000 networklab-1.5.2/networklab.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-21 16:48:35.000000 networklab-1.5.2/requirements.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-04-27 06:48:13.509812 networklab-1.5.2/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.2/setup.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-27 06:48:13.509301 networklab-1.5.2/tests/
--rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.2/tests/test_transformation.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.355123 networklab-1.5.2.dev1/
+-rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/LICENSE.md
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/MANIFEST.in
+-rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-04-15 09:01:42.354911 networklab-1.5.2.dev1/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)     3367 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/README.md
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.190458 networklab-1.5.2.dev1/netsim/
+-rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-04-15 09:01:29.000000 networklab-1.5.2.dev1/netsim/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)    13342 2022-11-23 16:13:46.000000 networklab-1.5.2.dev1/netsim/addressing.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.191990 networklab-1.5.2.dev1/netsim/ansible/
+-rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     2714 2023-04-08 06:22:10.000000 networklab-1.5.2.dev1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/create-config.ansible
+-rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.2.dev1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3424 2023-01-25 10:08:09.000000 networklab-1.5.2.dev1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.2.dev1/netsim/ansible/missing.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.192720 networklab-1.5.2.dev1/netsim/ansible/tasks/
+-rw-r--r--   0 pipi       (501) staff       (20)      684 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.197240 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-07 18:34:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3084 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2142 2023-01-25 10:08:09.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.204485 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.204971 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205182 networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205457 networklab-1.5.2.dev1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205691 networklab-1.5.2.dev1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206299 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206473 networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206699 networklab-1.5.2.dev1/netsim/ansible/templates/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.208437 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.215119 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     7934 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3252 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.215519 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.217728 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1580 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1708 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      405 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.219761 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.228224 networklab-1.5.2.dev1/netsim/ansible/templates/initial/
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     5271 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.229012 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      906 2022-12-22 08:29:57.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2918 2022-12-22 09:39:24.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1933 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-01-30 13:30:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3431 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4711 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.231501 networklab-1.5.2.dev1/netsim/ansible/templates/isis/
+-rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.242141 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      472 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      732 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.251456 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.252895 networklab-1.5.2.dev1/netsim/ansible/templates/sr/
+-rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.253197 networklab-1.5.2.dev1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.256696 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.274088 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      807 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.276942 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1651 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2219 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/api.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.280663 networklab-1.5.2.dev1/netsim/augment/
+-rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-10 10:09:55.000000 networklab-1.5.2.dev1/netsim/augment/components.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/augment/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/augment/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)    17286 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/groups.py
+-rw-r--r--   0 pipi       (501) staff       (20)    39765 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/links.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3138 2023-04-10 10:09:55.000000 networklab-1.5.2.dev1/netsim/augment/main.py
+-rw-r--r--   0 pipi       (501) staff       (20)    12464 2023-04-13 14:55:11.000000 networklab-1.5.2.dev1/netsim/augment/nodes.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2866 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/augment/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5710 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/augment/topology.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/callback.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.295676 networklab-1.5.2.dev1/netsim/cli/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     8522 2023-04-10 10:10:02.000000 networklab-1.5.2.dev1/netsim/cli/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.2.dev1/netsim/cli/alias.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1758 2022-03-20 09:00:36.000000 networklab-1.5.2.dev1/netsim/cli/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4192 2022-12-11 09:34:30.000000 networklab-1.5.2.dev1/netsim/cli/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.2.dev1/netsim/cli/collect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.2.dev1/netsim/cli/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3684 2022-12-14 06:39:46.000000 networklab-1.5.2.dev1/netsim/cli/connect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2966 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/cli/create.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5295 2023-04-13 15:09:55.000000 networklab-1.5.2.dev1/netsim/cli/down.py
+-rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/cli/empty.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3362 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/cli/external_commands.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/initial.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2038 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/cli/install.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9143 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.2.dev1/netsim/cli/read.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1408 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/cli/restart.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/cli/show.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4785 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3453 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/cli/test.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9366 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/up.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.2.dev1/netsim/cli/usage.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/cli/usage.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/cli/version.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1488 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/common.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.297070 networklab-1.5.2.dev1/netsim/data/
+-rw-r--r--   0 pipi       (501) staff       (20)     5148 2023-04-10 13:06:35.000000 networklab-1.5.2.dev1/netsim/data/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1097 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/data/global_vars.py
+-rw-r--r--   0 pipi       (501) staff       (20)    20668 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/data/types.py
+-rw-r--r--   0 pipi       (501) staff       (20)    19276 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/data/validate.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.298529 networklab-1.5.2.dev1/netsim/defaults/
+-rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/addressing.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2282 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/defaults/attributes.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/automation.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/hints.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/multilab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/ports.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.309720 networklab-1.5.2.dev1/netsim/devices/
+-rw-r--r--   0 pipi       (501) staff       (20)     1844 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      886 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/devices/arubacx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/devices/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      996 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/asav.py
+-rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/devices/asav.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1184 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/csr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2273 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/eos.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1554 2023-02-12 08:44:04.000000 networklab-1.5.2.dev1/netsim/devices/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      927 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      854 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosv.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1372 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosv.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/junos.py
+-rw-r--r--   0 pipi       (501) staff       (20)      705 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      858 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1311 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1634 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vmx.py
+-rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vmx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vsrx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vsrx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.186664 networklab-1.5.2.dev1/netsim/extra/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.309915 networklab-1.5.2.dev1/netsim/extra/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.2.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.312621 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.312811 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313104 networklab-1.5.2.dev1/netsim/extra/multilab/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313364 networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313614 networklab-1.5.2.dev1/netsim/extra/none/
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/extra/none/none.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.314216 networklab-1.5.2.dev1/netsim/extra/proxy-arp/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.314782 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.316152 networklab-1.5.2.dev1/netsim/install/
+-rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.2.dev1/netsim/install/ansible.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3484 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.2.dev1/netsim/install/grpc.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319478 networklab-1.5.2.dev1/netsim/install/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319741 networklab-1.5.2.dev1/netsim/install/libvirt/asav/
+-rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.2.dev1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosv.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319959 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr/iosxr_config.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.2.dev1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.2.dev1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.320289 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3179 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.328574 networklab-1.5.2.dev1/netsim/modules/
+-rw-r--r--   0 pipi       (501) staff       (20)    21902 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6194 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/_dataplane.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10483 2023-01-14 11:38:47.000000 networklab-1.5.2.dev1/netsim/modules/_routing.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.2.dev1/netsim/modules/bfd.py
+-rw-r--r--   0 pipi       (501) staff       (20)      702 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/bfd.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    20279 2023-03-20 10:56:19.000000 networklab-1.5.2.dev1/netsim/modules/bgp.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1470 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/bgp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.2.dev1/netsim/modules/eigrp.py
+-rw-r--r--   0 pipi       (501) staff       (20)      324 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/eigrp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    17812 2022-11-13 15:34:41.000000 networklab-1.5.2.dev1/netsim/modules/evpn.py
+-rw-r--r--   0 pipi       (501) staff       (20)      892 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/evpn.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6795 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/gateway.py
+-rw-r--r--   0 pipi       (501) staff       (20)      960 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/gateway.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/modules/isis.py
+-rw-r--r--   0 pipi       (501) staff       (20)      906 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/isis.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7057 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/mpls.py
+-rw-r--r--   0 pipi       (501) staff       (20)      879 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/mpls.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3036 2023-01-14 10:57:46.000000 networklab-1.5.2.dev1/netsim/modules/ospf.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1033 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/ospf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/sr.py
+-rw-r--r--   0 pipi       (501) staff       (20)      390 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/sr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.2.dev1/netsim/modules/srv6.py
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/srv6.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    58915 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/vlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1022 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vlan.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    20566 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/vrf.py
+-rw-r--r--   0 pipi       (501) staff       (20)      431 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vrf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     9079 2022-12-11 09:34:30.000000 networklab-1.5.2.dev1/netsim/modules/vxlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)      564 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.334088 networklab-1.5.2.dev1/netsim/outputs/
+-rw-r--r--   0 pipi       (501) staff       (20)     2277 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7081 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1745 2022-01-21 21:02:25.000000 networklab-1.5.2.dev1/netsim/outputs/common.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9596 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/d2.py
+-rw-r--r--   0 pipi       (501) staff       (20)      468 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/d2.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2739 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/format.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7581 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/graph.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     5504 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.2.dev1/netsim/outputs/json.py
+-rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.2.dev1/netsim/outputs/none.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/provider.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1711 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/yaml.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.340730 networklab-1.5.2.dev1/netsim/providers/
+-rw-r--r--   0 pipi       (501) staff       (20)     7882 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/providers/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3733 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/providers/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)      517 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.2.dev1/netsim/providers/external.py
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/providers/external.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    11317 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)      481 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.2.dev1/netsim/providers/virtualbox.py
+-rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/providers/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7937 2023-04-10 09:56:31.000000 networklab-1.5.2.dev1/netsim/read_topology.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.340903 networklab-1.5.2.dev1/netsim/templates/
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.2.dev1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.187894 networklab-1.5.2.dev1/netsim/templates/provider/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341175 networklab-1.5.2.dev1/netsim/templates/provider/clab/
+-rw-r--r--   0 pipi       (501) staff       (20)     3077 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341380 networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341706 networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.342041 networklab-1.5.2.dev1/netsim/templates/provider/external/
+-rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.349287 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)      541 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:30:59.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.351375 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 pipi       (501) staff       (20)      782 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.352201 networklab-1.5.2.dev1/netsim/templates/tests/
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.2.dev1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.2.dev1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.2.dev1/netsim/templates/tests/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/topology-defaults.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.353490 networklab-1.5.2.dev1/netsim/utils/
+-rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/utils/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4068 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/utils/log.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/utils/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1277 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/utils/strings.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4906 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/utils/templates.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.354484 networklab-1.5.2.dev1/networklab.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)    20481 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       51 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      122 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        7 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      183 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/requirements.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-04-15 09:01:42.355170 networklab-1.5.2.dev1/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.2.dev1/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.354616 networklab-1.5.2.dev1/tests/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/tests/test_transformation.py
```

### Comparing `networklab-1.5.2/LICENSE.md` & `networklab-1.5.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/PKG-INFO` & `networklab-1.5.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.2
+Version: 1.5.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.2/README.md` & `networklab-1.5.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/addressing.py` & `networklab-1.5.2.dev1/netsim/addressing.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 import types
 
 import netaddr
 from box import Box
 
 # Related modules
 from . import common
-from .data import get_empty_box,get_box,null_to_string
+from .data import get_empty_box,null_to_string
 from .data.validate import validate_attributes
 
 def normalize_prefix(pfx: typing.Union[str,Box]) -> Box:
 
   # Normalize IP addr strings, e.g. 2001:001::/48 becomes 2001:1::/48
   def normalize_ip(ip:typing.Union[str,bool]) -> typing.Union[str,bool]:
     try:
@@ -69,37 +69,37 @@
       common.error(
         f'Cannot parse address prefix: {ex}',
         common.IncorrectValue,
         'addressing')
       return False
 
   if not pfx:
-    return get_empty_box()
+    return Box({},default_box=True,box_dots=True)
   if not isinstance(pfx,dict):
-    return get_box({ 'ipv4': normalize_ip(pfx) })
+    return Box({ 'ipv4': normalize_ip(pfx) },default_box=True,box_dots=True)
   for af in 'ipv4','ipv6':
     if af in pfx:
       if not pfx[af] or 'unnumbered' in pfx:  # If 'unnumbered' is set, ipv4/ipv6 will be based on loopback afs (per node)
         del pfx[af]
       else:
         pfx[af] = normalize_ip(pfx[af])
 
   return pfx
 
 def rebuild_prefix(pfx: typing.Union[dict,Box]) -> Box:
-  out_pfx = get_empty_box()
+  out_pfx = Box({})
   for af in ('ipv4','ipv6'):
     if af in pfx:
       out_pfx[af] = str(pfx[af]) if not isinstance(pfx[af],bool) else pfx[af]
   return out_pfx
 
 def setup_pools(addr_pools: typing.Optional[Box] = None, defaults: typing.Optional[Box] = None) -> Box:
-  addrs = addr_pools or get_empty_box()
-  defaults = defaults or get_empty_box()
-  legacy = get_empty_box()
+  addrs = addr_pools or Box({},default_box=True)
+  defaults = defaults or Box({},default_box=True)
+  legacy = Box({},default_box=True)
 
   legacy.lan = { 'ipv4': defaults.get('lan','10.0.0.0/16'), 'prefix': defaults.get('lan_subnet',24) }
   if not 'lan' in defaults and not 'lan' in addrs:
     legacy['lan']['start'] = 1
   legacy.loopback = { 'ipv4': (defaults.get('loopback','10.0.0.%d') % 0) + '/24', 'prefix': 32 }
   legacy.p2p = { 'ipv4': defaults.get('p2p','10.2.0.0/16'), 'prefix': defaults.get('p2p_subnet',30) }
 
@@ -123,15 +123,15 @@
       data_name=f'address pool',
       attr_list=['pool'],                             # We're checking address pool attributes
       modules=[],                                     # No module attributes in pools yet
 #      modules=n_data.get('module',[]),                # ... against node modules
       module='addressing')
 
   if not addrs:       # pragma: no cover (pretty hard not to have address pools)
-    addrs = get_empty_box()
+    addrs = Box({})
   for k in ('lan','loopback'):
     if not k in addrs:          # pragma: no cover (lan and loopback pools are always created in setup_pools)
       common.error(
         "'%s' addressing pool is missing" % k,
         category=common.MissingValue,
         module='addressing')
 
@@ -280,15 +280,15 @@
 def get(pools: Box, pool_list: typing.Optional[typing.List[str]] = None, n: typing.Optional[int] = None) -> Box:
   if not pool_list:
     pool_list = ['lan']                   # pragma: no cover
   p = get_pool(pools,pool_list)
   if p:
     return get_pool_prefix(pools,p,n)
   else:
-    return get_empty_box()                # pragma: no cover -- can't figure out how to get here
+    return Box({})                        # pragma: no cover -- can't figure out how to get here
 
 def setup(topology: Box) -> None:
   defaults = topology.defaults
   null_to_string(topology.addressing)
   addrs = setup_pools(defaults.addressing + topology.addressing,defaults)
 
   if common.debug_active('addressing'):
@@ -312,17 +312,17 @@
     print(f"parse prefix: {prefix} type={type(prefix)}")
 
   empty_box = get_empty_box()
   if not prefix:
     return empty_box
 
   supported_af = ['ipv4','ipv6']
-  prefix_list = get_empty_box()
+  prefix_list = Box({})
   if not isinstance(prefix,Box):
-    return get_box({ 'ipv4' : netaddr.IPNetwork(prefix) })
+    return Box({ 'ipv4' : netaddr.IPNetwork(prefix) })
 
   if 'ip' in prefix:                                  # Deal with legacy 'ip' address family -- rename it to ipv4
     if 'ipv4' in prefix:
       common.error( \
         f'Cannot have IP and IPv4 address families in prefix {prefix}',
         category=common.IncorrectValue,
         module='addressing')
```

### Comparing `networklab-1.5.2/netsim/ansible/collect-configs.ansible` & `networklab-1.5.2.dev1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/config.ansible` & `networklab-1.5.2.dev1/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/create-config.ansible` & `networklab-1.5.2.dev1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/initial-config.ansible` & `networklab-1.5.2.dev1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/create-config.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/api.py` & `networklab-1.5.2.dev1/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/augment/components.py` & `networklab-1.5.2.dev1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/augment/config.py` & `networklab-1.5.2.dev1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/augment/devices.py` & `networklab-1.5.2.dev1/netsim/augment/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 import typing
 
 from box import Box
 
 from .. import common
-from .. import data
 
 """
 Get generic device attribute:
 
 * Use node.device to find device used by the current node
 * Use defaults.provider (future: node data) to find the provider
 * Fetch required data using the following inheritance rules:
@@ -48,19 +47,19 @@
 
 """
 Get device feature flags -- uses get_device_attribute but returns a Box to keep mypy happy
 """
 def get_device_features(node: Box, defaults: Box) -> Box:
   features = get_device_attribute(node,'features',defaults)
   if not features:
-    return data.get_empty_box()
+    return Box({},default_box=True,box_dots=True)
 
   if not isinstance(features,Box):
     common.fatal('Device features for device type {node.device} should be a dictionary')
-    return data.get_empty_box()
+    return Box({})
 
   return features
 
 """
 Get all device data for current provider
 """
 def get_provider_data(node: Box, defaults: Box) -> Box:
```

### Comparing `networklab-1.5.2/netsim/augment/groups.py` & `networklab-1.5.2.dev1/netsim/augment/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from box import Box
 
 from .. import common
 from .. import data
 from .. import modules
 from ..modules import bgp
-from ..data import get_box,get_empty_box
+from ..data import get_box
 from ..data.validate import validate_attributes
 from ..data.types import must_be_dict,must_be_list,must_be_string,must_be_id
 from . import nodes
 
 '''
 Return members of the specified group. Recurse through child groups if needed
 '''
@@ -44,15 +44,15 @@
   return members
 
 '''
 Check validity of 'groups' data structure
 '''
 def check_group_data_structure(topology: Box) -> None:
   if not 'groups' in topology:
-    topology.groups = get_empty_box()
+    topology.groups = Box({},default_box=True,box_dots=True)
 
   if must_be_dict(topology,'groups','topology',create_empty=True,module='groups') is None:
     return
 
   '''
   Transform group-as-list into group-as-dictionary
   '''
@@ -67,40 +67,38 @@
 
   '''
   Sanity checks on global group data
   '''
 
   list_of_modules = modules.list_of_modules(topology)
   group_attr = topology.defaults.attributes.group
-
-  extra = list(topology.defaults.providers.keys())        # Allow provider-specific node attributes
-  extra.extend(list(topology.get('tools',{}).keys()))     # ... plus tool-specific attributes
+  providers = list(topology.defaults.providers.keys())
   for grp,gdata in topology.groups.items():
     must_be_id(parent=None,key=grp,path=f'NOATTR:group name {grp}',module='groups')
     if must_be_dict(topology.groups,grp,'topology.groups',create_empty=True,module='groups') is None:
       continue
 
     gpath=f'topology.groups.{grp}'
     g_modules = gdata.get('module',[])
-    if g_modules:                           # Modules specified in the group -- we know what these nodes will use
+    if g_modules:                          # Modules specified in the group -- we know what these nodes will use
       gm_source = 'group'
     else:
       gm_source = 'topology'
       g_modules = topology.get('module',[])
 
     validate_attributes(
       data=gdata,
       topology=topology,
       data_path=gpath,
       data_name='group',
       attr_list=[ 'group','node' ],
       module='groups',
       modules=g_modules,
       module_source=gm_source,
-      extra_attributes=extra)               # Allow provider- and tool-specific settings (not checked at the moment)
+      extra_attributes=providers)          # Allow provider-specific settings (not checked at the moment)
 
     if not 'members' in gdata:
       gdata.members = []
 
     if grp == 'all' and gdata.members:
       common.error('Group "all" should not have explicit members')
 
@@ -116,15 +114,15 @@
         topology=topology,
         data_path=f'{gpath}.node_data',
         data_name='node',
         attr_list=[ 'node' ],
         module='groups',
         modules=g_modules,
         module_source=gm_source,
-        extra_attributes=extra)              # Allow provider- and tool-specific settings (not checked at the moment)
+        extra_attributes=providers)          # Allow provider-specific settings (not checked at the moment)
 
       for k in ('module','device'):          # Check that the 'module' or 'device' attributes are not in node_data
         if k in gdata.node_data:
           common.error(
             f'Cannot use attribute {k} in node_data in group {grp}, set it as a group attribute',
             common.IncorrectValue,
             'groups')
@@ -183,15 +181,15 @@
 
 def check_recursive_groups(topology : Box) -> None:
   for gname in topology.groups.keys():
     if check_recursive_chain(topology,[],gname):
       return
 
 def reverse_topsort(topology: Box) -> list:
-  group_copy = get_box(topology.groups)        # Make a copy of the group dictionary
+  group_copy = Box(topology.groups)            # Make a copy of the group dictionary
   sort_list: typing.List[str] = []
   while group_copy:                            # Keep iterating until we got all groups in order
     for g in sorted(group_copy.keys()):        # Iterate over remaining groups
       OK_to_add = True                         # ... sort them by name to have consistent results
       for m in group_copy[g].members:          # Now go check the group members
         if m in group_copy:                    # ... if a member of this group is still in groups we're not yet ready
           OK_to_add = False                    # ... to add it to sorted list
@@ -256,15 +254,15 @@
       print(f'copy node data {grp}: {gdata.node_data}')
     for name in g_members:                                            # Iterate over group members
       if not name in topology.nodes:                                  # Member is not a node, skip it
         continue
 
       if common.debug_active('groups'):
         print(f'... merging node data with {name}')
-      merge_data = data.get_box(gdata.node_data)
+      merge_data=Box(gdata.node_data)
       if 'module' in topology.nodes[name]:
         for m in topo_modules:
           if not m in topology.nodes[name].module:
             merge_data.pop(m,None)
 
       topology.nodes[name] = merge_data + topology.nodes[name]
 
@@ -334,19 +332,15 @@
     n_module = n_data.get('module',g_module)                    # Get node or global module (global modules haven't been propagated yet)
     if not isinstance(n_module,list):                           # Node list of modules is insane, someone else will complain
       continue
 
     if not 'bgp' in n_module:                                   # Looks like this node does not care about BGP
       continue
 
-    try:
-      n_bgpas = n_data.get('bgp.as') or g_bgpas                 # Get node-level or global BGP AS
-    except:
-      n_bgpas = g_bgpas
-
+    n_bgpas = data.get_from_box(n_data,'bgp.as') or g_bgpas     # Get node-level or global BGP AS
     if not n_bgpas:
       continue
 
     grpname = f"as{n_bgpas}"                                    # BGP auto-group name
     if not 'members' in topology.groups[grpname]:               # Set members of a new group to an empty list
       topology.groups[grpname].members = []                     # ... because we're using Box this also creates an empty group dict
```

### Comparing `networklab-1.5.2/netsim/augment/links.py` & `networklab-1.5.2.dev1/netsim/augment/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,27 @@
 from .. import data
 from .. import utils
 from ..data.validate import validate_attributes
 from ..data.types import must_be_string,must_be_list,must_be_dict,must_be_id
 from .. import addressing
 from . import devices
 
-VIRTUAL_INTERFACE_TYPES: typing.Final[typing.List[str]] = [
-  'loopback', 'tunnel' ]
-
 def adjust_interface_list(iflist: list, link: Box, nodes: Box) -> list:
   link_intf = []
   intf_cnt  = 0
   for n in iflist:                      # Sanity check of interface data
     intf_cnt = intf_cnt + 1
     if isinstance(n,str):               # Another shortcut: node name as string
       if not n in nodes:                # ... is it a valid node name?
         common.error(                   # ... it's not, get lost
           f'Interface {link._linkname}.interfaces.{intf_cnt} refers to an unknown node {n}',
           common.IncorrectValue,
           'links')
         continue
-      n = data.get_box({ 'node': n })
+      n = Box({ 'node': n },default_box=True,box_dots=True)
       
     if not isinstance(n,Box):          # Still facing non-dict data type?
       common.error(                     # ... report an error
         f'Interface data in {link._linkname}.interfaces[{intf_cnt}] must be a dictionary, found {type(n).__name__}',
         common.IncorrectValue,
         'links')
     elif not 'node' in n:               # Do we have node name in interface data?
@@ -201,72 +198,56 @@
     ifindex_offset = 1
 
   # Allow user to select a specific interface index per link
   ifindex = ifdata.get('ifindex',None)
 
   # When computing default ifindex, consider only non-loopback interfaces
   if not ifindex:
-   ifindex = len([
-               intf for intf in node.interfaces
-                 if not intf.get('type',None) in VIRTUAL_INTERFACE_TYPES
-                 ]) + ifindex_offset
+   ifindex = len([intf for intf in node.interfaces if intf.get('type',None) != 'loopback']) + ifindex_offset
 
   ifname_format = devices.get_device_attribute(node,'interface_name',defaults)
 
   ifdata.ifindex = ifindex
   if ifname_format and not 'ifname' in ifdata:
     ifdata.ifname = utils.strings.eval_format(ifname_format,ifdata)
 
   pdata = devices.get_provider_data(node,defaults).get('interface',{})
-  pdata = data.get_box(pdata)                     # Create a copy of the provider interface data
+  pdata = Box(pdata,box_dots=True,default_box=True)                     # Create a copy of the provider interface data
   if 'name' in pdata:
     pdata.name = utils.strings.eval_format(pdata.name,ifdata)
 
   if pdata:
     provider = devices.get_provider(node,defaults)
     ifdata[provider] = pdata
 
-def create_virtual_interface(node: Box, ifdata: Box, defaults: Box) -> None:
-  devtype = ifdata.get('type','loopback')         # Get virtual interface type, default to loopback interface
-  ifindex_offset = (
-    devices.get_device_attribute(node,f'{devtype}_offset',defaults) or
-    1 if devtype == 'loopback' else 0)            # Loopback interfaces have to start with 1 to prevent overlap with built-in loopback
-
+def create_loopback_interface(node: Box, ifdata: Box, defaults: Box) -> None:
+  ifindex_offset = devices.get_device_attribute(node,'loopback_offset',defaults) or 0
+  ifdata.ifindex = ifindex_offset + ifdata.linkindex
   ifdata.virtual_interface = True
-  ifdata.pop('bridge',None)
+  ifname_format  = devices.get_device_attribute(node,'loopback_interface_name',defaults)
 
-  if not 'ifindex' in ifdata:
-    ifdata.ifindex = len([intf for intf in node.interfaces if intf.get('type',None) == devtype]) + ifindex_offset
-  ifname_format  = devices.get_device_attribute(node,f'{devtype}_interface_name',defaults)
+  if not ifname_format:
+    common.error(
+      f'Device {node.device}/node {node.name} does not support loopback links',
+      common.IncorrectValue,
+      'links')
+    return
 
   if not 'ifname' in ifdata:
-    if not ifname_format:
-      if devtype == 'loopback':
-        common.error(
-          f'Device {node.device}/node {node.name} does not support loopback links',
-          common.IncorrectValue,
-          'links')
-        return
-      else:
-        print(ifdata)
-        common.error(
-          f'Need explicit interface name (ifname) for {devtype} interface on node {node.name} ({node.device})',
-          common.IncorrectValue,
-          'links')
-        return
     ifdata.ifname = utils.strings.eval_format(ifname_format,ifdata)
 
-  # Adjust ifindex to prevent overlap between device types
+  # If the device uses 'loopback_offset' then we're assuming it's large enough to prevent overlap with physical interfaces
+  # Otherwise, create fake ifindex for loopback interfaces to prevent that overlap
   #
-  ifindex_offset = (VIRTUAL_INTERFACE_TYPES.index(devtype)+1) * 10000
-  ifdata.ifindex += ifindex_offset
+  if not ifindex_offset:
+    ifdata.ifindex = 10000 + ifdata.ifindex
 
 def add_node_interface(node: Box, ifdata: Box, defaults: Box) -> Box:
-  if ifdata.get('type',None) in VIRTUAL_INTERFACE_TYPES:
-    create_virtual_interface(node,ifdata,defaults)
+  if ifdata.get('type') == 'loopback':
+    create_loopback_interface(node,ifdata,defaults)
   else:
     create_regular_interface(node,ifdata,defaults)
 
   for af in ('ipv4','ipv6'):
     if af in ifdata and not ifdata[af]:
       del ifdata[af]
 
@@ -296,27 +277,19 @@
       if not k in ifdata:
         ifdata[k] = link[k]
       elif isinstance(link[k],dict) and isinstance(ifdata[k],dict):
         ifdata[k] = link[k] + ifdata[k]
   return ifdata
 
 """
-Get gateway ID -- return None if not set or if 'gateway' is not a dict
-"""
-def get_gateway_id(link: Box) -> typing.Optional[int]:
-  if not isinstance(link.get('gateway',None),Box):
-    return None
-  return link.gateway.get('id',None)
-
-"""
 Set FHRP (anycast/VRRP/...) gateway on a link
 """
 
 def set_fhrp_gateway(link: Box, pfx_list: Box, nodes: Box, link_path: str) -> None:
-  gwid = get_gateway_id(link)
+  gwid = data.get_from_box(link,'gateway.id')
   if not gwid:                                                        # No usable gateway ID, nothing to do
     return
 
   fhrp_assigned = False
   for af in common.AF_LIST:
     if not af in pfx_list or isinstance(pfx_list[af],bool):           # No usable IPv4/IPv6 prefix, nothing to do
       continue
@@ -370,15 +343,15 @@
     if isinstance(link.prefix,str):
       link.prefix = addressing.rebuild_prefix(pfx_list)   # convert str to prefix dictionary
 
     set_fhrp_gateway(link,pfx_list,nodes,link_path)
     return pfx_list
 
   if 'unnumbered' in link:                                # User requested an unnumbered link
-    link.prefix = data.get_box({ 'unnumbered': True })
+    link.prefix = Box({ 'unnumbered': True })
     return link.prefix
 
   if must_be_string(link,'pool',link_path):
     if not link.pool in addr_pools:
       common.error(
         f'Unknown address pool {link.pool} used in {link_path}',
         common.IncorrectValue,
@@ -408,39 +381,39 @@
 
 Return 'error' if the prefix size is too small
 """
 def get_prefix_IPAM_policy(link: Box, pfx: typing.Union[netaddr.IPNetwork,bool], ndict: Box) -> str:
   if isinstance(pfx,bool):
     return 'unnumbered'
 
-  gwid = get_gateway_id(link) or 0                                    # Get link gateway ID (if set) --- must be int for min to work
+  gwid = data.get_from_box(link,'gateway.id') or 0                    # Get link gateway ID (if set) --- must be int for min to work
   if link.type == 'p2p' and not gwid:                                 # P2P allocation policy cannot be used with default gateway
     return 'p2p' if pfx.first != pfx.last else 'error'
 
   pfx_size = pfx.last - pfx.first + 1
   add_extra_ip = 0
   subtract_reserved_ip = -2
 
   if pfx_size > 2:
     if gwid > 0:                                                      # Gateway ID at the front of the subnet -- need one extra IP
       add_extra_ip = 1
     if gwid < 0:                                                      # Don't allow node address allocation beyond last-in-subnet gateway
-      subtract_reserved_ip = min(subtract_reserved_ip,gwid-1)
+      subtract_reserved_ip = min(subtract_reserved_ip,gwid)
 
     pfx_size = pfx_size + subtract_reserved_ip
 
   max_id = max([ ndict[intf.node].id for intf in link.interfaces if intf.node in ndict ])
-  if pfx_size == 1:                                                   # Do we have a single node attached to a /32 link?
-    return 'loopback' if len(link.interfaces) == 1 else 'error'       # ... if so, we'll use loopback address allocation
-
-  if max_id <= pfx_size:                                              # If we can fit all node IDs attached to this link into the prefix
+  if max_id < pfx_size:                                               # If we can fit all node IDs attached to this link into the prefix
     return 'id_based'                                                 # ... we'll use ID-based address allocation
-  if len(link.interfaces) + add_extra_ip <= pfx_size:                 # Otherwise, if the prefix is big enough
+  if len(link.interfaces) + add_extra_ip < pfx_size:                  # Otherwise, if the prefix is big enough
     return 'sequential'                                               # ... we'll use sequential address allocation
 
+  if pfx_size < 2 and link.type == 'loopback':                        # Final straw: maybe we're dealing with a loopback?
+    return 'loopback'
+
   return 'error'
 
 """
 Get Nth IP address in a prefix returned as a nice string with a subnet mask
 
 *** WARNING *** WARNING *** WARNING ***
 
@@ -504,24 +477,24 @@
 Unnumbered AF IPAM -- set interface address to 'True'
 
 If the interface address is set, validate that it's a valid address (can't be int)
 """
 def IPAM_unnumbered(link: Box, af: str, pfx: typing.Optional[bool], ndict: Box) -> None:
   for intf in link.interfaces:
     if not af in intf:            # No static address, set it to link bool value or use loopback AF presence for old-style unnumbereds
-      intf[af] = pfx if isinstance(pfx,bool) else bool(ndict[intf.node].get(f'loopback.{af}',False))
+      intf[af] = pfx if isinstance(pfx,bool) else bool(data.get_from_box(ndict[intf.node],f'loopback.{af}'))
     elif data.is_true_int(intf[af]):
       common.error(
         f'Node {intf.node} is using host index {intf[af]} for {af} on an unnumbered link',
         common.IncorrectValue,
         'links')
 
 def IPAM_sequential(link: Box, af: str, pfx: netaddr.IPNetwork, ndict: Box) -> None:
   start = 1 if pfx.last != pfx.first + 1 else 0
-  gwid = get_gateway_id(link)
+  gwid = data.get_from_box(link,'gateway.id')
   for count,intf in enumerate(link.interfaces):
     if count + start == gwid:                                   # Would the next address overlap with gateway ID
       start = start + 1                                         # ... no big deal, just move the starting point ;)
     set_interface_address(intf,af,pfx,count+start)
 
 def IPAM_p2p(link: Box, af: str, pfx: netaddr.IPNetwork, ndict: Box) -> None:
   start = 1 if pfx.last != pfx.first + 1 else 0
@@ -589,15 +562,15 @@
       if 'allocation' in pfx_list:
         allocation_policy = pfx_list.allocation
       else:
         allocation_policy = get_prefix_IPAM_policy(link,pfx_net,ndict)    # get IPAM policy based on prefix and link size
 
     if allocation_policy == 'error':                                      # Something went wrong, cannot assing IP addresses
       rq = f'{len(link.interfaces)} nodes'
-      if get_gateway_id(link):
+      if data.get_from_box(link,'gateway.id'):
         rq = rq + f' plus first-hop gateway'
       common.error(
         f'Cannot use {af} prefix {pfx_list[af]} to address {rq} on {link._linkname}\n' + \
         common.extra_data_printout(f'link data: {link}',width=90),
         common.IncorrectValue,
         'links')
       continue
@@ -679,15 +652,15 @@
     node = value.node
     #
     # Create node interface data from interfaces attributes augmented with link attributes
     # and node-relevant link module attributes
     ifdata = interface_data(
                 link=link,
                 link_attr=link_attr_propagate.union(ndict[node].get('module',[])) - set(defaults.attributes.link_module_no_propagate),
-                ifdata=data.get_box(value))
+                ifdata=Box(value))
     set_interface_name(ifdata,link,intf_cnt)
     ifdata.pop('node',None)                                       # Remove the node name (not needed within the node)
     node_intf = add_node_interface(ndict[node],ifdata,defaults)   # Attach new interface to its node
     value.ifindex = node_intf.ifindex                             # Save ifindex and ifname in link interface data
     value.ifname  = node_intf.ifname                              # ... needed for things like Graph output module that works with links
     interfaces.append({ 'node': node, 'data': node_intf })        # Save newly-created interface for the next step
                                                                   # ... must use dict not Box as Box creates a copy of the data structure
@@ -701,15 +674,15 @@
     ifdata = node_if['data']                                      # Get a pointer to interface data
     ifdata.neighbors = []
     for remote_if in interfaces:                                  # Iterate over all interfaces created from this link
       if remote_if is node_if:                                    # ... and skip the current interface
         continue
       remote_node = remote_if['node']                             # Remote node name in a handier format
       remote_ifdata = remote_if['data']                           # ... and a pointer to remote interface data
-      ngh_data = data.get_box({ 'ifname': remote_ifdata.ifname, 'node': remote_node })
+      ngh_data = Box({ 'ifname': remote_ifdata.ifname, 'node': remote_node })
       #
       # Find relevant modules that have interface attributes
       mods_with_attr = set([ m for m in ndict[remote_node].get('module',[])
                               if defaults[m].attributes.get('interface',None) or
                                  defaults[m].attributes.get('link_to_neighbor',None) ])
       #
       # Merge neighbor module data + AF with baseline neighbor data
@@ -799,14 +772,20 @@
   if link_type == 'loopback' and node_cnt != 1:
     common.error(
       f'Looopback link {data._linkname} can have a single node attached\n... {data}',
       common.IncorrectValue,
       'links')
     return False
 
+  if not link_type in [ 'stub','p2p','lan','loopback','vlan_member']:
+    common.error(
+      f'Invalid link type {link_type} in {data._linkname}\n... {data}',
+      common.IncorrectValue,
+      'links')
+    return False
   return True
 
 #
 # Interface Feature Check -- validate that the selected addressing works on target lab devices
 #
 
 def interface_feature_check(nodes: Box, defaults: Box) -> None:
```

### Comparing `networklab-1.5.2/netsim/augment/main.py` & `networklab-1.5.2.dev1/netsim/augment/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     augment.links.links_init(topology)
 
   augment.components.expand_components(topology)
 
   augment.devices.augment_device_settings(topology)
   augment.plugin.init(topology)                                         # Initialize plugins very early on in case they modify extra attributes
   augment.plugin.execute('init',topology)
-  augment.topology.check_tools(topology)
   common.exit_on_error()
 
   augment.topology.extend_attribute_list(topology.defaults)             # Attributes have to be extended before group init
   augment.topology.extend_module_attribute_list(topology)               # ... or we won't recognize node attributes in groups
   augment.groups.init_groups(topology)
   common.exit_on_error()
```

### Comparing `networklab-1.5.2/netsim/augment/nodes.py` & `networklab-1.5.2.dev1/netsim/augment/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 * Set loopback and management interface data
 '''
 import typing
 
 from box import Box
 
 from .. import common
-from .. import data
 from .. import utils
 from .. import addressing
 from .. import providers
 from . import devices
 from ..data.validate import validate_attributes
 from ..data.types import must_be_int,must_be_string,must_be_id
 from ..modules._dataplane import extend_id_set,is_id_used,set_id_counter,get_next_id
@@ -36,28 +35,28 @@
 Or lists of strings into a unified dictionary structure
 """
 
 def create_node_dict(nodes: Box) -> Box:
   if isinstance(nodes,dict):
     node_dict = nodes
   else:
-    node_dict = data.get_empty_box()
+    node_dict = Box({},default_box=True,box_dots=True)
     for n in nodes or []:
       if isinstance(n,dict):
         if not 'name' in n:
           common.error(f'Node is missing a "name" attribute: {n}',common.IncorrectValue,'nodes')
           continue
       elif isinstance(n,str):
-        n = data.get_box({ 'name': n })
+        n = Box({ 'name': n },default_box=True,box_dots=True)
       node_dict[n.name] = n
 
   for name in list(node_dict.keys()):
     ndata = node_dict[name]
     if ndata is None:
-      ndata = data.get_box({'name': name})
+      ndata = Box({'name': name},default_box=True)
     elif not isinstance(ndata,dict):
       common.error(f'Node data for node {name} must be a dictionary')
       node_dict[name] = { 'name': name, 'extra': ndata }
       ndata = node_dict[name]
     else:
       ndata['name'] = name
 
@@ -69,25 +68,24 @@
 
 """
 Validate node attributes
 """
 def validate(topology: Box) -> None:
   for n_name,n_data in topology.nodes.items():
     must_be_id(parent=None,key=n_name,path=f'NOATTR:node name {n_name}',module='nodes')
-    extra = list(topology.defaults.providers.keys())        # Allow provider-specific node attributes
-    extra.extend(list(topology.get('tools',{}).keys()))     # ... plus tool-specific attributes
+    providers = list(topology.defaults.providers.keys())
     validate_attributes(
       data=n_data,                                    # Validate node data
       topology=topology,
       data_path=f'nodes.{n_name}',                    # Topology path to node name
       data_name=f'node',
       attr_list=['node'],                             # We're checking node attributes
       modules=n_data.get('module',[]),                # ... against node modules
       module='nodes',                                 # Function is called from 'nodes' module
-      extra_attributes=extra)                         # Allow provider- and tool-specific settings
+      extra_attributes = providers)                   # Allow provider-specific settings (not checked at the moment)
 
 def augment_mgmt_if(node: Box, defaults: Box, addrs: typing.Optional[Box]) -> None:
   if 'ifname' not in node.mgmt:
     mgmt_if = devices.get_device_attribute(node,'mgmt_if',defaults)
     if not mgmt_if:
       ifname_format = devices.get_device_attribute(node,'interface_name',defaults)
       if not isinstance(ifname_format,str):
@@ -358,12 +356,12 @@
 
 '''
 Return a copy of the topology (leaving original topology unchanged) with unmanaged devices removed
 '''
 def ghost_buster(topology: Box) -> Box:
   common.print_verbose('Removing unmanaged devices from topology')
   # Create a copy of topology
-  topo_copy = data.get_box(topology)
+  topo_copy = Box(topology,default_box=True,box_dots=True)
   
   # Remove all nodes with "unmanaged" flag set
   topo_copy.nodes = { k:v for k,v in topo_copy.nodes.items() if not v.get('unmanaged',False) }  
   return topo_copy
```

### Comparing `networklab-1.5.2/netsim/augment/plugin.py` & `networklab-1.5.2.dev1/netsim/augment/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,18 @@
       return None
 
   module_name = plugin.replace('.py','')
   module_name = f'netlab.plugin.{module_name}'
 
   try:
     modspec  = importlib.util.spec_from_file_location(module_name,module_path)
-    assert(modspec is not None)
+    assert(isinstance(modspec,importlib.machinery.ModuleSpec))
     pymodule = importlib.util.module_from_spec(modspec)
     sys.modules[module_name] = pymodule
-    assert(modspec.loader is not None)
+    assert(isinstance(modspec.loader,importlib.abc.Loader))
     modspec.loader.exec_module(pymodule)
   except:
     print(f"Cannot load plugin {module_name} from {module_path}\n{str(sys.exc_info()[1])}")
     common.fatal('Aborting the transformation process','plugin')
 
   if config_name:
     setattr(pymodule,'config_name',config_name)
```

### Comparing `networklab-1.5.2/netsim/augment/topology.py` & `networklab-1.5.2.dev1/netsim/augment/topology.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 '''
 
 import os
 from box import Box
 
 from .. import common
 from .. import data
-from ..data.validate import validate_attributes
-from ..data.types import must_be_list,must_be_string,must_be_dict
+from ..data.validate import must_be_list,validate_attributes,must_be_string
 
 #
 # Extend link/node/global attribute lists with extra attributes
 #
 def extend_attribute_list(settings: Box, attribute_path: str = 'topology.defaults', always_valid: list = []) -> None:
   if not 'extra_attributes' in settings:
     return
@@ -69,16 +68,14 @@
       invalid_topo = True
 
   if invalid_topo:
     common.fatal("Fatal topology errors, aborting")
 
   if not 'name' in topology:
     topo_name = os.path.basename(os.path.dirname(os.path.realpath(topology['input'][0])))[:12]
-    for bad_char in (' ','.'):
-      topo_name = topo_name.replace(bad_char,'_')
     topology.name = topo_name
 
   if 'module' in topology:
     must_be_list(topology,'module','')
     topology.defaults.module = topology.module
 
   if must_be_string(topology,'name','',module='topology'):
@@ -92,56 +89,14 @@
     data_path='topology',                           # Topology path to node name
     data_name=f'topology',
     attr_list=['global','internal'],                # We're checking global (+ internal) attributes
     modules=topology.get('module',[]),              # ... against topology modules
     module='topology',                              # Function is called from 'nodes' module
     extra_attributes = providers)                   # Allow provider-specific settings (not checked at the moment)
 
-"""
-Check the 'tools' section of the topology file
-
-* Tools section must be a dictionary
-"""
-def check_tools(topology: Box) -> None:
-  if not 'tools' in topology:
-    return
-
-  try:
-    must_be_dict(topology,'tools','',module='topology',abort=True)
-  except:
-    topology.pop('tools')
-    return
-
-  for tool in topology.tools.keys():                # Iterate over tools     
-    must_be_dict(                                   # Make sure the tool configuration is a dictionary    
-      parent=topology.tools,
-      key=tool,path=f'topology.tools',
-      create_empty=True,
-      module='topology')
-    if not isinstance(topology.tools[tool],dict):   # Skip if we have an error
-      continue
-    if not tool in topology.defaults.tools:         # Check that the tool is valid
-      common.error(
-        f'Invalid tool {tool}\n... valid tools are {",".join(topology.defaults.tools.keys())}',
-        common.IncorrectValue,
-        'topology')
-      continue
-    if not 'runtime' in topology.tools[tool]:       # Check that the tool has a runtime defined
-      topology.tools[tool].runtime = 'docker'       # Default is Docker
-
-    # Merge tool defaults and tool-specific settings, then check that the runtime is valid
-    #
-    tool_data = topology.defaults.tools[tool] + topology.tools[tool] 
-    if not tool_data[tool_data.runtime] or not 'up' in tool_data[tool_data.runtime]:            
-      valid_runtimes = [k for k in tool_data.keys() if 'up' in k ]
-      common.error(
-        f'Invalid runtime {tool_data.runtime} for tool {tool}\n... valid runtimes are {",".join(valid_runtimes)}',
-        common.IncorrectValue,
-        'topology')
-
 #
 # Find virtualization provider, set provider and defaults.provider to that value
 #
 # Note: defaults.provider is needed in some output routines that get defaults data structure
 # but not the whole topology
 #
 def adjust_global_parameters(topology: Box) -> None:
@@ -168,15 +123,15 @@
       topology.defaults[k] = topology.defaults[k] + topology.defaults.providers[topology.provider][k]
 
 #
 # Cleanup the topology
 #
 
 def cleanup_topology(topology: Box) -> Box:
-  topo_copy = Box(topology,box_dots=True)
+  topo_copy = Box(topology)
 
   # Remove PFX generators from addressing section
   #
   for k,v in topo_copy.addressing.items():
     for p in list(v.keys()):
       if "_pfx" in p or "_eui" in p:
         v.pop(p,None)
```

### Comparing `networklab-1.5.2/netsim/callback.py` & `networklab-1.5.2.dev1/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/__init__.py` & `networklab-1.5.2.dev1/netsim/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 from box import Box
 
 from . import usage
 from .. import augment, common, read_topology
 from .. import __version__
 from ..utils import status
-
-DRY_RUN: bool = False
+from ..data import get_from_box
 
 def common_parse_args(debugging: bool = False) -> argparse.ArgumentParser:
   parser = argparse.ArgumentParser(description='Common argument parsing',add_help=False)
   parser.add_argument('--log', dest='logging', action='store_true',
                   help='Enable basic logging')
   parser.add_argument('-q','--quiet', dest='quiet', action='store_true',
                   help='Report only major errors')
@@ -46,47 +45,28 @@
                   help='Local topology defaults file')
   parser.add_argument('-d','--device', dest='device', action='store', help='Default device type')
   parser.add_argument('-p','--provider', dest='provider', action='store',help='Override virtualization provider')
   parser.add_argument('--plugin',dest='plugin',action='append',help='Additional plugin(s)')
   parser.add_argument('-s','--set',dest='settings', action='append',help='Additional parameters added to topology file')
   return parser
 
-def set_dry_run(args: argparse.Namespace) -> None:
-  global DRY_RUN
-
-  if 'dry_run' in args:
-    DRY_RUN = args.dry_run
-  else:
-    DRY_RUN = False
-
-def is_dry_run() -> bool:
-  global DRY_RUN
-  return DRY_RUN
-
 #
 # Common file/directory cleanup routine, used by collect/clab/down
 #
 
 def fs_cleanup(filelist: typing.List[str], verbose: bool = False) -> None:
-  global DRY_RUN
   for fname in filelist:
     if os.path.isdir(fname):
-      if DRY_RUN:
-        print(f"DRY RUN: removing directory tree {fname}")
-        continue
       if verbose:
         print(f"... removing directory tree {fname}")
       try:
         shutil.rmtree(fname)
       except Exception as ex:
         common.fatal(f"Cannot clean up directory {fname}: {ex}")
     elif os.path.exists(fname):
-      if DRY_RUN:
-        print(f"DRY RUN: removing {fname}")
-        continue
       if verbose:
         print(f"... removing {fname}")
       try:
         os.remove(fname)
       except Exception as ex:
         common.fatal(f"Cannot remove {fname}: {ex}")
 
@@ -101,27 +81,14 @@
     read_topology.add_cli_args(topology,args)
 
   common.exit_on_error()
   return topology
 
 # Snapshot-or-topology loader (used by down)
 
-def load_snapshot(args: typing.Union[argparse.Namespace,Box]) -> Box:
-  if not os.path.isfile(args.snapshot):
-    print(f"The topology snapshot file {args.snapshot} does not exist.\n"+
-          "Looks like no lab was started from this directory")
-    sys.exit(1)
-
-  topology = read_topology.read_yaml(filename=args.snapshot)
-  if topology is None:
-    print(f"Cannot read the topology snapshot file {args.snapshot}")
-    sys.exit(1)
-
-  return topology
-
 def load_snapshot_or_topology(args: typing.Union[argparse.Namespace,Box]) -> typing.Optional[Box]:
   common.set_logging_flags(args)
   if args.device or args.provider or args.settings:     # If we have -d, -p or -s flag
     if not args.topology:                               # ... then the user wants to use the topology file
       args.topology = 'topology.yml'                    # ... so let's set the default value if needed
 
   if args.topology:
@@ -133,16 +100,15 @@
     args.snapshot = args.snapshot or 'netlab.snapshot.yml'
     return read_topology.read_yaml(filename=args.snapshot)
 
 # get_message: get action-specific message from topology file
 #
 
 def get_message(topology: Box, action: str, default_message: bool = False) -> typing.Optional[str]:
-  global DRY_RUN
-  if not 'message' in topology or DRY_RUN:
+  if not 'message' in topology:
     return None
 
   if isinstance(topology.message,str):                      # We have a single message
     return topology.message if default_message else None    # If the action is OK with getting the default message return it
 
   if not isinstance(topology.message,Box):                  # Otherwise we should be dealing with a dict
     common.fatal('topology message should be a string or a dict')
@@ -155,24 +121,22 @@
 
 * Get the lab ID (or default)
 * Map lab ID into current directory
 * Merge status dictionary or perform status-specific callback
 """
 
 def get_lab_id(topology: Box) -> str:
-  return topology.get('defaults.multilab.id','default') or 'default'    # id could be set to {} due to tool f-string evals
+  return str(get_from_box(topology,'defaults.multilab.id') or 'default')
 
 def lab_status_update(
       topology: Box,
       status: Box,
       update: typing.Optional[dict] = None,
       cb: typing.Optional[typing.Callable] = None) -> None:
 
-  if DRY_RUN:                                               # Don't update status if we're in dry-run mode 
-    return
   lab_id = get_lab_id(topology)                             # Get the lab ID (or default)
   if not lab_id in status:
     status[lab_id].dir = os.getcwd()                        # Map lab ID into current directory
   if not 'providers' in status[lab_id]:                     # Initialize provider list
     status[lab_id].providers = []
 
   if update is not None:                                    # Update lab status from a dictionary
@@ -192,18 +156,14 @@
   if cb is not None:                                        # If needed, perform status-specific callback        
     cb(status[lab_id])
 
 """
 lab_status_change -- change current lab status
 """
 def lab_status_change(topology: Box, new_status: str) -> None:
-  global DRY_RUN
-  if DRY_RUN:                                              # Don't update status if we're in dry-run mode 
-    return
-
   status.change_status(
     topology,
     callback = lambda s,t: 
       lab_status_update(t,s,
         update = { 'status': new_status }))
 
 #
```

### Comparing `networklab-1.5.2/netsim/cli/ansible.py` & `networklab-1.5.2.dev1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/clab.py` & `networklab-1.5.2.dev1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/collect.py` & `networklab-1.5.2.dev1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/config.py` & `networklab-1.5.2.dev1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/create.py` & `networklab-1.5.2.dev1/netsim/cli/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
   args = create_topology_parse(cli_args, cli_command, cli_describe, cli_extra_args)
   if not 'output' in args:
     args.output = None
   if not 'devices' in args:
     args.devices = None
 
   if not args.output:
-    args.output = ['provider','yaml=netlab.snapshot.yml','tools']
+    args.output = ['provider','yaml=netlab.snapshot.yml']
     args.output.append('devices' if args.devices else 'ansible:dirs')
   elif args.devices:
     common.error('--output and --devices flags are mutually exclusive',common.IncorrectValue,'create')
 
   topology = load_topology(args)
   augment.main.transform(topology)
   common.exit_on_error()
```

### Comparing `networklab-1.5.2/netsim/cli/down.py` & `networklab-1.5.2.dev1/netsim/cli/down.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import argparse
 import typing
 import textwrap
 import os
 import sys
 from box import Box
 
-from . import external_commands, set_dry_run, is_dry_run
-from . import lab_status_change,get_lab_id,fs_cleanup,load_snapshot
+from . import external_commands
+from . import lab_status_change,get_lab_id,fs_cleanup
 from .. import read_topology,common,providers
 from ..utils import status,strings
 from .up import provider_probes
 #
 # CLI parser for 'netlab down' command
 #
 def down_parse(args: typing.List[str]) -> argparse.Namespace:
@@ -33,19 +33,14 @@
     help='Verbose logging (where applicable)')
   parser.add_argument(
     '--cleanup',
     dest='cleanup',
     action='store_true',
     help='Remove all configuration files created by netlab create')
   parser.add_argument(
-    '--dry-run',
-    dest='dry_run',
-    action='store_true',
-    help='Print the commands that would be executed, but do not execute them')
-  parser.add_argument(
     '--force',
     dest='force',
     action='store_true',
     help='Force shutdown or cleanup (use at your own risk)')
   parser.add_argument(
     '--snapshot',
     dest='snapshot',
@@ -53,60 +48,39 @@
     nargs='?',
     default='netlab.snapshot.yml',
     const='netlab.snapshot.yml',
     help='Transformed topology snapshot file')
 
   return parser.parse_args(args)
 
-#
-# Cleanup common configuration files
-#
 def down_cleanup(topology: Box, verbose: bool = False) -> None:
   p_provider = topology.provider
   cleanup_list = topology.defaults.providers[p_provider].cleanup or []
 
   for s_provider in topology[p_provider].providers:
     cleanup_list.extend(topology.defaults.providers[s_provider].cleanup or [])
     s_filename = topology.defaults.providers[p_provider][s_provider].filename
     if s_filename:
       cleanup_list.append(s_filename)
 
   cleanup_list.extend(topology.defaults.automation.ansible.cleanup)
   cleanup_list.append('netlab.snapshot.yml')
   fs_cleanup(cleanup_list,verbose)
 
-#
-# Cleanup tool configuration directories and other tool-related stuff
-#
-def tool_cleanup(topology: Box, verbose: bool = False) -> None:
-  for tool in list(topology.tools.keys()):
-    cmds = external_commands.get_tool_command(tool,'cleanup',topology,verbose=False) or []
-    cmds.append(f'rm -fr {tool}')
-    external_commands.execute_tool_commands(cmds,topology)
-    if not is_dry_run():
-      print(f"... cleaned up {tool} data")
-
-#
-# Stop the provider-specific workloads
-#
-def stop_provider_lab(
-      topology: Box,
-      pname: str,
-      sname: typing.Optional[str] = None,
-      step: int = 2) -> None:
+def stop_provider_lab(topology: Box, pname: str, sname: typing.Optional[str] = None) -> None:
   p_name = sname or pname
   p_topology = providers.select_topology(topology,p_name)
   p_module   = providers._Provider.load(p_name,topology.defaults.providers[p_name])
 
   exec_command = None
   if sname is not None:
     exec_command = topology.defaults.providers[pname][sname].stop
 
   p_module.call('pre_stop_lab',p_topology)
-  external_commands.stop_lab(topology.defaults,p_name,step,"netlab down",exec_command)
+  external_commands.stop_lab(topology.defaults,p_name,2,"netlab down",exec_command)
   p_module.call('post_stop_lab',p_topology)
 
 '''
 lab_dir_mismatch -- check if the lab instance is running in the current directory
 '''
 def lab_dir_mismatch(topology: Box) -> bool:
   lab_id = get_lab_id(topology)
@@ -134,80 +108,56 @@
 def remove_lab_status(topology: Box) -> None:
   lab_id = get_lab_id(topology)
 
   status.change_status(
     topology,
     callback = lambda s,t: s.pop(lab_id,None))
 
-"""
-Stop external tools
-"""
-def stop_external_tools(args: argparse.Namespace, topology: Box) -> None:
-  lab_status_change(topology,f'stopping external tools')
-  for tool in list(topology.tools.keys()):
-    cmds = external_commands.get_tool_command(tool,'down',topology)
-    if cmds is None:
-      continue
-    external_commands.execute_tool_commands(cmds,topology)
-    if not is_dry_run():
-      print(f"... {tool} tool stopped")
-
-  lab_status_change(topology,f'external tools stopped')
-
 def run(cli_args: typing.List[str]) -> None:
   args = down_parse(cli_args)
-  set_dry_run(args)
-
-  topology = load_snapshot(args)
-  print(f"Read transformed lab topology from snapshot file {args.snapshot}")
+  if not os.path.isfile(args.snapshot):
+    print(f"The topology snapshot file {args.snapshot} does not exist.\n"+
+          "Looks like no lab was started from this directory")
+    sys.exit(1)
+
+  print(f"Reading transformed lab topology from snapshot file {args.snapshot}")
+  topology = read_topology.read_yaml(filename=args.snapshot)
+  if topology is None:
+    common.fatal('... could not read the lab topology, aborting')
+    return
 
   mismatch = lab_dir_mismatch(topology)
 
   lab_status_change(topology,f'lab shutdown requested{" in conflicting directory" if mismatch else ""}')
   try:
-    provider_probes(topology,1)
+    provider_probes(topology)
   except:
     if not args.force:
       return
 
-  stop_step = 2
-  if 'tools' in topology:
-    external_commands.print_step(stop_step,"Stopping external tools",spacing=True)
-    stop_step = stop_step + 1
-    stop_external_tools(args,topology)
-
   p_provider = topology.provider
   p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
   for s_provider in topology[p_provider].providers:
     lab_status_change(topology,f'stopping {s_provider} provider')
     try:
-      stop_provider_lab(topology,p_provider,s_provider,step=stop_step)
-      stop_step = stop_step + 1
+      stop_provider_lab(topology,p_provider,s_provider)
     except:
       if not args.force:
         return
     print()
 
   try:
-    stop_provider_lab(topology,p_provider,step=stop_step)
-    stop_step = stop_step + 1
+    stop_provider_lab(topology,p_provider)
   except:
     if not args.force:
       return
 
   if args.cleanup:
-    if 'tools' in topology:
-      external_commands.print_step(stop_step,"Cleanup tool configurations",spacing=True)
-      stop_step = stop_step + 1
-      tool_cleanup(topology,True)
-
-    external_commands.print_step(stop_step,"Cleanup configuration files",spacing=True)
+    external_commands.print_step(3,"Cleanup configuration files",spacing = True)
     down_cleanup(topology,True)
 
   if not mismatch:
     remove_lab_status(topology)
-
-  if not is_dry_run():
-    status.unlock_directory()
+  status.unlock_directory()
```

### Comparing `networklab-1.5.2/netsim/cli/initial.py` & `networklab-1.5.2.dev1/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/install.py` & `networklab-1.5.2.dev1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/libvirt.py` & `networklab-1.5.2.dev1/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/read.py` & `networklab-1.5.2.dev1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/restart.py` & `networklab-1.5.2.dev1/netsim/cli/restart.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #
 # netlab restart command
 #
 # Perform 'netlab down' followed by 'netlab up'
 #
 import typing
 import argparse
+import os
+import glob
+import subprocess
+import shutil
 
 from box import Box
 
 from .. import common
 from . import down, up
 from . import common_parse_args
```

### Comparing `networklab-1.5.2/netsim/cli/show.py` & `networklab-1.5.2.dev1/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/status.py` & `networklab-1.5.2.dev1/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/test.py` & `networklab-1.5.2.dev1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/cli/up.py` & `networklab-1.5.2.dev1/netsim/cli/up.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 # * Transform lab topology and create provider and automation files,
 #   or read transformed lab topology from snapshot file
 # * Start the lab, including provider-specific pre- and post-start hooks
 #
 import typing
 import argparse
 import os
+import glob
+import subprocess
+import shutil
 
 from box import Box
 from pathlib import Path
 
 from .. import common
 from . import create
-from . import external_commands, set_dry_run, is_dry_run
+from . import external_commands
 from . import common_parse_args, get_message
 from . import lab_status_update, lab_status_change, get_lab_id
 from .. import providers
 from .. import read_topology
 from ..utils import status
+from ..data import get_box,get_from_box
 
 #
 # Extra arguments for 'netlab up' command
 #
 def up_parse_args(standalone: bool) -> argparse.ArgumentParser:
   parse_parents = [ common_parse_args() ] if standalone else []
   parser = argparse.ArgumentParser(
@@ -32,24 +36,14 @@
     add_help=standalone)
   parser.add_argument(
     '--no-config',
     dest='no_config',
     action='store_true',
     help='Do not configure lab devices')
   parser.add_argument(
-    '--no-tools',
-    dest='no_tools',
-    action='store_true',
-    help='Do not start the external tools')
-  parser.add_argument(
-    '--dry-run',
-    dest='dry_run',
-    action='store_true',
-    help='Print the commands that would be executed, but do not execute them')
-  parser.add_argument(
     '--fast-config',
     dest='fast_config',
     action='store_true',
     help='Use fast device configuration (Ansible strategy = free)')
   parser.add_argument(
     '--snapshot',
     dest='snapshot',
@@ -161,20 +155,20 @@
 delete it.
 ''')
   common.fatal(f'aborting "netlab up" request')
 
 """
 Execute provider probes
 """
-def provider_probes(topology: Box, step: int = 2) -> None:
+def provider_probes(topology: Box) -> None:
   p_provider = topology.provider
 
-  external_commands.run_probes(topology.defaults,p_provider,step)
+  external_commands.run_probes(topology.defaults,p_provider,2)
   for s_provider in topology[p_provider].providers:
-    external_commands.run_probes(topology.defaults,s_provider,step)
+    external_commands.run_probes(topology.defaults,s_provider,2)
 
 """
 Start lab topology for a single provider
 """
 def start_provider_lab(topology: Box, pname: str, sname: typing.Optional[str] = None) -> None:
   p_name   = sname or pname
   p_module = providers._Provider.load(p_name,topology.defaults.providers[p_name])
@@ -209,67 +203,24 @@
   sp_module  = providers._Provider.load(s_provider,topology.defaults.providers[s_provider])
   s_topology = providers.select_topology(topology,s_provider)         # Create secondary provider subtopology
   filename = sp_data.filename                                         # Get the secondary configuration filename
   print(f"Recreating {filename} configuration file for {s_provider} provider")
   sp_module.create(s_topology,filename)                               # ... and create the new configuration file
 
 """
-Deploy initial configuration
-"""
-def deploy_initial_config(args: argparse.Namespace, topology: Box) -> None:
-  if args.no_config:
-    print("\nInitial configuration skipped, run 'netlab initial' to configure the devices")
-    return
-
-  lab_status_change(topology,f'deploying initial configuration')
-  external_commands.deploy_configs(4,"netlab up",args.fast_config)
-  message = get_message(topology,'up',False)
-  if message:
-    print(f"\n\n{message}")
-  lab_status_change(topology,f'initial configuration complete')
-
-"""
-Deploy external tools
-"""
-def start_external_tools(args: argparse.Namespace, topology: Box) -> None:
-  if not 'tools' in topology:
-    return
-  if args.no_tools:
-    print("\nExternal tools not started, start them manually")
-    return
-
-  print ("\nStarting external tools...")
-  lab_status_change(topology,f'starting external tools')
-  for tool in topology.tools.keys():
-    cmds = external_commands.get_tool_command(tool,'up',topology)
-    if cmds is None:
-      continue
-    external_commands.execute_tool_commands(cmds,topology)
-    msg = external_commands.get_tool_message(tool,topology)
-    if not is_dry_run():
-      print(f"... {tool} tool started")
-
-    if msg:
-      print(("DRY_RUN: " if is_dry_run() else "") + msg + "\n")
-
-  lab_status_change(topology,f'external tools started')
-
-"""
 Main "lab start" process
 """
 def run(cli_args: typing.List[str]) -> None:
   up_args_parser = up_parse_args(False)                       # Try to parse the up-specific arguments
   (args,rest) = up_args_parser.parse_known_args(cli_args)
-  set_dry_run(args)
-  if not args.snapshot and not is_dry_run():
+  if not args.snapshot:
     check_existing_lab()
 
   topology = get_topology(args,cli_args)
-  if not is_dry_run():
-    check_lab_instance(topology)
+  check_lab_instance(topology)
 
   settings = topology.defaults
   if common.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
   provider_probes(topology)
 
@@ -279,19 +230,26 @@
   p_module.call('pre_output_transform',topology)
 
   status_start_lab(topology)
   if 'err_conflict' in topology.defaults:
     common.fatal(f'race condition, lab instance already running in {topology.defaults.err_conflict}')
     return
 
-  if not is_dry_run():
-    status.lock_directory()
+  status.lock_directory()
 
   start_provider_lab(topology,p_provider)
   for s_provider in topology[p_provider].providers:
     print()
     recreate_secondary_config(topology,p_provider,s_provider)
     start_provider_lab(topology,p_provider,s_provider)
 
-  deploy_initial_config(args,topology)
-  start_external_tools(args,topology)
+  if not args.no_config:
+    lab_status_change(topology,f'deploying initial configuration')
+    external_commands.deploy_configs(4,"netlab up",args.fast_config)
+    message = get_message(topology,'up',False)
+    if message:
+      print(f"\n\n{message}")
+    lab_status_change(topology,f'initial configuration complete')
+  else:
+    print("\nInitial configuration skipped, run 'netlab initial' to configure the devices")
+
   lab_status_change(topology,'started')
```

### Comparing `networklab-1.5.2/netsim/cli/usage.txt` & `networklab-1.5.2.dev1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/common.py` & `networklab-1.5.2.dev1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/data/__init__.py` & `networklab-1.5.2.dev1/netsim/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from box import Box
 from .. import common
 
 #
 # I had enough -- here's a function that returns a box with proper default settings
 
 def get_box(init: dict) -> Box:
-  return Box(init,default_box=True,default_box_none_transform=False,box_dots=True)
+  return Box(init,default_box=True,box_dots=True)
 
 def get_empty_box() -> Box:
   return get_box({})
 
 #
 # Change all NULL values in a nested dictionary structure to empty strings
 # to make them nicer in YAML printouts
@@ -27,15 +27,14 @@
       d[k] = ""
 
 #
 # Safe get from a hierarchical dictionary (won't create new objects)
 #
 
 def get_from_box(b: Box, selector: typing.Union[str,typing.List[str]], partial: bool = False) -> typing.Optional[typing.Any]:
-  print('WARNING: get_from_box is deprecated, please fix your plugins')
   if isinstance(selector,str):
     selector = selector.split('.')
 
   for idx,k in enumerate(selector):
     if not k in b:
       return b if partial and idx > 0 else None   # return partial result if request assuming we got at least one match before
 
@@ -54,29 +53,23 @@
 # default and topology settings
 #
 # Use 'get_global_settings' when you need a dictionary of global module parameters if the module uses
 # 'no_propagate' flag to stop leaking into nodes.
 #
 
 def get_global_parameter(topology: Box, selector: str) -> typing.Optional[typing.Any]:
-  try:
-    return topology.get(selector,None) or topology.defaults.get(selector,None)
-  except:
-    return None
+  value = get_from_box(topology,selector)
+  if value is None:
+    return get_from_box(topology.defaults,selector)
+  else:
+    return value
 
 def get_global_settings(topology: Box, selector: str) -> typing.Optional[typing.Any]:
-  try:                                                                # Wrapping 'get' operations in tries
-    g_set = topology.get(selector,None)                               # ... because they may fail if an intermediate
-  except:                                                             # ... value is not a dictionary
-    g_set = None
-
-  try:
-    d_set = topology.defaults.get(selector,None)
-  except:
-    d_set = None
+  g_set = get_from_box(topology,selector)
+  d_set = get_from_box(topology.defaults,selector)
 
   if d_set:                                                           # Found default settings
     if 'attributes' in d_set:                                         # ... filter them down to actual global attributes
       d_set = get_box({ k:v for k,v in d_set.items() if k in d_set.attributes['global'] })
   else:                                                               # No default settings? Just return the g_set
     return g_set
 
@@ -84,14 +77,44 @@
     return d_set
 
   if isinstance(g_set,Box) and isinstance(d_set,Box):                 # We can merge two boxes but nothing else
     return d_set + g_set                                              # Return a merged value, be careful about precedences
 
   return g_set                                                        # Can't merge, and we know g_set has some value
 
+#
+# Set a dictionary value specified by a list of keys
+#
+def set_dots(b : dict,k_list : list,v : typing.Any) -> None:
+  if len(k_list) <= 1:
+    b[k_list[0]] = v
+    return
+  if not k_list[0] in b:
+    b[k_list[0]] = {}
+  elif b[k_list[0]] is None:
+    b[k_list[0]] = {}
+  set_dots(b[k_list[0]],k_list[1:],v)
+
+#
+# Change dotted dictionary keys into nested dictionaries
+#
+def unroll_dots(b : typing.Any) -> None:
+  if isinstance(b,dict):
+    for k in list(b.keys()):
+      unroll_dots(b[k])
+      if isinstance(k,str) and ('.' in k) and not ('/' in k):
+        v = b[k]
+        del b[k]     # If you're using Box with box_dots parameter
+        set_dots(b,k.split('.'),v)
+  elif isinstance(b,list):
+    for v in b:
+      unroll_dots(v)
+  else:
+    return
+
 """
 bool_to_defaults: 
 
 * remove a parameter set to False just to prevent default propagation
 * replace a True value with a default dictionary
 * dive recursively into all keys specified in default dictionary
 """
```

### Comparing `networklab-1.5.2/netsim/data/global_vars.py` & `networklab-1.5.2.dev1/netsim/data/global_vars.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,25 +27,17 @@
 '''
 get -- get a pointer to a global Box (referenced by name) hidden in topology
 '''
 
 def get(varname: str) -> Box:
   if _globals is None:
     from ..common import fatal
-    from ..data import get_empty_box
 
     fatal(f'Trying to get global variable {varname} before the global_vars subsystem is initialized')
-    return get_empty_box()              # pragma: no cover -- fatal aborts, but we need to return the right object to keep mypy happy
+    return Box({})                  # pragma: no cover -- fatal aborts, but we need to return the right object to keep mypy happy
 
   return _globals[varname]
 
 def get_topology() -> typing.Optional[Box]:
   global _topology
 
   return _topology
-
-def get_const(varname: str, default: typing.Any) -> typing.Any:
-  topology = get_topology()
-  if topology is None:
-    return default
-
-  return topology.defaults.const.get(varname, default)
```

### Comparing `networklab-1.5.2/netsim/data/types.py` & `networklab-1.5.2.dev1/netsim/data/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import typing,typing_extensions,types
 import functools
 import netaddr
 import re
 from box import Box
 from .. import common
+from . import get_from_box,set_dots
 
 """
 Common error checking routines:
 
 * wrong_type_text: return the type of the data item, tranforming Box into dict
 * wrong_type_message: prints the 'wrong data type' error message
 * int_value_error: prints out-of-bounds error message
@@ -137,29 +138,29 @@
       parent: Box,                                      # Parent object
       key: str,                                         # Key within the parent object, may include dots.
       empty_value: typing.Optional[typing.Any] = None,  # Optional value to use when there is no value
       create_empty: typing.Optional[bool] = None,       # Do we need to create an empty value?
       true_value: typing.Optional[typing.Any] = None,   # Value to use to replace _true_
       false_value: typing.Optional[typing.Any] = None,  # Value to use to replace _false_
       abort: bool = False) -> typing.Any:
-  value = parent.get(key,None)                          # Try to get the value from the parent object
+  value = get_from_box(parent,key)                      # Otherwise, try to get the value from the parent object
   if value is None:                                     # No value was found, now what?
     if empty_value is not None:                         # ... is there empty value for this data type?
       if create_empty is None:                          # Empty value is defined, and we'll use it to create an empty object if the caller
         create_empty = True                             # did not specify its preferencehs
 
       if create_empty:                                  # Now for the real deal
         value = empty_value                             # ... if we should create an empty value do so
-        parent[key] = empty_value                       # ... and store it in the parent object
+        set_dots(parent,key.split('.'),empty_value)     # ... and store it in the parent object (dedottifying the key)
       else:
         if abort:                                       # Empty value was specified, 'create_empty' is False, and there's no actual value
           raise common.IncorrectValue()                 # ... raise an exception if requested
 
-    if not key in parent:                               # We can skip further processing if the key is missing.
-      return value
+    if not key in parent:                               # We can skip the validation of the key is missing.
+      return value                                      # ... if the key is there, then we have to make sure the value is valid
 
   # Handle boolean-to-data-type conversions if the value is bool and the caller specified true_value
   #
   if isinstance(value,bool) and not (true_value is None):
     if value is True:                                   # Replace True with true_value and move on
       value = true_value
       parent[key] = value
```

### Comparing `networklab-1.5.2/netsim/data/validate.py` & `networklab-1.5.2.dev1/netsim/data/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # Data validation routines
 #
 
-import typing
+import typing,typing_extensions
 import builtins as _bi
 from box import Box
 from .. import common
-from . import get_empty_box
+from . import get_from_box,set_dots,get_empty_box,get_box
 
 #
 # Import functions from data.types to cope with legacy calls to must_be_something
 from .types import must_be_list,must_be_dict,must_be_string,must_be_int,must_be_bool
 
 # We also need to import the whole data.types module to be able to do validation function lookup
 from . import types as _tv
@@ -19,15 +19,15 @@
 get_valid_attributes
 
 Given an attribute dictionary, list of valid attribute categories, and extra attributes, return a list
 of valid attributes, or a string (type name) if the first attribute source in the list is a string
 """
 
 ##### REMOVE AFTER ATTRIBUTE MIGRATION #####
-def make_attr_dict(atlist: typing.Union[list,Box]) -> Box:
+def make_attr_dict(atlist: typing.Union[list,Box]) -> typing.Union[Box]:
   if isinstance(atlist,list):
     return Box({ k: None for k in atlist })
 
   return atlist
 
 def get_valid_attributes(
       attributes: Box,                                      # Where to get valid attributes from
```

### Comparing `networklab-1.5.2/netsim/defaults/attributes.yml` & `networklab-1.5.2.dev1/netsim/defaults/attributes.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,38 +6,36 @@
   groups:
   links:
   module:
   name: id
   nodes:
   plugin: list
   provider: id
-  tools: dict
 internal: [ input,includes,pools,Provider,Plugin,message ]
 can_be_false: [ link,interface ]
 link:
   bandwidth: int
   bridge: id
   name: str
   prefix:                                           # Prefix is too complex to validate here -- links module will do the job
   role: id
   pool: id
-  type: { type: str, valid_values: [ lan, p2p, stub, loopback, tunnel, vlan_member ] }
+  type: { type: str, valid_values: [ lan, p2p, stub, loopback, vlan_member ] }
   unnumbered: bool
   interfaces:
   mtu: { type: int, min_value: 64, max_value: 65535 }
   vlan_name: id
 link_internal: [ linkindex,parentindex ]
 link_no_propagate: [ prefix,interfaces,gateway ]
 link_module_no_propagate: [ vlan ]                  # Do not propagate VLAN attributes to node interfaces -- see #575
 interface:
   node: id
   ipv4: { type: ipv4, use: interface }
   ipv6: { type: ipv6, use: interface }
   ifindex: int
-  ifname: str
 node:
   name: id
   interfaces: list
   module: list
   device: id
   box: str
   id: { type: int, min_value: 1, max_value: 150 }
```

### Comparing `networklab-1.5.2/netsim/devices/__init__.py` & `networklab-1.5.2.dev1/netsim/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 import os
 
 from box import Box
 
 # Related modules
 from .. import common
+from ..data import get_from_box
 from ..callback import Callback
 from ..augment import devices
 
 class _Quirks(Callback):
 
   def __init__(self, data: Box) -> None:
     pass
```

### Comparing `networklab-1.5.2/netsim/devices/arubacx.py` & `networklab-1.5.2.dev1/netsim/devices/arubacx.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # # When using VRFs, the process ID is taken from the vrfidx, which usually is > 100.
 # # Here we are mapping every VRF to a specific ospfidx
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 class ARUBACX(_Quirks):
 
   @classmethod
   def device_quirks(self, node: Box, topology: Box) -> None:
     mods = node.get('module',[])
```

### Comparing `networklab-1.5.2/netsim/devices/arubacx.yml` & `networklab-1.5.2.dev1/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/asav.py` & `networklab-1.5.2.dev1/netsim/devices/asav.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #
 # Cisco ASA quirks
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 
 def check_isis_p2p_interfaces(node: Box, topology: Box) -> None:
   for intf in node.interfaces:
     if not 'isis' in intf:
       continue
     for neighbor in intf.neighbors:
       remote_node = neighbor.node
       remote_interfaces = topology.nodes[remote_node].interfaces
       for rintf in remote_interfaces:
         if rintf.ifname == neighbor.ifname:
-          if intf.get('isis.network_type',None) == "point-to-point":
+          if get_from_box(rintf, 'isis.network_type') == "point-to-point":
             common.error(
-              f'Cisco ASA does not support P2P IS-IS links.'
-              f'Problematic Interface: {remote_node} {neighbor.ifname}',
-              common.IncorrectType,
-              'quirks',
+                f'Cisco ASA does not support P2P IS-IS links.'
+                f'Problematic Interface: {remote_node} {neighbor.ifname}',
+                common.IncorrectType,
+                'quirks',
             )
 
 class ASA(_Quirks):
 
   @classmethod
   def device_quirks(self, node: Box, topology: Box) -> None:
     mods = node.get('module', [])
```

### Comparing `networklab-1.5.2/netsim/devices/asav.yml` & `networklab-1.5.2.dev1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/csr.yml` & `networklab-1.5.2.dev1/netsim/devices/eos.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-description: Cisco CSR 1000v
-interface_name: GigabitEthernet{ifindex}
+description: Arista vEOS VM or cEOS container
+interface_name: Ethernet{ifindex}
+mgmt_if: Management1
 loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
-ifindex_offset: 2
 virtualbox:
-  image: cisco/csr1000v
+  image: arista/veos
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
-  ansible_become_method: enable
-  ansible_become_password: vagrant
-  ansible_network_os: ios
+  ansible_network_os: eos
   ansible_connection: network_cli
-  netlab_device_type: csr
-node:
-  min_mtu: 1500
 features:
   bgp:
     local_as: True
     vrf_local_as: True
     local_as_ibgp: True
     activate_af: True
   initial:
+    system_mtu: True
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
   isis:
@@ -35,19 +30,40 @@
       network: True
   mpls:
     ldp: True
     bgp: True
     vpn: True
     6pe: True
   vlan:
-    model: switch
-    svi_interface_name: BDI{vlan}
+    model: l3-switch
+    svi_interface_name: Vlan{vlan}
+    subif_name: "{ifname}.{subif_index}"
+    native_routed: True
+  evpn:
+    irb: True
+    asymmetrical_irb: True
+    bundle: [ vlan_aware ]
   gateway:
-    protocol: [ vrrp ]
+    protocol: [ anycast, vrrp ]
+clab:
+  interface:
+    name: et{ifindex}
+  node:
+    kind: ceos
+    env:
+      INTFTYPE: et
+  mgmt_if: Management0
+  image: ceos:4.26.4M
+  group_vars:
+    ansible_user: admin
+    ansible_ssh_pass: admin
+    ansible_become: yes
+    ansible_become_method: enable
 libvirt:
-  image: cisco/csr1000v
-  create:
-    virt-install --connect=qemu:///system --name=vm_box --os-variant=rhel4.0 --arch=x86_64 --cpu host --vcpus=1 --hvm
-      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+  image: arista/veos
+  create_template: eos.xml.j2
+#      create: |
+#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=2 --hvm
+#          --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
 external:
   image: none
-graphite.icon: router
+graphite.icon: switch
```

### Comparing `networklab-1.5.2/netsim/devices/cumulus.yml` & `networklab-1.5.2.dev1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.2.dev1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/dellos10.yml` & `networklab-1.5.2.dev1/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/eos.py` & `networklab-1.5.2.dev1/netsim/devices/eos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #
 # Arista EOS quirks
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 def check_mlps_vlan_bundle(node: Box) -> None:
-  if node.get('evpn.transport',None) != 'mpls':                         # This quirk applies only to EVPN/MPLS
+  if get_from_box(node,'evpn.transport') != 'mpls':                     # This quirk applies only to EVPN/MPLS
     return
 
   for vname,vdata in node.get('vlans',{}).items():
-    if not vdata.get('evpn.bundle',False):                              # Check only VLANs within a bundle
+    if not get_from_box(vdata,'evpn.bundle'):                           # Check only VLANs within a bundle
       continue
     if vdata.get('mode','') != 'bridge':                                # They must be in pure bridging mode
       common.error(
         f'Arista EOS supports only bridge VLANs in an EVPN/MPLS VLAN bundle ({vname} on {node.name})',
         common.IncorrectType,
         'quirks')
     ifname = f'Vlan{vdata.id}'                                          # Now remove the VLAN interface
@@ -30,18 +31,18 @@
       'quirks')
 
 def check_shared_mac(node: Box, topology: Box) -> None:
   if devices.get_provider(node,topology) != 'clab':
     return
 
   for intf in node.interfaces:
-    if intf.get('gateway.protocol',None) != 'anycast':                  # We hope that VRRP works (not tested yet)
+    if get_from_box(intf,'gateway.protocol') != 'anycast':              # We hope that VRRP works (not tested yet)
       continue
 
-    if intf.get('vlan',None):                                           # Anycast works on VLAN cEOS interfaces
+    if get_from_box(intf,'vlan'):                                       # Anycast works on VLAN cEOS interfaces
       continue
 
     common.error(
       f'Anycast gateway (VARP) on non-VLAN interfaces does not work on Arista cEOS ({node.name}).\n.. Use vEOS VM with libvirt provider',
       common.IncorrectType,
       'quirks')
     return
```

### Comparing `networklab-1.5.2/netsim/devices/eos.yml` & `networklab-1.5.2.dev1/netsim/devices/csr.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-description: Arista vEOS VM or cEOS container
-interface_name: Ethernet{ifindex}
-mgmt_if: Management1
+description: Cisco CSR 1000v
+interface_name: GigabitEthernet{ifindex}
 loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
+ifindex_offset: 2
 virtualbox:
-  image: arista/veos
+  image: cisco/csr1000v
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
-  ansible_network_os: eos
+  ansible_become_method: enable
+  ansible_become_password: vagrant
+  ansible_network_os: ios
   ansible_connection: network_cli
+  netlab_device_type: csr
+node:
+  min_mtu: 1500
 features:
   bgp:
     local_as: True
     vrf_local_as: True
     local_as_ibgp: True
     activate_af: True
   initial:
-    system_mtu: True
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
   isis:
@@ -31,40 +34,19 @@
       network: True
   mpls:
     ldp: True
     bgp: True
     vpn: True
     6pe: True
   vlan:
-    model: l3-switch
-    svi_interface_name: Vlan{vlan}
-    subif_name: "{ifname}.{subif_index}"
-    native_routed: True
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-    bundle: [ vlan_aware ]
+    model: switch
+    svi_interface_name: BDI{vlan}
   gateway:
-    protocol: [ anycast, vrrp ]
-clab:
-  interface:
-    name: et{ifindex}
-  node:
-    kind: ceos
-    env:
-      INTFTYPE: et
-  mgmt_if: Management0
-  image: ceos:4.26.4M
-  group_vars:
-    ansible_user: admin
-    ansible_ssh_pass: admin
-    ansible_become: yes
-    ansible_become_method: enable
+    protocol: [ vrrp ]
 libvirt:
-  image: arista/veos
-  create_template: eos.xml.j2
-#      create: |
-#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=2 --hvm
-#          --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+  image: cisco/csr1000v
+  create:
+    virt-install --connect=qemu:///system --name=vm_box --os-variant=rhel4.0 --arch=x86_64 --cpu host --vcpus=1 --hvm
+      --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
 external:
   image: none
-graphite.icon: switch
+graphite.icon: router
```

### Comparing `networklab-1.5.2/netsim/devices/frr.yml` & `networklab-1.5.2.dev1/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/iosv.py` & `networklab-1.5.2.dev1/netsim/devices/iosv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #
 # Arista EOS quirks
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 # Cisco IOSv does not support VRRP on BVI interfaces. Go figure...
 #
 def check_vrrp_bvi(node: Box, topology: Box) -> None:
   for intf in node.interfaces:
-    if intf.get('gateway.protocol',None) != 'vrrp':                     # No VRRP, move on
+    if get_from_box(intf,'gateway.protocol') != 'vrrp':                 # No VRRP, move on
       continue
 
-    if intf.get('type',None) != 'svi':                                  # Not a BVI interface, move on
+    if get_from_box(intf,'type') != 'svi':                              # Not a BVI interface, move on
       continue
 
     common.error(
       f'Cisco IOSv cannot run VRRP on BVI interfaces.',
       common.IncorrectType,
       'quirks')
     return
```

### Comparing `networklab-1.5.2/netsim/devices/iosv.yml` & `networklab-1.5.2.dev1/netsim/devices/iosv.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 description: Cisco IOSv
 interface_name: GigabitEthernet0/{ifindex}
 loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
   ansible_become_method: enable
   ansible_become_password: vagrant
   ansible_network_os: ios
   ansible_connection: network_cli
```

### Comparing `networklab-1.5.2/netsim/devices/iosxr.yml` & `networklab-1.5.2.dev1/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/junos.py` & `networklab-1.5.2.dev1/netsim/devices/junos.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # # the same can apply to loopbacks, irbs, ...
 # # + if the vlan module is in use, and multiple units are present, set the unit 0 as untagged vlan but with the vlan-id (default 1)
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 def unit_0_trick(intf: Box, round: str ='global') -> None:
   oldname = intf.ifname
   newname = oldname + ".0"
   if common.debug_active('quirks'):
     print(" - [{}] Found interface {}, renaming to {}".format(round, intf.ifname, newname))
```

### Comparing `networklab-1.5.2/netsim/devices/linux.yml` & `networklab-1.5.2.dev1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/none.yml` & `networklab-1.5.2.dev1/netsim/devices/none.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 description: Dummy device used to test topology transformation
 #
 # Most features are enabled on the dummy device -- this file is a pretty
 # good template if you want to figure out what device features there are.
 #
 interface_name: eth{ifindex}
 loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
 virtualbox:
   image: none
 libvirt:
   image: none
 clab:
   image: none
 external:
```

### Comparing `networklab-1.5.2/netsim/devices/nxos.yml` & `networklab-1.5.2.dev1/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/routeros7.yml` & `networklab-1.5.2.dev1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/srlinux.yml` & `networklab-1.5.2.dev1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/sros.yml` & `networklab-1.5.2.dev1/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/vmx.py` & `networklab-1.5.2.dev1/netsim/devices/vmx.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # # the same can apply to loopbacks, irbs, ...
 # # + if the vlan module is in use, and multiple units are present, set the unit 0 as untagged vlan but with the vlan-id (default 1)
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 def unit_0_trick(intf: Box, round: str ='global') -> None:
   oldname = intf.ifname
   newname = oldname + ".0"
   if common.debug_active('quirks'):
     print(" - [{}] Found interface {}, renaming to {}".format(round, intf.ifname, newname))
```

### Comparing `networklab-1.5.2/netsim/devices/vmx.yml` & `networklab-1.5.2.dev1/netsim/devices/vmx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/vsrx.py` & `networklab-1.5.2.dev1/netsim/devices/vsrx.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # # the same can apply to loopbacks, irbs, ...
 # # + if the vlan module is in use, and multiple units are present, set the unit 0 as untagged vlan but with the vlan-id (default 1)
 #
 from box import Box
 
 from . import _Quirks
 from .. import common
+from ..data import get_from_box
 from ..augment import devices
 
 def unit_0_trick(intf: Box, round: str ='global') -> None:
   oldname = intf.ifname
   newname = oldname + ".0"
   if common.debug_active('quirks'):
     print(" - [{}] Found interface {}, renaming to {}".format(round, intf.ifname, newname))
```

### Comparing `networklab-1.5.2/netsim/devices/vsrx.yml` & `networklab-1.5.2.dev1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/devices/vyos.yml` & `networklab-1.5.2.dev1/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc` & `networklab-1.5.2.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,60 +23,58 @@
             'ebgp_utils')
 
 def post_transform(topology: Box) -> None:
     config_name = api.get_config_name(globals())
     # Iterate over node[x].interfaces
     for n, ndata in topology.nodes.items():
         for intf in ndata.interfaces:
-            if not isinstance(intf.get('bgp',None),Box):
-                continue
             #print("LINK START *******************")
             #print(intf)
             #print("LINK END   *******************")
             # Handle as_override
-            as_override = intf.get('bgp.as_override',None)
+            as_override = data.get_from_box(intf, 'bgp.as_override')
             if as_override:
                 # Report the parameter on the BGP session, based on ifindex
                 for neigh in ndata.get('bgp', {}).get('neighbors', []):
                     if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                         neigh.as_override = as_override
                 # Report the parameter on the BGP session (for VRF), based on ifindex
                 if 'vrf' in intf:
                     for neigh in ndata.vrfs[intf.vrf].get('bgp', {}).get('neighbors', []):
                         if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                             neigh.as_override = as_override
                 api.node_config(ndata,config_name)
             # Handle allowas_in
-            allowas_in = intf.get('bgp.allowas_in',None)
+            allowas_in = data.get_from_box(intf, 'bgp.allowas_in')
             if allowas_in:
                 # Report the parameter on the BGP session, based on ifindex
                 for neigh in ndata.get('bgp', {}).get('neighbors', []):
                     if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                         neigh.allowas_in = int(allowas_in)
                 # Report the parameter on the BGP session (for VRF), based on ifindex
                 if 'vrf' in intf:
                     for neigh in ndata.vrfs[intf.vrf].get('bgp', {}).get('neighbors', []):
                         if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                             neigh.allowas_in = int(allowas_in)
                 api.node_config(ndata,config_name)
             # Handle default_originate
-            default_originate = intf.get('bgp.default_originate',None)
+            default_originate = data.get_from_box(intf, 'bgp.default_originate')
             if default_originate:
                 # Report the parameter on the BGP session, based on ifindex
                 for neigh in ndata.get('bgp', {}).get('neighbors', []):
                     if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                         neigh.default_originate = default_originate
                 # Report the parameter on the BGP session (for VRF), based on ifindex
                 if 'vrf' in intf:
                     for neigh in ndata.vrfs[intf.vrf].get('bgp', {}).get('neighbors', []):
                         if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                             neigh.default_originate = default_originate
                 api.node_config(ndata,config_name)
             # Handle bgp_password
-            bgp_password = intf.get('bgp.password',None)
+            bgp_password = data.get_from_box(intf, 'bgp.password')
             if bgp_password:
                 # Report the parameter on the BGP session, based on ifindex
                 for neigh in ndata.get('bgp', {}).get('neighbors', []):
                     if neigh.ifindex == intf.ifindex and neigh.type == 'ebgp':
                         neigh.password = bgp_password
                 # Report the parameter on the BGP session (for VRF), based on ifindex
                 if 'vrf' in intf:
```

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/multilab/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/ansible.sh` & `networklab-1.5.2.dev1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/containerlab.sh` & `networklab-1.5.2.dev1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/grpc.sh` & `networklab-1.5.2.dev1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/arubacx.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.2.dev1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/csr.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/eos.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/iosv.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/nxos.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/libvirt.sh` & `networklab-1.5.2.dev1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/install/ubuntu.sh` & `networklab-1.5.2.dev1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/__init__.py` & `networklab-1.5.2.dev1/netsim/modules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # Module class and adding transformation methods
 #
 import typing
 
 from box import Box
 
 # Related modules
-from .. import common,data
+from .. import common
+from ..data import get_from_box
 from ..data.validate import must_be_list
 from ..callback import Callback
 from ..augment import devices
 
 # List of attributes we don't want propagated from defaults to global/node
 #
 no_propagate_list = ["attributes","extra_attributes","requires","supported_on","no_propagate","config_after","transform_after"]
@@ -188,15 +189,15 @@
 #
 # settings - dictionary with module settings
 # mod_settings - default module settings
 #
 def get_propagated_global_module_params(module: str, settings: Box,mod_settings: Box) -> Box:
   global no_propagate_list
 
-  global_copy = data.get_box(settings)         # Make a fresh copy of the settings
+  global_copy = Box(settings)                  # Make a fresh copy of the settings
   no_propagate = list(no_propagate_list)       # ... and global no_propagate list
   if "no_propagate" in mod_settings:
     no_propagate.extend(mod_settings.no_propagate)
   no_propagate.extend([ k for k in mod_settings.keys() if "no_propagate" in k ])
   for remove_key in no_propagate:
     global_copy.pop(remove_key,None)
   return global_copy
@@ -253,15 +254,15 @@
         common.IncorrectValue,
         'module')
       continue                                                  # Nope. Weird, but doesn't matter right now.
     mod_def = topology.defaults[m]
     if not isinstance(mod_def,dict):                               # Are module defaults a dict?
       common.fatal("Defaults for module %s should be a dict" % m)  # Nope? Too bad, crash right now, we can't live like that...
 
-    default_copy = data.get_box(mod_def)                        # Got module defaults. Now copy them (we're gonna clobber them)
+    default_copy = Box(mod_def)                                 # Got module defaults. Now copy them (we're gonna clobber them)
     no_propagate = list(no_propagate_list)                      # Always remove these default attributes (and make a fresh copy of the list)
     no_propagate.extend(default_copy.get("no_propagate", []))   # ... and whatever the module wishes to be removed
     no_propagate.extend([ k for k in mod_def.keys() if "no_propagate" in k ])
                                                                 # ... including all attributes with 'no_propagate' in the name
     for remove_key in no_propagate:                             # We got the list of unwanted attributes.
       default_copy.pop(remove_key,None)                         # ... remove them with extreme prejudice
 
@@ -328,24 +329,25 @@
 
 * Add propagatable link attributes to interface attributes
 * Copy global attributes to node attributes if the node attributes are not specified
 """
 
 def parse_module_attributes(a: typing.Union[typing.Dict, Box]) -> Box:
   if isinstance(a,dict):
-    attr = data.get_box(a)
+    attr = Box(a,default_box=True,box_dots=True)
     if not isinstance(attr.interface,str):
       attr.interface = list(set(attr.link) - set(attr.link_no_propagate) | set(attr.interface))
     attr.node = attr.get("node",attr["global"])
   else:
-    attr = data.get_box({
+    attr = Box({
       "global": a,
       "node": a,
       "link": a,
-      "interface": a})
+      "interface": a
+    },default_box=True,box_dots=True)
   return attr
 
 """
 check_module_dependencies:
 
 For every module used by the topology, check is the module has "requires" attribute, and if
 it does, check that everything in that list is also in the topology modules list.
@@ -428,26 +430,26 @@
 def copy_node_data_into_interfaces(topology: Box) -> None:
   for n in topology.nodes.values():
     for m in n.get('module',[]):                                 # Iterate over node modules
       mod_attr = topology.defaults[m].attributes                 # ... get a pointer to module attributes to make code easier to read
       if not mod_attr.node_copy:                                 # Any copyable attributes for this module?
         continue                                                 # ... nope, get out of here
 
-      copy_attr = data.get_box({ k: v
+      copy_attr = Box({ k: v
         for k,v in n.get(m,{}).items()
           if k in mod_attr.node_copy })                          # Build a Box of node attributes that could be copied to interfaces
 
       for intf in n.get('interfaces',[]):                        # We might have some work to do, iterate over all interfaces
         if not isinstance(intf.get(m,{}),dict):                  # ... if the interface module data is not a dict, we can't merge
           continue
-        vrf_attr = data.get_empty_box()                          # Assume we have no VRF attributes
+        vrf_attr = Box({})                                       # Assume we have no VRF attributes
         if 'vrf' in intf and mod_attr.vrf_aware:                 # Do we have to deal with VRF-aware attributes?
           vrf_mod_data = n.vrfs[intf.vrf].get(m,{})
           if not vrf_mod_data is False:                          # Deal with things like 'ospf: False' on VRF level
-            vrf_attr = data.get_box({ k: v
+            vrf_attr = Box({ k: v
               for k,v in vrf_mod_data.items()
                 if k in mod_attr.vrf_aware })                    # Build a Box of VRF attributes that could be copied to interfaces
 
         if copy_attr or vrf_attr:                                # ... modify interface data only if we have something to merge
           intf[m] = copy_attr + vrf_attr + intf[m]
 
 """
@@ -464,15 +466,15 @@
     defaults: typing.Optional[Box] = None,
     merge_dict: bool = True) -> typing.Optional[typing.Any]:
 
   composite_value: typing.Optional[Box] = None
   for obj in (intf,link,node,topology,defaults):
     if obj is None:
       continue
-    value = obj.get(path,None)
+    value = get_from_box(obj,path)
     if not value:
       continue
     if not isinstance(value,Box) or not merge_dict:
       return value
     if composite_value:
       composite_value = value + composite_value
     else:
```

### Comparing `networklab-1.5.2/netsim/modules/_dataplane.py` & `networklab-1.5.2.dev1/netsim/modules/_dataplane.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Generic data plane routines
 #
 import typing
 from box import Box
 
 from .. import common
-from ..data import global_vars
+from ..data import global_vars,get_from_box,set_dots
 from ..data.validate import must_be_list
 
 """
 The ID Set routines provide a common interface to identifiers that can be auto-assigned or static:
 
 Creating and updating the ID set:
 * build_id_set -- create the set of static identifiers
@@ -136,29 +136,29 @@
                 module=module,
                 create_empty=False)                           	# If the attribute is there, it must be a list
 
   if not ref_list:
     if not reference_dictionary in parent:                          # If there are no local objects, we don't need the default value
       return True
     if not create_default:																					# Do we need a default value for the list?
-      return True
+    	return True
 
     # Create the default list based on local objects
     ref_list = [ k for k,v in parent[reference_dictionary].items() if default_filter(v) ]
     if merge_topology:																							# Do we need to merge the object default list with topology value?
-      topo_ref_list = topology.get(list_name,None)    			        # ... get global list
+      topo_ref_list = get_from_box(topology,list_name)			        # ... get global list
       if not topo_ref_list is None:
         for k in topo_ref_list:																 			# ... now carefully append global list to local one retaining element order
           if not k in ref_list:																			# ... of course we could use dirty one-line tricks, but why should we?
             ref_list.append(k)
 
     if not ref_list:																								# Still nothing to do? OK, get out of here
       return True
 
-    parent[list_name] = ref_list
+    set_dots(parent,list_name.split('.'),ref_list)
 
   list_ok = True
   for obj_name in ref_list:                                         # Now check whether the names of reference objects are valid
     if obj_name in parent.get(reference_dictionary,{}):             # ... but very carefully, we don't want to create extra boxes
       continue
     if obj_name in topology.get(reference_dictionary,{}):           # ... global name is also OK
       continue
```

### Comparing `networklab-1.5.2/netsim/modules/_routing.py` & `networklab-1.5.2.dev1/netsim/modules/_routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from box import Box
 import typing
 import netaddr
 
 from .. import common
 from .. import addressing
-from .. import data
+from ..data import get_from_box
 
 # Build routing protocol address families
 #
 # * If the address families are not set, calculate them based on interface address families
 # * Otherwise parse and validate the AF attribute
 #
 def routing_af(node: Box, proto: str) -> None:
@@ -174,28 +174,24 @@
         l.pop(proto,None)
         continue
       if not 'interfaces' in node.vrfs[l.vrf][proto]:                       # Start with an empty interface list
         node.vrfs[l.vrf][proto].interfaces = []
       if not 'active' in node.vrfs[l.vrf][proto]:                           # Assume there are no IGP neighbors in this VRF
         node.vrfs[l.vrf][proto].active = False
       node.vrfs[l.vrf][proto] = node[proto] + node.vrfs[l.vrf][proto]       # Add node IGP parameters to VRF IGP parameters
-      node.vrfs[l.vrf][proto].interfaces.append(data.get_box(l))            # Append a copy of the interface data
+      node.vrfs[l.vrf][proto].interfaces.append(Box(l))                     # Append a copy of the interface data
       l.pop(proto,None)                                                     # ... and remove global IGP parameters from interface
                                                                             # Next we need to find if the VRF instance of IGP matters
       for neighbor in l.neighbors:                                          # ... iterate over the list of neighbors
         n_data = topology.nodes[neighbor.node]
         if proto in n_data.get('module',[]):                                # ... and check if at least one of them uses the IGP
           node.vrfs[l.vrf][proto].active = True
                                                                             # Cleanup IGP data
   for vdata in node.get('vrfs',{}).values():                                # ... iterate over the list of VRFs
-    try:
-      proto_active = vdata.get(f'{proto}.active',False)                     # Get the IGP data for the VRF
-    except:                                                                 # ... assume 'not active' if get fails
-      proto_active = False
-    if not proto_active:                                                    # If there's no record of active IGP neighbors
+    if not get_from_box(vdata,f'{proto}.active'):                           # ... and if there's no record of active IGP neighbors
       vdata.pop(proto,None)                                                 # ... remove the VRF IGP instance
 
 #
 # remove_unaddressed_intf -- remove all interfaces without IPv4 or IPv6 address from IGP
 #
 # This routing should be called BEFORE build_vrf_interface_list to ensure the interfaces without any usable
 # L3 address are not copied into VRF interface list
```

### Comparing `networklab-1.5.2/netsim/modules/bfd.py` & `networklab-1.5.2.dev1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/bfd.yml` & `networklab-1.5.2.dev1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/bgp.py` & `networklab-1.5.2.dev1/netsim/modules/bgp.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 * n - neighbor node data
 * intf - neighbor interface data (could be addressing prefix or whatever is in the interface neighbor list)
 * ctype - session type (ibgp or ebgp)
 * extra_data - anything else we might want to pass to the neighbor data structure
 """
 def bgp_neighbor(n: Box, intf: Box, ctype: str, sessions: Box, extra_data: typing.Optional[dict] = None) -> typing.Optional[Box]:
-  ngb = data.get_box(extra_data or {})
+  ngb = Box(extra_data or {},default_box=True,box_dots=True)
   ngb.name = n.name
   ngb["as"] = n.bgp.get("as")
   ngb["type"] = ctype
   af_count = 0
   for af in ["ipv4","ipv6"]:
     if ctype in sessions[af]:
       if af in intf:
@@ -164,15 +164,15 @@
   # in different AS numbers, and create BGP neighbors
   for l in node.get("interfaces",[]):
     if 'bgp' in l and l.bgp is False:
       l.pop('bgp',None)                                               # Cleanup the flag
       continue                                                        # ... and skip interfaces with 'bgp: False'
 
     node_as =  node.bgp.get("as")                                     # Get our real AS number and the AS number of the peering session
-    node_local_as = l.get('bgp.local_as',None) or node.get('bgp.local_as',None) or node_as
+    node_local_as = data.get_from_box(l,'bgp.local_as') or data.get_from_box(node,'bgp.local_as') or node_as
 
     af_list = [ af for af in ('ipv4','ipv6','unnumbered') if af in l ]
     if not af_list:                                                   # This interface has no usable address
       continue
 
     if node_as != node_local_as:
       if not features.bgp.local_as:
@@ -193,29 +193,24 @@
       if not af_list:                                                 # Neighbor has no usable address
         continue
       #
       # Get neighbor node data and its true or interface-local AS
       #
       ngb_name = ngb_ifdata.node
       neighbor = topology.nodes[ngb_name]
-      neighbor_real_as = neighbor.get('bgp.as',None)
-      try:                                                            # Try to get neighbor local_as
-        neighbor_local_as = ( ngb_ifdata.get('bgp.local_as',None) or
-                              neighbor.get('bgp.local_as',None) or
-                              neighbor_real_as )
-      except:                                                         # Neighbor could have bgp set to False
-        neighbor_local_as = neighbor_real_as
+      neighbor_real_as = data.get_from_box(neighbor,'bgp.as')
+      neighbor_local_as = data.get_from_box(ngb_ifdata,'bgp.local_as') or data.get_from_box(neighbor,'bgp.local_as') or neighbor_real_as
 
       if not neighbor_local_as:                                       # Neighbor has no usable BGP AS number, move on
         continue
 
       if node_as == neighbor_real_as and node_local_as == neighbor_local_as:
         continue                                                      # Routers in the same AS + no local-as trickery => nothing to do here
 
-      extra_data = data.get_empty_box()
+      extra_data = Box({})
       extra_data.ifindex = l.ifindex
 
       # Figure out whether both neighbors have IPv6 LLA and/or unnumbered IPv4 interfaces
       #
       ipv6_lla = l.get('ipv6',None) is True and ngb_ifdata.get('ipv6',None) is True
       ipv6_num = isinstance(l.get('ipv6',None),str) and isinstance(ngb_ifdata.get('ipv6',None),str)
       rfc8950  = l.get('unnumbered',None) is True and ngb_ifdata.get('unnumbered',None) is True
@@ -242,15 +237,15 @@
           common.error(
             text=f'{node.name} (device {node.device}) does not support IPv4 RFC 8950-style AF over IPv6 LLA EBGP sessions (interface {l.name})',
             category=common.IncorrectValue,
             module='bgp')
           continue
 
       for k in ('local_as','replace_global_as'):
-        local_as_data = l.get(f'bgp.{k}',None) or node.get(f'bgp.{k}',None)
+        local_as_data = data.get_from_box(l,f'bgp.{k}') or data.get_from_box(node,f'bgp.{k}')
         if not local_as_data is None:
           extra_data[k] = local_as_data
 
       session_type = 'localas_ibgp' if neighbor_local_as == node_local_as else 'ebgp'
       if session_type == 'localas_ibgp':
         if not features.bgp.local_as_ibgp:
           common.error(
@@ -335,20 +330,20 @@
 
 BGP_DEFAULT_SESSIONS: typing.Final[dict] = {
   'ipv4': [ 'ibgp', 'ebgp', 'localas_ibgp' ],
   'ipv6': [ 'ibgp', 'ebgp', 'localas_ibgp' ]
 }
 
 def build_bgp_sessions(node: Box, topology: Box) -> None:
-  if not isinstance(node.get('bgp',None),Box) or not node.get('bgp.as',None):   # Sanity check
+  if not data.get_from_box(node,'bgp.as'):                        # Sanity check: do we have usable AS number
     common.fatal(f'build_bgp_sessions: node {node.name} has no usable BGP AS number, how did we get here???')
-    return                                                                      # ... it's insane, get out of here
+    return                                                        # ... not really, get out of here
 
   node.bgp.neighbors = []
-  bgp_sessions = node.bgp.get('sessions') or data.get_box(BGP_DEFAULT_SESSIONS)
+  bgp_sessions = node.bgp.get('sessions') or Box(BGP_DEFAULT_SESSIONS)
   if not validate_bgp_sessions(node,bgp_sessions,'sessions'):
     return
 
   build_ibgp_sessions(node,bgp_sessions,topology)
   build_ebgp_sessions(node,bgp_sessions,topology)
 
   # Calculate BGP address families
@@ -365,15 +360,15 @@
     if not features.bgp.activate_af:
       common.error(
         f'node {node.name} (device {node.device}) does not support configurable activation of default BGP address families',
         common.IncorrectValue,
         'bgp')
       return
 
-  activate = node.bgp.get('activate') or data.get_box(BGP_DEFAULT_SESSIONS)
+  activate = node.bgp.get('activate') or Box(BGP_DEFAULT_SESSIONS)
   if not validate_bgp_sessions(node,activate,'activate'):
     return
 
   activate_bgp_default_af(node,activate,topology)
 
 """
 bgp_set_advertise: set bgp.advertise flag on stub links and on loopback interfaces
@@ -395,23 +390,23 @@
 
 """
 process_as_list:
   If the global BGP parameters have as_list attribute, set node AS numbers and node
   RR flags accordingly
 """
 def process_as_list(topology: Box) -> None:
-  if not topology.get('bgp.as_list'):       # Do we have global bgp.as_list setting?
-    return                                  # ... nope, no work for me ;))
+  if not data.get_from_box(topology,'bgp.as_list'):         # Do we have global bgp.as_list setting?
+    return                                                  # ... nope, no work for me ;)) 
 
   try:
     must_be_dict(topology.bgp,'as_list','bgp',create_empty=False,module='bgp',abort=True)
   except Exception as ex:
     return
 
-  node_data = data.get_empty_box()
+  node_data = Box({},default_box=True,box_dots=True)
   node_list = list(topology.nodes.keys())
   for asn,as_data in topology.bgp.as_list.items():
     if not isinstance(as_data,Box):
       common.error(
         f"Invalid value in bgp.as_list for ASN {asn}\n" + \
         f"... Each ASN in a BGP as_list must be a dictionary with (at least) members key:\n"+
         f"... Found: {as_data}",
```

### Comparing `networklab-1.5.2/netsim/modules/bgp.yml` & `networklab-1.5.2.dev1/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/evpn.py` & `networklab-1.5.2.dev1/netsim/modules/evpn.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,31 +35,31 @@
     parent_path=obj_path,
     topology=topology, 
     list_name='evpn.vrfs',
     reference_dictionary='vrfs',
     reference_name='VLAN',
     create_default=create,
     merge_topology=False,
-    default_filter=lambda v: False if not isinstance(v,Box) else v.get('evpn.transit_vni',False),
+    default_filter=lambda v: False if not isinstance(v,Box) else data.get_from_box(v,'evpn.transit_vni'),
     module='evpn')
 
 def enable_evpn_af(node: Box, topology: Box) -> None:
-  bgp_session = node.get('evpn.session',[])
+  bgp_session = data.get_from_box(node,'evpn.session') or []
 
   # Enable EVPN AF on all BGP neighbors with the correct session type
   # that also use EVPN module
   #
   for bn in node.bgp.get('neighbors',[]):
     if bn.type in bgp_session and 'evpn' in topology.nodes[bn.name].get('module'):
       bn.evpn = True
 
 def get_usable_evpn_asn(topology: Box) -> int:
-  asn = ( topology.get('evpn.as',None) or
-          topology.get('vrf.as',None) or
-          topology.get('bgp.as',None) )
+  asn = data.get_from_box(topology,'evpn.as') or \
+        data.get_from_box(topology,'vrf.as') or \
+        data.get_from_box(topology,'bgp.as')
 
   if asn and data.is_true_int(asn):
     return asn
 
   common.error(
     f'Cannot get a usable global AS number to use in EVPN route targets',
     common.IncorrectValue,
@@ -120,15 +120,15 @@
 """
 
 def get_vlan_bundle_flag(vlan: Box, vname: str, topology: Box) -> bool:
   if not 'vrf' in vlan:                                             # VLAN not part of a VRF ==> VLAN service
     return False
 
   vrf = topology.vrfs[vlan.vrf]
-  if not vrf.get('evpn.bundle',None):                               # VRF does not have evpn.bundle attribute ==> VLAN service
+  if not data.get_from_box(vrf,'evpn.bundle'):                      # VRF does not have evpn.bundle attribute ==> VLAN service
     return False
 
   must_be_string(
     parent=vrf,
     key='evpn.bundle',
     path=f'vrfs.{vlan.vrf}',
     module='evpn',
@@ -151,15 +151,15 @@
 Validate that there's no evpn.bundle setting on node VRFs
 """
 
 def validate_no_node_vrf_bundle(node: Box, topology: Box) -> None:
   if not 'vrfs' in node:                                            # No VRFs defined in the node, move on
     return
   for vname,vdata in node.vrfs.items():
-    if not vdata.get('evpn.bundle',None):                           # EVPN bundle not set in VRF, move on
+    if not data.get_from_box(vdata,'evpn.bundle'):                  # EVPN bundle not set in VRF, move on
       continue
     common.error(
       f'VRF {vname} in node {node.name} cannot have evpn.bundle attribute',
       common.IncorrectValue,
       'evpn',
       hint='node_bundle')
 
@@ -167,30 +167,30 @@
 Validate transit VNI values and register them with the VNI set
 """
 def register_static_transit_vni(topology: Box) -> None:
   vni_set = _dataplane.get_id_set('vni')
   for vrf_name,vrf_data in topology.get('vrfs',{}).items():
     must_be_dict(vrf_data,'evpn',f'vrfs.{vrf_name}',create_empty=False)
 
-    transit_vni = vrf_data.get('evpn.transit_vni',None)
+    transit_vni = data.get_from_box(vrf_data,'evpn.transit_vni')
     if data.is_true_int(transit_vni):
       if transit_vni in vni_set:
         common.error(
           f'transit VNI {transit_vni} for VRF {vrf_name} is already used elsewhere',
           common.IncorrectValue,
           'evpn')
         continue
       vni_set.add(transit_vni)
 
   for n in topology.nodes.values():
     if not 'vrfs' in n:
       continue
 
     for vrf_name,vrf_data in n.vrfs.items():
-      if vrf_data.get('evpn.transit_vni',None):
+      if data.get_from_box(vrf_data,'evpn.transit_vni'):
         common.error(
           f'evpn.transit_vni can be specified only on global VRFs (found in {vrf_name} on {n.name}',
           common.IncorrectValue,
           'evpn')
 
 """
 Set transit VNI values for symmetrical IRB VRFs (REFACTOR to use _dataplane)
@@ -204,18 +204,18 @@
 def vrf_transit_vni(topology: Box) -> None:
   if not 'vrfs' in topology:
     return
 
   vni_list: typing.List[int] = []                               # List of static transit VNIs
   vni_error = False                                             # "A horrible error" flag that causes abort after the first loop
   vni_count = 0                                                 # Number of VRFs with evpn.transit_vni
-  evpn_transport = topology.get('evpn.transport','vxlan')       # Default to VXLAN transport
+  evpn_transport = data.get_from_box(topology,'evpn.transport') or 'vxlan'
 
   for vrf_name,vrf_data in topology.vrfs.items():               # First pass: build a list of statically configured VNIs
-    vni = vrf_data.get('evpn.transit_vni',None)                 # transit_vni makes no sense with MPLS transport
+    vni = data.get_from_box(vrf_data,'evpn.transit_vni')        # transit_vni makes no sense with MPLS transport
     if vni and evpn_transport != 'vxlan':
       common.error(
         f'evpn.transit_vni in VRF {vrf_name} is not allowed with mpls evpn.transport',
         common.IncorrectValue,
         'evpn')
       vni_error = True
       continue
@@ -235,15 +235,15 @@
   if vni_error:                                                 # Found serious errors, makes no sense to continue
     return
   if not vni_count:                                             # No VRF found with evpn.transit_vni, no need to waste further CPU cycles
     return
 
   vni_start = topology.defaults.evpn.start_transit_vni
   for vrf_name,vrf_data in topology.vrfs.items():               # Second pass: set transit VNI values for VRFs with "transit_vni: True"
-    if isinstance(vrf_data.get('evpn.transit_vni',None),str):
+    if isinstance(data.get_from_box(vrf_data,'evpn.transit_vni'),str):
       continue                                                  # Skip transit_vni string values (will be checked in third pass)
     transit_vni = must_be_int(
                     vrf_data,
                     key='evpn.transit_vni',
                     path=f'vrfs.{vrf_name}',
                     module='evpn',
                     min_value=4096,                             # As recommended by Cisco, outside of VLAN range
@@ -251,24 +251,24 @@
                     true_value=vni_start)                       # Make sure evpn.transit_vni is an integer
     if transit_vni == vni_start:                                # If we had to assign the default value, increment the default transit VNI
       vni_start = get_next_vni(vni_start,vni_list)
 
   for vrf_name,vrf_data in topology.vrfs.items():               # Third pass: set shared VNI values across VRFs
     if vrf_data is None:                                        # Skip empty VRF definitions
       continue
-    transit_vni = vrf_data.get('evpn.transit_vni',None)
+    transit_vni = data.get_from_box(vrf_data,'evpn.transit_vni')
     if not isinstance(transit_vni,str):                         # Skip if transit_vni is not a string
       continue
     if not transit_vni in topology.vrfs:                        # Does transit VNI refer to a valid VRF name?
       common.error(
         f'evpn.transit_vni "{transit_vni}" in VRF {vrf_name} does not refer to a valid VRF',
         common.IncorrectValue,
         'evpn')
       continue
-    foreign_vni = topology.vrfs.get(f'{transit_vni}.evpn.transit_vni',None)
+    foreign_vni = data.get_from_box(topology.vrfs,f'{transit_vni}.evpn.transit_vni')
     if not data.is_true_int(foreign_vni):
       common.error(
         f'evpn.transit_vni "{transit_vni}" in VRF {vrf_name} refers to a VRF that does not have a valid evpn.transit_vni',
         common.IncorrectValue,
         'evpn')
       continue
     vrf_data.evpn.transit_vni = foreign_vni
@@ -348,21 +348,21 @@
       hint='irb_group')
 
 """
 Check whether VXLAN IRB mode is supported by the device
 """
 def check_node_vrf_irb(node: Box, topology: Box) -> None:
   features = devices.get_device_features(node,topology.defaults)
-  evpn_transport = node.get('evpn.transport','vxlan')
+  evpn_transport = data.get_from_box(node,'evpn.transport') or 'vxlan'
 
   for vrf_name,vrf_data in node.get('vrfs',{}).items():
     if not vrf_data.get('af',None):                             # Cannot do IRB without L3 addresses ;)
       continue
 
-    symmetric_irb = vrf_data.get('evpn.transit_vni',False) or evpn_transport == 'mpls'
+    symmetric_irb = data.get_from_box(vrf_data,'evpn.transit_vni') or evpn_transport == 'mpls'
     if symmetric_irb:
       if not features.evpn.irb and evpn_transport == 'vxlan':   # ... does this device support IRB?
         common.error(
           f'VRF {vrf_name} on {node.name} uses symmetrical EVPN IRB which is not supported by {node.device} device',
           common.IncorrectValue,
           'evpn')
         continue
@@ -381,15 +381,15 @@
 """
 Check whether the node supports the requested EVPN bundle type
 """
 
 def check_node_vrf_bundle(node: Box, topology: Box) -> None:
   features = devices.get_device_features(node,topology.defaults)      # Get device features
   for vrf_name,vrf_data in node.get('vrfs',{}).items():               # Iterate over all VRFs defined on the device
-    b_type = vrf_data.get('evpn.bundle',None)                         # Get evpn.bundle value, skip if not defined
+    b_type = data.get_from_box(vrf_data,'evpn.bundle')                # Get evpn.bundle value, skip if not defined
     if not b_type:
       continue
     if not b_type in features.evpn.bundle:                            # EVPN bundle type not supported by the device
       common.error(
         f"'{b_type}'' EVPN bundle service used in VRF {vrf_name} is not supported by device {node.device} (node: {node.name})",
         common.IncorrectValue,
         'evpn')
@@ -413,15 +413,15 @@
 
   def module_post_node_transform(self, topology: Box) -> None:
     validate_evpn_lists(topology,'topology',topology,create=True)
     for n in topology.nodes.values():
       validate_evpn_lists(n,f'nodes.{n.name}',topology,create=False)
 
     vrf_transit_vni(topology)
-    for vname in topology.get('evpn.vlans',[]):
+    for vname in data.get_from_box(topology,'evpn.vlans') or []:
       create_vlan_service(vname,topology)
 
     vrf_irb_setup(topology)
 
   """
   Node post-transform: runs after VXLAN module
```

### Comparing `networklab-1.5.2/netsim/modules/evpn.yml` & `networklab-1.5.2.dev1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/gateway.py` & `networklab-1.5.2.dev1/netsim/modules/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 
 #
 # Remove unicast IPv4 addresses from interfaces that use 'anycast' gateway protocol
 # and have 'gateway.anycast.unicast' set to False
 #
 def cleanup_unicast_ip(node: Box) -> None:
   for intf in node.interfaces:
-    if not intf.get('gateway',False):                       # This interface not using FHRP or FHRP is disabled
+    if not intf.get('gateway',False):                               # This interface not using FHRP or FHRP is disabled
       continue
 
-    if intf.gateway.protocol != 'anycast':                  # Leave non-anycast FHRP implementations alone, they need node IP addresses
+    if intf.gateway.protocol != 'anycast':                          # Leave non-anycast FHRP implementations alone, they need node IP addresses
       continue
 
-    if intf.get('gateway.anycast.unicast',None) is False:   # Are we forbidden to use unicast IP addresses together with anycast ones?
-      intf.pop('ipv4',None)                                 # No unicast with anycast ==> pop the address
+    if data.get_from_box(intf,'gateway.anycast.unicast') is False:  # Are we forbidden to use unicast IP addresses together with anycast ones?
+      intf.pop('ipv4',None)                                         # No unicast with anycast ==> pop the address
 
 #
 # Default settings copied onto individual links have parameters for every known FHRP protocol.
 # We don't need those parameters on every interface -- this function cleans up unusud gateway protocol
 # parameters from interfaces and returns a list of active protocols so we know what to clean on the
 # node level.
```

### Comparing `networklab-1.5.2/netsim/modules/gateway.yml` & `networklab-1.5.2.dev1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/isis.py` & `networklab-1.5.2.dev1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/isis.yml` & `networklab-1.5.2.dev1/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/mpls.py` & `networklab-1.5.2.dev1/netsim/modules/mpls.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   node.ldp = node.mpls.ldp
   node.mpls.pop('ldp',None)
   _routing.router_id(node,'ldp',topology.pools)
 
   for intf in node.get('interfaces',[]):
     if not 'ipv4' in intf:
       continue                                                    # Cannot run MPLS LDP on non-IPv4 interface
-    intf_ldp = intf.get('mpls.ldp',None)                          # ... get interface LDP status (if set)
+    intf_ldp = data.get_from_box(intf,'mpls.ldp')                 # ... get interface LDP status (if set)
     if 'vrf' in intf:
       if not intf_ldp:                                            # ... VRF LDP must be enabled on individual interfaces (MPLS CSC)
         continue
       if not features.mpls.csc:
         common.error(
           f'Device {node.device} does not support MPLS CsC (LDP in VRF) configured on {node.name}',
           common.IncorrectValue,
@@ -75,15 +75,15 @@
         key=feature,
         path=f'nodes.{node.name}.mpls.{feature}',
         valid_values=BGP_SESSIONS,
         create_empty=False,
         module='mpls'):
       return False
 
-    node.mpls[feature] = data.get_empty_box()
+    node.mpls[feature] = Box({})
     for af in node.af:
       node.mpls[feature][af] = session_list
   elif isinstance(node.mpls[feature],Box):
     for af in AF_LIST:
       if not af in node.mpls[feature]:
         continue
 
@@ -144,15 +144,15 @@
   for n in node.bgp.neighbors:                          # Now iterate over BGP neighbors
     if 'ipv4' in n and n.type in node.mpls['6pe']:      # Do we have an IPv4 session with the neighbor and 6PE enabled?
       n['6pe'] = True                                   # ... enable 6PE AF on IPv4 neighbor session
 
       # If the neighbor is also using 6PE and will enable 6PE on this session
       # ... then we don't need IPv6 BGP session --> remove it
       #
-      if n.type in topology.nodes[n.name].get('mpls.6pe',[]):
+      if n.type in (data.get_from_box(topology.nodes[n.name],'mpls.6pe') or []):
         n.pop('ipv6',None)
 
 def prune_mplsvpn_af(setting: Box, node: Box) -> None:
   vrf_af :dict = {}
 
   for af in AF_LIST:
     for vdata in node.get('vrfs',{}).values():
```

### Comparing `networklab-1.5.2/netsim/modules/mpls.yml` & `networklab-1.5.2.dev1/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/ospf.py` & `networklab-1.5.2.dev1/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/ospf.yml` & `networklab-1.5.2.dev1/netsim/modules/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/srv6.py` & `networklab-1.5.2.dev1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/vlan.py` & `networklab-1.5.2.dev1/netsim/modules/vlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 import typing
 from box import Box
 
 from . import _Module,_routing,get_effective_module_attribute,_dataplane
 from .. import common
 from .. import data
-from ..data import global_vars,get_empty_box,get_box,get_global_parameter
+from ..data import global_vars,get_from_box,get_empty_box,get_box,get_global_parameter
 from ..data.validate import validate_attributes
 from ..data.types import must_be_id,must_be_list,must_be_dict
 from .. import addressing
 from ..augment import devices,groups
 from ..augment import links
 
 # Static lists of keywords
@@ -33,59 +33,59 @@
   for n in topology.nodes.values():
     _dataplane.extend_id_set('vlan_id',_dataplane.build_id_set(n,'vlans','id',f'nodes.{n.name}'))
 
 #
 # routed_access_vlan: Given a link with access/native VLAN, check if all nodes on the link use routed VLAN
 #
 def routed_access_vlan(link: Box, topology: Box, vlan: str) -> bool:
-  def_link  = link.get('vlan.mode',None)
-  def_vlan  = topology.get(f'vlans.{vlan}.mode',None)
-  def_global = topology.get('vlan.mode','irb')
+  def_link  = get_from_box(link,'vlan.mode')
+  def_vlan  = get_from_box(topology,f'vlans.{vlan}.mode')
+  def_global = get_from_box(topology,'vlan.mode') or 'irb'
 
   if common.debug_active('vlan'):
     print(f'routed_access_vlan: {link}')
     print(f'... vlan {vlan} def_mode {def_vlan}')
   for intf in link.interfaces:
-    mode = (
-      intf.get('vlan.mode',def_link) or
-      topology.nodes[intf.node].get(f'vlans.{vlan}.mode',def_vlan) or
-      topology.nodes[intf.node].get('vlan.mode',def_global) or
-      'irb')
+    mode = get_from_box(intf,'vlan.mode') or \
+           def_link or \
+           get_from_box(topology.nodes[intf.node],f'vlans.{vlan}.mode') or \
+           def_vlan or \
+           get_from_box(topology.nodes[intf.node],'vlan.mode') or \
+           def_global or 'irb'
     if mode != 'route':
       return False
 
   if common.debug_active('vlan'):
     print(f'... VLAN is routed (returning True)')
   return True
 
 #
 # interface_vlan_mode: Given an interface, a node, and topology, find interface VLAN mode
 #
 def interface_vlan_mode(intf: Box, node: Box, topology: Box) -> str:
-  vlan = intf.get('vlan.access',None) or intf.get('vlan.native',None)
+  vlan = get_from_box(intf,'vlan.access') or get_from_box(intf,'vlan.native')
   if not vlan:
     return 'irb'
-  return (
-    intf.get('vlan.mode',None) or
-    node.get(f'vlans.{vlan}.mode',None) or
-    node.get('vlan.mode',None) or
-    topology.get(f'vlans.{vlan}.mode',None) or
-    topology.get('vlan.mode',None) or 'irb' )
+  return get_from_box(intf,'vlan.mode') or \
+         get_from_box(node,f'vlans.{vlan}.mode') or \
+         get_from_box(node,'vlan.mode') or \
+         get_from_box(topology,f'vlans.{vlan}.mode') or \
+         get_from_box(topology,'vlan.mode') or 'irb'
 
 #
 # Validate VLAN attributes and set missing attributes:
 #
 # * VLAN and VNI
 # * Subnet prefix
 # * VLAN forwarding mode
 #
 def validate_vlan_attributes(obj: Box, topology: Box) -> None:
   obj_name = 'global VLANs' if obj is topology else obj.name
   obj_path = 'vlans' if obj is topology else f'nodes.{obj.name}.vlans'
-  default_fwd_mode = obj.get('vlan.mode',None) or get_global_parameter(topology,'vlan.mode')
+  default_fwd_mode = get_from_box(obj,'vlan.mode') or get_global_parameter(topology,'vlan.mode')
 
   if not 'vlans' in obj:
     return
 
   for vname in list(obj.vlans.keys()):
     must_be_id(parent=None,key=vname,path=f'NOATTR:VLAN name {vname} in {obj_name}',module='vlan')
 
@@ -415,15 +415,15 @@
 
 """
 create_vlan_link_data: Create initial link data for a VLAN member link
 
 Used by create_vlan_links and create_loopback_vlan_links
 """
 def create_vlan_link_data(init: typing.Union[Box,dict],vname: str, parent: typing.Any, topology: Box) -> Box:
-  link_data = data.get_box(init)
+  link_data = Box(init,default_box=True,box_dots=True)
   link_data.linkindex = topology.links[-1].linkindex + 1
   link_data.parentindex = parent
   link_data.vlan.access = vname
   link_data.vlan_name = vname
   link_data.type = 'vlan_member'
   link_data.interfaces = []
   fix_vlan_mode_attribute(link_data)
@@ -446,20 +446,20 @@
 def create_vlan_member_interface(
       init: typing.Union[Box,dict],               # Initial VLAN parameters taken from vlan.trunk
       vname: str,                                 # VLAN name
       parent_intf: Box,                           # Parent interface data (used to get node name etc)
       topology: Box,
       loop_index: int) -> Box:                    # selfloop_ifindex to support crazy topologies
 
-  intf_data = data.get_box(init)
+  intf_data = Box(init,default_box=True,box_dots=True)
   intf_data.node = parent_intf.node
   intf_data._selfloop_ifindex = loop_index                  # Used in find_parent_interface to disambiguate self-links
   intf_data.vlan.access = vname
 
-  if 'mode' in parent_intf.vlan and not intf_data.get('vlan.mode',None):
+  if 'mode' in parent_intf.vlan and not get_from_box(intf_data,'vlan.mode'):
     intf_data.vlan.mode = parent_intf.vlan.mode             # vlan.mode is inherited from trunk dictionary or parent interface
 
   intf_node = topology.nodes[parent_intf.node]
   if interface_vlan_mode(intf_data,intf_node,topology) == 'bridge':     # Is this VLAN interface in bridge mode?
     intf_data.ipv4 = False                                              # ... if so, disable addressing on this interface
     intf_data.ipv6 = False
 
@@ -543,38 +543,38 @@
       link_data = { '_linkname': f'nodes.{n.name}.vlans.{vname}' }      # Create a vlan_member link with fake parent (nobody should ever use it)
       link_data = create_vlan_link_data(link_data,vname,'loopback',topology)
       prefix = topology.vlans[vname].get('prefix',None)                 # Copy VLAN prefix into link_data
       if prefix:
         link_data.prefix = prefix
 
       # Create interface data using fake parent interface
-      fake_parent = data.get_box({'node': n.name})
+      fake_parent = Box({'node': n.name},default_box=True,box_dots=True)
       intf_data = create_vlan_member_interface({},vname,fake_parent,topology,0)
 
       if interface_vlan_mode(intf_data,n,topology) == 'irb':            # We're adding loopback links only for IRB VLANs
         link_data.interfaces.append(intf_data)
         topology.links.append(link_data)
 
 """
 get_vlan_data: Get VLAN data structure (node or topology or interface neighbors)
 """
 def get_vlan_data(vlan: str, node: Box, topology: Box, intf: Box) -> typing.Optional[Box]:
-  vlan_data = topology.get(f'vlans.{vlan}',None) or node.get(f'vlans.{vlan}',None)
+  vlan_data = get_from_box(topology,f'vlans.{vlan}') or get_from_box(node,f'vlans.{vlan}')
   if not vlan_data and 'neighbors' in intf:
     for n in intf.neighbors:  # Look for local vlan in neighbor
-      vlan_data = topology.nodes[n.node].get(f'vlans.{vlan}',None)
+      vlan_data = get_from_box(topology.nodes[n.node],f'vlans.{vlan}')
       if vlan_data:
         break
   return vlan_data
 
 """
 get_vlan_mode: Get VLAN mode attribute (node or topology), default 'irb'
 """
 def get_vlan_mode(node: Box, topology: Box) -> str:
-  return node.get('vlan.mode',None) or topology.get('vlan.mode',None) or 'irb'
+  return get_from_box(node,'vlan.mode') or get_from_box(topology,'vlan.mode') or 'irb'
 
 """
 update_vlan_neighbor_list: Build a VLAN-wide list of neighbors
 """
 def update_vlan_neighbor_list(vlan: str, phy_if: Box, svi_if: Box, node: Box,topology: Box) -> None:
   vlan_data = get_vlan_data(vlan,node,topology,phy_if)                  # Try to get global or node-level VLAN data
   if vlan_data is None:                                                 # ... and get out if there's none
@@ -591,28 +591,26 @@
     n_map[node.name].ifname = svi_if.ifname                             # ... it is, fix the interface name
     for af in ('ipv4','ipv6'):
       if af in svi_if:
         n_map[node.name][af] = svi_if[af]
       else:
         n_map[node.name].pop(af,None)
   else:
-    n_data = data.get_box({
-               'ifname': svi_if.ifname,
-               'node': node.name })                                     # ... not yet, create neighbor data
+    n_data = { 'ifname': svi_if.ifname, 'node': node.name }             # ... not yet, create neighbor data
     for af in ('ipv4','ipv6'):
       if af in svi_if:                                                  # ... copy SVI interface addresses to neighbor data
         n_data[af] = svi_if[af]
     vlan_data.neighbors.append(n_data)                                  # Add current node as a neighbor to VLAN neighbor list
 
 """
 create_node_vlan: Create a local (node) copy of a VLAN used on an interface
 """
 def create_node_vlan(node: Box, vlan: str, topology: Box) -> typing.Optional[Box]:
   if not vlan in node.vlans:                                        # Do we have VLAN defined in the node?
-    node.vlans[vlan] = data.get_box(topology.vlans[vlan])           # ... no, create a copy of the global definition
+    node.vlans[vlan] = Box(topology.vlans[vlan])                    # ... no, create a copy of the global definition
     if not node.vlans[vlan]:                                        # pragma: no cover -- we don't have a global definition?
       common.fatal(                                                 # ... this should have been detected way earlier
         f'Unknown VLAN {vlan} used on node {node.name}','vlan')
       return None
     for m in list(node.vlans[vlan].keys()):                         # Remove irrelevant module parameters
       if not m in node.module and m in topology.module:             # ... it's safe to use direct references, everyone is using VLAN module
         node.vlans[vlan].pop(m,None)
@@ -644,16 +642,16 @@
   #
   svi_skipattr = [ k for k in list(topology.defaults.vlan.attributes.vlan_no_propagate or []) if k != "mode" ] + \
                   list(topology.defaults.vlan.attributes.vlan_svi_no_propagate)
 
   iflist_len = len(node.interfaces)
   for ifidx in range(0,iflist_len):
     ifdata = node.interfaces[ifidx]
-    native_vlan = ifdata.get('vlan.native',None)
-    access_vlan = ifdata.get('vlan.access',native_vlan)
+    native_vlan = get_from_box(ifdata,'vlan.native')
+    access_vlan = get_from_box(ifdata,'vlan.access') or native_vlan
     if not access_vlan:                                                     # No access VLAN on this interface?
       continue                                                              # ... good, move on
 
     routed_intf = interface_vlan_mode(ifdata,node,topology) == 'route'      # Identify routed VLAN interfaces
     vlan_subif  = routed_intf and ifdata.get('type','') == 'vlan_member'    # ... and VLAN-based subinterfaces
 
     vlan_data = create_node_vlan(node,access_vlan,topology)
@@ -666,15 +664,15 @@
     if routed_intf:                                                         # Routed VLAN access interface, turn it back into native interface
       for k in ('access','native'):                                         # ... remove access VLAN attributes
         ifdata.vlan.pop(k,None)
 
       if not ifdata.vlan:                                                   # ... and VLAN dictionary if there's nothing else left
         ifdata.pop('vlan',None)
 
-      vlan_copy = get_box({ k:v for (k,v) in vlan_data.items() if not k in svi_skipattr and k != 'mode' })
+      vlan_copy = { k:v for (k,v) in vlan_data.items() if not k in svi_skipattr and k != 'mode' }
 
       if vlan_subif:
         ifdata.vlan.mode = 'route'
         ifdata.vlan.access_id = vlan_data.id
       else:
         ifdata._vlan_mode = 'route'                                         # Flags we need to clean up up the routed native VLAN mess
         if native_vlan:                                                     # ... we can't use the vlan.* attributes as they might get removed
@@ -694,16 +692,18 @@
 
     if not access_vlan in vlan_ifmap:                                       # Do we need to create a SVI interface?
       skip_attr = list(skip_ifattr)                                         # Create a local copy of the attribute skip list
       vlan_mode = ifdata.vlan.get('mode','') or vlan_data.get('mode','')    # Get VLAN forwarding mode
       if vlan_mode == 'bridge':                                             # ... and skip IP addresses for bridging-only VLANs
         skip_attr.extend(['ipv4','ipv6'])
         # continue  # JvB: in fact, skip creating SVI for L2-only VLANs
-      vlan_ifdata = data.get_box(                                           # Copy non-physical interface attributes into SVI interface
-        { k:v for k,v in ifdata.items() if k not in skip_attr })            # ... that will also give us IP addresses
+      vlan_ifdata = Box(                                                    # Copy non-physical interface attributes into SVI interface
+        { k:v for k,v in ifdata.items() if k not in skip_attr },            # ... that will also give us IP addresses
+        default_box=True,
+        box_dots=True)
       if vlan_mode:                                                         # Set VLAN forwarding mode for completness' sake
         vlan_ifdata.vlan.mode = vlan_mode
       vlan_ifdata.ifindex = node.interfaces[-1].ifindex + 1                 # Fill in the rest of interface data:
       vlan_ifdata.ifname = svi_name.format(                                 # ... ifindex, ifname, description
                               vlan=vlan_data.id,
                               bvi=vlan_data.bridge_group,
                               ifname=ifdata.ifname)
@@ -731,15 +731,15 @@
 
 """
 set_svi_neighbor_list: set SVI neighbor list from VLAN neighbor list
 """
 def set_svi_neighbor_list(node: Box, topology: Box) -> None:
   for ifdata in node.interfaces:
     if 'vlan_name' in ifdata:
-      if ifdata.get('vlan.routed_link',False):                              # Don't update neighbors on a routed VLAN link
+      if get_from_box(ifdata,'vlan.routed_link'):                           # Don't update neighbors on a routed VLAN link
         continue
 
       vlan_data = get_vlan_data(ifdata.vlan_name,node,topology,ifdata)      # Try to get global or local VLAN data
       if vlan_data is None:                                                 # Not found?
         continue                                                            # ... too bad
 
       if not 'host_count' in vlan_data:                                     # Calculate the number of hosts attached to the VLAN
@@ -756,15 +756,15 @@
         ifdata.name = ifdata.name + " -> [" + ",".join([ n.node for n in ifdata.neighbors]) + "]"
 
 """
 map_trunk_vlans: build a list of VLAN IDs on trunk interfaces
 """
 def map_trunk_vlans(node: Box, topology: Box) -> None:
   for intf in node.interfaces:
-    trunk = intf.get('vlan.trunk',None)
+    trunk = get_from_box(intf,'vlan.trunk')
     if not trunk:
       continue
 
     vlan_list = []
     for vlan in list(trunk.keys()):
       if not vlan in node.vlans:
         common.fatal(f'Internal error: VLAN {vlan} should be already defined on node {node.name}\n... interface {intf}')
@@ -776,15 +776,15 @@
 """
 find_parent_interface: Find the parent interface of a VLAN member subinterface
 """
 def find_parent_interface(intf: Box, node: Box, topology: Box) -> typing.Optional[Box]:
   if common.debug_active('vlan'):
     print( f"find_parent_interface node={node.name} intf.parentindex={intf.parentindex} selfloop_ifindex={intf._selfloop_ifindex}" )
 
-  candidates = [ i for i in node.interfaces if i.get('linkindex',None) == intf.parentindex ]
+  candidates = [ i for i in node.interfaces if i.get('linkindex') == intf.parentindex ]
   if candidates:
     return candidates[ 0 if len(candidates)==1 else intf._selfloop_ifindex ]
 
   if common.debug_active('vlan'):
     print( f"find_parent_interface node={node.name} not found -> returns None" )
   return None
 
@@ -860,15 +860,15 @@
       parent_intf.subif_index = parent_intf.subif_index + 1
     else:
       parent_intf.subif_index = features.vlan.first_subif_id or 1
 
     ifname_data = parent_intf + intf                                  # Add parent interface data to subinterface data
     ifname_data.ifname = parent_intf.ifname                           # ... making sure ifname is coming from parent interface
 
-    old_intf = data.get_box({ 'ifname': intf.ifname })                # Create a fake interface with old interface name
+    old_intf = Box({ 'ifname': intf.ifname })                         # Create a fake interface with old interface name
     intf.ifname = subif_name.format(**ifname_data)
     intf.parent_ifindex = parent_intf.ifindex
     intf.parent_ifname = parent_intf.ifname
     intf.virtual_interface = True
     if 'vlan_name' in intf:                                           # Update VLAN neighbor list if we have the VLAN name
       link_data = topology.links[intf.linkindex - 1]
       if not routed_access_vlan(link_data,topology,intf.vlan_name):   # ... and if the VLAN is not a routed access VLAN
@@ -939,15 +939,15 @@
     parent_intf_list = [ x for x in node.interfaces if x.ifindex == intf.parent_ifindex ]
     if not parent_intf_list:
       common.fatal(f'Internal error: cannot find parent interface for {intf} in node {node.name}')
       return
 
     parent_intf = parent_intf_list[0]
     if parent_intf is None \
-         or parent_intf.get('vlan.trunk_id',None) is None:            # No VLAN trunk left on the parent interface?
+         or get_from_box(parent_intf,'vlan.trunk_id') is None:        # No VLAN trunk left on the parent interface?
       continue                                                        # ... cool, we're done
 
     if not parent_intf.ifindex in err_ifmap:                          # We have a problem. Do we have to generate an error?
       common.error(
         f'Device type {node.device} does not support mixed bridged/routed VLAN trunks\n'+ \
         f'... node {node.name} interface {parent_intf.ifname}: {parent_intf.name}',
         common.IncorrectValue,
@@ -979,20 +979,20 @@
 VLAN (because a VLAN is modeled as a number of link).
 """
 def fix_vlan_gateways(topology: Box) -> None:
   for node in topology.nodes.values():
     if node.get('role') != 'host':                                    # Fix first-hop gateways only for hosts
       continue
     for intf in node.get('interfaces',[]):                            # Iterate over all interfaces
-      if intf.get('gateway.ipv4',None):                               # ... that don't have an IPv4 gateway
+      if get_from_box(intf,'gateway.ipv4'):                           # ... that don't have an IPv4 gateway
         continue
 
       gw_found = False
       for neighbor in intf.get('neighbors',[]):                       # Iterate over all neighbors trying to find first-hop gateway
-        if not neighbor.get('gateway.ipv4',None):                     # ... does the neighbor have first-hop gateway set?
+        if not get_from_box(neighbor,'gateway.ipv4'):                 # ... does the neighbor have first-hop gateway set?
           continue                                                    # ... nope, keep going
 
         n_node = topology.nodes[neighbor.node]
         if n_node.get('role') == 'host':                              # Check whether the neighbor is a host
           continue                                                    # ... don't trust gateway information coming from another host
 
         gw_found = True                                               # Found a first-hop gateway on a non-host. Mission Accomplished
@@ -1014,15 +1014,15 @@
 """
 populate_node_vlan_data -- merge topology VLANs into node VLANs that were copied from groups.node_data
 """
 def populate_node_vlan_data(n: Box, topology: Box) -> None:
   if 'vlans' in n:                                                          # Copy topology VLAN data into node VLAN data
     for vname in n.vlans.keys():                                            # ... to cope with nodes that had VLANs defined
       if vname in topology.get('vlans',{}):                                 # ... through groups.node_data
-        topo_data = data.get_box(topology.vlans[vname])                     # Create a copy of topology VLAN
+        topo_data = Box(topology.vlans[vname])                              # Create a copy of topology VLAN
         topo_data.pop('neighbors',None)                                     # ... remove neighbors
         for m in list(topo_data.keys()):                                    # ... and irrelevant module attributes
           if not m in n.module and m in topology.module:
             topo_data.pop(m,None)
         n.vlans[vname] = topo_data + n.vlans[vname]                         # ... now merge with the VLAN data
 
 """
@@ -1084,15 +1084,15 @@
           module='vlan')      # Check that we're dealing with a VLAN dictionary and return if there's an error
       except:
         return
 
     if 'groups' in topology:
       groups.export_group_node_data(topology,'vlans','vlan',copy_keys=['id','vni'])
 
-    if topology.get('vlan.mode',None):
+    if get_from_box(topology,'vlan.mode'):
       if topology.vlan.mode not in vlan_mode_kwd:     # pragma: no cover
         common.error(
           f'Invalid global vlan.mode value {topology.vlan.mode}',
           common.IncorrectValue,
           'vlan')
         return
 
@@ -1102,15 +1102,15 @@
       create_vlan_access_links(topology)
       validate_vlan_attributes(topology,topology)
 
   def node_pre_transform(self, node: Box, topology: Box) -> None:
     if 'vlans' in node:
       for vname in node.vlans.keys():
         if node.vlans[vname] is None:
-          node.vlans[vname] = get_empty_box()
+          node.vlans[vname] = {}
         if vname in topology.get('vlans',{}):                                     # We have a VLAN defined globally and in a node
           for kw in ('prefix','id','vni'):                                        # These three attributes MUST NOT be different
             if not kw in node.vlans[vname]:                                       # OK, attribute not in node VLAN, move on
               continue
 
             if kw in topology.vlans[vname] and node.vlans[vname][kw] == topology.vlans[vname][kw]:
               continue                                                            # Overlap, but the attributes match. OK...
@@ -1124,15 +1124,15 @@
 
     validate_vlan_attributes(node,topology)
 
   def link_pre_transform(self, link: Box, topology: Box) -> None:
     if link.get('type','') == 'vlan_member':                                      # Skip VLAN member links, we've been there...
       return
 
-    v_attr = data.get_empty_box()
+    v_attr = Box({},default_box=True,box_dots=True)
     link_ok = check_link_vlan_attributes(link,link,v_attr,topology)               # Check link-level VLAN attributes
 
     for intf in link.interfaces:
       link_ok = link_ok and check_link_vlan_attributes(intf,link,v_attr,topology) # Check interface VLAN attributes
 
     if not link_ok:
       return
@@ -1157,18 +1157,19 @@
       create_vlan_links(link,v_attr,topology)
 
     svi_skipattr = topology.defaults.vlan.attributes.vlan_no_propagate or []      # VLAN attributes not copied into link data
     link_vlan = get_link_access_vlan(v_attr)
     routed_vlan = False
     if not link_vlan is None:
       routed_vlan = routed_access_vlan(link,topology,link_vlan)
-      vlan_data = topology.get(f'vlans.{link_vlan}',None)                         # Get global VLAN data
+      vlan_data = get_from_box(topology,f'vlans.{link_vlan}')                     # Get global VLAN data
       if isinstance(vlan_data,Box):
-        vlan_data = data.get_box({ k:v for (k,v) in vlan_data.items() \
-                                if k not in svi_skipattr })                       # Remove VLAN-specific data
+        vlan_data = Box({ k:v for (k,v) in vlan_data.items() \
+                                if k not in svi_skipattr },
+                        default_box=True,box_dots=True)                           # Remove VLAN-specific data
         fix_vlan_mode_attribute(vlan_data)                                        # ... and turn mode into vlan.mode
         for (k,v) in vlan_data.items():                                           # Now add the rest to link data
           if not k in link:                                                       # ... have to do the deep merge manually as
             link[k] = v                                                           # ... we cannot just replace link data structure
           elif isinstance(link[k],Box) and isinstance(vlan_data[k],Box):
             link[k] = vlan_data[k] + link[k]
```

### Comparing `networklab-1.5.2/netsim/modules/vlan.yml` & `networklab-1.5.2.dev1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/modules/vrf.py` & `networklab-1.5.2.dev1/netsim/modules/vrf.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing, re
 import netaddr
 from box import Box
 
 from . import _Module,_routing,_dataplane,get_effective_module_attribute
 from .. import common
 from .. import data
-from ..data import global_vars
+from ..data import get_from_box,global_vars
 from ..data.validate import validate_attributes
 from ..data.types import must_be_list,must_be_dict,must_be_id
 from ..augment import devices,groups,links
 from .. import addressing
 
 def populate_vrf_static_ids(topology: Box) -> None:
   for k in ('id','rd'):
@@ -25,19 +25,19 @@
     for k in ('id','rd'):
       _dataplane.extend_id_set(f'vrf_{k}',_dataplane.build_id_set(n,'vrfs',k,f'nodes.{n.name}'))
 
 #
 # Get a usable AS number. Try bgp.as then vrf.as from node and global settings
 #
 def get_rd_as_number(obj: Box, topology: Box) -> typing.Optional[typing.Any]:
-  return (
-    obj.get('bgp.as',None) or
-    obj.get('vrf.as',None) or
-    topology.get('bgp.as',None) or
-    topology.get('vrf.as',None) )
+  return \
+    get_from_box(obj,'bgp.as') or \
+    get_from_box(obj,'vrf.as') or \
+    get_from_box(topology,'bgp.as') or \
+    get_from_box(topology,'vrf.as')
 
 #
 # Parse rd/rt value -- check whether the RD/RT value is in N:N format
 #
 
 def parse_rdrt_value(value: str) -> typing.Optional[typing.List[typing.Union[int,str]]]:
   try:
@@ -137,16 +137,15 @@
 # Get VRF RD value needed for import/export values. 
 #
 # WARNING: Global value takes precedence over node value because you might want to change per-node RD
 # values for weird topologies like hub-and-spoke
 #
 def get_vrf_id(vname: str, obj: Box, topology: Box) -> typing.Optional[str]:
   obj_name = 'global VRFs' if obj is topology else obj.name
-  vpath = f'vrfs.{vname}'
-  vdata = topology.get(vpath,None) or obj.get(vpath,None)
+  vdata = get_from_box(topology,['vrfs',vname]) or get_from_box(obj,['vrfs',vname]) or None
 
   if vdata is None:
     common.error(
       f'Cannot get VRF ID for unknown VRF {vname} needed in {obj_name}',
       common.MissingValue,
       'vrf')
     return None
@@ -239,48 +238,49 @@
 
 def validate_vrf_route_leaking(node : Box) -> None:
   for vname,vdata in node.vrfs.items():
     simple_rt = [ vdata.rd ]
     leaked_routes = vdata['import'] and vdata['import'] != simple_rt
     leaked_routes = leaked_routes or (vdata['export'] and vdata['export'] != simple_rt)
     if leaked_routes:
-      if not node.get('bgp.as',None):
-        if node.get('vrf.as',None):
+      if not get_from_box(node,'bgp.as'):
+        if get_from_box(node,'vrf.as'):
           node.bgp['as'] = node.vrf['as']
         else:
           common.error(
             f"VRF {vname} on {node.name} uses inter-VRF route leaking, but there's no BGP AS configured on the node",
             common.MissingValue,
             'vrf')
 
 def vrf_loopbacks(node : Box, topology: Box) -> None:
-  loopback_name = devices.get_device_attribute(node,'loopback_interface_name',topology.defaults)
+  loopback_name = devices.get_device_attribute(node,'loopback_interface_name',topology.defaults) or \
+                  devices.get_device_attribute(node,'features.vrf.loopback_interface_name',topology.defaults)
 
   if not loopback_name:                                                        # pragma: no cover -- hope we got device settings right ;)
     common.print_verbose(f'Device {node.device} used by {node.name} does not support VRF loopback interfaces - skipping assignment.')
     return
 
   node_vrf_loopback = get_effective_module_attribute(
                         path = 'vrf.loopback',
                         node = node,
                         topology = topology)
   for vrfname,v in node.vrfs.items():
-    vrf_loopback = v.get('loopback',None) or node_vrf_loopback        # Do we have VRF loopbacks enabled in the node or in the VRF?
-    if not vrf_loopback:                                              # ... nope, move on
+    vrf_loopback = get_from_box(v,'loopback') or node_vrf_loopback          # Do we have VRF loopbacks enabled in the node or in the VRF?
+    if not vrf_loopback:                                                    # ... nope, move on
       continue
 
-    # Note: set interface ifindex to v.vrfidx if you want to have VRF-numbered loopbacks
-    #
-    ifdata = data.get_box({                                           # Create interface data structure
+    ifdata = Box({
+      'virtual_interface': True,
       'type': "loopback",
       'name': f'VRF Loopback {vrfname}',
+      'ifindex': node.interfaces[-1].ifindex + 1,
+      'ifname': loopback_name.format(vrfidx=v.vrfidx,ifindex=v.vrfidx),     # Use VRF-specific and generic loopback index
       'neighbors': [],
-      'vrf': vrfname,})
-
-    links.create_virtual_interface(node,ifdata,topology.defaults)     # Use common function to create loopback interface
+      'vrf': vrfname,
+    },default_box=True,box_dots=True)
 
     if isinstance(vrf_loopback,bool):
       vrfaddr = addressing.get(topology.pools, ['vrf_loopback'])
     else:
       vrfaddr = addressing.parse_prefix(vrf_loopback)
 
     if not vrfaddr:
@@ -459,15 +459,15 @@
   #
   def node_post_link_transform(self, node: Box, topology: Box) -> None:
     for ifdata in node.interfaces:
       if not 'vrf' in ifdata:                                           # Check only VRF interfaces
         continue
 
       vrf_data_path = f'vrfs.{ifdata.vrf}'
-      if not topology.get(vrf_data_path,None) and not node.get(vrf_data_path,None):
+      if not get_from_box(topology,vrf_data_path) and not get_from_box(node,vrf_data_path):
         common.error(
           f'VRF {ifdata.vrf} used on an interface in {node.name} is not defined in the node or globally',
           common.MissingValue,
           'vrf')
         continue
 
       if not ifdata.vrf in node.vrfs:                                   # Local VRF not present, mark as required
@@ -525,9 +525,9 @@
       validate_vrf_route_leaking(node)
 
       # Set additional loopbacks (one for each defined VRF)
       vrf_loopbacks(node, topology)
 
     # Finally, set BGP router ID if we set BGP AS number
     #
-    if node.get('bgp.as',None) and not node.get('bgp.router_id',None):
+    if get_from_box(node,'bgp.as') and not get_from_box(node,'bgp.router_id'):
       _routing.router_id(node,'bgp',topology.pools)
```

### Comparing `networklab-1.5.2/netsim/modules/vxlan.py` & `networklab-1.5.2.dev1/netsim/modules/vxlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typing
 from box import Box
 import netaddr
 
 from . import _Module,get_effective_module_attribute,_dataplane
 from .. import common
 from .. import data
+from ..data import get_from_box
 from ..data.validate import must_be_int,must_be_string
 from ..augment import devices
 from .. import addressing
 
 """
 register_static_vni -- register all static VNIs
 """
@@ -47,15 +48,15 @@
 
 Inputs:
 * toponode: Topology or node
 * obj_path: object path (topology or nodes.x)
 * topology: pointer to topology so we can access global VLANs
 """
 def assign_vni(toponode: Box, obj_path: str, topology: Box) -> None:
-  vxlan_vlans = toponode.get('vxlan.vlans',None)
+  vxlan_vlans = get_from_box(toponode,'vxlan.vlans')
   if not vxlan_vlans:                                             # No VXLAN-enabled VLANs in the current data object ==> nothing to do
     return
 
   vni_ids = _dataplane.get_id_set('vni')
   for vname in vxlan_vlans:
     if not vname in toponode.get('vlans',{}):                     # Skip VXLAN-enabled VLANs that are not present on a node
       continue
```

### Comparing `networklab-1.5.2/netsim/modules/vxlan.yml` & `networklab-1.5.2.dev1/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/outputs/__init__.py` & `networklab-1.5.2.dev1/netsim/outputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #
 # Dynamic output framework
 # 
 # Individual output routines are defined in modules within this directory inheriting
 # TopologyOutput class and replacing or augmenting its methods (most commonly, write)
 #
 
+import platform
+import subprocess
+import os
 import typing
 import re
 
 # Related modules
 from box import Box
 
 from ..utils import status,log
```

### Comparing `networklab-1.5.2/netsim/outputs/ansible.py` & `networklab-1.5.2.dev1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/outputs/common.py` & `networklab-1.5.2.dev1/netsim/outputs/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 # Common inventory-related routines (used by Ansible and Devices)
 #
 
 import typing
 from box import Box
 from ..augment import devices
-from ..data import get_empty_box
 
 topo_to_host = { 'mgmt.ipv4': 'ansible_host', 'hostname': 'ansible_host', 'id': 'id' }
 topo_to_host_skip = [ 'name','device' ]
 
 def provider_inventory_settings(node: Box, defaults: Box) -> None:
   p_data = defaults.providers[defaults.provider]
   if not p_data:
@@ -36,15 +35,15 @@
 
 def adjust_inventory_host(
       node: Box,
       defaults: Box,
       translate: typing.Optional[dict] = None,
       ignore: typing.Optional[list] = None,
       group_vars: typing.Optional[bool] = False) -> Box:
-  host = get_empty_box()
+  host = Box({})
 
   translate = translate or topo_to_host
   ignore = ignore or topo_to_host_skip
 
   if group_vars:
     add_group_vars(host,node,defaults)
```

### Comparing `networklab-1.5.2/netsim/outputs/d2.py` & `networklab-1.5.2.dev1/netsim/outputs/d2.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import yaml
 import os
 from box import Box
 
 from .. import common
-from ..data import get_box
+from ..data import get_from_box,get_box
 from ..data.validate import must_be_list
 from . import _TopologyOutput
 
 '''
 Copy default settings into a D2 map converting Python dictionaries into
 dotted-name format D2 is using
 '''
@@ -46,42 +46,34 @@
 Create a node in D2 graph and add a label and styling attributes to it
 
 indent parameter is used to create indented definitions within containers
 '''
 def node_with_label(f : typing.TextIO, n: Box, settings: Box, indent: str = '') -> None:
   f.write(f'{indent}{n.d2.name} {{\n')
   node_ip_str = ""
-  node_ip = n.loopback.ipv4 or n.loopback.ipv6
-  if settings.node_address_label and not settings.node_interfaces:
+  if settings.node_address_label:
+    node_ip = n.loopback.ipv4 or n.loopback.ipv6
     if not node_ip and n.interfaces:
       node_ip = n.interfaces[0].ipv4 or n.interfaces[0].ipv6
     if node_ip:
       node_ip_str = f'\\n{node_ip}'
+
   f.write(f"  {indent}label: \"{n.name} [{n.device}]{node_ip_str}\"\n")
-  if settings.node_interfaces:
-    node_intf = f'    {indent}* Loopback: {node_ip}' if node_ip else ''
-    for i in n.interfaces:
-      node_intf += f'\n    {indent}* {i.ifname}: {i.ipv4 or i.ipv6 or "l2_only"}'
-    f.write(f'{indent}  interfaces: |md\n{node_intf}\n{indent}  |\n')
   d2_node_attr(f,n,settings,indent+'  ')
   f.write(f'{indent}}}\n')
 
 '''
 Similar to node-with-label, create a LAN segment node in the D2 graph. Node name is
 the LAN bridge name, node label is its IPv4 or IPv6 prefix.
 '''
 def network_with_label(f : typing.TextIO, n: Box, settings: Box, indent: str = '') -> None:
-  f.write(f'{indent}{n.bridge} {{\n')
-  if settings.node_interfaces:
-    if n.prefix.ipv4 or n.prefix.ipv6:
-      f.write(f'{indent}  interfaces: |md\n{indent}    {n.prefix.ipv4 or n.prefix.ipv6}\n{indent}  |\n')
-  else:
-    f.write(f'{indent}  label: {n.prefix.ipv4 or n.prefix.ipv6 or n.bridge}\n')
+  f.write(f'{indent}{n.bridge}' + '{\n')
+  f.write(f'  label: {n.prefix.ipv4 or n.prefix.ipv6 or n.bridge}\n')
   copy_d2_attr(f,'lan',settings,'  '+indent)
-  f.write(f'{indent}}}\n')
+  f.write('}\n')
 #  f.write('style=filled fillcolor="%s" fontsize=11' % (settings.colors.get("stub","#d1bfab")))
 
 '''
 Add an arrowhead label to a connection
 '''
 def edge_label(f : typing.TextIO, direction: str, data: Box, subnet: bool = True) -> None:
   addr = data.ipv4 or data.ipv6
@@ -132,15 +124,15 @@
 def build_maps(topology: Box) -> Box:
   maps = Box({},default_box=True,box_dots=True)
   for name,n in topology.nodes.items():
     maps.nodes[name] = n
 
   if 'bgp' in topology.get('module',[]):
     for name,n in topology.nodes.items():
-      bgp_as = n.get('bgp.as',None)
+      bgp_as = get_from_box(n,'bgp.as')
       if bgp_as:
         bgp_as = f'AS_{bgp_as}'
         maps.bgp[bgp_as].nodes[n.name] = n
 
   if 'bgp' in topology and 'as_list' in topology.bgp:
     for (asn,asdata) in topology.bgp.as_list.items():
       if 'name' in asdata and asn in maps.bgp:
@@ -190,15 +182,17 @@
 
   for l in topology.links:
     for intf in l.interfaces:
       intf.node = topology.nodes[intf.node].d2.name
     if l.type == "p2p":
       edge_p2p(f,l,settings.interface_labels)
     else:
-      l.bridge = l.name or f'{l.type}_{l.linkindex}'
+      if not l.bridge:
+        common.error('Found a lan/stub link without a bridge name, skipping',common.IncorrectValue,'graph')
+        next
       network_with_label(f,l,settings)
       for ifdata in l.interfaces:
         if ifdata.node in maps.nodes:
           edge_node_net(f,l,ifdata,settings.interface_labels)
 
   f.close()
   return True
```

### Comparing `networklab-1.5.2/netsim/outputs/devices.py` & `networklab-1.5.2.dev1/netsim/outputs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Create devices inventory in YAML format
+# Create Ansible inventory
 #
 import typing
 
 import yaml
 import os
 import sys
 from box import Box
```

### Comparing `networklab-1.5.2/netsim/outputs/format.py` & `networklab-1.5.2.dev1/netsim/outputs/format.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/outputs/graph.py` & `networklab-1.5.2.dev1/netsim/outputs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typing
 
 import yaml
 import os
 from box import Box
 
 from .. import common
+from ..data import get_from_box
 from ..data.validate import must_be_list
 from . import _TopologyOutput
 
 def node_with_label(f : typing.TextIO, n: Box, settings: Box, indent: typing.Optional[str] = '') -> None:
   f.write('%s  "%s" [\n' % (indent,n.name))
   node_ip_str = ""
   if settings.node_address_label:
@@ -79,15 +80,15 @@
 def build_maps(topology: Box) -> Box:
   maps = Box({},default_box=True,box_dots=True)
   for name,n in topology.nodes.items():
     maps.nodes[name] = n
 
   if 'bgp' in topology.get('module',[]):
     for name,n in topology.nodes.items():
-      bgp_as = n.get('bgp.as',None)
+      bgp_as = get_from_box(n,'bgp.as')
       if bgp_as:
         bgp_as = f'AS_{bgp_as}'
         maps.bgp[bgp_as].nodes[n.name] = n
 
   if 'bgp' in topology and 'as_list' in topology.bgp:
     for (asn,asdata) in topology.bgp.as_list.items():
       if 'name' in asdata and asn in maps.bgp:
```

### Comparing `networklab-1.5.2/netsim/outputs/provider.py` & `networklab-1.5.2.dev1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/outputs/yaml.py` & `networklab-1.5.2.dev1/netsim/outputs/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     output = common.open_output_file(outfile)
 
     for fmt in self.format:
       if fmt == 'nodefault':
         cleantopo.pop('defaults')
       elif fmt == 'noaddr':
         cleantopo.pop('addressing')
-      elif cleantopo.get(fmt,None):
-        result = cleantopo.get(fmt)
+      elif data.get_from_box(cleantopo,fmt):
+        result = data.get_from_box(cleantopo,fmt)
         if not isinstance(result,Box) and not isinstance(result,BoxList):
           common.fatal(f'Selecting {fmt} did not result in a usable dictionary, aborting')
           return
         cleantopo = result
         break
       else:
         common.error('Invalid format modifier %s' % fmt,common.IncorrectValue,modname)
```

### Comparing `networklab-1.5.2/netsim/providers/__init__.py` & `networklab-1.5.2.dev1/netsim/providers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import typing
 
 # Related modules
 from box import Box
 
 from .. import common
 from ..callback import Callback
-from ..augment import devices,links
-from ..data import get_box,filemaps
+from ..augment import devices
+from ..data import get_from_box,get_box
 
 class _Provider(Callback):
   def __init__(self, provider: str, data: Box) -> None:
     self.provider = provider
     if 'template' in data:
       self._default_template_name = data.template
 
@@ -85,54 +85,52 @@
   def create_extra_files_mappings(
       self,
       node: Box,
       topology: Box,
       inkey: str = 'config_templates',
       outkey: str = 'binds') -> None:
 
-    mappings = node.get(f'{self.provider}.{inkey}',None)
-    if not mappings:
-      return
-    
-    map_dict = filemaps.mapping_to_dict(mappings)
-    cur_binds = node.get(f'{self.provider}.{outkey}',[])
-    bind_dict = filemaps.mapping_to_dict(cur_binds)
-    for file,mapping in map_dict.items():
-      if file in bind_dict:
-        continue
-      if not self.find_extra_template(node,file):
-        common.error(
-          f"Cannot find template {file}.j2 for extra file {self.provider}.{inkey}.{file} on node {node.name}",
-          common.IncorrectValue,
-          self.provider)
-        continue
+    mappings = get_from_box(node,f'{self.provider}.{inkey}')
+    if mappings:
+      cur_binds = get_from_box(node,f'{self.provider}.{outkey}') or {}
+      for file,mapping in mappings.items():
+        if mapping in cur_binds.values():
+          continue
+        if not isinstance(mapping,str):
+          common.error(
+            f"Malformed extra file mapping for {self.provider}.{inkey}.{file} on node {node.name} -- should be string",
+            common.IncorrectType,
+            self.provider)
+          continue
 
-      out_folder = f"{self.provider}_files/{node.name}"
-      bind_dict[f"{out_folder}/{file}"] = mapping
+        if not self.find_extra_template(node,file):
+          common.error(
+            f"Cannot find template {file}.j2 for extra file {self.provider}.{inkey}.{file} on node {node.name}",
+            common.IncorrectValue,
+            self.provider)
+          continue
 
-    node[self.provider][outkey] = filemaps.dict_to_mapping(bind_dict)
+        out_folder = f"{self.provider}_files/{node.name}"
+        node[self.provider][outkey][f"{out_folder}/{file}"] = mapping
 
   def create_extra_files(
       self,
       node: Box,
       topology: Box,
       inkey: str = 'config_templates',
       outkey: str = 'binds') -> None:
 
-    binds = node.get(f'{self.provider}.{outkey}',None)
+    binds = get_from_box(node,f'{self.provider}.{outkey}')
     if not binds:
       return
 
     sys_folder = str(common.get_moddir())+"/"
     out_folder = f"{self.provider}_files/{node.name}"
 
-    bind_dict = filemaps.mapping_to_dict(binds)
-    for file,mapping in bind_dict.items():
-      if not out_folder in file:                  # Skip files that are not mapped into the temporary provider folder
-        continue
+    for file,mapping in binds.items():
       file_name = file.replace(out_folder+"/","")
       template_name = self.find_extra_template(node,file_name)
       if template_name:
         node_data = node + { 'hostvars': topology.nodes }
         common.write_template(
           in_folder=os.path.dirname(template_name),
           j2=os.path.basename(template_name),
@@ -140,14 +138,15 @@
           out_folder=out_folder, filename=file_name)
         print( f"Created {out_folder}/{file_name} from {template_name.replace(sys_folder,'')}, mapped to {node.name}:{mapping}" )
 
   def create(self, topology: Box, fname: typing.Optional[str]) -> None:
     self.transform(topology)
     fname = self.get_output_name(fname,topology)
     output = common.open_output_file(fname)
+#    print(topology.nodes.to_yaml())
     output.write(common.template(self.get_root_template(),topology.to_dict(),self.get_template_path(),self.provider))
     if fname != '-':
       common.close_output_file(output)
       print("Created provider configuration file: %s" % fname)
       self.post_configuration_create(topology)
     else:
       output.write("\n")
@@ -185,16 +184,15 @@
   """
   Generic provider pre-output transform: remove loopback links
   """
   def pre_output_transform(self, topology: Box) -> None:
     if not 'links' in topology:
       return
 
-    topology.links = [
-      link for link in topology.links if link.type not in links.VIRTUAL_INTERFACE_TYPES ]
+    topology.links = [ link for link in topology.links if link.type != 'loopback' ]
 
 """
 Get a pointer to provider module. Cached in topology._Providers
 """
 def get_provider_module(topology: Box, pname: str) -> _Provider:
   if not pname in topology._Providers:
     topology._Providers[pname] = _Provider.load(pname,topology.defaults.providers[pname])
```

### Comparing `networklab-1.5.2/netsim/providers/clab.yml` & `networklab-1.5.2.dev1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/providers/external.py` & `networklab-1.5.2.dev1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/providers/libvirt.py` & `networklab-1.5.2.dev1/netsim/providers/libvirt.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 import typing
 from box import Box
 import pathlib
 import tempfile
 import netaddr
 
 from .. import common
-from ..data import types
+from ..data import get_from_box,types
 from . import _Provider
 from ..augment.links import get_link_by_index
-from ..cli import is_dry_run,external_commands
 
 LIBVIRT_MANAGEMENT_NETWORK_NAME = "vagrant-libvirt"
 LIBVIRT_MANAGEMENT_BRIDGE_NAME  = "libvirt-mgmt"
 LIBVIRT_MANAGEMENT_NETWORK_FILE = "templates/provider/libvirt/vagrant-libvirt.xml"
 LIBVIRT_MANAGEMENT_SUBNET       = "192.168.121.0/24"
 
 """
@@ -100,36 +99,32 @@
     tfile.write(xml)
     tfile.close()
     return tfile.name
 
 def create_vagrant_network(topology: typing.Optional[Box] = None) -> None:
   mgmt_net = topology.addressing.mgmt._network if topology is not None else ''
   mgmt_net = mgmt_net or LIBVIRT_MANAGEMENT_NETWORK_NAME
+  try:
+    subprocess.run(['virsh','net-destroy',mgmt_net],capture_output=True,text=True,check=False)    # Remove management network
+    subprocess.run(['virsh','net-undefine',mgmt_net],capture_output=True,text=True,check=False)   # ... if it exists
+    common.print_verbose(f'creating libvirt management network {mgmt_net}')
+
+    if topology is None:
+      net_template = get_libvirt_mgmt_template()                    # When called without topology data use the default template
+    else:
+      net_template = create_network_template(topology)              # Otherwise create a temporary XML file
+    result2 = subprocess.run(['virsh','net-define',net_template],capture_output=True,check=True,text=True)
+    if not topology is None:                                        # Remove the temporary XML file if needed
+      os.remove(net_template)
 
-  external_commands.run_command(
-    ['virsh','net-destroy',mgmt_net],check_result=True,ignore_errors=True)    # Remove management network
-  external_commands.run_command(
-    ['virsh','net-undefine',mgmt_net],check_result=True,ignore_errors=True)   # ... if it exists
-  common.print_verbose(f'creating libvirt management network {mgmt_net}')
-
-  if topology is None:
-    net_template = get_libvirt_mgmt_template()                    # When called without topology data use the default template
-  else:
-    net_template = create_network_template(topology)              # Otherwise create a temporary XML file
-  external_commands.run_command(
-    ['virsh','net-define',net_template],check_result=True)
-  if not topology is None:                                        # Remove the temporary XML file if needed
-    os.remove(net_template)
-
+  except subprocess.CalledProcessError as e:
+    common.fatal(f'Exception in net handling for libvirt network {mgmt_net}: {e.returncode}\n{e.stderr}')
   return
 
 def get_linux_bridge_name(virsh_bridge: str) -> typing.Optional[str]:
-  if is_dry_run():
-    print(f"DRY RUN: Assuming Linux bridge name {virsh_bridge} for libvirt network {virsh_bridge}")
-    return virsh_bridge
   try:
     result = subprocess.run(['virsh','net-info',virsh_bridge],capture_output=True,check=True,text=True)
   except:
     common.error('Cannot run net-info for libvirt network %s' % virsh_bridge, module='libvirt')
     return None
 
   match = None
@@ -178,15 +173,15 @@
   """
   def pre_transform(self, topology: Box) -> None:
     _Provider.pre_transform(self,topology)
     if not 'links' in topology:
       return
 
     for l in topology.links:
-      if l.get('libvirt.provider',None):
+      if get_from_box(l,'libvirt.provider'):
         l.type = 'lan'
         if not 'bridge' in l:
           l.bridge = "%s_%d" % (topology.name[0:10],l.linkindex)
 
   def transform_node_images(self, topology: Box) -> None:
     self.node_image_version(topology)
 
@@ -269,14 +264,13 @@
 
       linux_bridge = get_linux_bridge_name(brname)
       if linux_bridge is None:
         continue
 
       l.bridge = linux_bridge
       common.print_verbose(f"... network {brname} maps into {linux_bridge}")
-      if not external_commands.run_command(
-          ['sudo','sh','-c',f'echo 0x4000 >/sys/class/net/{linux_bridge}/bridge/group_fwd_mask'],
-          check_result=True):
+      try:
+        subprocess.run(['sudo','sh','-c',f'echo 0x4000 >/sys/class/net/{linux_bridge}/bridge/group_fwd_mask'],check=True)
+      except:
         common.error(f"Cannot set forwarding mask on Linux bridge {linux_bridge}")
         continue
-
       common.print_verbose(f"... setting LLDP enabled flag on {linux_bridge}")
```

### Comparing `networklab-1.5.2/netsim/read_topology.py` & `networklab-1.5.2.dev1/netsim/read_topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
       read_cache[filename] = Box(yaml_data)
     except:
       common.fatal("Cannot read YAML from %s: %s " % (filename,str(sys.exc_info()[1])))
 
   if common.LOGGING or common.VERBOSE:
     print("Read YAML data from %s" % (filename or "string"))
 
+  data.unroll_dots(yaml_data)
   return yaml_data
 
 def include_defaults(topo: Box, fname: str) -> None:
   defaults = read_yaml(fname)
   if defaults:
     topo.input.append(fname)
     topo.defaults = defaults + topo.defaults
@@ -193,24 +194,27 @@
     topo.plugin.extend(args.plugin)
 
   if args.settings:
     for s in args.settings:
       if not "=" in s:
         common.error("Invalid CLI setting %s, should be in format key=value" % s)
       (k,v) = s.split("=")
-      try:
-        topo[k] = v
-      except TypeError as ex:
-        if 'nodes.' in k:
-          common.error(
-            f'Cannot set {k}:\n... nodes element must be a dictionary if you want to set values via CLI arguments',
-            common.IncorrectValue,
-            'cli')
-        elif 'links.' in k:
-          common.error(
-            f'Cannot set link value {k} through CLI arguments',
-            common.IncorrectValue,
-            'cli')
-        else:
+      if '.' in k:
+        try:
+          data.set_dots(topo,k.split('.'),v)
+        except TypeError as ex:
+          if 'nodes.' in k:
+            common.error(
+              f'Cannot set {k}:\n... nodes element must be a dictionary if you want to set values via CLI arguments',
+              common.IncorrectValue,
+              'cli')
+          elif 'links.' in k:
+            common.error(
+              f'Cannot set link value {k} through CLI arguments',
+              common.IncorrectValue,
+              'cli')
+          else:
+            common.fatal(f"Cannot set topology value {k}\n... {ex}")
+        except Exception as ex:
           common.fatal(f"Cannot set topology value {k}\n... {ex}")
-      except Exception as ex:
-        common.fatal(f"Cannot set topology value {k}\n... {ex}")
+      else:
+        topo[k] = v
```

### Comparing `networklab-1.5.2/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/clab.j2`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 {%    endif %}
 {% if 'srl-agents' in clab %}
       extras:
         srl-agents: {{ clab['srl-agents'] }}
 {% endif %}
 {% if 'binds' in clab %}
       binds:
-{% for bind_item in clab.binds %}
-      - {{ bind_item }}
+{% for f,m in clab.binds.items() %}
+      - {{ f }}:{{ m }}
 {% endfor %}
 {% endif %}
 {% if 'startup-config' in clab %}
       startup-config: {{ clab['startup-config'] }}
 {% endif %}
 {% if clab.license is defined %}
       license: {{ clab.license }}
```

### Comparing `networklab-1.5.2/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/external/external.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/tools/graphite.py` & `networklab-1.5.2.dev1/netsim/outputs/graphite.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 # docker run -d \
 #  -v "$(pwd)/graphite-default.json":/var/www/localhost/htdocs/default/default.json \
 #  -p 8080:80 \
 #  --name graphite \
 #  netreplica/graphite:webssh2
 #
 
+from array import array
 import typing
 
 import json
+import os
 from box import Box
 
 from .. import common
-from . import _ToolOutput
+from .. import data
+from . import _TopologyOutput
 
 DEFAULT_NODE_ICON = "router"
 HOST_BRIDGE_NODE_NAME = "({type}:{index})"
 
 short_ifname_lookup = {
     'GigabitEthernet': 'ge',
     'Ethernet': 'eth',
@@ -37,19 +40,18 @@
             return n.replace(long_name,short_ifname_lookup[long_name],1)
 
     return n
 
 def nodes_items(topology: Box) -> list:
     r = []
     for name,n in topology.nodes.items():
-        node_icon = (
-            n.get('graphite.icon',None) or
-            topology.get(f'defaults.devices.{n.device}.graphite.icon',None) or
+        node_icon = ( data.get_from_box(n,'graphite.icon') or 
+            data.get_from_box(topology,f'defaults.devices.{n.device}.graphite.icon') or 
             DEFAULT_NODE_ICON )
-        graph_level = n.get('graphite.level',1)
+        graph_level = data.get_from_box(n,'graphite.level') or 1
         node_group = "tier-1"
         node_as = n.get('bgp', {}).get('as')
         if node_as:
             node_group = "as{}".format(node_as)
         r.append(
             {
                 'name': name,
@@ -65,15 +67,15 @@
     # Special Case:
     # Create a fake node to identify a host bridge, in case there are 1 or more than 2 nodes attached to it.
     for l in topology.links:
         if (l.type == "lan" and l.node_count != 2) or l.type == "stub":
             # Create fake node
             # Inherit graph level and group from first node (l.interfaces[0].node)
             node_item = topology.nodes[l.interfaces[0].node]
-            graph_level = node_item.get('graphite.level',1)
+            graph_level = data.get_from_box(node_item,'graphite.level') or 1
             node_group = "tier-1"
             node_as = node_item.get('bgp', {}).get('as')
             if node_as:
                 node_group = "as{}".format(node_as)
             r.append(
                 {
                     'name': HOST_BRIDGE_NODE_NAME.format(type=l.type, index=l.linkindex),
@@ -129,15 +131,27 @@
                             "source_endpoint": "",
                             "target": bridge_intf.node,
                             "target_endpoint": get_lan_intf_name(topology, bridge_intf.node, l.bridge),
                         }
                     )
     return r
 
-class Graphite(_ToolOutput):
+class Graphite(_TopologyOutput):
+
+  def write(self, topology: Box) -> None:
+    outfile = self.settings.filename or 'graphite-default.json'
 
-  def write(self, topology: Box, fmt: str) -> str:
     graphite_json = {
         'nodes': nodes_items(topology),
         'links': links_items(topology),
     }
-    return json.dumps(graphite_json, indent=2,sort_keys=True)
+
+    output = common.open_output_file(outfile)
+
+    output.write(json.dumps(graphite_json, indent=2,sort_keys=True))
+    output.write("\n")
+
+    if outfile != '-':
+      common.close_output_file(output)
+      print("Created Graphite topology file in %s" % outfile)
+    else:
+      output.write("\n")
```

### Comparing `networklab-1.5.2/netsim/utils/log.py` & `networklab-1.5.2.dev1/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/utils/status.py` & `networklab-1.5.2.dev1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/netsim/utils/strings.py` & `networklab-1.5.2.dev1/netsim/utils/strings.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 def print_structured_dict(d: Box, prefix: str = '') -> None:
   print(format_structured_dict(d,prefix))
 
 #
 # eval_format: emulate f'strings' evaluated on a data structure
 #
 def eval_format(fmt: str, data: dict) -> str:
-  fmt = fmt.replace("'","\\'")                    # Escape single quotes to prevent eval crashes
-  return str(eval(f"f'{fmt}'",dict(data)))        # An awful hack to use f-string specified in a string variable
+  return str(eval(f"f'{fmt}'",dict(data)))                            # An awful hack to use f-string specified in a string variable
 
 """
 confirm: print the prompt and wait for a yes/no answer
 """
 def confirm(prompt: str) -> bool:
   prompt = f'{prompt} [y/n]'
```

### Comparing `networklab-1.5.2/netsim/utils/templates.py` & `networklab-1.5.2.dev1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/networklab.egg-info/PKG-INFO` & `networklab-1.5.2.dev1/networklab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.2
+Version: 1.5.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.2/networklab.egg-info/SOURCES.txt` & `networklab-1.5.2.dev1/networklab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,14 @@
 netsim/cli/status.py
 netsim/cli/test.py
 netsim/cli/up.py
 netsim/cli/usage.py
 netsim/cli/usage.txt
 netsim/cli/version.py
 netsim/data/__init__.py
-netsim/data/filemaps.py
 netsim/data/global_vars.py
 netsim/data/types.py
 netsim/data/validate.py
 netsim/defaults/addressing.yml
 netsim/defaults/attributes.yml
 netsim/defaults/automation.yml
 netsim/defaults/hints.yml
@@ -405,24 +404,21 @@
 netsim/extra/ebgp.utils/junos.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/ebgp.utils/routeros7.j2
 netsim/extra/ebgp.utils/srlinux.j2
 netsim/extra/ebgp.utils/topology.yml
 netsim/extra/ebgp.utils/vyos.j2
 netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
-netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
 netsim/extra/multilab/plugin.py
 netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
-netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
 netsim/extra/none/none.j2
 netsim/extra/proxy-arp/plugin.py
 netsim/extra/proxy-arp/srlinux.j2
 netsim/extra/proxy-arp/sros.j2
 netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
 netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
 netsim/install/libvirt/arubacx.txt
@@ -479,15 +475,14 @@
 netsim/outputs/format.py
 netsim/outputs/graph.py
 netsim/outputs/graph.yml
 netsim/outputs/graphite.py
 netsim/outputs/json.py
 netsim/outputs/none.py
 netsim/outputs/provider.py
-netsim/outputs/tools.py
 netsim/outputs/yaml.py
 netsim/providers/__init__.py
 netsim/providers/clab.py
 netsim/providers/clab.yml
 netsim/providers/external.py
 netsim/providers/external.yml
 netsim/providers/libvirt.py
@@ -529,19 +524,14 @@
 netsim/templates/provider/virtualbox/linux-domain.j2
 netsim/templates/provider/virtualbox/nxos-domain.j2
 netsim/templates/provider/virtualbox/virtualbox-network.j2
 netsim/templates/provider/virtualbox/virtualbox-ports.j2
 netsim/templates/tests/clab.yml
 netsim/templates/tests/libvirt.yml
 netsim/templates/tests/virtualbox.yml
-netsim/tools/__init__.py
-netsim/tools/graphite.py
-netsim/tools/graphite.yml
-netsim/tools/suzieq.yml
-netsim/tools/suzieq/suzieq-cfg.yml
 netsim/utils/__init__.py
 netsim/utils/log.py
 netsim/utils/status.py
 netsim/utils/strings.py
 netsim/utils/templates.py
 networklab.egg-info/PKG-INFO
 networklab.egg-info/SOURCES.txt
```

### Comparing `networklab-1.5.2/setup.py` & `networklab-1.5.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.2/tests/test_transformation.py` & `networklab-1.5.2.dev1/tests/test_transformation.py`

 * *Files identical despite different names*

