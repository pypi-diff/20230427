# Comparing `tmp/xoa-driver-1.2.0.tar.gz` & `tmp/xoa-driver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-driver-1.2.0.tar", last modified: Fri Mar  3 10:11:01 2023, max compression
+gzip compressed data, was "xoa-driver-1.3.0.tar", last modified: Thu Apr 27 09:40:36 2023, max compression
```

## Comparing `xoa-driver-1.2.0.tar` & `xoa-driver-1.3.0.tar`

### file list

```diff
@@ -1,356 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.929109 xoa-driver-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-03-03 10:11:01.929109 xoa-driver-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-03 10:11:01.929109 xoa-driver-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.893108 xoa-driver-1.2.0/xoa_driver/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.893108 xoa-driver-1.2.0/xoa_driver/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/anlt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/anlt_ll_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/mgmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/functions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/hlfuncs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.893108 xoa-driver-1.2.0/xoa_driver/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.893108 xoa-driver-1.2.0/xoa_driver/internals/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.897108 xoa-driver-1.2.0/xoa_driver/internals/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/c_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    43363 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/m4_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/m4e_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    61413 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/m_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    73098 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4e_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)   299854 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4g_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)   168258 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/p_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pd_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    40101 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pe_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pec_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/ped_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    91205 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pef_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pf_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pl1_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pm_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    76126 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pp_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pr_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    90606 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/ps_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/pt_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/px_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/commands/subtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.897108 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/command_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/add_on.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/protocol/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/commands_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/events_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/core/transporter/transportation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/exceptions/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/exceptions/testers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/base_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.901108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/l2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/l3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.905108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/genuine_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/length_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/match_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/port_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.905108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/base_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/genuine_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.905108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/__interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_l23ve.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_l47.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_l47ve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.905108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_combi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_f.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_h.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_i.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_j.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_n.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/module_l23_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.905108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/base_port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.909108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.909108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23_genuine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_reception_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transceiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transmission_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.909108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/working.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_custom_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/reception_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/transmission_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_combi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_e.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_f.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_h.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_i.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/fault_jkl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ghijkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ijkl_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/port_l23ve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/counters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/packet_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/_base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/_tester_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/management_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l23_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l23ve_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l47_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l47ve_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.913108 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/base_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/l2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/l3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/genuine_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/length_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/match_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/port_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/base_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/genuine_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/__interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_l23ve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_l47.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_l47ve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_combi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_f.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_h.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_i.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_j.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/module_l23_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.917109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/base_port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.921109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.921109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23_genuine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_reception_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transceiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transmission_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.921109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/working.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_custom_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/reception_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/transmission_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_combi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_e.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_f.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_h.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_i.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/fault_jkl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ghijkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ijkl_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/port_l23ve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/counters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/packet_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/_base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/_tester_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/management_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l23_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l23ve_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l47_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l47ve_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/state_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/state_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/state_storage/_speed_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/state_storage/modules_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/state_storage/ports_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/state_storage/testers_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.925109 xoa-driver-1.2.0/xoa_driver/internals/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/_base_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/cap_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.929109 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/header_modifier_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/index_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/indices/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/modules_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/ports_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/internals/utils/rev_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/lli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/testers.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.929109 xoa-driver-1.2.0/xoa_driver/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/v2/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/v2/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-03 10:10:46.000000 xoa-driver-1.2.0/xoa_driver/v2/testers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:11:01.893108 xoa-driver-1.2.0/xoa_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-03-03 10:11:01.000000 xoa-driver-1.2.0/xoa_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-03-03 10:11:01.000000 xoa-driver-1.2.0/xoa_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:11:01.000000 xoa-driver-1.2.0/xoa_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 10:11:01.000000 xoa-driver-1.2.0/xoa_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-03 10:11:01.000000 xoa-driver-1.2.0/xoa_driver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.030312 xoa-driver-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-27 09:40:36.030312 xoa-driver-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 09:40:36.030312 xoa-driver-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.946310 xoa-driver-1.3.0/xoa_driver/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.950310 xoa-driver-1.3.0/xoa_driver/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/anlt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/anlt_ll_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/functions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/hlfuncs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.950310 xoa-driver-1.3.0/xoa_driver/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.950310 xoa-driver-1.3.0/xoa_driver/internals/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.958310 xoa-driver-1.3.0/xoa_driver/internals/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65399 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/c_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44878 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/m4_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/m4e_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61833 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/m_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73098 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4e_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)   299854 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4g_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168261 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/p_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pd_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40101 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pe_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pec_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/ped_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90908 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pef_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pf_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pl1_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pm_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76126 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pp_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32823 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pr_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90606 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/ps_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/pt_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/px_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/commands/subtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.958310 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/command_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.958310 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/add_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/protocol/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.962311 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/commands_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/events_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/core/transporter/transportation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.962311 xoa-driver-1.3.0/xoa_driver/internals/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/exceptions/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/exceptions/testers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.962311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.966311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/base_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.966311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/l2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/l3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.966311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/base_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/genuine_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/length_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/match_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/port_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.970311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/base_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/genuine_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.970311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/__interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_l23ve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_l47.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_l47ve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.974311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_combi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_h.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_i.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/module_l23_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.974311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/base_port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.978311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.978311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23_genuine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_reception_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transceiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transmission_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.982311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.982311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_custom_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/reception_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/transmission_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_combi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_h.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/fault_jkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ghijkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ijkl_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/port_l23ve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.986311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/counters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/packet_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.990311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/_base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/_tester_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.990311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.994311 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l23_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l23ve_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l47_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l47ve_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.994311 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.994311 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/base_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.998312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/l2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/l3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.998312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/base_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/genuine_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/length_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/match_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/port_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.998312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/base_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/genuine_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.002312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/__interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_l23ve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_l47.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_l47ve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.006312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_combi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_h.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_i.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/module_l23_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.006312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/base_port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.010312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.014312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23_genuine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_reception_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transceiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transmission_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.014312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.018312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_custom_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/reception_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/transmission_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_combi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_h.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/fault_jkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ghijkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ijkl_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/port_l23ve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.018312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/counters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/packet_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.022312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/_base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/_tester_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.022312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.022312 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l23_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l23ve_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l47_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l47ve_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.026312 xoa-driver-1.3.0/xoa_driver/internals/state_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/state_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/state_storage/_speed_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/state_storage/modules_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/state_storage/ports_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/state_storage/testers_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.026312 xoa-driver-1.3.0/xoa_driver/internals/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/_base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/cap_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.026312 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/header_modifier_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/index_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/indices/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/modules_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/ports_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/utils/rev_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/internals/warn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/lli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/testers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:36.030312 xoa-driver-1.3.0/xoa_driver/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/v2/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/v2/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-27 09:40:14.000000 xoa-driver-1.3.0/xoa_driver/v2/testers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:40:35.950310 xoa-driver-1.3.0/xoa_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-27 09:40:35.000000 xoa-driver-1.3.0/xoa_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-04-27 09:40:35.000000 xoa-driver-1.3.0/xoa_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:40:35.000000 xoa-driver-1.3.0/xoa_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:40:35.000000 xoa-driver-1.3.0/xoa_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 09:40:35.000000 xoa-driver-1.3.0/xoa_driver.egg-info/top_level.txt
```

### Comparing `xoa-driver-1.2.0/LICENSE` & `xoa-driver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/PKG-INFO` & `xoa-driver-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-driver
-Version: 1.2.0
+Version: 1.3.0
 Summary: Xena OpenAutomation (XOA) Python API is a driver providing user-friendly communication interfaces to Xena's physical and virtual Traffic Generation and Analysis (TGA) testers. It provides a rich collection of programming interfaces that can be used to either write test scripts or develop applications.
 Home-page: https://github.com/xenanetworks/open-automation-python-api
 Author: Artem Constantinov, Ron Ding, Leonard Yu
 Author-email: aco@xenanetworks.com, rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
@@ -18,24 +18,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-driver) [![PyPI](https://img.shields.io/pypi/v/xoa-driver)](https://pypi.python.org/pypi/xoa-driver) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-python-api) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-python-api/badge/?version=stable)](https://xena-openautomation-python-api.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Python API
-Xena OpenAutomation (XOA) Python API is a driver providing user-friendly communication interfaces to Xena's physical and virtual Traffic Generation and Analysis (TGA) testers. It provides a rich collection of programming interfaces that can be used to either write test scripts or develop applications.
+Xena OpenAutomation Python API is a standalone Python library that provides a user-friendly and powerful interface for automating network testing tasks using Xena Networks test equipment. Xena test equipment is a high-performance network test device designed for testing and measuring the performance of network equipment and applications.
 
 ## Introduction
-Many of our customers choose to develop their own test scripts, where they automate performance verification, regression test, development verification, and so on.
+The XOA Python API is designed to be easy to use and integrate with other automation tools and frameworks. It provides a comprehensive set of methods and classes for interacting with Xena test equipment, including the ability to create and run complex test scenarios, generate and analyze traffic at line rate, and perform detailed analysis of network performance and behavior.
 
-At Xena Networks, we have always been providing customers with the best tool for test automation. To help our customers achieve a more efficient quality control and continuous development verification, we have developed a new platform Xena OpenAutomation, overlaying various Xena hardware and virtual testers, to offer not only automated test suites but also the power to build programs from simple scripts to advanced applications with endless possibilities.
+The XOA Python API simplifies the process of automating network testing tasks using Xena test equipment. It provides a simple, yet powerful, interface for interacting with Xena test equipment using the Python programming language. With the XOA Python API, network engineers and testing professionals can easily create and execute test scenarios, generate and analyze traffic, and perform detailed analysis of network performance and behavior, all while leveraging the power and flexibility of the Python programming language.
 
-The cornerstone component of Xena OpenAutomation is its Python API, which contains more than 600 commands, from basic streams creation to advance eye diagrams measurement. With this rich collection of programming interfaces, we empower our customers to either write test scripts or develop applications with almost limitless possibilities.
-
-Moving forward, all Xena’s automated test suites will be based on Xena OpenAutomation.
+Overall, the XOA Python API is a valuable tool for anyone looking to automate their network testing tasks using Xena test equipment. With its simple, yet powerful, interface and support for the Python programming language, the XOA Python API provides a flexible and extensible framework for automating network testing tasks and improving the quality of network infrastructure.
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Python API Documentation](https://docs.xenanetworks.com/projects/xoa-python-api)
 
 ## Key Features
 * Objected-oriented, high-level abstraction, to help users save time on parsing command responses.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xoa-driver-1.2.0/README.md` & `xoa-driver-1.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-driver) [![PyPI](https://img.shields.io/pypi/v/xoa-driver)](https://pypi.python.org/pypi/xoa-driver) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-python-api) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-python-api/badge/?version=stable)](https://xena-openautomation-python-api.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Python API
-Xena OpenAutomation (XOA) Python API is a driver providing user-friendly communication interfaces to Xena's physical and virtual Traffic Generation and Analysis (TGA) testers. It provides a rich collection of programming interfaces that can be used to either write test scripts or develop applications.
+Xena OpenAutomation Python API is a standalone Python library that provides a user-friendly and powerful interface for automating network testing tasks using Xena Networks test equipment. Xena test equipment is a high-performance network test device designed for testing and measuring the performance of network equipment and applications.
 
 ## Introduction
-Many of our customers choose to develop their own test scripts, where they automate performance verification, regression test, development verification, and so on.
+The XOA Python API is designed to be easy to use and integrate with other automation tools and frameworks. It provides a comprehensive set of methods and classes for interacting with Xena test equipment, including the ability to create and run complex test scenarios, generate and analyze traffic at line rate, and perform detailed analysis of network performance and behavior.
 
-At Xena Networks, we have always been providing customers with the best tool for test automation. To help our customers achieve a more efficient quality control and continuous development verification, we have developed a new platform Xena OpenAutomation, overlaying various Xena hardware and virtual testers, to offer not only automated test suites but also the power to build programs from simple scripts to advanced applications with endless possibilities.
+The XOA Python API simplifies the process of automating network testing tasks using Xena test equipment. It provides a simple, yet powerful, interface for interacting with Xena test equipment using the Python programming language. With the XOA Python API, network engineers and testing professionals can easily create and execute test scenarios, generate and analyze traffic, and perform detailed analysis of network performance and behavior, all while leveraging the power and flexibility of the Python programming language.
 
-The cornerstone component of Xena OpenAutomation is its Python API, which contains more than 600 commands, from basic streams creation to advance eye diagrams measurement. With this rich collection of programming interfaces, we empower our customers to either write test scripts or develop applications with almost limitless possibilities.
-
-Moving forward, all Xena’s automated test suites will be based on Xena OpenAutomation.
+Overall, the XOA Python API is a valuable tool for anyone looking to automate their network testing tasks using Xena test equipment. With its simple, yet powerful, interface and support for the Python programming language, the XOA Python API provides a flexible and extensible framework for automating network testing tasks and improving the quality of network infrastructure.
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Python API Documentation](https://docs.xenanetworks.com/projects/xoa-python-api)
 
 ## Key Features
 * Objected-oriented, high-level abstraction, to help users save time on parsing command responses.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xoa-driver-1.2.0/setup.py` & `xoa-driver-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,18 @@
         author="Artem Constantinov, Ron Ding, Leonard Yu",
         author_email="aco@xenanetworks.com, rdi@xenanetworks.com, hyu@xenanetworks.com",
         maintainer="Xena Networks",
         maintainer_email="support@xenanetworks.com",
         url="https://github.com/xenanetworks/open-automation-python-api",
         packages=setuptools.find_packages(),
         license='Apache 2.0',
-        install_requires=["typing_extensions", "loguru"],
+        install_requires=[
+        "typing_extensions", 
+        "loguru"
+        ],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "Topic :: Software Development :: Libraries :: Python Modules",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
```

### Comparing `xoa-driver-1.2.0/xoa_driver/enums.py` & `xoa-driver-1.3.0/xoa_driver/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .internals.core.commands.enums import *  # noqa: F403
 from .internals.core.protocol.constants import CommandStatus
 
 __all__ = (  # noqa: F405
     "AlgorithmMethod",
     "AlignLockStatus",
+    "AnLtLogControl",
     "ApplicationLayerBehavior",
     "AutoNegFECOption",
     "AutoNegFECStatus",
     "AutoNegFECType",
     "AutoNegMode",
     "AutoNegStatus",
     "AutoNegTecAbility",
```

### Comparing `xoa-driver-1.2.0/xoa_driver/functions/anlt.py` & `xoa-driver-1.3.0/xoa_driver/functions/anlt.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from xoa_driver.misc import Token
 from .tools import (
     get_ctx,
     dictionize_autoneg_status,
     dictionize_lt_status,
     dictionize_txtap_get,
     dictionize_anlt_status,
+    dictionize_lt_im_status,
+    dictionize_lt_algorithm_status
 )
 import asyncio
 
 PcsPmaSupported = (FamilyL, FamilyL1)
 AutoNegSupported = (FamilyL, FamilyL1)
 LinkTrainingSupported = FamilyL
 
@@ -75,18 +77,21 @@
         self, serdes: int, config_type: int, values: list[int]
     ) -> Token:
         return commands.PL1_CFG_TMP(*self._group, serdes, config_type).set(
             values=values
         )
 
     def __select_modes(self) -> tuple[enums.LinkTrainingMode, enums.TimeoutMode]:
-        if self.should_do_an:
+        if self.should_do_an == True and self.should_lt_interactive == False:
             lt_mode = enums.LinkTrainingMode.START_AFTER_AUTONEG
             timeout_mode = enums.TimeoutMode.DEFAULT
-        elif self.should_lt_interactive:
+        elif self.should_do_an == True and self.should_lt_interactive == True:
+            lt_mode = enums.LinkTrainingMode.INTERACTIVE
+            timeout_mode = enums.TimeoutMode.DISABLED
+        elif self.should_do_an == False and self.should_lt_interactive == True:
             lt_mode = enums.LinkTrainingMode.INTERACTIVE
             timeout_mode = enums.TimeoutMode.DISABLED
         else:
             lt_mode = enums.LinkTrainingMode.STANDALONE
             timeout_mode = enums.TimeoutMode.DEFAULT
         return lt_mode, timeout_mode
 
@@ -142,15 +147,18 @@
     should_do_lt: bool,
     an_allow_loopback: bool,
     lt_preset0: enums.NRZPreset,
     lt_initial_modulations: dict[str, enums.LinkTrainEncoding],
     should_lt_interactive: bool,
     lt_algorithm: dict[str, enums.LinkTrainAlgorithm],
 ) -> None:
-    """Start ANLT on a port
+    """
+    .. versionadded:: 1.1
+
+    Start ANLT on a port
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param should_do_an: should the port do autoneg?
     :type should_do_an: bool
     :param should_do_lt: should the port do link training?
     :type should_do_lt: bool
@@ -176,29 +184,33 @@
         should_lt_interactive,
         lt_algorithm,
     )
     await anlt.run()
 
 
 async def autoneg_status(port: GenericL23Port) -> dict[str, t.Any]:
-    """Get the auto-negotiation status
+    """
+    .. versionadded:: 1.1
+
+    Get the auto-negotiation status
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :return:
     :rtype: typing.Dict[str, typing.Any]
     """
     conn, mid, pid = get_ctx(port)
-    loopback, auto_neg_info = await apply(
+    loopback, auto_neg_info, status = await apply(
         commands.PL1_CFG_TMP(
             conn, mid, pid, 0, enums.Layer1ConfigType.AN_LOOPBACK
         ).get(),
         commands.PL1_AUTONEGINFO(conn, mid, pid, 0).get(),
+        commands.PP_AUTONEGSTATUS(conn, mid, pid).get(),
     )
-    return dictionize_autoneg_status(loopback, auto_neg_info)
+    return dictionize_autoneg_status(loopback, auto_neg_info, status)
 
 
 LinkTrainType = t.Union[
     enums.LinkTrainCoeffs,
     enums.LinkTrainPresets,
     enums.LinkTrainEncoding,
     enums.LinkTrainAnnounce,
@@ -223,15 +235,18 @@
         await asyncio.sleep(0.01)
     return enums.LinkTrainCmdResults.UNKNOWN
 
 
 async def lt_coeff_inc(
     port: GenericL23Port, serdes: int, emphasis: enums.LinkTrainCoeffs
 ) -> enums.LinkTrainCmdResults:
-    """Ask the remote port to increase coeff of the specified serdes.
+    """
+    .. versionadded:: 1.1
+    
+    Ask the remote port to increase coeff of the specified serdes.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :param emphasis: the emphasis to increase
     :type emphasis: enums.LinkTrainCoeffs
@@ -240,15 +255,18 @@
     """
     return await __lt_coeff(port, serdes, emphasis, cmd=enums.LinkTrainCmd.CMD_INC)
 
 
 async def lt_coeff_dec(
     port: GenericL23Port, serdes: int, emphasis: enums.LinkTrainCoeffs
 ) -> enums.LinkTrainCmdResults:
-    """Ask the remote port to decrease coeff of the specified serdes.
+    """
+    .. versionadded:: 1.1
+    
+    Ask the remote port to decrease coeff of the specified serdes.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :param emphasis: the emphasis to decrease
     :type emphasis: enums.LinkTrainCoeffs
@@ -257,15 +275,18 @@
     """
     return await __lt_coeff(port, serdes, emphasis, cmd=enums.LinkTrainCmd.CMD_DEC)
 
 
 async def lt_preset(
     port: GenericL23Port, serdes: int, preset: enums.LinkTrainPresets
 ) -> enums.LinkTrainCmdResults:
-    """Ask the remote port to use the preset of the specified serdes.
+    """
+    .. versionadded:: 1.1
+    
+    Ask the remote port to use the preset of the specified serdes.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :param preset: preset index to select for the serdes, 0,1,2,3,4,
     :type preset: enums.LinkTrainPresets
@@ -274,30 +295,36 @@
     """
     return await __lt_coeff(port, serdes, preset, cmd=enums.LinkTrainCmd.CMD_PRESET)
 
 
 async def lt_encoding(
     port: GenericL23Port, serdes: int, encoding: enums.LinkTrainEncoding
 ) -> enums.LinkTrainCmdResults:
-    """Ask the remote port to use the encoding of the specified serdes.
+    """
+    .. versionadded:: 1.1
+    
+    Ask the remote port to use the encoding of the specified serdes.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :param encoding: link training encoding
     :type encoding: enums.LinkTrainCoeffs
     :return:
     :rtype: None
     """
     return await __lt_coeff(port, serdes, encoding, cmd=enums.LinkTrainCmd.CMD_ENCODING)
 
 
 async def lt_trained(port: GenericL23Port, serdes: int) -> enums.LinkTrainCmdResults:
-    """Tell the remote port that the current serdes is trained.
+    """
+    .. versionadded:: 1.1
+    
+    Tell the remote port that the current serdes is trained.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :return:
     :rtype: None
@@ -307,15 +334,18 @@
         serdes,
         arg=enums.LinkTrainAnnounce.TRAINED,
         cmd=enums.LinkTrainCmd.CMD_LOCAL_TRAINED,
     )
 
 
 async def lt_status(port: GenericL23Port, serdes: int) -> dict[str, t.Any]:
-    """Show the link training status.
+    """
+    .. versionadded:: 1.1
+    
+    Show the link training status.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :return: LT status of the serdes
     :rtype: typing.Dict[str, typing.Any]
@@ -338,15 +368,18 @@
     )
     return dictionize_lt_status(
         status, info, ltconf, cfg, ber, total_bit_count, total_error_bit_count
     )
 
 
 async def txtap_get(port: GenericL23Port, serdes: int) -> dict[str, int]:
-    """Get the tap value of the local TX tap.
+    """
+    .. versionadded:: 1.1
+    
+    Get the tap value of the local TX tap.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :return: tap values of the serdes
     :rtype: typing.Dict[str, int]
@@ -361,15 +394,18 @@
     serdes: int,
     pre3: int,
     pre2: int,
     pre: int,
     main: int,
     post1: int,
 ) -> None:
-    """Set the tap value of the local TX tap.
+    """
+    .. versionadded:: 1.1
+    
+    Set the tap value of the local TX tap.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param serdes: the serdes index, starting from 0
     :type serdes: int
     :param pre3: pre3 value
     :type pre3: int
@@ -393,15 +429,18 @@
         pre2=pre2,
         post2=pre3,
         post3=0,
     )
 
 
 async def anlt_link_recovery(port: GenericL23Port, enable: bool) -> None:
-    """Should xenaserver automatically do link recovery when detecting down signal.
+    """
+    .. versionadded:: 1.1
+    
+    Should xenaserver automatically do link recovery when detecting down signal.
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :param enable: should the port automatically do link recovery when link is down.
     :type enable: bool
     :return:
     :rtype:  None
@@ -410,15 +449,18 @@
     cmd_ = commands.PL1_CFG_TMP(
         conn, mid, pid, 0, enums.Layer1ConfigType.ANLT_INTERACTIVE
     )
     await cmd_.set(values=[int(enable)])
 
 
 async def anlt_status(port: GenericL23Port) -> dict[str, t.Any]:
-    """Get the overview of ANLT status
+    """
+    .. versionadded:: 1.1
+    
+    Get the overview of ANLT status
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :return: AN/LT status of the port
     :rtype: typing.Dict[str, typing.Any]
     """
 
@@ -431,51 +473,182 @@
         ).get(),
         commands.PP_AUTONEGSTATUS(conn, mid, pid).get(),
         commands.PP_LINKTRAIN(conn, mid, pid).get(),
         commands.P_CAPABILITIES(conn, mid, pid).get(),
         commands.PL1_CFG_TMP(conn, mid, pid, 0, enums.Layer1ConfigType.AN_LOOPBACK).get(),
     )
     link_recovery, autoneg, linktrain, capabilities, allow_loopback= r
-    initial_mods = {}
-    algorithms = {}
-    for i in range(0, capabilities.serdes_count):
-        # resp = await apply(
-        #     commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.LT_INITIAL_MODULATION).get(),
-        #     commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.LT_TRAINING_ALGORITHM).get()
-        # )
-        # im, alg = resp
-        # im = resp
-        im = await commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.LT_INITIAL_MODULATION).get()
-        initial_mods[str(i)] = enums.LinkTrainEncoding(im.values[0]).name
-        # algorithms[str(i)] = enums.LinkTrainAlgorithm(alg.values[0]).name
 
-    return dictionize_anlt_status(link_recovery, autoneg, linktrain, capabilities, allow_loopback, initial_mods)
+    return dictionize_anlt_status(link_recovery, autoneg, linktrain, capabilities, allow_loopback)
 
 
 async def anlt_log(port: GenericL23Port) -> str:
-    """Get the anlt log messages
+    """
+    .. versionadded:: 1.1
+    
+    Get the anlt log messages
 
     :param port: the port object
     :type port: :class:`~xoa_driver.ports.GenericL23Port`
     :return: AN/LT protocol log traces of the port
     :rtype: str
     """
     conn, mid, pid = get_ctx(port)
     log = await commands.PL1_LOG(conn, mid, pid).get()
     return log.log_string
 
 
+async def anlt_stop(port: GenericL23Port) -> None:
+    """
+    .. versionadded:: 1.3
+
+    Stop AN & LT
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    """
+    
+    anlt = DoAnlt(
+        port=port,
+        should_do_an=False,
+        should_do_lt=False,
+        an_allow_loopback=False,
+        lt_preset0=enums.NRZPreset.NRZ_NO_PRESET,
+        lt_initial_modulations={},
+        should_lt_interactive=False,
+        lt_algorithm={}
+    )
+    await anlt.run()
+
+
+async def txtap_autotune(
+    port: GenericL23Port,
+    serdes: int,
+) -> None:
+    """
+    .. versionadded:: 1.3
+    
+    Auto tune the tap value of the local TX tap.
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    :param serdes: the serdes index, starting from 0
+    :type serdes: int
+    :return:
+    :rtype: None
+    """
+    conn, mid, pid = get_ctx(port)
+    phy_autotune = commands.PP_PHYAUTOTUNE(conn, mid, pid, serdes)
+    await phy_autotune.set(on_off=enums.OnOff.OFF)
+    await phy_autotune.set(on_off=enums.OnOff.ON)
+
+
+async def lt_im_status(port: GenericL23Port) -> dict[str, t.Any]:
+    """
+    .. versionadded:: 1.3
+    
+    Get LT initial modulation config
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    :return: LT initial modulation configuration of the port
+    :rtype: typing.Dict[str, typing.Any]
+    """
+
+    # if not isinstance(port, LinkTrainingSupported):
+    #     raise NotSupportLinkTrainError(port)
+    conn, mid, pid = get_ctx(port)
+    capabilities = await commands.P_CAPABILITIES(conn, mid, pid).get()
+    initial_mods = {}
+    for i in range(0, capabilities.serdes_count):
+        im = await commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.LT_INITIAL_MODULATION).get()
+        initial_mods[str(i)] = enums.LinkTrainEncoding(im.values[0]).name
+
+    return dictionize_lt_im_status(capabilities, initial_mods)
+
+
+async def lt_algorithm_status(port: GenericL23Port) -> dict[str, t.Any]:
+    """
+    .. versionadded:: 1.3
+    
+    Get LT initial modulation config
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    :return: LT initial modulation configuration of the port
+    :rtype: typing.Dict[str, typing.Any]
+    """
+
+    # if not isinstance(port, LinkTrainingSupported):
+    #     raise NotSupportLinkTrainError(port)
+    conn, mid, pid = get_ctx(port)
+    capabilities = await commands.P_CAPABILITIES(conn, mid, pid).get()
+    algorithms = {}
+    for i in range(0, capabilities.serdes_count):
+        alg = await commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.LT_TRAINING_ALGORITHM).get()
+        algorithms[str(i)] = enums.LinkTrainAlgorithm(alg.values[0]).name
+
+    return dictionize_lt_algorithm_status(capabilities, algorithms)
+
+
+async def anlt_strict(port: GenericL23Port, enable: bool) -> None:
+    """
+    .. versionadded:: 1.3
+    
+    Should ANLT strict mode be enabled
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    :param enable: should ANLT strict mode be enabled
+    :type enable: bool
+    :return:
+    :rtype:  None
+    """
+    conn, mid, pid = get_ctx(port)
+    capabilities = await commands.P_CAPABILITIES(conn, mid, pid).get()
+    for i in range(0, capabilities.serdes_count):
+        await commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.ANLT_STRICT_MODE).set(values=[int(enable)])
+
+
+async def anlt_log_control(port: GenericL23Port, types: t.List[enums.AnLtLogControl]) -> None:
+    """
+    .. versionadded:: 1.3
+    
+    Control what should be logged for ANLT by xenaserver
+
+    :param port: the port object
+    :type port: :class:`~xoa_driver.ports.GenericL23Port`
+    :param types: control what should be logged for ANLT by xenaserver
+    :type types: t.List[enums.AnLtLogControl]
+    :return:
+    :rtype:  None
+    """
+    conn, mid, pid = get_ctx(port)
+    capabilities = await commands.P_CAPABILITIES(conn, mid, pid).get()
+    type = 0
+    for _type in types:
+        type |= _type.value
+    for i in range(0, capabilities.serdes_count):
+        await commands.PL1_CFG_TMP(conn, mid, pid, i, enums.Layer1ConfigType.ANLT_LOG_CONTROL).set(values=[int(type)])
+
+
 __all__ = (
+    "anlt_link_recovery",
     "anlt_log",
     "anlt_start",
+    "anlt_status",
+    "anlt_stop",
+    "autoneg_status",
     "lt_coeff_inc",
     "lt_coeff_dec",
     "lt_encoding",
     "lt_preset",
     "lt_status",
     "lt_trained",
-    "autoneg_status",
-    "anlt_link_recovery",
-    "anlt_status",
     "txtap_get",
     "txtap_set",
+    "txtap_autotune",
+    "lt_im_status",
+    "lt_algorithm_status",
+    "anlt_strict",
+    "anlt_log_control",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/functions/anlt_ll_debug.py` & `xoa-driver-1.3.0/xoa_driver/functions/anlt_ll_debug.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 from dataclasses import dataclass
 from enum import IntEnum
 from .tools import get_ctx
 
 
 class AnLtD(IntEnum):
     PMD_CONFIG_REGISTER = 0x02
+    AN_TX_CONFIG_REGISTER = 0x10
+    AN_RX_CONFIG_REGISTER = 0x18
+    AN_RX_STATUS_REGISTER = 0x19
+    AN_TX_PAGE_0_REGISTER = 0x14
+    AN_TX_PAGE_1_REGISTER = 0x15
+    AN_RX_PAGE_0_REGISTER = 0x1C
+    AN_RX_PAGE_1_REGISTER = 0x1D
+
     LT_TX_CONFIG_REGISTER = 0x20
     LT_TX_FRAME_REGISTER = 0x24
     LT_RX_STATUS_REGISTER = 0x29
     LT_RX_CONFIG_REGISTER = 0x28
     LT_RX_FRAME_REGISTER = 0x2C
     LT_RX_ERROR_STAT_0 = 0x2A
     LT_RX_ERROR_STAT_1 = 0x2B
-    LT_RX_ANALYZER_CONFIG = 0x38
-    LT_RX_ANALYZER_TRIG_MASK = 0x39
-    LT_RX_ANALYZER_STATUS = 0x3A
-    LT_RX_ANALYZER_RD_ADDR = 0x3B
-    LT_RX_ANALYZER_RD_PAGE = 0x3C
-    LT_RX_ANALYZER_RD_DATA = 0x3D
+    XLA_CONFIG = 0x38
+    XLA_TRIG_MASK = 0x39
+    XLA_STATUS = 0x3A
+    XLA_RD_ADDR = 0x3B
+    XLA_RD_PAGE = 0x3C
+    XLA_RD_DATA = 0x3D
 
 
 @dataclass
 class AnLtLowLevelInfo:
     base: int
     rx_gtm_base: int
     rx_serdes: int
@@ -95,14 +103,30 @@
     await r.set(f"0x{value:08X}")
     return None
 
 
 mode_get = partial(__get, reg=AnLtD.PMD_CONFIG_REGISTER)
 mode_set = partial(__set, reg=AnLtD.PMD_CONFIG_REGISTER)
 
+an_status = partial(__get, reg=AnLtD.AN_RX_STATUS_REGISTER)
+
+an_tx_config_get = partial(__get, reg=AnLtD.AN_TX_CONFIG_REGISTER)
+an_tx_config_set = partial(__set, reg=AnLtD.AN_TX_CONFIG_REGISTER)
+
+an_rx_config_get = partial(__get, reg=AnLtD.AN_RX_CONFIG_REGISTER)
+an_rx_config_set = partial(__set, reg=AnLtD.AN_RX_CONFIG_REGISTER)
+
+an_rx_page0_get = partial(__get, reg=AnLtD.AN_RX_PAGE_0_REGISTER)
+an_rx_page1_get = partial(__get, reg=AnLtD.AN_RX_PAGE_1_REGISTER)
+
+an_tx_page0_get = partial(__get, reg=AnLtD.AN_TX_PAGE_0_REGISTER)
+an_tx_page0_set = partial(__set, reg=AnLtD.AN_TX_PAGE_0_REGISTER)
+an_tx_page1_get = partial(__get, reg=AnLtD.AN_TX_PAGE_1_REGISTER)
+an_tx_page1_set = partial(__set, reg=AnLtD.AN_TX_PAGE_1_REGISTER)
+
 lt_tx_config_get = partial(__get, reg=AnLtD.LT_TX_CONFIG_REGISTER)
 lt_tx_config_set = partial(__set, reg=AnLtD.LT_TX_CONFIG_REGISTER)
 
 lt_rx_config_get = partial(__get, reg=AnLtD.LT_RX_CONFIG_REGISTER)
 lt_rx_config_set = partial(__set, reg=AnLtD.LT_RX_CONFIG_REGISTER)
 
 lt_tx_tf_get = partial(__get, reg=AnLtD.LT_TX_FRAME_REGISTER)
@@ -111,29 +135,30 @@
 lt_rx_tf_get = partial(__get, reg=AnLtD.LT_RX_FRAME_REGISTER)
 
 lt_status = partial(__get, reg=AnLtD.LT_RX_STATUS_REGISTER)
 
 lt_rx_error_stat0_get = partial(__get, reg=AnLtD.LT_RX_ERROR_STAT_0)
 lt_rx_error_stat1_get = partial(__get, reg=AnLtD.LT_RX_ERROR_STAT_1)
 
-lt_rx_analyzer_config_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_CONFIG)
-lt_rx_analyzer_config_set = partial(__set, reg=AnLtD.LT_RX_ANALYZER_CONFIG)
+xla_config_get = partial(__get, reg=AnLtD.XLA_CONFIG)
+xla_config_set = partial(__set, reg=AnLtD.XLA_CONFIG)
 
-lt_rx_analyzer_trig_mask_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_TRIG_MASK)
-lt_rx_analyzer_trig_mask_set = partial(__set, reg=AnLtD.LT_RX_ANALYZER_TRIG_MASK)
+xla_trig_mask_get = partial(__get, reg=AnLtD.XLA_TRIG_MASK)
+xla_trig_mask_set = partial(__set, reg=AnLtD.XLA_TRIG_MASK)
 
-lt_rx_analyzer_status_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_STATUS)
+xla_status_get = partial(__get, reg=AnLtD.XLA_STATUS)
 
-lt_rx_analyzer_rd_addr_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_RD_ADDR)
-lt_rx_analyzer_rd_addr_set = partial(__set, reg=AnLtD.LT_RX_ANALYZER_RD_ADDR)
+xla_rd_addr_get = partial(__get, reg=AnLtD.XLA_RD_ADDR)
+xla_rd_addr_set = partial(__set, reg=AnLtD.XLA_RD_ADDR)
 
-lt_rx_analyzer_rd_page_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_RD_PAGE)
-lt_rx_analyzer_rd_page_set = partial(__set, reg=AnLtD.LT_RX_ANALYZER_RD_PAGE)
+xla_rd_page_get = partial(__get, reg=AnLtD.XLA_RD_PAGE)
+xla_rd_page_set = partial(__set, reg=AnLtD.XLA_RD_PAGE)
+
+xla_rd_data_get = partial(__get, reg=AnLtD.XLA_RD_DATA)
 
-lt_rx_analyzer_rd_data_get = partial(__get, reg=AnLtD.LT_RX_ANALYZER_RD_DATA)
 
 
 async def lt_prbs(
     port: GenericL23Port,
     serdes: int,
     inf: t.Optional[AnLtLowLevelInfo] = None,
 ) -> dict[str, float]:
@@ -165,68 +190,91 @@
     v = await lt_rx_error_stat1_get(port, serdes, inf=inf)
     error_bits |= v << 32
     error_bits &= 0x0000FFFFFFFFFFFF
     ber = (error_bits) / (total_bits) if total_bits > 0 else float("nan")
     return {"total_bits": total_bits, "error_bits": error_bits, "ber": float(ber)}
 
 
-async def lt_rx_analyzer_dump(
+async def xla_dump(
     port: GenericL23Port,
     serdes: int,
     inf: t.Optional[AnLtLowLevelInfo] = None
-) -> str:
+) -> t.Dict[str, str]:
     """This will dump the 320bit words in the capture buffer"""
     if inf is None:
         inf = await init(port, serdes)
-    string = []
+    result = {}
     trigger_pos, capture_done = await asyncio.gather(
-        lt_rx_analyzer_config_get(port, serdes, inf=inf),
-        lt_rx_analyzer_status_get(port, serdes, inf=inf),
+        xla_config_get(port, serdes, inf=inf),
+        xla_status_get(port, serdes, inf=inf),
     )
-    string.append(f"Trigger position: {trigger_pos}\n")
-    string.append(f"Analyzer status : {capture_done}\n")
+    result["Trigger Position"] = str(trigger_pos)
+    result["Analyzer Status"] = str(capture_done)
     if not capture_done:
-        string.append("No capture\n")
-        result = "".join(string)
+        result["Data"] = ""
         return result
-    string.append("Capture\n")
+    data_list = []
     for r in range(256):
         # Set the read address
-        await lt_rx_analyzer_rd_addr_set(port, serdes, inf=inf, value=r)
+        await xla_rd_addr_set(port, serdes, inf=inf, value=r)
         for p in range(10):
             # Read the data
-            await lt_rx_analyzer_rd_page_set(port, serdes, inf=inf, value=p)
-            d = await lt_rx_analyzer_rd_data_get(port, serdes, inf=inf)
-            string.append(f"{d:08X}")
-        string.append("\n")
-    result = "".join(string)
+            await xla_rd_page_set(port, serdes, inf=inf, value=9-p)
+            d = await xla_rd_data_get(port, serdes, inf=inf)
+            data_list.append(f"{d:08X}")
+        data_list.append("\n")
+    result["Data"] = "".join(data_list)
     return result
 
 
+async def px_get(
+    port: GenericL23Port,
+    page_address: int,
+    register_address: int
+) -> t.Tuple[bool, str]:
+    resp = await port.transceiver.access_rw(page_address, register_address).get()
+
+    if resp.value.lower().find("dead") != -1:
+        return (False, resp.value)
+    else:
+        return (True, resp.value)
+    
+async def px_set(
+    port: GenericL23Port,
+    page_address: int,
+    register_address: int,
+    value: int
+) -> None:
+    value_hexstr = hex(value)
+    await port.transceiver.access_rw(page_address, register_address).set(value_hexstr)
+
+
 __all__ = (
     "init",
     "serdes_reset",
     "mode_get",
     "mode_set",
     "lt_prbs",
-    "lt_rx_analyzer_config_get",
-    "lt_rx_analyzer_config_set",
-    "lt_rx_analyzer_dump",
-    "lt_rx_analyzer_rd_addr_get",
-    "lt_rx_analyzer_rd_addr_set",
-    "lt_rx_analyzer_rd_data_get",
-    "lt_rx_analyzer_rd_page_get",
-    "lt_rx_analyzer_rd_page_set",
+    "xla_config_get",
+    "xla_config_set",
+    "xla_dump",
+    "xla_rd_addr_get",
+    "xla_rd_addr_set",
+    "xla_rd_data_get",
+    "xla_rd_page_get",
+    "xla_rd_page_set",
     "lt_tx_config_get",
     "lt_tx_config_set",
-    "lt_rx_analyzer_status_get",
-    "lt_rx_analyzer_trig_mask_get",
-    "lt_rx_analyzer_trig_mask_set",
+    "xla_status_get",
+    "xla_trig_mask_get",
+    "xla_trig_mask_set",
     "lt_rx_config_get",
     "lt_rx_config_set",
     "lt_rx_error_stat0_get",
     "lt_tx_tf_get",
     "lt_rx_error_stat1_get",
     "lt_rx_tf_get",
     "lt_status",
     "lt_tx_tf_set",
+    "px_get",
+    "px_set",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/functions/exceptions.py` & `xoa-driver-1.3.0/xoa_driver/functions/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from xoa_driver.ports import GenericAnyPort
-
+from xoa_driver.modules import GenericAnyModule
 
 class ConfigError(Exception):
     msg: str
 
 
 class NotConnectedError(ConfigError):
     def __init__(self) -> None:
@@ -54,19 +54,32 @@
 
 class NotRightLaneValueError(ConfigError):
     def __init__(self, serdes: list[int]) -> None:
         self.msg = f"Serdes {serdes} should be a list of 4 integers ranges from 0 to 255!"
         super().__init__(self.msg)
 
 
+class NotSupportMedia(ConfigError):
+    def __init__(self, module: GenericAnyModule) -> None:
+        module_id = module.module_id
+        self.msg = f"This module {module_id} does not support the media configuration!"
+
+    
+class NotSupportPortSpeed(ConfigError):
+    def __init__(self, module: GenericAnyModule) -> None:
+        module_id = module.module_id
+        self.msg = f"This module {module_id} does not support the port-speed configuration under its current media configuration!"
+
 
 __all__ = (
     "ConfigError",
     "NoSuchModuleError",
     "NoSuchPortError",
     "NotConnectedError",
     "NotRightLaneLengthError",
     "NotRightLaneValueError",
     "NotSupportAutoNegError",
     "NotSupportLinkTrainError",
     "NotSupportPcsPmaError",
+    "NotSupportMedia",
+    "NotSupportPortSpeed",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/functions/tools.py` & `xoa-driver-1.3.0/xoa_driver/functions/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 def get_ctx(port: GenericAnyPort) -> tuple["itf.IConnection", int, int]:
     return port._conn, port.kind.module_id, port.kind.port_id
 
 
 def dictionize_autoneg_status(
     loopback: commands.PL1_CFG_TMP.GetDataAttr,
     auto_neg_info: commands.PL1_AUTONEGINFO.GetDataAttr,
+    status: commands.PP_AUTONEGSTATUS.GetDataAttr,
 ) -> dict:
+    is_enabled = True if status.mode == enums.AutoNegMode.ANEG_ON else False
     return {
+        
+        "is_enabled": is_enabled,
         "loopback": "allowed" if loopback.values[0] else "not allowed",
         "duration": auto_neg_info.duration_us,
         "successes": auto_neg_info.negotiation_success_count,
         "timeouts": auto_neg_info.negotiation_timeout_count,
         "loss_of_sync": auto_neg_info.negotiation_loss_of_sync_count,
         "fec_negotiation_fails": auto_neg_info.negotiation_fec_fail_count,
         "hcd_negotiation_fails": auto_neg_info.negotiation_hcd_fail_count,
@@ -128,21 +132,68 @@
 
 def dictionize_anlt_status(
     link_recovery: commands.PL1_CFG_TMP.GetDataAttr,
     autoneg: commands.PP_AUTONEGSTATUS.GetDataAttr,
     linktrain: commands.PP_LINKTRAIN.GetDataAttr,
     capabilities: commands.P_CAPABILITIES.GetDataAttr,
     allow_loopback: commands.PL1_CFG_TMP.GetDataAttr,
-    initial_mods: dict[str, str],
-    # algorithms: dict[str, str]
 ) -> dict:
     return {
         "autoneg_enabled": enums.AutoNegMode(autoneg.mode).name.lower().lstrip("aneg_"),
         "link_training_mode": enums.LinkTrainingMode(linktrain.mode).name.lower(),
         "link_training_timeout": enums.TimeoutMode(linktrain.timeout_mode).name.lower(),
         "link_recovery": "on" if link_recovery.values[0] == 1 else "off",
         "serdes_count": capabilities.serdes_count,
         "autoneg_allow_loopback": allow_loopback.values,
         "link_training_preset0": enums.NRZPreset(linktrain.nrz_preset).name.lower(),
+    }
+
+def dictionize_lt_im_status(
+    capabilities: commands.P_CAPABILITIES.GetDataAttr,
+    initial_mods: dict[str, str]
+) -> dict:
+    return {
+        "serdes_count": capabilities.serdes_count,
         "initial_mods": initial_mods,
-        # "algorithms": algorithms
     }
+
+def dictionize_lt_algorithm_status(
+    capabilities: commands.P_CAPABILITIES.GetDataAttr,
+    algorithms: dict[str, str]
+) -> dict:
+    return {
+        "serdes_count": capabilities.serdes_count,
+        "algorithms": algorithms
+    }
+
+def module_eol_info() -> dict[str, str]:
+    m_eol = {
+        "01": "2014-04-01",
+        "02": "2024-09-01",
+        "03": "2016-03-01",
+        "09": "2022-01-01",
+        "17": "2023-01-01",
+        "18": "2023-01-01",
+        "20": "2024-11-01",
+        "22": "2018-11-01",
+        "24": "2024-11-01",
+        "26": "2023-06-01",
+        "27": "2025-10-01",
+        "30": "2024-01-01",
+        "31": "2021-09-01",
+        "32": "2024-04-01",
+        "34": "2024-08-01",
+        "36": "2024-04-01",
+        "40": "2023-03-01",
+        "50": "2022-02-01",
+        "51": "2023-08-01",
+        "54": "2023-01-01",
+        "55": "2024-01-01",
+        "60": "2025-10-01",
+        "66": "2025-01-31",
+        "90": "2025-10-01",
+        "91": "2025-10-01",
+        "93": "2025-10-01",
+        "94": "2025-10-01",
+        "97": "2025-10-01",
+        }
+    return m_eol
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/__init__.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/c_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/c_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
 class C_PORTCOUNTS:
     """
     Gets the number of ports in each module slot of the chassis, and indirectly
     the number of slots and modules.
 
     .. note::
 
-        CFP modules return the number 8 which is the maximum number of 10G ports, but the actual number of ports can be configured dynamically using the M_CFPCONFIG` command.
+        CFP modules return the number 8 which is the maximum number of 10G ports, but the actual number of ports can be configured dynamically using the M_CFPCONFIGEXT` command.
 
     """
 
     code: typing.ClassVar[int] = 13
     pushed: typing.ClassVar[bool] = False
 
     _connection: "interfaces.IConnection"
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/enums.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -2080,14 +2080,24 @@
 
     LL_DEBUG_INFO = 3
     """Return the an/lt module base and RX and TX (serdes index, base address)"""
 
     LT_TRAINING_ALGORITHM = 4
     """The link training algorithm to use"""
 
+    ANLT_LOG_CONTROL = 5
+    """Control what should be logged by anlt"""
+
+    ANLT_STRICT_MODE = 6
+    """Set AN/LT strict mode. In strict mode errored framed will be ignored"""
+
+    AN_LT_XLA_MODE = 7
+    """Set XLA mode. If enabled XLA dumps will, if triggered, be logged automatically"""
+
+
 
 class Layer1LogType(IntEnum):
     """
 
     .. versionadded:: 1.1
 
     .. warning::
@@ -2298,9 +2308,55 @@
 
     """
 
     TRAINED = 0
     """The lane is trained"""
 
 
+class AnLtLogControl(IntEnum):
+    """
+    .. versionadded:: 1.3
+
+    ANLT log control bits
+
+    """
+    # 1st nibble
+    LOG_TYPE_DEBUG = 0x2
+    """debug log output"""
+
+    LOG_TYPE_AN_TRACE = 0x4
+    """autonegotiation trace output"""
+
+    LOG_TYPE_LT_TRACE = 0x8
+    """link training trace output"""
+
+    # 2nd nibble
+    LOG_TYPE_ALG_TRACE = 0x10
+    """link training algorithm trace"""
+
+    # 5th nibble
+    LOG_TYPE_FSM_PORT = 0x10000
+    """port state machine transitions"""
+
+    LOG_TYPE_FSM_ANEG = 0x20000
+    """autonegotiation state machine transitions. What we act on"""
+
+    LOG_TYPE_FSM_ANEG_STIMULI = 0x40000
+    """autonegotiation stimuli state machine transitions. What we ask"""
+
+    LOG_TYPE_FSM_LT = 0x80000
+    """link training state machine transitions"""
+
+    # 6th nibble
+    LOG_TYPE_FSM_LT_COEFF = 0x100000
+    """link training coefficient state machine transitions. What we act on"""
+
+    LOG_TYPE_FSM_LT_STIMULI = 0x200000
+    """link training stimuli state machine transitions. What we ask"""
+
+    LOG_TYPE_FSM_LT_ALG0 = 0x400000
+    """link training algorithm 0 state machine transitions"""
+
+    LOG_TYPE_FSM_LT_ALG1 = 0x800000
+    """link training algorithm -1 state machine transitions"""
 
 # endregion
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/m4_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/m4_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/m4e_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/m4e_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/m_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/m_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 from .. import interfaces
 from ..transporter.token import Token
 from ..protocol.fields import data_types as xt
 from ..protocol.fields.field import XmpField
 from ..registry import register_command
 from .enums import *  # noqa: F403
+from xoa_driver.internals import warn
 
 
 @register_command
 @dataclass
 class M_RESERVATION:
     """
     Set this command to reserve, release, or relinquish a module itself (as
@@ -163,14 +164,15 @@
     """
 
     code: typing.ClassVar[int] = 77
     pushed: typing.ClassVar[bool] = True
 
     _connection: "interfaces.IConnection"
     _module: int
+
     @dataclass(frozen=True)
     class GetDataAttr:
         version: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer, the hardware image version number.
 
     def get(self) -> "Token[GetDataAttr]":
         """Gets the version number of the hardware image installed on the test module.
 
@@ -210,15 +212,15 @@
 @dataclass
 class M_PORTCOUNT:
     """
     Gets the maximum number of ports on a module.
 
     .. note::
 
-        For a CFP-type module this number refers to the maximum number of ports possible on the module regardless of the media configuration. So if a CFP-type module can be set in for instance either 1x100G mode or 8x10G mode then this command will always return 8. If you want the current number of ports for a CFP-type module you need to read the M_CFPCONFIG` command which returns the number of current ports.
+        For a CFP-type module this number refers to the maximum number of ports possible on the module regardless of the media configuration. So if a CFP-type module can be set in for instance either 1x100G mode or 8x10G mode then this command will always return 8. If you want the current number of ports for a CFP-type module you need to read the M_CFPCONFIGEXT` command which returns the number of current ports.
 
     """
 
     code: typing.ClassVar[int] = 80
     pushed: typing.ClassVar[bool] = False
 
     _connection: "interfaces.IConnection"
@@ -384,14 +386,16 @@
         return Token(self._connection, build_get_request(self, module=self._module))
 
 
 @register_command
 @dataclass
 class M_CFPCONFIG:
     """
+    .. deprecated:: 1.3
+
     The current number of ports and their speed of a CFP test module. If the CFP
     type is NOTFLEXIBLE then it reflects the transceiver currently in the CFP cage.
     If the CFP type is FLEXIBLE (or NOTPRESENT) then the configuration can be changed
     explicitly. The following combinations are possible: 4x10G, 8x10G, 1x40G, 2x40G,
     and 1x100G. (replaced by :class:`M_CFPCONFIGEXT`)
     """
 
@@ -415,24 +419,30 @@
         """Get the current number of ports and their speed of a CFP test module.
 
         :return:
             - number of ports
             - port speed, in Gbps
         :rtype: M_CFPCONFIG.GetDataAttr
         """
+
+        warn.depricated("module.cfp.config.get() (M_CFPCONFIG) is deprecated. Please use module.cfp.config_extended.get() (M_CFPCONFIGEXT) instead.")
+
         return Token(self._connection, build_get_request(self, module=self._module))
 
     def set(self, port_count: int, port_speed: int) -> "Token":
         """Set the current number of ports and their speed of a CFP test module.
 
         :param port_count: number of ports
         :type port_count: int
         :param port_speed: port speed, in Gbps
         :type port_speed: int
         """
+
+        warn.depricated("module.cfp.config.set() (M_CFPCONFIG) is deprecated. Please use module.cfp.config_extended.set() (M_CFPCONFIGEXT) instead.")
+
         return Token(self._connection, build_set_request(self, module=self._module, port_count=port_count, port_speed=port_speed))
 
 
 @register_command
 @dataclass
 class M_COMMENT:
     """
@@ -1424,25 +1434,31 @@
 
     _connection: "interfaces.IConnection"
     _module: int
 
     @dataclass(frozen=True)
     class SetDataAttr:
         mode: XmpField[xt.XmpInt] = XmpField(xt.XmpInt, choices=PPMSweepMode)  # coded byte, specifying the sweeping function: OFF or TRIANGLE
-        ppb_step: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0, the numeric clock adjustment in ppb per step of the sweep. If set to 0, the sweep will use as small steps as possible, creating a "linear" sweep of the clock rate.
-        step_delay: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >0 the delay in µs between each step in the sweep. If ppb_step is 0: The total time in µs to sweep linearly from 0 to max_ppb.
-        max_ppb: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer != 0, the numeric maximum clock adjustment. The sign of max_ppb determines if the sweep will start with positive or negative offsets. When the next step would exceed the limit set by max_ppb, the sweep changes direction. I.e. the deviation will sweep from 0 to max_ppb, to (-max_ppb), and back to 0.
+        # integer >=0, the numeric clock adjustment in ppb per step of the sweep. If set to 0, the sweep will use as small steps as possible, creating a "linear" sweep of the clock rate.
+        ppb_step: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
+        # integer >0 the delay in µs between each step in the sweep. If ppb_step is 0: The total time in µs to sweep linearly from 0 to max_ppb.
+        step_delay: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
+        # integer != 0, the numeric maximum clock adjustment. The sign of max_ppb determines if the sweep will start with positive or negative offsets. When the next step would exceed the limit set by max_ppb, the sweep changes direction. I.e. the deviation will sweep from 0 to max_ppb, to (-max_ppb), and back to 0.
+        max_ppb: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
         loops: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0, the number of full sweeps performed. 0 means "indefinitely".
 
     @dataclass(frozen=True)
     class GetDataAttr:
         mode: XmpField[xt.XmpInt] = XmpField(xt.XmpInt, choices=PPMSweepMode)  # coded byte, specifying the sweeping function.
-        ppb_step: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0, the numeric clock adjustment in ppb per step of the sweep. If set to 0, the sweep will use as small steps as possible, creating a "linear" sweep of the clock rate.
-        step_delay: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >0 the delay in µs between each step in the sweep. If ppb_step is 0: The total time in µs to sweep linearly from 0 to max_ppb.
-        max_ppb: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer != 0, the numeric maximum clock adjustment. The sign of max_ppb determines if the sweep will start with positive or negative offsets. When the next step would exceed the limit set by max_ppb, the sweep changes direction. I.e. the deviation will sweep from 0 to max_ppb, to (-max_ppb), and back to 0.
+        # integer >=0, the numeric clock adjustment in ppb per step of the sweep. If set to 0, the sweep will use as small steps as possible, creating a "linear" sweep of the clock rate.
+        ppb_step: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
+        # integer >0 the delay in µs between each step in the sweep. If ppb_step is 0: The total time in µs to sweep linearly from 0 to max_ppb.
+        step_delay: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
+        # integer != 0, the numeric maximum clock adjustment. The sign of max_ppb determines if the sweep will start with positive or negative offsets. When the next step would exceed the limit set by max_ppb, the sweep changes direction. I.e. the deviation will sweep from 0 to max_ppb, to (-max_ppb), and back to 0.
+        max_ppb: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
         loops: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0, the number of full sweeps performed. 0 means "indefinitely".
 
     def get(self) -> "Token[GetDataAttr]":
         """Get the PPM sweep parameters from the module.
 
         :return: the PPM sweep parameters from the module.
         :rtype: M_CLOCKPPBSWEEP.GetDataAttr
@@ -1485,15 +1501,16 @@
     @dataclass(frozen=True)
     class GetDataAttr:
         state: XmpField[xt.XmpByte] = XmpField(xt.XmpByte, choices=PPMSweepStatus)  # coded byte, specifying if a sweep is active: OFF or SWEEPING
 
         curr_sweep: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0, the current full sweep number, counting from 0.
         curr_step: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer >=0 the current step number inside the sweep, counting from 0.
 
-        max_steps: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)  # integer, >0, the total number of steps comprising a full sweep. For "linear" sweeps (ppb_step=0, see M_CLOCKPPBSWEEP) this number is determined by the chassis. In other cases, the number is implicitly given by the M_CLOCKPPBSWEEP parameters.
+        # integer, >0, the total number of steps comprising a full sweep. For "linear" sweeps (ppb_step=0, see M_CLOCKPPBSWEEP) this number is determined by the chassis. In other cases, the number is implicitly given by the M_CLOCKPPBSWEEP parameters.
+        max_steps: XmpField[xt.XmpInt] = XmpField(xt.XmpInt)
 
     def get(self) -> "Token[GetDataAttr]":
         """Get the current status of the :class:`M_CLOCKPPBSWEEP` function.
 
         :return: the current status of the :class:`M_CLOCKPPBSWEEP` function.
         :rtype: M_CLOCKSWEEPSTATUS.GetDataAttr
         """
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4e_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4e_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/p4g_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/p4g_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/p_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/p_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
 @dataclass
 class P_SPEEDSELECTION:
     """
     The speed mode of an autoneg port with an interface type supporting multiple speeds.
 
     .. note::
 
-        This is only a settable command when speed is selected at the port level. Use the M_CFPCONFIG` command when speed is selected at the module level.
+        This is only a settable command when speed is selected at the port level. Use the M_CFPCONFIGEXT` command when speed is selected at the module level.
 
     """
 
     code: typing.ClassVar[int] = 109
     pushed: typing.ClassVar[bool] = True
 
     _connection: "interfaces.IConnection"
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pc_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pc_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pd_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pd_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pe_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pe_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pec_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pec_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/ped_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/ped_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pef_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pef_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1752,39 +1752,37 @@
     _module: int
     _port: int
     _flow_xindex: int
     _filter_type: FilterType  # integer, the sub-index value which indicates the filter type - “shadow-copy”(0) or “working-copy”(1).
 
     @dataclass(frozen=True)
     class SetDataAttr:
-        use: XmpField[xt.XmpByte] = XmpField(xt.XmpByte, choices=FilterUse)  # coded byte, specifies the use of TPLD information.
         action: XmpField[xt.XmpByte] = XmpField(xt.XmpByte, choices=InfoAction)  # coded byte, specifies the action of TPLD information.
 
     @dataclass(frozen=True)
     class GetDataAttr:
-        use: XmpField[xt.XmpByte] = XmpField(xt.XmpByte, choices=FilterUse)  # coded byte, specifies the use of TPLD information.information.
         action: XmpField[xt.XmpByte] = XmpField(xt.XmpByte, choices=InfoAction)  # coded byte, specifies the action of TPLD information.
 
     def get(self) -> "Token[GetDataAttr]":
         """Get the settings of filtering on TPLD field in a packet.
 
         :return: the settings of filtering on TPLD field in a packet.
         :rtype: PEF_TPLDSETTINGS.GetDataAttr
         """
         return Token(self._connection, build_get_request(self, module=self._module, port=self._port, indices=[self._flow_xindex, self._filter_type]))
 
-    def set(self, use: FilterUse, action: InfoAction) -> "Token":
+    def set(self, action: InfoAction) -> "Token":
         """Set the settings of filtering on TPLD field in a packet.
 
         :param use: specifies the use of TPLD information.
         :type use: FilterUse
         :param action: specifies the action of TPLD information.
         :type action: InfoAction
         """
-        return Token(self._connection, build_set_request(self, module=self._module, port=self._port, indices=[self._flow_xindex, self._filter_type], use=use, action=action))
+        return Token(self._connection, build_set_request(self, module=self._module, port=self._port, indices=[self._flow_xindex, self._filter_type], action=action))
 
 
 @register_command
 @dataclass
 class PEF_TPLDCONFIG:
     """
     Defines the TPLD filter configuration. There are only 16 TPLD filter, thus the index values are from 0 to 15.
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pf_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pf_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pl1_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pl1_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     _port: int
     _serdes_xindex: int
     _page_xindex: int
 
     @dataclass(frozen=True)
     class GetDataAttr:
 
-        duration_us: XmpField[xt.XmpUnsignedInt] = XmpField(xt.XmpUnsignedInt)  # duration of the auto-negotiation process in microseconds, from autoneg is enabled on the port to the negotiation is finished.
+        duration_us: XmpField[xt.XmpUnsignedInt] = XmpField(xt.XmpUnsignedInt)  # duration of the link training process in microseconds, from LT is enabled on the port to the LT is finished.
 
         lock_lost_count: XmpField[xt.XmpUnsignedInt] = XmpField(xt.XmpUnsignedInt)  # number of lost locks on auto-neg.
 
         pre1_current_level: XmpField[xt.XmpUnsignedInt] = XmpField(xt.XmpUnsignedInt)  # c(-1) current level.
 
         pre1_rx_increment_req_count: XmpField[xt.XmpUnsignedInt] = XmpField(xt.XmpUnsignedInt)  # c(-1) received number of increment requests.
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pl_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pl_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pm_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pm_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pp_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pp_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pr_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pr_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/ps_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/ps_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/pt_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/pt_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/px_commands.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/px_commands.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/commands/subtypes.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/commands/subtypes.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/interfaces.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/command_builders.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/command_builders.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/constants.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/add_on.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/add_on.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/data_types.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/data_types.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/exceptions.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/field.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/field.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/fields/interfaces.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_header.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_header.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_request.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_request.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/struct_response.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/struct_response.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/protocol/utils.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/registry.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/registry.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/commands_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/commands_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/events_observer.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/events_observer.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/exceptions.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/funcs.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/funcs.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/logging.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/logging.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/request_id.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/request_id.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/token.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/token.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/core/transporter/transportation_handler.py` & `xoa-driver-1.3.0/xoa_driver/internals/core/transporter/transportation_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             self.process_data(header, body_bytes)
         )
         return slice(BODY_POS.stop)
 
     async def process_data(self, header, data: bytearray) -> None:
         try:
             response = await self.__serialize_to_response(header, data)
-        except t_ex.RepeatedRequestID as e:
+        except (t_ex.RepeatedRequestID, RuntimeError) as e:
             self.__log.error(f"{e} Original Data: {data}")
         else:
             if response.header.is_pushed:
                 self.__handle_push_response(response)
             else:
                 self.__handle_param_response(response)
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/base_index.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/base_index.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/cg.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/cg.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/histogram.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/histogram.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/l2.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/l2.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/l3.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/l3.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/raw.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/raw.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/replay.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/replay.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/tcp.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/tcp.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/tls.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/tls.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/udp.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/udp.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/connection_group/user_state.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/connection_group/user_state.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/base_filter.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/filter/genuine_filter.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/filter/genuine_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/length_term.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/length_term.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/match_term.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/match_term.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/port_dataset.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/port_dataset.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/base_stream.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/base_stream.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/indices/streams/genuine_stream.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/indices/streams/genuine_stream.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/base_module.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_chimera.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,233 +4,189 @@
 from typing import TYPE_CHECKING
 from typing_extensions import Self
 from xoa_driver.internals.core.commands import (
     M_STATUS,
     M_UPGRADE,
     M_UPGRADEPROGRESS,
     M_CFPTYPE,
+    M_CFPCONFIGEXT,
     M_CFPCONFIG,
     M_COMMENT,
     M_CAPABILITIES,
     M_CLOCKPPB,
     M_TXCLOCKSOURCE_NEW,
     M_TXCLOCKSTATUS_NEW,
     M_EMULBYPASS,
     M_LATENCYMODE,
-    M_REVISION,
-    M_MEDIA,
-    M_MEDIASUPPORT,
-    M_TIMESYNC,
-    M_CLOCKSYNCSTATUS,
-    M_NAME,
 )
 
-from xoa_driver.internals.hli_v1 import revisions
+from xoa_driver.internals.hli_v2 import revisions
 from xoa_driver.internals.utils import ports_manager as pm
 from xoa_driver.internals.utils import attributes as utils
 from xoa_driver.internals.state_storage import modules_state
-from xoa_driver import ports
+from xoa_driver.v2 import ports
 from . import base_module as bm
 if TYPE_CHECKING:
     from xoa_driver.internals.core import interfaces as itf
     from . import __interfaces as m_itf
 
 
 class ChTXClock:
     """
     Advanced timing feature (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.source = M_TXCLOCKSOURCE_NEW(conn, module_id)
         """
         The source that drives the TX clock rate of the ports on the test module.
-        
-        :type: M_TXCLOCKSOURCE_NEW
+        Representation of M_TXCLOCKSOURCE_NEW
         """
         self.status = M_TXCLOCKSTATUS_NEW(conn, module_id)
         """
         TX clock status of the test module.
-        
-        :type: M_TXCLOCKSTATUS_NEW
+        Representation of M_TXCLOCKSTATUS_NEW
         """
 
 
 class ChCFP:
     """
     CFP test module (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.type = M_CFPTYPE(conn, module_id)
         """
         The transceiver's CFP type currently inserted.
-        
-        :type: M_CFPTYPE
+        Representation of M_CFPTYPE
         """
         self.config = M_CFPCONFIG(conn, module_id)
         """
         The CFP configuration of the test module.
-        
-        :type: M_CFPCONFIG
+        Representation of M_CFPCONFIG
+        """
+        self.config_extended = M_CFPCONFIGEXT(conn, module_id)
+        """
+        The CFP configuration of the test module.
+        Representation of M_CFPCONFIGEXT
         """
 
 
 class ChUpgrade:
     """
     Upgrade test module (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.start = M_UPGRADE(conn, module_id)
         """
         Start the upgrade progress of the test module.
-        
-        :type: M_UPGRADE
+        Representation of M_UPGRADE
         """
         self.progress = M_UPGRADEPROGRESS(conn, module_id)
         """
         Upgrade progress status of the test module.
-        
-        :type: M_UPGRADEPROGRESS
+        Representation of M_UPGRADEPROGRESS
         """
 
+
 class ChTiming:
     """Test module timing and clock configuration"""
-
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
-        self.source = M_TIMESYNC(conn, module_id)
-        """Timing source of the test module.
-
-        :type: M_TIMESYNC
-        """
 
         self.clock_local_adjust = M_CLOCKPPB(conn, module_id)
         """Time adjustment controlling of the local clock of the test module, which drives the TX rate of the test ports.
-        
-        :type: M_CLOCKPPB
+        Representation of M_CLOCKPPB
         """
 
-        self.clock_sync_status = M_CLOCKSYNCSTATUS(conn, module_id)
-        """Test module's clock sync status.
 
-        :type: M_CLOCKSYNCSTATUS
+class ChAdvancedTiming:
+    """Advanced Timing config and control"""
+    def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
+        self.clock = ChTXClock(conn, module_id)
+        """Advanced timing clock config and status
         """
 
 
 class ModuleChimera(bm.BaseModule["modules_state.ModuleLocalState"]):
     """
-    This is a conceptual class of Chimera module.
+    Representation of a Chimera module on physical tester.
     """
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
 
         self._local_states = modules_state.ModuleLocalState()
 
         self.tx_clock = ChTXClock(conn, self.module_id)
         """
-        TX clock config (Chimera).
-
-        :type: ChTXClock
-        """
-
-        self.timing = ChTiming(conn, self.module_id)
-        """
-        Timing config (Chimera).
-
-        :type: ChTiming
+        Advanced timing feature (Chimera).
         """
 
         self.cfp = ChCFP(conn, self.module_id)
         """
         CFP test module (Chimera).
-
-        :type:  ChCFP
         """
 
         self.upgrade = ChUpgrade(conn, self.module_id)
         """
         Upgrade test module (Chimera).
-
-        :type: ChUpgrade
         """
 
         self.capabilities = M_CAPABILITIES(conn, self.module_id)
         """
         Test module's capabilities.
-        
-        :type: M_CAPABILITIES
+        Representation of M_CAPABILITIES
         """
 
         self.comment = M_COMMENT(conn, self.module_id)
         """
         Test module's description.
-        
-        :type: M_COMMENT
+        Representation of M_COMMENT
         """
 
         self.status = M_STATUS(conn, self.module_id)
         """
         Test module's status.
-        
-        :type: M_STATUS
+        Representation of M_STATUS
         """
 
         self.clock_ppb = M_CLOCKPPB(conn, self.module_id)
         """
         Test module's local clock adjustment.
-        
-        :type: M_CLOCKPPB
+        Representation of M_CLOCKPPB
         """
 
         self.emulator_bypass_mode = M_EMULBYPASS(conn, self.module_id)
         """
         Bypass mode of the Chimera module.
-        
-        :type: M_EMULBYPASS
+        Representation of M_EMULBYPASS
         """
 
         self.latency_mode = M_LATENCYMODE(conn, self.module_id)
         """
         Latency mode of the Chimera module.
-        
-        :type: M_LATENCYMODE
+        Representation of M_LATENCYMODE
         """
 
-        self.revision = M_REVISION(conn, self.module_id)
-        """Test module's model P/N name.
-
-        :type: M_REVISION
-        """
-
-        self.media = M_MEDIA(conn, self.module_id)
-        """Test module's media type.
+        self.timing = ChTiming(conn, self.module_id)
+        """Test module's timing configuration."""
 
-        :type: M_MEDIA
+        self.bypass_mode = M_EMULBYPASS(conn, self.module_id)
         """
-
-        self.available_speeds = M_MEDIASUPPORT(conn, self.module_id)
-        """Test module's available speeds.
-
-        :type: M_MEDIASUPPORT
+        Bypass mode of the Chimera module.
+        Representation of M_EMULBYPASS
         """
 
-        self.name = M_NAME(conn, self.module_id)
-        """Test module's name.
-
-        :type: M_NAME
-        """
+        self.adv_timing = ChAdvancedTiming(conn, self.module_id)
 
         self.ports: pm.PortsManager["ports.PortChimera"] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PortChimera,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
         """
         Port index manager of the Chimera module.
-
-        :type: PortsManager
         """
 
     @property
     def info(self) -> modules_state.ModuleLocalState:
         return self._local_states
 
     async def _setup(self) -> Self:
@@ -239,104 +195,74 @@
             self.ports.fill()
         )
         self._local_states.register_subscriptions(self)
         return self
 
     on_cfp_type_change = functools.partialmethod(utils.on_event, M_CFPTYPE)
     """
-    Register a callback function to the event that the module's CFP type changes.
+    Register a callback to the event that the module's CFP type changes.
     """
 
     on_cfp_config_change = functools.partialmethod(utils.on_event, M_CFPCONFIG)
     """
-    Register a callback function to the event that the module's CFP configuration changes.
-    """
-
-    on_status_change = functools.partialmethod(utils.on_event, M_STATUS)
-    """
-    Register a callback function to the event that the module's model changes.
-    """
-
-    on_latency_mode_change = functools.partialmethod(utils.on_event, M_LATENCYMODE)
-    """
-    Register a callback function to the event that the module's latency mode changes.
+    Register a callback to the event that the module's CFP configuration changes.
     """
 
-    on_media_change = functools.partialmethod(utils.on_event, M_MEDIA)
+    on_cfp_config_extended_change = functools.partialmethod(utils.on_event, M_CFPCONFIGEXT)
     """
-    Register a callback to the event that the module's media and available speeds change.
+    Register a callback to the event that the module's CFP configuration changes.
     """
 
-    on_media_support_change = functools.partialmethod(utils.on_event, M_MEDIASUPPORT)
-    """
-    Register a callback to the event that the module's supported media changes.
-    """
-
-    on_timing_source_change = functools.partialmethod(utils.on_event, M_TIMESYNC)
+    on_status_change = functools.partialmethod(utils.on_event, M_STATUS)
     """
-    Register a callback to the event that the module's timesync mode changes.
+    Register a callback to the event that the module's model changes.
     """
 
-    on_timing_clock_local_adjust_change = functools.partialmethod(utils.on_event, M_CLOCKPPB)
+    on_latency_mode_change = functools.partialmethod(utils.on_event, M_LATENCYMODE)
     """
-    Register a callback to the event that the module's clock adjustment ppb changes.
+    Register a callback to the event that the module's latency mode changes.
     """
 
-    on_adv_timing_clock_tx_status_change = functools.partialmethod(utils.on_event, M_TXCLOCKSTATUS_NEW)
-    """Register a callback to the event that the module's TX clock status changes."""
-
-    on_adv_timing_clock_tx_source_change = functools.partialmethod(utils.on_event, M_TXCLOCKSOURCE_NEW)
-    """Register a callback to the event that the module's clock that drives the port TX rates changes."""
-
 
 @typing.final
 @revisions.register_chimera_module(rev="Chimera-100G-5S-2P")
 class MChi100G5S2P(ModuleChimera):
     """Chimera module Chi-100G-5S-2P"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
         self.ports: pm.PortsManager[ports.PChi100G5S2P] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PChi100G5S2P,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-100G-5S-2P
-        
-        :type: PortsManager
-        """
+        """Port index manager of Chi-100G-5S-2P"""
 
 
 @typing.final
 @revisions.register_chimera_module(rev="Chimera-100G-5S-2P[b]")
 class MChi100G5S2P_b(ModuleChimera):
     """Chimera module Chi-100G-5S-2P[b]"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
         self.ports: pm.PortsManager[ports.PChi100G5S2P_b] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PChi100G5S2P_b,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-100G-5S-2P[b]
-        
-        :type: PortsManager
-        """
+        """Port index manager of Chi-100G-5S-2P[b]"""
 
 
 @typing.final
-@revisions.register_chimera_module(rev="Chimera-40G-5S-2P")
-class MChi40G5S2P(ModuleChimera):
-    """Chimera module Chi-40G-5S-2P"""
+@revisions.register_chimera_module(rev="Chimera-40G-2S-2P")
+class MChi40G2S2P(ModuleChimera):
+    """Chimera module Chi-40G-2S-2P"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
-        self.ports: pm.PortsManager[ports.PChi40G5S2P] = pm.PortsManager(
+        self.ports: pm.PortsManager[ports.PChi40G2S2P] = pm.PortsManager(
             conn=conn,
-            ports_type=ports.PChi40G5S2P,
+            ports_type=ports.PChi40G2S2P,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-40G-5S-2P
-
-        :type: PortsManager
-        """
+        """Port index manager of Chi-40G-2S-2P"""
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_l23ve.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_l23ve.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/module_l47.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_l47.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_combi.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_combi.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_d.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_d.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_e.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_e.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_f.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_f.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_g.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_g.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,7 +49,22 @@
         self.ports: pm.PortsManager[ports.PLoki100G3S1PSE] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PLoki100G3S1PSE,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
         """Port Index Manager of Loki-100G-3S-1P-SE"""
+
+
+@typing.final
+@revisions.register_valkyrie_module(rev="Loki-100G-3S-1P-B")
+class MLoki100G3S1PB(ModuleL23):
+    """Test module Loki-100G-3S-1P-B"""
+    def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
+        super().__init__(conn, init_data)
+        self.ports: pm.PortsManager[ports.PLoki100G3S1PB] = pm.PortsManager(
+            conn=conn,
+            ports_type=ports.PLoki100G3S1PB,
+            module_id=self.module_id,
+            ports_count=self.ports_count
+        )
+        """Port index manager of Loki-100G-3S-1P-B"""
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_h.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_h.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_i.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_i.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_j.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_j.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_k.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_k.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l1.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_l1.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_m.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_m.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_n.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/family_n.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/modules/modules_l23/module_l23_base.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/modules_l23/module_l23_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from typing_extensions import Self
 from xoa_driver.internals.core.commands import (
     M_STATUS,
     M_UPGRADE,
     M_UPGRADEPROGRESS,
     M_TIMESYNC,
     M_CFPTYPE,
-    M_CFPCONFIG,
     M_COMMENT,
     # M_TIMEADJUSTMENT,
     M_CAPABILITIES,
     M_MEDIASUPPORT,
     M_FPGAREIMAGE,
     M_MULTIUSER,
     M_CFPCONFIGEXT,
+    M_CFPCONFIG,
     M_CLOCKPPB,
     M_SMAINPUT,
     M_SMAOUTPUT,
     M_SMASTATUS,
     M_NAME,
     M_REVISION,
     M_MEDIA,
@@ -114,15 +114,15 @@
         self.config = M_CFPCONFIG(conn, module_id)
         """The CFP configuration of the test module.
 
         :type: M_CFPCONFIG
         """
 
         self.config_extended = M_CFPCONFIGEXT(conn, module_id)
-        """The extended CFP configuration of the test module.
+        """The CFP configuration of the test module.
 
         :type: M_CFPCONFIGEXT
         """
 
 
 class MTiming:
     """Test module timing and clock configuration"""
@@ -279,15 +279,15 @@
     on_cfp_type_change = functools.partialmethod(utils.on_event, M_CFPTYPE)
     """Register a callback to the event that the module's CFP type (:class:`M_CFPTYPE`) changes."""
 
     on_cfp_config_change = functools.partialmethod(utils.on_event, M_CFPCONFIG)
     """Register a callback to the event that the module's CFP configuration changes."""
 
     on_cfp_config_extended_change = functools.partialmethod(utils.on_event, M_CFPCONFIGEXT)
-    """Register a callback to the event that the module's CFP extended configuration changes."""
+    """Register a callback to the event that the module's CFP configuration changes."""
 
     on_status_change = functools.partialmethod(utils.on_event, M_STATUS)
     """Register a callback to the event that the module's status changes."""
 
     on_revision_change = functools.partialmethod(utils.on_event, M_REVISION)
     """Register a callback to the event that the module's model type changes."""
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/base_port.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/base_port.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_capture.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_capture.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23_genuine.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_l23_genuine.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_reception_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_reception_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transceiver.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transceiver.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transmission_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/bases/port_transmission_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/general.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,50 +54,50 @@
 
 
 class FEthernet:
     """Filter for Ethernet field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_ETHSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on Ethernet field.
-        
+
         :type: PEF_ETHSETTINGS
         """
         self.src_address = prevent_set(PEF_ETHSRCADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Ethernet source address settings for the filter.
-        
+
         :type: PEF_ETHSRCADDR
         """
         self.dest_address = prevent_set(PEF_ETHDESTADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Ethernet destination address settings for the filter.
-        
+
         :type: PEF_ETHDESTADDR
         """
 
 
 class FPerVlanType:
     """Filter for VLAN tag."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType, vlan_type: FilterVlanType) -> None:
         self.tag = prevent_set(PEF_VLANTAG(conn, module_id, port_id, flow_index, filter_type, vlan_type), filter_type)
         """VLAN tag setting for the filter.
-        
+
         :type: PEF_VLANTAG
         """
         self.pcp = prevent_set(PEF_VLANPCP(conn, module_id, port_id, flow_index, filter_type, vlan_type), filter_type)
         """VLAN PCP setting for the filter.
-        
+
         :type: PEF_VLANPCP
         """
 
 
 class FVlan:
     """Filter for VLAN field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_VLANSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on VLAN field.
-        
+
         :type: PEF_VLANSETTINGS
         """
 
         self.inner = FPerVlanType(conn, module_id, port_id, flow_index, filter_type, FilterVlanType.INNER)
         """Filter for inner VLAN tag."""
 
         self.outer = FPerVlanType(conn, module_id, port_id, flow_index, filter_type, FilterVlanType.OUTER)
@@ -105,95 +105,95 @@
 
 
 class FUdp:
     """Filer for UDP field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_UDPSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on UDP field.
-        
+
         :type: PEF_UDPSETTINGS
         """
         self.src_port = prevent_set(PEF_UDPSRCPORT(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """UDP source port settings for the filter.
-        
+
         :type: PEF_UDPSRCPORT
         """
         self.dest_port = prevent_set(PEF_UDPDESTPORT(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """UDP destination port settings for the filter.
-        
+
         :type: PEF_UDPDESTPORT
         """
 
 
 class FTcp:
     """Filter for TCP."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_TCPSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on TCP field.
-        
+
         :type: PEF_TCPSETTINGS
         """
         self.src_port = prevent_set(PEF_TCPSRCPORT(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """TCP source port settings for the filter.
-        
+
         :type: PEF_TCPSRCPORT
         """
         self.dest_port = prevent_set(PEF_TCPDESTPORT(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """TCP destination port settings for the filter.
-        
+
         :type: PEF_TCPDESTPORT
         """
 
 
 class FIPv4:
     """Filter for IPv4 field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_IPV4SETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on IPv4 field.
-        
+
         :type: PEF_IPV4SETTINGS
         """
         self.src_address = prevent_set(PEF_IPV4SRCADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv4 source address settings for the filter.
-        
+
         :type: PEF_IPV4SRCADDR
         """
         self.dest_address = prevent_set(PEF_IPV4DESTADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv4 destination address settings for the filter.
-        
+
         :type: PEF_IPV4DESTADDR
         """
         self.dscp = prevent_set(PEF_IPV4DSCP(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv4 DSCP/TOS settings for the filter.
-        
+
         :type: PEF_IPV4DSCP
         """
 
 
 class FIPv6:
     """Filter for IPv6 field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_IPV6SETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on IPv6 field.
-        
+
         :type: PEF_IPV6SETTINGS
         """
         self.src_address = prevent_set(PEF_IPV6SRCADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv6 source address settings for the filter.
-        
+
         :type: PEF_IPV6SRCADDR
         """
         self.dest_address = prevent_set(PEF_IPV6DESTADDR(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv6 destination address settings for the filter.
-        
+
         :type: PEF_IPV6DESTADDR
         """
         self.traffic_class = prevent_set(PEF_IPV6TC(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """IPv6 traffic class settings for the filter.
-        
+
         :type: PEF_IPV6TC
         """
 
 
 class FIp:
     """Filter for IP field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
@@ -205,151 +205,151 @@
 
 
 class FMpls:
     """Filter for MPLS field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_MPLSSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on MPLS field.
-        
+
         :type: PEF_MPLSSETTINGS
         """
         self.label = prevent_set(PEF_MPLSLABEL(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """MPLS label settings for the filter.
-        
+
         :type: PEF_MPLSLABEL
         """
         self.toc = prevent_set(PEF_MPLSTOC(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """"MPLS TOC settings for the filter.
-        
+
         :type: PEF_MPLSTOC
         """
 
 
 class FTpld:
     """Filter for Xena TPLD field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_TPLDSETTINGS(conn, module_id, port_id, flow_index, filter_type))
         """Filter action on Xena TPLD field.
-        
+
         :type: PEF_TPLDSETTINGS
         """
 
         self.test_payload_filters_config = tuple(
             prevent_set(PEF_TPLDCONFIG(conn, module_id, port_id, flow_index, filter_type, test_payload_filter_index), filter_type)
             for test_payload_filter_index in range(16)  # range need to put to the constants place
         )
         """TPLD filter configurations.
-        
+
         :type: PEF_TPLDCONFIG
         """
 
 
 class FAny:
     """Filter for any field."""
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.settings = prevent_set(PEF_ANYSETTINGS(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Filter action on any field.
-        
+
         :type: PEF_ANYSETTINGS
         """
         self.config = prevent_set(PEF_ANYCONFIG(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """Any field's filter configurations.
-        
+
         :type: PEF_ANYCONFIG
         """
 
 
 class ModeBasic:
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self.l2plus_use = prevent_set(PEF_L2PUSE(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """L2 protocol to use.
-        
+
         :type: PEF_L2PUSE
         """
         self.l3_use = prevent_set(PEF_L3USE(conn, module_id, port_id, flow_index, filter_type), filter_type)
         """L3 protocol to use.
-        
+
         :type: PEF_L3USE
         """
         self.any = FAny(conn, module_id, port_id, flow_index, filter_type)
         """Filter for any field.
-        
+
         :type: FAny
         """
 
         self.tpld = FTpld(conn, module_id, port_id, flow_index, filter_type)
         """Filter for Xena TPLD field.
-        
+
         :type: FTpld
         """
 
         self.mpls = FMpls(conn, module_id, port_id, flow_index, filter_type)
         """Filter for MPLS field.
-        
+
         :type: FMpls
         """
 
         self.ip = FIp(conn, module_id, port_id, flow_index, filter_type)
         """Filter for IP field.
-        
+
         :type: FIp
         """
 
         self.tcp = FTcp(conn, module_id, port_id, flow_index, filter_type)
         """Filter for TCP field.
-        
+
         :type: FTcp
         """
 
         self.udp = FUdp(conn, module_id, port_id, flow_index, filter_type)
         """Filter for UDP field.
-        
+
         :type: FUdp
         """
 
         self.vlan = FVlan(conn, module_id, port_id, flow_index, filter_type)
         """Filter for VLAN field.
-        
+
         :type: FVlan
         """
 
         self.ethernet = FEthernet(conn, module_id, port_id, flow_index, filter_type)
         """Filter for Ethernet field.
-        
+
         :type: FEthernet
         """
 
 
 class ProtocolSegment:
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType, protocol_segment_index: int, segment_type: ProtocolOption) -> None:  # noqa: E501
         self.segment_type = segment_type
 
         self.value = prevent_set(PEF_VALUE(conn, module_id, port_id, flow_index, filter_type, protocol_segment_index), filter_type)
         """Value bytes match for the filter.
-        
+
         :type: PEF_VALUE
         """
         self.mask = prevent_set(PEF_MASK(conn, module_id, port_id, flow_index, filter_type, protocol_segment_index), filter_type)
         """Mask byte value.
-        
+
         :type: PEF_MASK
         """
 
 
 class ModeExtended:
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, filter_type: FilterType) -> None:
         self._conn = conn
         self._module_id = module_id
         self._port_id = port_id
         self._flow_index = flow_index
         self._filter_type = filter_type
 
         # self.protocol = prevent_set(PEF_PROTOCOL(conn, module_id, port_id, flow_index, filter_type))
         # """Protocol segments match for the filter.
-        # 
+        #
         # :type: PEF_PROTOCOL
         # """
 
     async def get_protocol_segments(self) -> Tuple[ProtocolSegment, ...]:
         segments_raw = (
             await PEF_PROTOCOL(
                 self._conn,
@@ -362,15 +362,15 @@
         return tuple(
             ProtocolSegment(
                 self._conn,
                 self._module_id,
                 self._port_id,
                 self._flow_index,
                 self._filter_type,
-                idx,  # TODO: need to discuss with Leo
+                idx + 1,  # TODO: need to discuss with Leo
                 ProtocolOption(segment_type)
             )
             for idx, segment_type in enumerate(segments_raw)
         )
 
 
 T = TypeVar("T")
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/shadow.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/shadow.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/working.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/filter_definition/working.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_custom_distribution.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_custom_distribution.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_distribution.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/pe_distribution.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_chimera.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,11 +101,11 @@
 
 class PChi100G5S2P_b(PortChimera):
     """Impairment port on Chi-100G-5S-2P[b] module.
     """
     ...
 
 
-class PChi40G5S2P(PortChimera):
-    """Impairment port on Chi-40G-5S-2P module.
+class PChi40G2S2P(PortChimera):
+    """Impairment port on Chi-40G-2S-2P module.
     """
     ...
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_emulation.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/port_emulation.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/reception_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/reception_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/transmission_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/chimera/transmission_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_combi.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_combi.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_d.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_d.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_e.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_e.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_f.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_f.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_g.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_g.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,7 +66,12 @@
     ...
 
 
 class PLoki100G3S1PSE(FamilyG):
     """L23 port on Loki-100G-3S-1P-SE module.
     """
     ...
+
+class PLoki100G3S1PB(FamilyG):
+    """L23 port on Loki-100G-3S-1P-B module.
+    """
+    ...
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_h.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_h.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_i.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_i.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_j.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_j.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_k.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_k.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l1.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_l1.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/family_m.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/family_m.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/fault_jkl.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/fault_jkl.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ghijkl.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ghijkl.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ijkl_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_ijkl_chimera.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/pcs_pma_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l23/port_l23ve.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l23/port_l23ve.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/counters.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/counters.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/main.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/main.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/ports/port_l47/packet_engine.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/ports/port_l47/packet_engine.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/_base_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/_base_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/_tester_session.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/_tester_session.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/rest_api.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/rest_api.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/time_keeper.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/time_keeper.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/upload_file.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/l_23/upload_file.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/genuine/management_interface.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/genuine/management_interface.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l23_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l23_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l23ve_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l23ve_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l47_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l47_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v1/testers/l47ve_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/testers/l47ve_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/base_index.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/base_index.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/cg.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/cg.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/histogram.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/histogram.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/l2.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/l2.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/l3.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/l3.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/raw.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/raw.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/replay.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/replay.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/tcp.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/tcp.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/tls.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/tls.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/udp.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/udp.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/connection_group/user_state.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/connection_group/user_state.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/base_filter.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/filter/genuine_filter.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/filter/genuine_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/length_term.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/length_term.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/match_term.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/match_term.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/port_dataset.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/port_dataset.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/base_stream.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/base_stream.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/indices/streams/genuine_stream.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/indices/streams/genuine_stream.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/base_module.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v1/modules/module_chimera.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,183 +4,240 @@
 from typing import TYPE_CHECKING
 from typing_extensions import Self
 from xoa_driver.internals.core.commands import (
     M_STATUS,
     M_UPGRADE,
     M_UPGRADEPROGRESS,
     M_CFPTYPE,
-    M_CFPCONFIG,
     M_COMMENT,
     M_CAPABILITIES,
     M_CLOCKPPB,
     M_TXCLOCKSOURCE_NEW,
     M_TXCLOCKSTATUS_NEW,
     M_EMULBYPASS,
     M_LATENCYMODE,
+    M_REVISION,
+    M_MEDIA,
+    M_MEDIASUPPORT,
+    M_TIMESYNC,
+    M_CLOCKSYNCSTATUS,
+    M_NAME,
+    M_CFPCONFIGEXT,
+    M_CFPCONFIG,
 )
 
-from xoa_driver.internals.hli_v2 import revisions
+from xoa_driver.internals.hli_v1 import revisions
 from xoa_driver.internals.utils import ports_manager as pm
 from xoa_driver.internals.utils import attributes as utils
 from xoa_driver.internals.state_storage import modules_state
-from xoa_driver.v2 import ports
+from xoa_driver import ports
 from . import base_module as bm
 if TYPE_CHECKING:
     from xoa_driver.internals.core import interfaces as itf
     from . import __interfaces as m_itf
 
 
 class ChTXClock:
     """
     Advanced timing feature (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.source = M_TXCLOCKSOURCE_NEW(conn, module_id)
         """
         The source that drives the TX clock rate of the ports on the test module.
-        Representation of M_TXCLOCKSOURCE_NEW
+        
+        :type: M_TXCLOCKSOURCE_NEW
         """
         self.status = M_TXCLOCKSTATUS_NEW(conn, module_id)
         """
         TX clock status of the test module.
-        Representation of M_TXCLOCKSTATUS_NEW
+        
+        :type: M_TXCLOCKSTATUS_NEW
         """
 
 
 class ChCFP:
     """
     CFP test module (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.type = M_CFPTYPE(conn, module_id)
         """
         The transceiver's CFP type currently inserted.
-        Representation of M_CFPTYPE
+        
+        :type: M_CFPTYPE
         """
         self.config = M_CFPCONFIG(conn, module_id)
         """
         The CFP configuration of the test module.
-        Representation of M_CFPCONFIG
+        
+        :type: M_CFPCONFIG
+        """
+        self.config_extended = M_CFPCONFIGEXT(conn, module_id)
+        """
+        The CFP configuration of the test module.
+        
+        :type: M_CFPCONFIGEXT
         """
 
 
 class ChUpgrade:
     """
     Upgrade test module (Chimera).
     """
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
         self.start = M_UPGRADE(conn, module_id)
         """
         Start the upgrade progress of the test module.
-        Representation of M_UPGRADE
+        
+        :type: M_UPGRADE
         """
         self.progress = M_UPGRADEPROGRESS(conn, module_id)
         """
         Upgrade progress status of the test module.
-        Representation of M_UPGRADEPROGRESS
+        
+        :type: M_UPGRADEPROGRESS
         """
 
-
 class ChTiming:
     """Test module timing and clock configuration"""
+
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
+        self.source = M_TIMESYNC(conn, module_id)
+        """Timing source of the test module.
+
+        :type: M_TIMESYNC
+        """
 
         self.clock_local_adjust = M_CLOCKPPB(conn, module_id)
         """Time adjustment controlling of the local clock of the test module, which drives the TX rate of the test ports.
-        Representation of M_CLOCKPPB
+        
+        :type: M_CLOCKPPB
         """
 
+        self.clock_sync_status = M_CLOCKSYNCSTATUS(conn, module_id)
+        """Test module's clock sync status.
 
-class ChAdvancedTiming:
-    """Advanced Timing config and control"""
-    def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
-        self.clock = ChTXClock(conn, module_id)
-        """Advanced timing clock config and status
+        :type: M_CLOCKSYNCSTATUS
         """
 
 
 class ModuleChimera(bm.BaseModule["modules_state.ModuleLocalState"]):
     """
-    Representation of a Chimera module on physical tester.
+    This is a conceptual class of Chimera module.
     """
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
 
         self._local_states = modules_state.ModuleLocalState()
 
         self.tx_clock = ChTXClock(conn, self.module_id)
         """
-        Advanced timing feature (Chimera).
+        TX clock config (Chimera).
+
+        :type: ChTXClock
+        """
+
+        self.timing = ChTiming(conn, self.module_id)
+        """
+        Timing config (Chimera).
+
+        :type: ChTiming
         """
 
         self.cfp = ChCFP(conn, self.module_id)
         """
         CFP test module (Chimera).
+
+        :type:  ChCFP
         """
 
         self.upgrade = ChUpgrade(conn, self.module_id)
         """
         Upgrade test module (Chimera).
+
+        :type: ChUpgrade
         """
 
         self.capabilities = M_CAPABILITIES(conn, self.module_id)
         """
         Test module's capabilities.
-        Representation of M_CAPABILITIES
+        
+        :type: M_CAPABILITIES
         """
 
         self.comment = M_COMMENT(conn, self.module_id)
         """
         Test module's description.
-        Representation of M_COMMENT
+        
+        :type: M_COMMENT
         """
 
         self.status = M_STATUS(conn, self.module_id)
         """
         Test module's status.
-        Representation of M_STATUS
+        
+        :type: M_STATUS
         """
 
         self.clock_ppb = M_CLOCKPPB(conn, self.module_id)
         """
         Test module's local clock adjustment.
-        Representation of M_CLOCKPPB
+        
+        :type: M_CLOCKPPB
         """
 
         self.emulator_bypass_mode = M_EMULBYPASS(conn, self.module_id)
         """
         Bypass mode of the Chimera module.
-        Representation of M_EMULBYPASS
+        
+        :type: M_EMULBYPASS
         """
 
         self.latency_mode = M_LATENCYMODE(conn, self.module_id)
         """
         Latency mode of the Chimera module.
-        Representation of M_LATENCYMODE
+        
+        :type: M_LATENCYMODE
         """
 
-        self.timing = ChTiming(conn, self.module_id)
-        """Test module's timing configuration."""
+        self.revision = M_REVISION(conn, self.module_id)
+        """Test module's model P/N name.
 
-        self.bypass_mode = M_EMULBYPASS(conn, self.module_id)
+        :type: M_REVISION
         """
-        Bypass mode of the Chimera module.
-        Representation of M_EMULBYPASS
+
+        self.media = M_MEDIA(conn, self.module_id)
+        """Test module's media type.
+
+        :type: M_MEDIA
+        """
+
+        self.available_speeds = M_MEDIASUPPORT(conn, self.module_id)
+        """Test module's available speeds.
+
+        :type: M_MEDIASUPPORT
         """
 
-        self.adv_timing = ChAdvancedTiming(conn, self.module_id)
+        self.name = M_NAME(conn, self.module_id)
+        """Test module's name.
+
+        :type: M_NAME
+        """
 
         self.ports: pm.PortsManager["ports.PortChimera"] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PortChimera,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
         """
         Port index manager of the Chimera module.
+
+        :type: PortsManager
         """
 
     @property
     def info(self) -> modules_state.ModuleLocalState:
         return self._local_states
 
     async def _setup(self) -> Self:
@@ -189,69 +246,109 @@
             self.ports.fill()
         )
         self._local_states.register_subscriptions(self)
         return self
 
     on_cfp_type_change = functools.partialmethod(utils.on_event, M_CFPTYPE)
     """
-    Register a callback to the event that the module's CFP type changes.
+    Register a callback function to the event that the module's CFP type changes.
     """
 
     on_cfp_config_change = functools.partialmethod(utils.on_event, M_CFPCONFIG)
     """
-    Register a callback to the event that the module's CFP configuration changes.
+    Register a callback function to the event that the module's CFP configuration changes.
+    """
+
+    on_cfp_config_extended_change = functools.partialmethod(utils.on_event, M_CFPCONFIGEXT)
+    """
+    Register a callback function to the event that the module's CFP configuration changes.
     """
 
     on_status_change = functools.partialmethod(utils.on_event, M_STATUS)
     """
-    Register a callback to the event that the module's model changes.
+    Register a callback function to the event that the module's model changes.
     """
 
     on_latency_mode_change = functools.partialmethod(utils.on_event, M_LATENCYMODE)
     """
-    Register a callback to the event that the module's latency mode changes.
+    Register a callback function to the event that the module's latency mode changes.
+    """
+
+    on_media_change = functools.partialmethod(utils.on_event, M_MEDIA)
+    """
+    Register a callback to the event that the module's media and available speeds change.
+    """
+
+    on_media_support_change = functools.partialmethod(utils.on_event, M_MEDIASUPPORT)
+    """
+    Register a callback to the event that the module's supported media changes.
     """
 
+    on_timing_source_change = functools.partialmethod(utils.on_event, M_TIMESYNC)
+    """
+    Register a callback to the event that the module's timesync mode changes.
+    """
+
+    on_timing_clock_local_adjust_change = functools.partialmethod(utils.on_event, M_CLOCKPPB)
+    """
+    Register a callback to the event that the module's clock adjustment ppb changes.
+    """
+
+    on_adv_timing_clock_tx_status_change = functools.partialmethod(utils.on_event, M_TXCLOCKSTATUS_NEW)
+    """Register a callback to the event that the module's TX clock status changes."""
+
+    on_adv_timing_clock_tx_source_change = functools.partialmethod(utils.on_event, M_TXCLOCKSOURCE_NEW)
+    """Register a callback to the event that the module's clock that drives the port TX rates changes."""
+
 
 @typing.final
 @revisions.register_chimera_module(rev="Chimera-100G-5S-2P")
 class MChi100G5S2P(ModuleChimera):
     """Chimera module Chi-100G-5S-2P"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
         self.ports: pm.PortsManager[ports.PChi100G5S2P] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PChi100G5S2P,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-100G-5S-2P"""
+        """Port index manager of Chi-100G-5S-2P
+        
+        :type: PortsManager
+        """
 
 
 @typing.final
 @revisions.register_chimera_module(rev="Chimera-100G-5S-2P[b]")
 class MChi100G5S2P_b(ModuleChimera):
     """Chimera module Chi-100G-5S-2P[b]"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
         self.ports: pm.PortsManager[ports.PChi100G5S2P_b] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PChi100G5S2P_b,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-100G-5S-2P[b]"""
+        """Port index manager of Chi-100G-5S-2P[b]
+        
+        :type: PortsManager
+        """
 
 
 @typing.final
-@revisions.register_chimera_module(rev="Chimera-40G-5S-2P")
-class MChi40G5S2P(ModuleChimera):
-    """Chimera module Chi-40G-5S-2P"""
+@revisions.register_chimera_module(rev="Chimera-40G-2S-2P")
+class MChi40G2S2P(ModuleChimera):
+    """Chimera module Chi-40G-2S-2P"""
     def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
         super().__init__(conn, init_data)
-        self.ports: pm.PortsManager[ports.PChi40G5S2P] = pm.PortsManager(
+        self.ports: pm.PortsManager[ports.PChi40G2S2P] = pm.PortsManager(
             conn=conn,
-            ports_type=ports.PChi40G5S2P,
+            ports_type=ports.PChi40G2S2P,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
-        """Port index manager of Chi-40G-5S-2P"""
+        """Port index manager of Chi-40G-2S-2P
+
+        :type: PortsManager
+        """
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_l23ve.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_l23ve.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/module_l47.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/module_l47.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_combi.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_combi.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_d.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_d.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_e.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_e.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_f.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_f.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_g.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_g.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,7 +49,22 @@
         self.ports: pm.PortsManager[ports.PLoki100G3S1PSE] = pm.PortsManager(
             conn=conn,
             ports_type=ports.PLoki100G3S1PSE,
             module_id=self.module_id,
             ports_count=self.ports_count
         )
         """Port index manager of Loki-100G-3S-1P-SE"""
+
+
+@typing.final
+@revisions.register_valkyrie_module(rev="Loki-100G-3S-1P-B")
+class MLoki100G3S1PB(ModuleL23):
+    """Test module Loki-100G-3S-1P-B"""
+    def __init__(self, conn: "itf.IConnection", init_data: "m_itf.ModuleInitData") -> None:
+        super().__init__(conn, init_data)
+        self.ports: pm.PortsManager[ports.PLoki100G3S1PB] = pm.PortsManager(
+            conn=conn,
+            ports_type=ports.PLoki100G3S1PB,
+            module_id=self.module_id,
+            ports_count=self.ports_count
+        )
+        """Port index manager of Loki-100G-3S-1P-B"""
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_h.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_h.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_i.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_i.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_j.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_j.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_k.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_k.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l1.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_l1.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_m.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_m.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_n.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/family_n.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/modules/modules_l23/module_l23_base.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/modules/modules_l23/module_l23_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from typing_extensions import Self
 from xoa_driver.internals.core.commands import (
     M_STATUS,
     M_UPGRADE,
     M_UPGRADEPROGRESS,
     M_TIMESYNC,
     M_CFPTYPE,
-    M_CFPCONFIG,
     M_COMMENT,
     # M_TIMEADJUSTMENT,
     M_CAPABILITIES,
     M_MEDIASUPPORT,
     M_FPGAREIMAGE,
     M_MULTIUSER,
     M_CFPCONFIGEXT,
+    M_CFPCONFIG,
     M_CLOCKPPB,
     M_SMAINPUT,
     M_SMAOUTPUT,
     M_SMASTATUS,
     M_NAME,
     M_REVISION,
     M_MEDIA,
@@ -102,15 +102,15 @@
 
         self.config = M_CFPCONFIG(conn, module_id)
         """The CFP configuration of the test module.
         Representation of M_CFPCONFIG
         """
 
         self.config_extended = M_CFPCONFIGEXT(conn, module_id)
-        """The extended CFP configuration of the test module.
+        """The CFP configuration of the test module.
         Representation of M_CFPCONFIGEXT
         """
 
 
 class MTiming:
     """Test module timing and clock configuration"""
     def __init__(self, conn: "itf.IConnection", module_id: int) -> None:
@@ -233,15 +233,15 @@
     on_cfp_type_change = functools.partialmethod(utils.on_event, M_CFPTYPE)
     """Register a callback to the event that the module's CFP type changes."""
 
     on_cfp_config_change = functools.partialmethod(utils.on_event, M_CFPCONFIG)
     """Register a callback to the event that the module's CFP configuration changes."""
 
     on_cfp_config_extended_change = functools.partialmethod(utils.on_event, M_CFPCONFIGEXT)
-    """Register a callback to the event that the module's CFP extended configuration changes."""
+    """Register a callback to the event that the module's CFP configuration changes."""
 
     on_status_change = functools.partialmethod(utils.on_event, M_STATUS)
     """Register a callback to the event that the module's status changes."""
 
     on_revision_change = functools.partialmethod(utils.on_event, M_REVISION)
     """Register a callback to the event that the module's model type changes."""
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/base_port.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/base_port.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_capture.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_capture.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23_genuine.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_l23_genuine.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_reception_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_reception_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transceiver.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transceiver.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transmission_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/bases/port_transmission_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/general.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         return tuple(
             ProtocolSegment(
                 self._conn,
                 self._module_id,
                 self._port_id,
                 self._flow_index,
                 self._filter_type,
-                idx,  # TODO: need to discuss with Leo
+                idx + 1,  # TODO: need to discuss with Leo
                 ProtocolOption(segment_type)
             )
             for idx, segment_type in enumerate(segments_raw)
         )
 
 
 T = TypeVar("T")
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/shadow.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/shadow.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/working.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/filter_definition/working.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_custom_distribution.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_custom_distribution.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_distribution.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/pe_distribution.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,130 +20,37 @@
     PED_CONST,
     PED_ACCBURST,
     PED_STEP,
     PED_ENABLE,
 )
 
 
-class ImpairmentDistributionConfig:
-    def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, impairment_type_index: "ImpairmentTypeIndex") -> None:
-        self.enable = PED_ENABLE(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Impairment distribution control.
-        Representation of PED_ENABLE
-        """
-
-        self.schedule = PED_SCHEDULE(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Impairment scheduling configuration.
-        Representation of PED_SCHEDULE
-        """
-
-        self.one_shot_status = PED_ONESHOTSTATUS(conn, module_id, port_id, flow_index, impairment_type_index)
-        """One-shot status.
-        Representation of PED_ONESHOTSTATUS
-        """
-
-        self.off = PED_OFF(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Impairments Distribution to OFF.
-        Representation of PED_OFF
-        """
-
-        self.fixed = PED_FIXED(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Fixed Rate distribution configuration.
-        Representation of PED_FIXED
-        """
-
-        self.random = PED_RANDOM(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Random Rate distribution configuration.
-        Representation of PED_RANDOM
-        """
-
-        self.bit_error_rate = PED_BER(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Bit Error Rate distribution configuration.
-        Representation of PED_BER
-        """
-
-        self.random = PED_RANDOMBURST(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Random Burst configuration.
-        Representation of PED_RANDOMBURST
-        """
-
-        self.ge = PED_GE(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Gilbert-Elliot distribution configuration.
-        Representation of PED_GE
-        """
-
-        self.uniform = PED_UNI(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Uniform distribution configuration.
-        Representation of PED_UNI
-        """
-
-        self.gaussian = PED_GAUSS(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Gaussian distribution configuration.
-        Representation of PED_GAUSS
-        """
-
-        self.poison = PED_POISSON(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Poisson distribution configuration.
-        Representation of PED_POISSON
-        """
-
-        self.gamma = PED_GAMMA(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Gamma distribution configuration.
-        Representation of PED_GAMMA
-        """
-
-        self.custom = PED_CUST(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Associate a custom distribution to a flow and impairment type.
-        Representation of PED_CUST
-        """
-
-        self.constant_delay = PED_CONST(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Constant Delay distribution configuration.
-        Representation of PED_CONST
-        """
-
-        self.accumulate_and_burst = PED_ACCBURST(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Accumulate & Burst distribution configuration.
-        Representation of PED_ACCBURST
-        """
-
-        self.step = PED_STEP(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Step distribution configuration.
-        Representation of PED_STEP
-        """
-
-        self.fixed_burst = PED_FIXEDBURST(conn, module_id, port_id, flow_index, impairment_type_index)
-        """Fixed Burst distribution configuration.
-        Representation of PED_FIXEDBURST
-        """
-
-
 class ImpairmentDistribution:
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int, impairment_type_index: "ImpairmentTypeIndex") -> None:
         self.off = PED_OFF(conn, module_id, port_id, flow_index, impairment_type_index)
         """Impairments Distribution to OFF.
         Representation of PED_OFF
         """
 
-        self.fixed = PED_FIXED(conn, module_id, port_id, flow_index, impairment_type_index)
+        self.fixed_rate = PED_FIXED(conn, module_id, port_id, flow_index, impairment_type_index)
         """Fixed Rate distribution configuration.
         Representation of PED_FIXED
         """
 
-        self.random = PED_RANDOM(conn, module_id, port_id, flow_index, impairment_type_index)
+        self.random_rate = PED_RANDOM(conn, module_id, port_id, flow_index, impairment_type_index)
         """Random Rate distribution configuration.
         Representation of PED_RANDOM
         """
 
         self.bit_error_rate = PED_BER(conn, module_id, port_id, flow_index, impairment_type_index)
         """Bit Error Rate distribution configuration.
         Representation of PED_BER
         """
 
-        self.random = PED_RANDOMBURST(conn, module_id, port_id, flow_index, impairment_type_index)
+        self.random_burst = PED_RANDOMBURST(conn, module_id, port_id, flow_index, impairment_type_index)
         """Random Burst configuration.
         Representation of PED_RANDOMBURST
         """
 
         self.ge = PED_GE(conn, module_id, port_id, flow_index, impairment_type_index)
         """Gilbert-Elliot distribution configuration.
         Representation of PED_GE
@@ -155,15 +62,15 @@
         """
 
         self.gaussian = PED_GAUSS(conn, module_id, port_id, flow_index, impairment_type_index)
         """Gaussian distribution configuration.
         Representation of PED_GAUSS
         """
 
-        self.poison = PED_POISSON(conn, module_id, port_id, flow_index, impairment_type_index)
+        self.poisson = PED_POISSON(conn, module_id, port_id, flow_index, impairment_type_index)
         """Poisson distribution configuration.
         Representation of PED_POISSON
         """
 
         self.gamma = PED_GAMMA(conn, module_id, port_id, flow_index, impairment_type_index)
         """Gamma distribution configuration.
         Representation of PED_GAMMA
@@ -188,8 +95,8 @@
         """Step distribution configuration.
         Representation of PED_STEP
         """
 
         self.fixed_burst = PED_FIXEDBURST(conn, module_id, port_id, flow_index, impairment_type_index)
         """Fixed Burst distribution configuration.
         Representation of PED_FIXEDBURST
-        """
+        """
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_chimera.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,11 +95,11 @@
 
 class PChi100G5S2P_b(PortChimera):
     """Impairment port on Chi-100G-5S-2P[b] module.
     """
     ...
 
 
-class PChi40G5S2P(PortChimera):
-    """Impairment port on Chi-40G-5S-2P module.
+class PChi40G2S2P(PortChimera):
+    """Impairment port on Chi-40G-2S-2P module.
     """
     ...
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_emulation.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/port_emulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     TYPE_CHECKING,
     Tuple,
 )
 from dataclasses import astuple
 from xoa_driver.internals.core.commands.enums import ImpairmentTypeIndex
 from xoa_driver.internals.core.commands.ped_commands import PED_ENABLE, PED_ONESHOTSTATUS, PED_SCHEDULE
 
-from xoa_driver.internals.hli_v2.ports.port_l23.chimera.pe_distribution import ImpairmentDistributionConfig
 if TYPE_CHECKING:
     from xoa_driver.internals.core import interfaces as itf
 
 from xoa_driver.internals.core.commands import (
     PE_FCSDROP,
     PE_TPLDMODE,
     PE_COMMENT,
@@ -275,15 +274,15 @@
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int) -> None:
 
         self.type = PE_CORRUPT(conn, module_id, port_id, flow_index)
         """Bandwidth policer configuration.
         Representation of PE_BANDPOLICER
         """
 
-        self.distribution = ImpairmentDistributionConfig(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.CORRUPTION)
+        self.distribution = ImpairmentDistribution(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.CORRUPTION)
 
         self.schedule = PED_SCHEDULE(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.CORRUPTION)
         """Impairment scheduling configuration.
         Representation of PED_SCHEDULE
         """
 
         self.one_shot_status = PED_ONESHOTSTATUS(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.CORRUPTION)
@@ -374,34 +373,24 @@
 
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int) -> None:
         self.config = PE_BANDSHAPER(conn, module_id, port_id, flow_index)
         """Bandwidth shaper configuration.
         Representation of PE_BANDSHAPER
         """
 
-        self.enable = PED_ENABLE(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.DROP)
-        """Impairment distribution control.
-        Representation of PED_ENABLE
-        """
-
 
 class CPolicerImpairment:
     """Bandwidth policer impairment configuration."""
 
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int) -> None:
         self.config = PE_BANDPOLICER(conn, module_id, port_id, flow_index)
         """Bandwidth policer configuration.
         Representation of PE_BANDPOLICER
         """
 
-        self.enable = PED_ENABLE(conn, module_id, port_id, flow_index, ImpairmentTypeIndex.DROP)
-        """Impairment distribution control.
-        Representation of PED_ENABLE
-        """
-
 
 class CFlow:
     """Flow settings."""
 
     def __init__(self, conn: "itf.IConnection", module_id: int, port_id: int, flow_index: int) -> None:
         self.comment = PE_COMMENT(conn, module_id, port_id, flow_index)
         """Flow description.
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/reception_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/reception_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/transmission_statistics.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/chimera/transmission_statistics.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_combi.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_combi.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_d.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_d.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_e.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_e.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_f.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_f.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_g.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_g.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,7 +50,12 @@
     ...
 
 
 class PLoki100G3S1PSE(FamilyG):
     """L23 port on Loki-100G-3S-1P-SE module.
     """
     ...
+
+class PLoki100G3S1PB(FamilyG):
+    """L23 port on Loki-100G-3S-1P-B module.
+    """
+    ...
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_h.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_h.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_i.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_i.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_j.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_j.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_k.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_k.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l1.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_l1.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/family_m.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/family_m.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/fault_jkl.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/fault_jkl.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ghijkl.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ghijkl.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ijkl_chimera.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_ijkl_chimera.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_l.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/pcs_pma_l.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l23/port_l23ve.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l23/port_l23ve.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/counters.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/counters.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/main.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/main.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/ports/port_l47/packet_engine.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/ports/port_l47/packet_engine.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/_base_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/_base_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/_tester_session.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/_tester_session.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/rest_api.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/rest_api.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/time_keeper.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/time_keeper.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/upload_file.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/l_23/upload_file.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/genuine/management_interface.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/genuine/management_interface.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l23_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l23_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l23ve_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l23ve_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l47_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l47_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/hli_v2/testers/l47ve_tester.py` & `xoa-driver-1.3.0/xoa_driver/internals/hli_v2/testers/l47ve_tester.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/state_storage/_speed_detector.py` & `xoa-driver-1.3.0/xoa_driver/internals/state_storage/_speed_detector.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/state_storage/modules_state.py` & `xoa-driver-1.3.0/xoa_driver/internals/state_storage/modules_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     cage_type: "enums.MediaConfigurationType"
     """Module Media Configuration
 
     :return: module media configuration
     :rtype: MediaConfigurationType
     """
 
-    avaliable_speeds: List["ModuleSpeed"] = field(default_factory=list)
+    available_speeds: List["ModuleSpeed"] = field(default_factory=list)
     """List of module's port-speed information
 
     :return: list of module's port-speed information
     :rtype: List[ModuleSpeed]
     """
```

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/state_storage/ports_state.py` & `xoa-driver-1.3.0/xoa_driver/internals/state_storage/ports_state.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/state_storage/testers_state.py` & `xoa-driver-1.3.0/xoa_driver/internals/state_storage/testers_state.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/_base_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/_base_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/attributes.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/attributes.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/cap_id.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/cap_id.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/indices/_interfaces.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/indices/_interfaces.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/indices/header_modifier_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/indices/header_modifier_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/indices/index_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/indices/index_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/modules_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/modules_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/ports_manager.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/ports_manager.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/internals/utils/rev_tool.py` & `xoa-driver-1.3.0/xoa_driver/internals/utils/rev_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 #     # family_h
 #     "Odin-100G-3S-1P": modules.MThor400G7S1P_d,
 
 #     # family_g
 #     "Loki-100G-3S-1P": modules.MLoki100G3S1P,
 #     "Loki-100G-3S-1P[b]": modules.MLoki100G3S1P_b,
 #     "Loki-100G-3S-1P-SE": modules.MLoki100G3S1PSE,
+#     "Loki-100G-3S-1P-B": modules.MLoki100G3S1PB,
 
 #     # family_h
 #     "Loki-100G-5S-1P": modules.MLoki100G5S1P,
 
 #     # family_i
 #     "Loki-100G-5S-2P": modules.MLoki100G5S2P,
 
@@ -97,15 +98,15 @@
 # # endregion
 
 # # region Chimera Modules
 
 # CHIMERA_MODULES = {
 #     "Chimera-100G-5S-2P": modules.MChi100G5S2P,
 #     "Chimera-100G-5S-2P[b]": modules.MChi100G5S2P_b,
-#     "Chimera-40G-5S-2P": modules.MChi40G5S2P,
+#     "Chimera-40G-2S-2P": modules.MChi40G2S2P,
 # }
 
 # # endregion
 
 # # region Vulcan Modules
 
 # VULCAN_MODULES = {
```

### Comparing `xoa-driver-1.2.0/xoa_driver/misc.py` & `xoa-driver-1.3.0/xoa_driver/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/modules.py` & `xoa-driver-1.3.0/xoa_driver/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     MOdin10G1S6P_b,
     MOdin10G1S12P,
 )
 from .internals.hli_v1.modules.modules_l23.family_g import (
     MLoki100G3S1P,
     MLoki100G3S1P_b,
     MLoki100G3S1PSE,
+    MLoki100G3S1PB,
 )
 from .internals.hli_v1.modules.modules_l23.family_h import (
     MLoki100G5S1P,
     MOdin100G3S1P,
 )
 from .internals.hli_v1.modules.modules_l23.family_i import MLoki100G5S2P
 from .internals.hli_v1.modules.modules_l23.family_j import MThor100G5S4P
@@ -63,15 +64,15 @@
     MOdin10G4S2PCombi_b,
 )
 from .internals.hli_v1.modules.module_l23ve import ModuleL23VE
 from .internals.hli_v1.modules.module_chimera import (
     ModuleChimera,
     MChi100G5S2P,
     MChi100G5S2P_b,
-    MChi40G5S2P,
+    MChi40G2S2P,
 )
 from .internals.hli_v1.modules.module_l47 import ModuleL47
 from .internals.hli_v1.modules.module_l47ve import ModuleL47VE
 
 import typing
 
 GenericL23Module = typing.Union[
@@ -95,14 +96,15 @@
     "MOdin10G1S12P",
     "MOdin40G2S2P",
     "MOdin40G2S2PB",
     "MOdin100G3S1P",
     "MLoki100G3S1P",
     "MLoki100G3S1P_b",
     "MLoki100G3S1PSE",
+    "MLoki100G3S1PB",
     "MLoki100G5S1P",
     "MLoki100G5S2P",
     "MThor100G5S4P",
     "MThor400G7S1P",
     "MThor400G7S1P_b",
     "MThor400G7S1P_c",
     "MThor400G7S1P_d",
@@ -119,15 +121,15 @@
 
 GenericAnyModule = typing.Union[
     GenericL23Module,
     "ModuleL23VE",
     "ModuleChimera",
     "MChi100G5S2P",
     "MChi100G5S2P_b",
-    "MChi40G5S2P",
+    "MChi40G2S2P",
     "ModuleL47",
     "ModuleL47VE",
 ]
 
 __all__ = (
     "ModuleL23",
     "MOdin1G3S6P",
@@ -150,14 +152,15 @@
     "MOdin10G1S12P",
     "MOdin40G2S2P",
     "MOdin40G2S2PB",
     "MOdin100G3S1P",
     "MLoki100G3S1P",
     "MLoki100G3S1P_b",
     "MLoki100G3S1PSE",
+    "MLoki100G3S1PB",
     "MLoki100G5S1P",
     "MLoki100G5S2P",
     "MThor100G5S4P",
     "MThor400G7S1P",
     "MThor400G7S1P_b",
     "MThor400G7S1P_c",
     "MThor400G7S1P_d",
@@ -170,13 +173,13 @@
     "MOdin1G3S6PT1RJ45",
     "MOdin10G4S2PCombi",
     "MOdin10G4S2PCombi_b",
     "ModuleL23VE",
     "ModuleChimera",
     "MChi100G5S2P",
     "MChi100G5S2P_b",
-    "MChi40G5S2P",
+    "MChi40G2S2P",
     "ModuleL47",
     "ModuleL47VE",
     "GenericL23Module",
     "GenericAnyModule",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/ports.py` & `xoa-driver-1.3.0/xoa_driver/ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .internals.hli_v1.ports.port_l47.main import PortL47
 
 from .internals.hli_v1.ports.port_l23.port_l23ve import PortL23VE
 from .internals.hli_v1.ports.port_l23.chimera.port_chimera import (
     PortChimera,
     PChi100G5S2P,
     PChi100G5S2P_b,
-    PChi40G5S2P,
+    PChi40G2S2P,
 )
 
 from .internals.hli_v1.ports.port_l23.bases.port_l23 import BasePortL23
 from xoa_driver.internals.hli_v1.ports.port_l23.family_combi import (
     POdin1G4S4PCombi,
     POdin1G4S4PCombi_b,
     POdin10G4S2PCombi,
@@ -52,14 +52,15 @@
     POdin40G2S2PB,
 )
 
 from xoa_driver.internals.hli_v1.ports.port_l23.family_g import (
     PLoki100G3S1P,
     PLoki100G3S1P_b,
     PLoki100G3S1PSE,
+    PLoki100G3S1PB,
 )
 
 from xoa_driver.internals.hli_v1.ports.port_l23.family_h import (
     PLoki100G5S1P,
     POdin100G3S1P,
 )
 
@@ -103,14 +104,15 @@
     "POdin10G1S12P",
     "POdin40G2S2P",
     "POdin40G2S2PB",
     "POdin100G3S1P",
     "PLoki100G3S1P",
     "PLoki100G3S1P_b",
     "PLoki100G3S1PSE",
+    "PLoki100G3S1PB",
     "PLoki100G5S1P",
     "PLoki100G5S2P",
     "PThor100G5S4P",
     "PThor400G7S1P",
     "PThor400G7S1P_b",
     "PThor400G7S1P_c",
     "PThor400G7S1P_d",
@@ -130,15 +132,15 @@
 GenericAnyPort = typing.Union[
     GenericL23Port,
     "PortL47",
     "PortL23VE",
     "PortChimera",
     "PChi100G5S2P",
     "PChi100G5S2P_b",
-    "PChi40G5S2P",
+    "PChi40G2S2P",
 ]
 
 __all__ = (
     "BasePortL23",
     "POdin1G3S6P",
     "POdin1G3S6P_b",
     "POdin1G3S6PE",
@@ -158,14 +160,15 @@
     "POdin10G1S12P",
     "POdin40G2S2P",
     "POdin40G2S2PB",
     "POdin100G3S1P",
     "PLoki100G3S1P",
     "PLoki100G3S1P_b",
     "PLoki100G3S1PSE",
+    "PLoki100G3S1PB",
     "PLoki100G5S1P",
     "PLoki100G5S2P",
     "PThor100G5S4P",
     "PThor400G7S1P",
     "PThor400G7S1P_b",
     "PThor400G7S1P_c",
     "PThor400G7S1P_d",
@@ -181,11 +184,11 @@
     "POdin10G4S2PCombi",
     "POdin10G4S2PCombi_b",
     "PortL47",
     "PortL23VE",
     "PortChimera",
     "PChi100G5S2P",
     "PChi100G5S2P_b",
-    "PChi40G5S2P",
+    "PChi40G2S2P",
     "GenericL23Port",
     "GenericAnyPort",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/testers.py` & `xoa-driver-1.3.0/xoa_driver/testers.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/v2/misc.py` & `xoa-driver-1.3.0/xoa_driver/v2/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver/v2/modules.py` & `xoa-driver-1.3.0/xoa_driver/v2/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     MOdin10G1S6P_b,
     MOdin10G1S12P,
 )
 from xoa_driver.internals.hli_v2.modules.modules_l23.family_g import (
     MLoki100G3S1P,
     MLoki100G3S1P_b,
     MLoki100G3S1PSE,
+    MLoki100G3S1PB,
 )
 from xoa_driver.internals.hli_v2.modules.modules_l23.family_h import (
     MLoki100G5S1P,
     MOdin100G3S1P,
 )
 from xoa_driver.internals.hli_v2.modules.modules_l23.family_i import MLoki100G5S2P
 from xoa_driver.internals.hli_v2.modules.modules_l23.family_j import MThor100G5S4P
@@ -59,15 +60,15 @@
     MOdin10G4S2PCombi_b,
 )
 from xoa_driver.internals.hli_v2.modules.module_l23ve import ModuleL23VE
 from xoa_driver.internals.hli_v2.modules.module_chimera import (
     ModuleChimera,
     MChi100G5S2P,
     MChi100G5S2P_b,
-    MChi40G5S2P,
+    MChi40G2S2P,
 )
 from xoa_driver.internals.hli_v2.modules.module_l47 import ModuleL47
 from xoa_driver.internals.hli_v2.modules.module_l47ve import ModuleL47VE
 
 import typing
 
 GenericL23Module = typing.Union[
@@ -91,14 +92,15 @@
     "MOdin10G1S12P",
     "MOdin40G2S2P",
     "MOdin40G2S2PB",
     "MOdin100G3S1P",
     "MLoki100G3S1P",
     "MLoki100G3S1P_b",
     "MLoki100G3S1PSE",
+    "MLoki100G3S1PB",
     "MLoki100G5S1P",
     "MLoki100G5S2P",
     "MThor100G5S4P",
     "MThor400G7S1P",
     "MThor400G7S1P_b",
     "MThor400G7S1P_c",
     "MThor400G7S1P_d",
@@ -115,15 +117,15 @@
 
 GenericAnyModule = typing.Union[
     GenericL23Module,
     "ModuleL23VE",
     "ModuleChimera",
     "MChi100G5S2P",
     "MChi100G5S2P_b",
-    "MChi40G5S2P",
+    "MChi40G2S2P",
     "ModuleL47",
     "ModuleL47VE",
 ]
 
 __all__ = (
     "ModuleL23",
     "MOdin1G3S6P",
@@ -146,14 +148,15 @@
     "MOdin10G1S12P",
     "MOdin40G2S2P",
     "MOdin40G2S2PB",
     "MOdin100G3S1P",
     "MLoki100G3S1P",
     "MLoki100G3S1P_b",
     "MLoki100G3S1PSE",
+    "MLoki100G3S1PB",
     "MLoki100G5S1P",
     "MLoki100G5S2P",
     "MThor100G5S4P",
     "MThor400G7S1P",
     "MThor400G7S1P_b",
     "MThor400G7S1P_c",
     "MThor400G7S1P_d",
@@ -166,13 +169,13 @@
     "MOdin1G3S6PT1RJ45",
     "MOdin10G4S2PCombi",
     "MOdin10G4S2PCombi_b",
     "ModuleL23VE",
     "ModuleChimera",
     "MChi100G5S2P",
     "MChi100G5S2P_b",
-    "MChi40G5S2P",
+    "MChi40G2S2P",
     "ModuleL47",
     "ModuleL47VE",
     "GenericL23Module",
     "GenericAnyModule",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/v2/ports.py` & `xoa-driver-1.3.0/xoa_driver/v2/ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from xoa_driver.internals.hli_v2.ports.port_l47.main import PortL47
 
 from xoa_driver.internals.hli_v2.ports.port_l23.port_l23ve import PortL23VE
 from xoa_driver.internals.hli_v2.ports.port_l23.chimera.port_chimera import (
     PortChimera,
     PChi100G5S2P,
     PChi100G5S2P_b,
-    PChi40G5S2P,
+    PChi40G2S2P,
 )
 
 from xoa_driver.internals.hli_v2.ports.port_l23.bases.port_l23 import BasePortL23
 from xoa_driver.internals.hli_v2.ports.port_l23.family_combi import (
     POdin1G4S4PCombi,
     POdin1G4S4PCombi_b,
     POdin10G4S2PCombi,
@@ -49,14 +49,15 @@
     POdin40G2S2PB,
 )
 
 from xoa_driver.internals.hli_v2.ports.port_l23.family_g import (
     PLoki100G3S1P,
     PLoki100G3S1P_b,
     PLoki100G3S1PSE,
+    PLoki100G3S1PB,
 )
 
 from xoa_driver.internals.hli_v2.ports.port_l23.family_h import (
     PLoki100G5S1P,
     POdin100G3S1P,
 )
 
@@ -100,14 +101,15 @@
     "POdin10G1S12P",
     "POdin40G2S2P",
     "POdin40G2S2PB",
     "POdin100G3S1P",
     "PLoki100G3S1P",
     "PLoki100G3S1P_b",
     "PLoki100G3S1PSE",
+    "PLoki100G3S1PB",
     "PLoki100G5S1P",
     "PLoki100G5S2P",
     "PThor100G5S4P",
     "PThor400G7S1P",
     "PThor400G7S1P_b",
     "PThor400G7S1P_c",
     "PThor400G7S1P_d",
@@ -127,15 +129,15 @@
 GenericAnyPort = typing.Union[
     GenericL23Port,
     "PortL47",
     "PortL23VE",
     "PortChimera",
     "PChi100G5S2P",
     "PChi100G5S2P_b",
-    "PChi40G5S2P",
+    "PChi40G2S2P",
 ]
 
 __all__ = (
     "BasePortL23",
     "POdin1G3S6P",
     "POdin1G3S6P_b",
     "POdin1G3S6PE",
@@ -155,14 +157,15 @@
     "POdin10G1S12P",
     "POdin40G2S2P",
     "POdin40G2S2PB",
     "POdin100G3S1P",
     "PLoki100G3S1P",
     "PLoki100G3S1P_b",
     "PLoki100G3S1PSE",
+    "PLoki100G3S1PB",
     "PLoki100G5S1P",
     "PLoki100G5S2P",
     "PThor100G5S4P",
     "PThor400G7S1P",
     "PThor400G7S1P_b",
     "PThor400G7S1P_c",
     "PThor400G7S1P_d",
@@ -178,11 +181,11 @@
     "POdin10G4S2PCombi",
     "POdin10G4S2PCombi_b",
     "PortL47",
     "PortL23VE",
     "PortChimera",
     "PChi100G5S2P",
     "PChi100G5S2P_b",
-    "PChi40G5S2P",
+    "PChi40G2S2P",
     "GenericL23Port",
     "GenericAnyPort",
 )
```

### Comparing `xoa-driver-1.2.0/xoa_driver/v2/testers.py` & `xoa-driver-1.3.0/xoa_driver/v2/testers.py`

 * *Files identical despite different names*

### Comparing `xoa-driver-1.2.0/xoa_driver.egg-info/PKG-INFO` & `xoa-driver-1.3.0/xoa_driver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-driver
-Version: 1.2.0
+Version: 1.3.0
 Summary: Xena OpenAutomation (XOA) Python API is a driver providing user-friendly communication interfaces to Xena's physical and virtual Traffic Generation and Analysis (TGA) testers. It provides a rich collection of programming interfaces that can be used to either write test scripts or develop applications.
 Home-page: https://github.com/xenanetworks/open-automation-python-api
 Author: Artem Constantinov, Ron Ding, Leonard Yu
 Author-email: aco@xenanetworks.com, rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
@@ -18,24 +18,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xoa-driver) [![PyPI](https://img.shields.io/pypi/v/xoa-driver)](https://pypi.python.org/pypi/xoa-driver) ![GitHub](https://img.shields.io/github/license/xenanetworks/open-automation-python-api) [![Documentation Status](https://readthedocs.org/projects/xena-openautomation-python-api/badge/?version=stable)](https://xena-openautomation-python-api.readthedocs.io/en/stable/?badge=stable)
 # Xena OpenAutomation Python API
-Xena OpenAutomation (XOA) Python API is a driver providing user-friendly communication interfaces to Xena's physical and virtual Traffic Generation and Analysis (TGA) testers. It provides a rich collection of programming interfaces that can be used to either write test scripts or develop applications.
+Xena OpenAutomation Python API is a standalone Python library that provides a user-friendly and powerful interface for automating network testing tasks using Xena Networks test equipment. Xena test equipment is a high-performance network test device designed for testing and measuring the performance of network equipment and applications.
 
 ## Introduction
-Many of our customers choose to develop their own test scripts, where they automate performance verification, regression test, development verification, and so on.
+The XOA Python API is designed to be easy to use and integrate with other automation tools and frameworks. It provides a comprehensive set of methods and classes for interacting with Xena test equipment, including the ability to create and run complex test scenarios, generate and analyze traffic at line rate, and perform detailed analysis of network performance and behavior.
 
-At Xena Networks, we have always been providing customers with the best tool for test automation. To help our customers achieve a more efficient quality control and continuous development verification, we have developed a new platform Xena OpenAutomation, overlaying various Xena hardware and virtual testers, to offer not only automated test suites but also the power to build programs from simple scripts to advanced applications with endless possibilities.
+The XOA Python API simplifies the process of automating network testing tasks using Xena test equipment. It provides a simple, yet powerful, interface for interacting with Xena test equipment using the Python programming language. With the XOA Python API, network engineers and testing professionals can easily create and execute test scenarios, generate and analyze traffic, and perform detailed analysis of network performance and behavior, all while leveraging the power and flexibility of the Python programming language.
 
-The cornerstone component of Xena OpenAutomation is its Python API, which contains more than 600 commands, from basic streams creation to advance eye diagrams measurement. With this rich collection of programming interfaces, we empower our customers to either write test scripts or develop applications with almost limitless possibilities.
-
-Moving forward, all Xena’s automated test suites will be based on Xena OpenAutomation.
+Overall, the XOA Python API is a valuable tool for anyone looking to automate their network testing tasks using Xena test equipment. With its simple, yet powerful, interface and support for the Python programming language, the XOA Python API provides a flexible and extensible framework for automating network testing tasks and improving the quality of network infrastructure.
 
 ## Documentation
 The user documentation is hosted:
 [Xena OpenAutomation Python API Documentation](https://docs.xenanetworks.com/projects/xoa-python-api)
 
 ## Key Features
 * Objected-oriented, high-level abstraction, to help users save time on parsing command responses.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xoa-driver-1.2.0/xoa_driver.egg-info/SOURCES.txt` & `xoa-driver-1.3.0/xoa_driver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 xoa_driver/functions/__init__.py
 xoa_driver/functions/anlt.py
 xoa_driver/functions/anlt_ll_debug.py
 xoa_driver/functions/exceptions.py
 xoa_driver/functions/mgmt.py
 xoa_driver/functions/tools.py
 xoa_driver/internals/__init__.py
+xoa_driver/internals/warn.py
 xoa_driver/internals/core/__init__.py
 xoa_driver/internals/core/interfaces.py
 xoa_driver/internals/core/registry.py
 xoa_driver/internals/core/commands/__init__.py
 xoa_driver/internals/core/commands/c_commands.py
 xoa_driver/internals/core/commands/enums.py
 xoa_driver/internals/core/commands/m4_commands.py
```

