# Comparing `tmp/robotframework-lsp-1.8.0.tar.gz` & `tmp/robotframework-lsp-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotframework-lsp-1.8.0.tar", last modified: Mon Jan 23 14:09:28 2023, max compression
+gzip compressed data, was "dist/robotframework-lsp-1.9.0.tar", last modified: Fri Feb  3 17:23:36 2023, max compression
```

## Comparing `robotframework-lsp-1.8.0.tar` & `robotframework-lsp-1.9.0.tar`

### file list

```diff
@@ -1,1190 +1,1193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/ThirdPartyNotices.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/_ignore_failures_in_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/base_launch_process_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/debug_adapter_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)    48825 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/debugger_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/events_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)    30896 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process_pydevd_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process_robot_target_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/prerun_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    24372 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/run_robot__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/safe_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/force_pydevd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/install_and_run_debug_py.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_calltip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_execfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_filesystem_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_getopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_imports_tipper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17063 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_jy_imports_tipper.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_saved_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_tipper_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_console_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console_011.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_is_thread_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_localhost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    40160 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_umd.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_pytest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_xml_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23085 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)   763496 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevconsole_code_for_ironpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info_regular.py
--rw-r--r--   0 runner    (1001) docker     (123)    49872 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_breakpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_bytecode_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_code_to_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    36357 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_collect_bytecode_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    74423 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_command_line_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_custom_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)  2006433 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.c
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    86683 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_daemon_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_exec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    59424 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_gevent_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_json_debug_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    55468 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_referrers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)    25500 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_safe_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_save_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_source_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_stackless.py
--rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_suspended_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_thread_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22202 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch_regular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_traceproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27603 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vm_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_main.py
--rw-r--r--   0 runner    (1001) docker     (123)   926546 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.template.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_modify_bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/release_mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22299 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/concrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/instr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    49634 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_concrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_instr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32993 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_peephole_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/util_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/pydevd_fix_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_osx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/check_no_git_modifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/generate_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/names_to_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/rename_pep8.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/gradlew.bat
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/interpreterInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pycompletionserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_app_engine_debug_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookglut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookpyglet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt4.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt5.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhooktk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookwx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/matplotlibtools.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_for_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_pysrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_run_in_console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)   142770 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_always_live_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/add_code_to_python_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_amd64.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    22760 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_amd64.so
--rwxr-xr-x   0 runner    (1001) docker     (123)    21388 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_x86.so
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_pydevd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    54736 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86_64.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_settrace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_version.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/python.h
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/ref_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   259072 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_amd64.exe
--rw-r--r--   0 runner    (1001) docker     (123)   203264 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_x86.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/attach.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/compile_linux.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/compile_mac.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll
--rw-r--r--   0 runner    (1001) docker     (123)    14336 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168168 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    65394 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    58709 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    24409 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    67241 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    83555 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    70615 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/module.py
--rw-r--r--   0 runner    (1001) docker     (123)   183635 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23798 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    45884 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    62691 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/textio.py
--rw-r--r--   0 runner    (1001) docker     (123)    75478 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    36223 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   120809 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/advapi32.py
--rw-r--r--   0 runner    (1001) docker     (123)    25137 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_amd64.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_i386.py
--rw-r--r--   0 runner    (1001) docker     (123)    46705 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/dbghelp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/gdi32.py
--rw-r--r--   0 runner    (1001) docker     (123)   164818 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/kernel32.py
--rw-r--r--   0 runner    (1001) docker     (123)    22847 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)   159230 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/peb_teb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/psapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shell32.py
--rw-r--r--   0 runner    (1001) docker     (123)    25807 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shlwapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/user32.py
--rw-r--r--   0 runner    (1001) docker     (123)    36813 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py
--rw-r--r--   0 runner    (1001) docker     (123)    24309 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/
--rw-r--r--   0 runner    (1001) docker     (123)    27447 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.h
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/compile_windows.bat
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/inject_dll.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/py_win_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_in_memory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/targetver.h
--rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/django_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py
--rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/jinja2_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/pydevd_line_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/runfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup_pydevd_cython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/_django_manager_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/test_pydevd_reload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_check_pydevconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_get_referrers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jyserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jysimpleTipper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydev_ipython_011.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydevconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pyserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_simpleTipper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-glut.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk3.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-pyglet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-tk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-wx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/check_debug_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debug_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    55462 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_exttype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/performance_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/regression_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/other.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_big_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_constructs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_many_names_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_overflow_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case1.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case13.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case14.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15_execfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case16.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case17.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case17a.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case18.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case19.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case2.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case20.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case3.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case4.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case56.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case89.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_adjust_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_multiple_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint2.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_condition_exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_remote_no_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_change_breaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_check_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_custom_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_custom_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deadlock_thread_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_debug_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deep_stacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dir_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dont_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dont_trace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_event_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_frame_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator2.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator3.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_py3.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_step_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_get_next_statement_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_get_thread_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop_qt5.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_hasattr_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_hit_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_ignore_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_import_imported.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_import_main.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_lambda_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_lamda.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_large_exception_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_linecache.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_linecache_existing_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_listen_dap_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables3.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_m_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_m_switch_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_method_single_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_module_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multi_threads_stepping.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiple_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_stopped_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_no_subprocess_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_odict.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_path_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pause_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pydevd_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_python_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread1.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread2.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread3.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread4.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_quoting.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_raise_with_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions2.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remove_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_return_value_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_scapy.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_set_next_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_settrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_show_bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_simple_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_skip_breakpoint_in_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into2.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into3.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_map_goto_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_and_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_jmc.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_stepping.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_stop_async_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_subprocess_and_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit_0.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit_none.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_creation_deadlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_started_exited.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trace_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trio.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_type_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exception_get_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_listcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_on_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_on_top_level2.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_just_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_user_unhandled.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_user_unhandled2.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_variables_with_same_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_yield_from.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_zip_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_cyrillic_encoding_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_cyrillic_encoding_py3.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_syntax_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydevd_test_find_main_thread_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled_no_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_double_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception_on_other.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception_user_unhandled.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_on_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry2.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/not_my_coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/other.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/other_noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/_debugger_case_wrong_bytecode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_additional_thread_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_bytecode_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_code_obj_to_source_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_collect_bytecode_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    23705 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_convert_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   173317 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)   236370 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_dump_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_evaluate_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_extract_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_eval_and_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_process_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydev_monkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevcoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_safe_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_save_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    28398 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_smart_step_into_bytecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_suspended_frames_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_timeout_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_gotchas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_on_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/tests_single_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/deep_nest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/non_test_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/non_test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/non_test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/simple4_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/non_test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simpleClass_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simpleModule_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevd_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevdio.py
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_runfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/cython_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/functools_lru_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/finders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    53910 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/isort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/natural.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pie_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pylama_isort.py
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/
--rw-r--r--   0 runner    (1001) docker     (123)   155972 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/autopep8.py
--rw-r--r--   0 runner    (1001) docker     (123)    88598 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/pycodestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-01-23 14:08:00.000000 robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/tests_cython_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/__dev__main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/config_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/ep_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/ep_resolve_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/ext/jupyter_lsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/html_to_markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/_code_action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/_symbols_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    70031 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/ast_utils_keyword_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/auto_import_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_others.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_quickfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_refactoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/code_lens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/collect_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/collect_robot_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context_dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context_workspace_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/dictionary_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/doc_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)    19056 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/doctree2md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/document_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/filesystem_section_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/find_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/flow_explorer_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/folding_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/hover.py
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_argument_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_parameter_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/keywords_in_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/library_names_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)    51252 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_markdown_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_warmup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/on_type_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    29722 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/provide_evaluatable_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/references.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_html_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_markuputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_normalizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_generated_lsp_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_lsp_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28116 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_specbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29347 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/robot_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/section_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/section_name_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/selection_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    23373 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/semantic_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/signature_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/snippets_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/string_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/text_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/variable_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/variable_completions_from_py.py
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/variable_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/variable_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/variables_from_arguments_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/impl/workspace_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/ls_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/rf_interactive_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/robot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/robot_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/robotframework_ls_completion_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    56677 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/robotframework_ls_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/monaco_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    55539 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_api/server__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25790 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/server_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/code_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/command_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/copytree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__main__gen_debug_adapter_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_base_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)   690379 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/debug_adapter_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/document_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ep_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ep_resolve_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/scandir_vendored.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/easter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58796 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/isoparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/relativedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)    66556 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/rrule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    62857 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/tz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/win.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tzwin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/rebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/bccache.py
--rw-r--r--   0 runner    (1001) docker     (123)    72172 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    61349 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31502 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    53509 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/idtracking.py
--rw-r--r--   0 runner    (1001) docker     (123)    29726 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nativetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    34550 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39595 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    33476 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_native.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_speedups.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging-21.3.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging-21.3.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pathspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/gitwildmatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_gitwildmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_pathspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)   213310 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/
--rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39129 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/
--rw-r--r--   0 runner    (1001) docker     (123)    35132 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29644 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    28744 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34549 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_re.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)   112782 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    28355 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35805 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging-21.3.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging-21.3.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pathspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/gitwildmatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_gitwildmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_pathspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)   213310 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/
--rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39129 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_re.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28864 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-310-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)    28864 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-38-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)    59312 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-39-darwin.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    24290 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/kqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/read_directory_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/winapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/delayed_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/dirsnapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/process_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24646 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/watchmedo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-5.3.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-5.3.1.dist-info/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28627 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    43006 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25495 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/load_ignored_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33304 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/lsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24371 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/python_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robocop_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robotframework_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robotidy_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/run_and_save_pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/run_with_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/subprocess_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/system_mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/cases_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/language_server_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/uris.py
--rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/watchdog_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31096 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/yaml_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39344 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    37600 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/robot_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-01-23 14:09:26.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/xml_to_rfstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/ast_to_code.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/main_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/robot_interactive_console.robot
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/robotfacade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_generated_lsp_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_ls_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    91436 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-23 14:09:27.000000 robotframework-lsp-1.8.0/robotframework_lsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 14:09:28.000000 robotframework-lsp-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-01-23 14:07:56.000000 robotframework-lsp-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/ThirdPartyNotices.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/_ignore_failures_in_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/base_launch_process_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/debug_adapter_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48825 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/debugger_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/events_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30896 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process_pydevd_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process_robot_target_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/prerun_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24372 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/run_robot__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/safe_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/force_pydevd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/install_and_run_debug_py.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_calltip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_completer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_filesystem_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_getopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_imports_tipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17063 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_jy_imports_tipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_saved_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_tipper_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23769 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_console_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console_011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_is_thread_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_localhost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40160 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_umd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_pytest2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_xml_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23085 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)   763496 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevconsole_code_for_ironpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info_regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49872 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_breakpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_bytecode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_code_to_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36357 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_collect_bytecode_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74423 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_command_line_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_custom_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2006433 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    86683 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_daemon_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_exec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59424 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_gevent_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_json_debug_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55468 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_referrers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25500 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_safe_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_save_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_source_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_stackless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_suspended_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_thread_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22202 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch_regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_traceproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27603 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vm_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   926546 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.template.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_modify_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/release_mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22299 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/instr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49634 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_concrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_instr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32993 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_peephole_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/util_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/pydevd_fix_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_osx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/check_no_git_modifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/generate_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/names_to_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/rename_pep8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/gradlew.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/interpreterInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pycompletionserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_app_engine_debug_startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookglut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookpyglet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhooktk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookwx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/matplotlibtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_for_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_pysrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_run_in_console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142770 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_always_live_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/add_code_to_python_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_amd64.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22760 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_amd64.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21388 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_x86.so
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_pydevd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54736 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86_64.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_settrace.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_version.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/python.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/ref_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   259072 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_amd64.exe
+-rw-r--r--   0 runner    (1001) docker     (123)   203264 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_x86.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/attach.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/compile_linux.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/compile_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    14336 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168168 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65394 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58709 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24409 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67241 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83555 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70615 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183635 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23798 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45884 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62691 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/textio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75478 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36223 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120809 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/advapi32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25137 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_amd64.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_i386.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46705 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/dbghelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/gdi32.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164818 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/kernel32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22847 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159230 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/peb_teb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/psapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shell32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25807 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shlwapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57177 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/user32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36813 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24309 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)    27447 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/compile_windows.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/inject_dll.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/py_win_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_in_memory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/targetver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/django_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/jinja2_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/pydevd_line_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/runfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup_pydevd_cython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/_django_manager_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/test_pydevd_reload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_check_pydevconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_get_referrers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jyserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jysimpleTipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydev_ipython_011.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydevconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pyserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_simpleTipper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-glut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-pyglet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-tk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-wx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/check_debug_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debug_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55462 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_exttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/performance_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/regression_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resource_path_translation/other.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_big_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_constructs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_many_names_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_overflow_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case17a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case56.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case89.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_adjust_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_multiple_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_condition_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_breakpoint_remote_no_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_change_breaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_check_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_custom_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_custom_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deadlock_thread_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_debug_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deep_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dir_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dont_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_dont_trace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_event_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_frame_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_generator_step_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_get_next_statement_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_get_thread_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop_qt5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_hasattr_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_hit_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_ignore_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_import_imported.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_import_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_lambda_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_lamda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_large_exception_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_linecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_linecache_existing_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_listen_dap_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_m_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_m_switch_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_method_single_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_module_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multi_threads_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiple_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_stopped_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_no_subprocess_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_odict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_path_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pause_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pydevd_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_python_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_quoting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_raise_with_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remove_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_return_value_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_scapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_set_next_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_settrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_show_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_simple_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_skip_breakpoint_in_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_smart_step_into3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_map_goto_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_and_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_jmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_stop_async_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_subprocess_and_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_sysexit_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_creation_deadlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_started_exited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trace_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_type_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exception_get_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_listcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_on_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_on_top_level2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_just_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_user_unhandled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_user_unhandled2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_variables_with_same_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_yield_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_zip_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_cyrillic_encoding_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_cyrillic_encoding_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydev_coverage_syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydevd_test_find_main_thread_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch/foo/bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/launch_py2/foo/bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled_no_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_double_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception_on_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_exception_user_unhandled.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_on_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/not_my_coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/other_noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/_debugger_case_wrong_bytecode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_additional_thread_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_bytecode_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_code_obj_to_source_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_collect_bytecode_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23705 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_convert_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173317 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236370 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_dump_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_evaluate_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_extract_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_eval_and_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_process_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydev_monkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_safe_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_save_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28398 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_smart_step_into_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_suspended_frames_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_timeout_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_gotchas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_on_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/tests_single_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/deep_nest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested2/non_test_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/nested3/non_test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/non_test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/nested_dir/simple4_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/non_test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simpleClass_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simpleModule_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevd_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_runfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/cython_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/functools_lru_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53910 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/isort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/natural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pie_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pylama_isort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/
+-rw-r--r--   0 runner    (1001) docker     (123)   155972 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/autopep8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88598 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/pycodestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-02-03 17:22:24.000000 robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/tests_cython_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/__dev__main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/config_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/ep_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/ep_resolve_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/ext/jupyter_lsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/html_to_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/_code_action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/_symbols_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71366 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/ast_utils_keyword_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/auto_import_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_others.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_quickfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_refactoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36231 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/code_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18131 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/collect_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/collect_robot_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context_dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context_workspace_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/dictionary_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/doc_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19056 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/doctree2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/document_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/filesystem_section_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/find_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20888 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/flow_explorer_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/folding_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_argument_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_parameter_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/keywords_in_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/library_names_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53734 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_markdown_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_warmup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/on_type_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/provide_evaluatable_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_html_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_markuputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_normalizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_generated_lsp_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_lsp_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_specbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29347 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/robot_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/section_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/section_name_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/selection_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23373 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/semantic_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/signature_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/snippets_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/string_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/text_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/variable_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/variable_completions_from_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/variable_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/variable_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/variables_from_arguments_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/impl/workspace_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/ls_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/rf_interactive_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/robot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/robot_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/robotframework_ls_completion_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56847 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/robotframework_ls_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/monaco_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55890 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_api/server__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25790 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/server_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/code_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/command_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/copytree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__main__gen_debug_adapter_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_base_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)   690379 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/debug_adapter_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/document_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ep_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ep_resolve_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/scandir_vendored.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/easter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58796 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/isoparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/relativedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66556 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62857 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/win.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tzwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/bccache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72172 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61349 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31502 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53509 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/idtracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29726 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nativetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34550 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39595 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33476 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_speedups.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging-21.3.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging-21.3.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pathspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/gitwildmatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_gitwildmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_pathspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213310 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39129 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/
+-rw-r--r--   0 runner    (1001) docker     (123)    35132 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29644 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28744 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34549 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112782 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16350 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28355 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35805 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30110 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging-21.3.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging-21.3.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pathspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/gitwildmatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15160 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_gitwildmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_pathspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213310 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39129 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28864 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-310-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28864 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-38-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59312 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-39-darwin.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24290 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/kqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/read_directory_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/winapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/delayed_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/dirsnapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/process_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24646 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/watchmedo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-6.0.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-6.0.dist-info/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/_yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43006 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25495 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51279 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/load_ignored_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/lsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24371 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/python_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robocop_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robotframework_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robotidy_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/run_and_save_pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/run_with_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/subprocess_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/system_mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/cases_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/language_server_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/watchdog_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31096 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/yaml_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39344 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37600 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/robot_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-02-03 17:23:35.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/xml_to_rfstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/ast_to_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/robot_interactive_console.robot
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/robot_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/robotfacade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_generated_lsp_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_ls_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    91581 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/robotframework_lsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 17:23:36.000000 robotframework-lsp-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-02-03 17:22:20.000000 robotframework-lsp-1.9.0/setup.py
```

### Comparing `robotframework-lsp-1.8.0/COPYRIGHT` & `robotframework-lsp-1.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/LICENSE` & `robotframework-lsp-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/PKG-INFO` & `robotframework-lsp-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-lsp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Language Server Protocol implementation for Robot Framework
 Home-page: https://github.com/robocorp/robotframework-lsp
 Author: Fabio Zadrozny
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,27 +49,27 @@
 
 ## Configuration
 
 After having `Robot Framework Language Server` installed, some configurations (such as specifying
 the python executable used for launching the Language Server or Robot Framework)
 may be needed.
 
-See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/config.md) for details.
+See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/config.md) for details.
 
-See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
+See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
 
 ## Contributing
 
-See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
+See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
 
 ## Reporting Issues
 
-See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
+See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
 
-## Features (1.8.0)
+## Features (1.9.0)
 
 -   Robot Output View:
     -   View current task/test being executed.
     -   Shows Keyword being executed in real time.
 -   Robot Documentation View:
     -   Select a library import for the full library documentation.
     -   Select another element for its docstring.
@@ -92,14 +92,15 @@
     -   Extract variable to variables section.
 -   Quick fixes (VSCode: `Ctrl + .`):
     -   Add import for unresolved keyword.
     -   Create local variable for unresolved variable.
     -   Create argument for unresolved variable.
     -   Creat variable in variables section for unresolved variable.
     -   Assign keyword to variable.
+    -   Surround with Try..Except.
 -   Symbols browser for keywords in workspace (VSCode: `Ctrl + T`).
 -   Document symbols (VSCode: `Ctrl + Shift + O`).
 -   Highlight of keywords and variables.
 -   Syntax highlighting (using `semanticTokens`).
 -   Syntax validation.
 -   Signature Help (VSCode: `Ctrl + Shift + Space`).
 -   Code Formatting (see: [Editor Settings](https://code.visualstudio.com/docs/getstarted/settings#_language-specific-editor-settings) for details on how to toggle code formatting just for `robotframework`).
@@ -113,10 +114,10 @@
     -   Pause at breakpoints to inspect the stack and see variables
     -   Breakpoint condition/hitCondition/logMessage
     -   Step in
     -   Step over
     -   Step return
     -   Continue
 
-See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/changelog.md) for details.
+See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/changelog.md) for details.
 
 ## License: Apache 2.0
```

### Comparing `robotframework-lsp-1.8.0/README.md` & `robotframework-lsp-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 ## Configuration
 
 After having `Robot Framework Language Server` installed, some configurations (such as specifying
 the python executable used for launching the Language Server or Robot Framework)
 may be needed.
 
-See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/config.md) for details.
+See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/config.md) for details.
 
-See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
+See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
 
 ## Contributing
 
-See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
+See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
 
 ## Reporting Issues
 
-See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
+See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
 
-## Features (1.8.0)
+## Features (1.9.0)
 
 -   Robot Output View:
     -   View current task/test being executed.
     -   Shows Keyword being executed in real time.
 -   Robot Documentation View:
     -   Select a library import for the full library documentation.
     -   Select another element for its docstring.
@@ -61,14 +61,15 @@
     -   Extract variable to variables section.
 -   Quick fixes (VSCode: `Ctrl + .`):
     -   Add import for unresolved keyword.
     -   Create local variable for unresolved variable.
     -   Create argument for unresolved variable.
     -   Creat variable in variables section for unresolved variable.
     -   Assign keyword to variable.
+    -   Surround with Try..Except.
 -   Symbols browser for keywords in workspace (VSCode: `Ctrl + T`).
 -   Document symbols (VSCode: `Ctrl + Shift + O`).
 -   Highlight of keywords and variables.
 -   Syntax highlighting (using `semanticTokens`).
 -   Syntax validation.
 -   Signature Help (VSCode: `Ctrl + Shift + Space`).
 -   Code Formatting (see: [Editor Settings](https://code.visualstudio.com/docs/getstarted/settings#_language-specific-editor-settings) for details on how to toggle code formatting just for `robotframework`).
@@ -82,10 +83,10 @@
     -   Pause at breakpoints to inspect the stack and see variables
     -   Breakpoint condition/hitCondition/logMessage
     -   Step in
     -   Step over
     -   Step return
     -   Continue
 
-See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/changelog.md) for details.
+See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/changelog.md) for details.
 
 ## License: Apache 2.0
```

### Comparing `robotframework-lsp-1.8.0/ThirdPartyNotices.txt` & `robotframework-lsp-1.9.0/ThirdPartyNotices.txt`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/__main__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/_ignore_failures_in_stack.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/_ignore_failures_in_stack.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/base_launch_process_target.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/base_launch_process_target.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/constants.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/debug_adapter_comm.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/debug_adapter_comm.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/debugger_impl.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/debugger_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/events_listener.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/events_listener.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/file_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/file_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process_pydevd_comm.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process_pydevd_comm.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/launch_process_robot_target_comm.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/launch_process_robot_target_comm.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/listeners.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/listeners.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/prerun_modifiers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/prerun_modifiers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/protocols.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/protocols.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/run_robot__main__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/run_robot__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/safe_repr.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/safe_repr.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/force_pydevd.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/force_pydevd.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/install_and_run_debug_py.sh` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/.github/install_and_run_debug_py.sh`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/LICENSE` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_calltip_util.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_calltip_util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_completer.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_completer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_execfile.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_execfile.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_filesystem_encoding.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_filesystem_encoding.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_getopt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_getopt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_imports_tipper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_imports_tipper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_jy_imports_tipper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_jy_imports_tipper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_log.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_log.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_saved_modules.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_saved_modules.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_sys_patch.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_sys_patch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_tipper_common.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/_pydev_tipper_common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/fsnotify/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_console_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_console_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_import_hook.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_import_hook.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console_011.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_ipython_console_011.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_is_thread_alive.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_is_thread_alive.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_localhost.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_localhost.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_log.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_log.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey_qt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_monkey_qt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_override.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_override.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_umd.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_bundle/pydev_umd.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_coverage.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_coverage.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_nose.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_nose.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel_client.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_parallel_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_pytest2.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_pytest2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_unittest.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_unittest.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_xml_rpc.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydev_runfiles/pydev_runfiles_xml_rpc.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevconsole_code_for_ironpython.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevconsole_code_for_ironpython.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info_regular.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_additional_thread_info_regular.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_api.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_breakpoints.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_breakpoints.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_bytecode_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_bytecode_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_code_to_source.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_code_to_source.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_collect_bytecode_info.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_collect_bytecode_info.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm_constants.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_comm_constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_command_line_handling.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_command_line_handling.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_console.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_console.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_constants.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_custom_frames.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_custom_frames.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.c` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.c`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pxd` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pxd`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pyx` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython.pyx`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_cython_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_daemon_thread.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_daemon_thread.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace_files.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_dont_trace_files.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_api.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_extension_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_filtering.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_filtering.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_frame_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_gevent_integration.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_gevent_integration.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_import_class.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_import_class.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_io.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_io.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_json_debug_options.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_json_debug_options.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_json.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_json.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_xml.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_net_command_factory_xml.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_plugin_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command_json.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_process_net_command_json.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_referrers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_referrers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_reload.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_reload.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_resolver.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_resolver.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_safe_repr.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_safe_repr.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_save_locals.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_save_locals.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_signature.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_signature.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_source_mapping.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_source_mapping.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_stackless.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_stackless.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_suspended_frames.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_suspended_frames.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_thread_lifecycle.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_thread_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_timeout.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_timeout.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_api.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch_regular.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_trace_dispatch_regular.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_traceproperty.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_traceproperty.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vars.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vars.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vm_type.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_vm_type.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_xml.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_bundle/pydevd_xml.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_main.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_eval_main.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.pxd` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.pxd`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.template.pyx` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.template.pyx`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_tracing.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_frame_tracing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_modify_bytecode.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/pydevd_modify_bytecode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/bytecode.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/bytecode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/cfg.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/cfg.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/concrete.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/concrete.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/flags.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/flags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/instr.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/instr.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_bytecode.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_cfg.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_code.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_concrete.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_concrete.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_flags.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_instr.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_instr.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_misc.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_peephole_opt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/bytecode/tests/test_peephole_opt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/pydevd_fix_code.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/_pydevd_frame_eval/vendored/pydevd_fix_code.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_osx.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_osx.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_windows.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/build_binaries_windows.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/check_no_git_modifications.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/check_no_git_modifications.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/generate_code.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/generate_code.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/names_to_rename.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/names_to_rename.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/rename_pep8.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/build_tools/rename_pep8.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/conftest.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/conftest.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/gradlew.bat` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/gradlew.bat`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/interpreterInfo.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/interpreterInfo.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pycompletionserver.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pycompletionserver.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_app_engine_debug_startup.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_app_engine_debug_startup.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_coverage.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_coverage.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhook.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhook.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookglut.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookglut.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk3.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookgtk3.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookpyglet.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookpyglet.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt4.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt4.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt5.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookqt5.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhooktk.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhooktk.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookwx.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/inputhookwx.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/matplotlibtools.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/matplotlibtools.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_for_kernel.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_for_kernel.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_loaders.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/qt_loaders.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/version.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_ipython/version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_run_in_console.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_run_in_console.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/sitecustomize.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydev_sitecustomize/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevconsole.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevconsole.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_always_live_program.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_always_live_program.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process_linux.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/_test_attach_to_process_linux.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/add_code_to_python_process.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/add_code_to_python_process.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_amd64.dll` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_amd64.dll`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_amd64.so` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_amd64.so`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_x86.so` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_linux_x86.so`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_pydevd.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_pydevd.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_script.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_script.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86.dll` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86.dll`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86_64.dylib` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/attach_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_settrace.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_settrace.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_utils.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_utils.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_version.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/py_version.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/python.h` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/python.h`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/ref_utils.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/common/ref_utils.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_amd64.exe` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_amd64.exe`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_x86.exe` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/inject_dll_x86.exe`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/attach.cpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/attach.cpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_x86.dll` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/run_code_on_dllmain_x86.dll`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/breakpoint.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/breakpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/compat.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/compat.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/crash.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/crash.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/debug.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/disasm.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/disasm.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/event.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/event.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/interactive.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/interactive.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/module.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/module.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/process.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/process.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/registry.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/registry.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/search.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/search.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/sql.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/sql.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/system.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/system.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/textio.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/textio.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/thread.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/thread.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/util.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/advapi32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/advapi32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_amd64.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_amd64.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_i386.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/context_i386.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/dbghelp.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/dbghelp.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/defines.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/defines.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/gdi32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/gdi32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/kernel32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/kernel32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/ntdll.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/ntdll.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/peb_teb.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/peb_teb.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/psapi.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/psapi.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shell32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shell32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shlwapi.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/shlwapi.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/user32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/user32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/version.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/window.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/winappdbg/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.cpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.cpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.h` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/attach.h`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/compile_windows.bat` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/compile_windows.bat`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/inject_dll.cpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/inject_dll.cpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/py_win_helpers.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/py_win_helpers.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_in_memory.hpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_in_memory.hpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.cpp` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.cpp`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.h` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/stdafx.h`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/targetver.h` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_attach_to_process/windows/targetver.h`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_file_utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_file_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/django_debug.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/django_debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/README.md` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_helpers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_helpers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/jinja2_debug.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/jinja2_debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/pydevd_line_validation.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_plugins/pydevd_line_validation.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_tracing.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/pydevd_tracing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/runfiles.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/runfiles.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup_pydevd_cython.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/setup_pydevd_cython.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/_django_manager_body.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/stubs/_django_manager_body.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/test_pydevd_reload.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/test_pydevd_reload/test_pydevd_reload.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_check_pydevconsole.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_check_pydevconsole.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_get_referrers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_get_referrers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jyserver.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jyserver.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jysimpleTipper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_jysimpleTipper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydev_ipython_011.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydev_ipython_011.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydevconsole.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pydevconsole.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pyserver.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_pyserver.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_simpleTipper.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests/test_simpleTipper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-glut.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-glut.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk3.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-gtk3.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-pyglet.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-pyglet.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-qt.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-qt.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-tk.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-tk.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-wx.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_mainloop/gui-wx.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/check_debug_python.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/check_debug_python.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debug_constants.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debug_constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_fixtures.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_fixtures.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_unittest.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/debugger_unittest.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/app.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/flask1/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/views.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_app/views.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/settings.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_17/my_django_proj_17/settings.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/manage.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/manage.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/tests.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/tests.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/urls.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/urls.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/views.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_app/views.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/settings.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/settings.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/urls.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_django_proj_21/my_django_proj_21/urls.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_events.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_events.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_exttype.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/my_extensions/pydevd_plugins/extensions/pydevd_plugin_test_exttype.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/performance_check.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/performance_check.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/regression_check.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/regression_check.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_big_method.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_big_method.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_constructs.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_constructs.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_many_names_example.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_many_names_example.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_overflow_example.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_bytecode_overflow_example.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case1.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case1.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case13.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case13.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case14.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case14.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case15.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case20.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case20.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_asyncio.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_asyncio.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_multiple_threads.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_multiple_threads.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_simple.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_attach_to_pid_simple.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_check_tracer.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_check_tracer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deadlock_thread_eval.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_deadlock_thread_eval.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_frame_eval.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_frame_eval.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gevent.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop_qt5.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_gui_event_loop_qt5.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_listen_dap_messages.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_listen_dap_messages.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables3.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_local_variables3.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multi_threads_stepping.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multi_threads_stepping.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiple_threads.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiple_threads.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_stopped_threads.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_multiprocessing_stopped_threads.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_no_subprocess_patching.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_no_subprocess_patching.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pydevd_customization.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_pydevd_customization.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_python_c.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_python_c.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread1.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread1.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread2.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread3.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread3.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread4.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_qthread4.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_redirect.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_redirect.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_1.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_1.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_threads.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_threads.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions2.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_remote_unhandled_exceptions2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_settrace.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_settrace.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_map_goto_target.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_map_goto_target.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_and_reference.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_and_reference.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_jmc.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_mapping_jmc.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_reference.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_source_reference.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_subprocess_and_fork.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_subprocess_and_fork.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_all.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_all.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_policy.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_suspend_policy.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_terminate.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_terminate.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_creation_deadlock.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_thread_creation_deadlock.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trio.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_trio.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_custom.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_unhandled_exceptions_custom.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach_impl.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_debugger_case_wait_for_attach_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_1.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_1.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_2.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_performance_2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydevd_test_find_main_thread_id.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/_pydevd_test_find_main_thread_id.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled_no_stop.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/my_code/my_code_coroutine_user_unhandled_no_stop.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry2.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/not_my_code/main_on_entry2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/_debugger_case_wrong_bytecode.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/_debugger_case_wrong_bytecode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/resources/wrong_bytecode/helper/helper/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_additional_thread_info.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_additional_thread_info.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_bytecode_manipulation.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_bytecode_manipulation.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_code_obj_to_source_code.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_code_obj_to_source_code.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_collect_bytecode_info.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_collect_bytecode_info.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_console.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_console.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_convert_utilities.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_convert_utilities.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger_json.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_debugger_json.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_evaluate_expression.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_evaluate_expression.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_extract_token.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_extract_token.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_fixtures.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_eval_and_tracing.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_eval_and_tracing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_evaluator.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_frame_evaluator.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_process_command_line.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_process_command_line.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydev_monkey.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydev_monkey.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevcoverage.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevcoverage.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_filtering.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_filtering.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_io.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_pydevd_io.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_resolvers.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_run.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_run.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_safe_repr.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_safe_repr.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_save_locals.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_save_locals.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_schema.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_schema.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_smart_step_into_bytecode.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_smart_step_into_bytecode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_suspended_frames_manager.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_suspended_frames_manager.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_timeout_tracker.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_timeout_tracker.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_gotchas.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_gotchas.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_on_top_level.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_tracing_on_top_level.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_utilities.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/test_utilities.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/tests_single_notification.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_python/tests_single_notification.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple_test.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/samples/simple_test.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevd_property.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevd_property.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevdio.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_pydevdio.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_runfiles.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/tests_runfiles/test_runfiles.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/cython_json.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/cython_json.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/functools_lru_cache.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/backports/functools_lru_cache.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__init__.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/finders.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/finders.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/hooks.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/hooks.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/isort.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/isort.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/main.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/main.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/natural.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/natural.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pie_slice.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pie_slice.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pylama_isort.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/pylama_isort.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/settings.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/settings.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/utils.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/isort_container/isort/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/autopep8.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/autopep8.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/pycodestyle.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/pep8/pycodestyle.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/tests_cython_json.py` & `robotframework-lsp-1.9.0/robotframework_debug_adapter/vendored/vendored_pydevd/third_party/tests_cython_json.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/__dev__main.py` & `robotframework-lsp-1.9.0/robotframework_ls/__dev__main.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 import os.path
 import sys
 
 __file__ = os.path.abspath(__file__)
 if __file__.endswith((".pyc", ".pyo")):
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/__main__.py` & `robotframework-lsp-1.9.0/robotframework_ls/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/commands.py` & `robotframework-lsp-1.9.0/robotframework_ls/commands.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/config_extension.py` & `robotframework-lsp-1.9.0/robotframework_ls/config_extension.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/ext/jupyter_lsp.py` & `robotframework-lsp-1.9.0/robotframework_ls/ext/jupyter_lsp.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/html_to_markdown.py` & `robotframework-lsp-1.9.0/robotframework_ls/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/_code_action_utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/_code_action_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/_symbols_cache.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/_symbols_cache.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/ast_utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/ast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,28 +314,28 @@
 
         if len(errors) >= MAX_ERRORS:
             break
 
     return errors
 
 
-def create_error_from_node(node, msg, tokens=None) -> Error:
+def create_error_from_node(node, msg, tokens=None, **kwargs) -> Error:
     if tokens is None:
         tokens = node.tokens
 
     if not tokens:
         log.info("No tokens found when visiting: %s.", node.__class__)
         start = (0, 0)
         end = (0, 0)
     else:
         # line is 1-based and col is 0-based (make both 0-based for the error).
         start = (tokens[0].lineno - 1, tokens[0].col_offset)
         end = (tokens[-1].lineno - 1, tokens[-1].end_col_offset)
 
-    error = Error(msg, start, end)
+    error = Error(msg, start, end, **kwargs)
     return error
 
 
 def print_ast(node, stream=None):
     if stream is None:
         stream = sys.stderr
     errors_visitor = _PrinterVisitor(stream)
@@ -625,18 +625,15 @@
     token_info = find_token(section, line, col)
     if token_info is not None:
         stack = token_info.stack
         node = token_info.node
         token = token_info.token
 
         try:
-            if (
-                token.type == token.ARGUMENT
-                and node.__class__.__name__ in CLASSES_WTH_EXPRESSION_ARGUMENTS
-            ):
+            if token.type == token.ARGUMENT and is_node_with_expression_argument(node):
                 for part, var_info in iter_expression_variables(token):
                     if part.type == token.VARIABLE:
                         if part.col_offset <= col <= part.end_col_offset:
                             return VarTokenInfo(
                                 stack,
                                 node,
                                 part,
@@ -1224,14 +1221,15 @@
         "KeywordCall",
         "LibraryImport",
         "ResourceImport",
         "TestTimeout",
         "Variable",
         "ForHeader",  # RF 4+
         "ForLoopHeader",  # RF 3
+        "ReturnStatement",  # RF 5
     ) + _FIXTURE_CLASS_NAMES:
         for node_info in ast.iter_indexed(clsname):
             stack = node_info.stack
             node = node_info.node
             token = None
             arg_i = 0
             for token in node.tokens:
@@ -1438,56 +1436,87 @@
                 if _same_line_col(keyword_usage.token, token):
                     return token
             else:
                 return keyword_usage.token
     return None
 
 
-def get_library_import_name_token(node, token: IRobotToken) -> Optional[IRobotToken]:
+def get_library_import_name_token(
+    node, token: IRobotToken, generate_empty_on_eol=False
+) -> Optional[IRobotToken]:
     """
     If the given ast node is a library import and the token is its name, return
     the name token, otherwise, return None.
     """
-
     if (
         token.type == token.NAME
         and isinstance_name(node, "LibraryImport")
         and node.name == token.value  # I.e.: match the name, not the alias.
     ):
         return token
+
+    if generate_empty_on_eol:
+        if token.type == token.EOL and isinstance_name(node, "LibraryImport"):
+            if len(node.tokens) == 2:
+                # i.e.: just `Library   EOL`
+                return create_empty_token_name_at_eol(token)
     return None
 
 
-def get_resource_import_name_token(node, token: IRobotToken) -> Optional[IRobotToken]:
+def create_empty_token_name_at_eol(token):
+    # i.e.: just `Library   EOL`
+    l = len(token.value)
+    if token.value.endswith("\r\n"):
+        l -= 2
+    elif token.value.endswith("\r") or token.value.endswith("\n"):
+        l -= 1
+    return copy_token_with_subpart(token, l, l, token.NAME)
+
+
+def get_resource_import_name_token(
+    node, token: IRobotToken, generate_empty_on_eol=False
+) -> Optional[IRobotToken]:
     """
     If the given ast node is a library import and the token is its name, return
     the name token, otherwise, return None.
     """
 
     if (
         token.type == token.NAME
         and isinstance_name(node, "ResourceImport")
         and node.name == token.value  # I.e.: match the name, not the alias.
     ):
         return token
+
+    if generate_empty_on_eol:
+        if token.type == token.EOL and isinstance_name(node, "ResourceImport"):
+            if len(node.tokens) == 2:
+                # i.e.: just `Library   EOL`
+                return create_empty_token_name_at_eol(token)
     return None
 
 
-def get_variables_import_name_token(ast, token):
+def get_variables_import_name_token(node, token, generate_empty_on_eol=False):
     """
     If the given ast node is a variables import and the token is its name, return
     the name token, otherwise, return None.
     """
 
     if (
         token.type == token.NAME
-        and isinstance_name(ast, "VariablesImport")
-        and ast.name == token.value  # I.e.: match the name, not the alias.
+        and isinstance_name(node, "VariablesImport")
+        and node.name == token.value  # I.e.: match the name, not the alias.
     ):
         return token
+
+    if generate_empty_on_eol:
+        if token.type == token.EOL and isinstance_name(node, "VariablesImport"):
+            if len(node.tokens) == 2:
+                # i.e.: just `Library   EOL`
+                return create_empty_token_name_at_eol(token)
     return None
 
 
 def _copy_of_node_replacing_token(node, token, token_type):
     """
     Workaround to create a new version of the same node but with the first
     occurrence of a token of the given type changed to another token.
@@ -1581,26 +1610,33 @@
         "col_offset": token.col_offset,
         "error": token.error,
     }
     new_kwargs.update(kwargs)
     return Token(**new_kwargs)
 
 
-def copy_token_with_subpart(token, start, end):
+def copy_token_with_subpart(token, start, end, token_type=None):
     from robot.api import Token
 
+    if token_type is None:
+        token_type = token.type
+
     return Token(
-        type=token.type,
+        type=token_type,
         value=token.value[start:end],
         lineno=token.lineno,
         col_offset=token.col_offset + start,
         error=token.error,
     )
 
 
+def copy_token_with_subpart_up_to_col(token, column):
+    return copy_token_with_subpart(token, 0, column)
+
+
 def create_range_from_token(token: IRobotToken) -> RangeTypedDict:
     start: PositionTypedDict = {"line": token.lineno - 1, "character": token.col_offset}
     end: PositionTypedDict = {
         "line": token.lineno - 1,
         "character": token.end_col_offset,
     }
     taken_range: RangeTypedDict = {"start": start, "end": end}
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/ast_utils_keyword_usage.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/ast_utils_keyword_usage.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/auto_import_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/auto_import_completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,18 +176,22 @@
             "data": data,
         }
         self.completion_items.append(completion_item)
         return completion_item
 
 
 def _collect_auto_import_completions(
-    completion_context: ICompletionContext, collector: _Collector
+    completion_context: ICompletionContext,
+    collector: _Collector,
+    collect_deprecated: bool = False,
 ):
     from robotframework_ls.impl.workspace_symbols import iter_symbols_caches
     from robotframework_ls.robot_config import create_convert_keyword_format_func
+    from robotframework_ls import robot_config
+    from robotframework_ls.impl.text_utilities import has_deprecated_text
 
     symbols_cache: ISymbolsCache
     selection = completion_context.sel
     token = collector.token
 
     ws: IWorkspace = completion_context.workspace
     folder_paths = []
@@ -199,24 +203,36 @@
     memo: Set[str] = set()
 
     default_convert_keyword_format = create_convert_keyword_format_func(
         completion_context.config
     )
     noop = lambda x: x
 
+    deprecated_name_to_replacement = (
+        robot_config.get_robot_libraries_deprecated_name_to_replacement(
+            completion_context.config
+        )
+    )
+
     for symbols_cache in iter_symbols_caches(
         None, completion_context, show_builtins=False
     ):
         library_info: Optional[ILibraryDoc] = symbols_cache.get_library_info()
         doc: Optional[IRobotDocument] = symbols_cache.get_doc()
 
         lib_import = None
         resource_path = None
 
         if library_info is not None:
+            if not collect_deprecated and (
+                library_info.name in deprecated_name_to_replacement
+                or has_deprecated_text(library_info.doc)
+            ):
+                continue
+
             if library_info.source:
                 if (
                     library_info.source
                     in collector.import_location_info.imported_libraries
                 ):
                     continue
             elif library_info.name in collector.import_location_info.imported_libraries:
@@ -391,11 +407,13 @@
                 token,
                 import_location_info,
                 imported_keyword_name_to_keyword,
                 exact_match=exact_match,
                 add_import=add_import,
                 prefix_module=prefix_module,
             )
-            _collect_auto_import_completions(completion_context, collector)
+            _collect_auto_import_completions(
+                completion_context, collector, collect_deprecated=False
+            )
 
             return collector.completion_items
     return []
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_action.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_action.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     context: TextDocumentContextTypedDict,
 ) -> List[CodeActionTypedDict]:
 
     from robotframework_ls.impl.code_action_refactoring import (
         code_action_refactoring,
     )
     from robotframework_ls.impl.code_action_quickfix import code_action_quickfix
-    from robotframework_ls.impl.code_action_others import code_action_others
+    from robotframework_ls.impl.code_action_others import (
+        code_action_others,
+        code_action_surround_with,
+    )
 
     # See:
     # codeActionProvider.codeActionKinds
     # at:
     # robotframework_ls.robotframework_ls_impl.RobotFrameworkLanguageServer.capabilities
     # to see what may be included in 'only'
 
@@ -38,8 +41,9 @@
             for diagnostic in diagnostics:
                 data: Optional[ICustomDiagnosticDataTypedDict] = diagnostic.get("data")
                 if data is not None:
                     found_data.append(data)
         ret.extend(code_action_quickfix(completion_context, found_data))
 
     ret.extend(code_action_others(completion_context, select_range, only))
+    ret.extend(code_action_surround_with(completion_context, select_range, only))
     return ret
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_common.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_others.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/provide_evaluatable_expression.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,50 @@
-from typing import Set, Iterable, List
+from typing import Optional
 
-from robocorp_ls_core.lsp import Range, CodeActionTypedDict, TextEditTypedDict
-from robotframework_ls.impl.protocols import ICompletionContext, IRobotToken
-from robotframework_ls.impl._code_action_utils import wrap_edits_in_snippet
+from robocorp_ls_core.protocols import EvaluatableExpressionTypedDict
+from robotframework_ls.impl.protocols import (
+    ICompletionContext,
+    IRobotToken,
+)
+
+
+def _create_evaluatable_expression_from_token(
+    token: IRobotToken, expression: str
+) -> EvaluatableExpressionTypedDict:
+    return {
+        "range": {
+            "start": {"line": token.lineno - 1, "character": token.col_offset},
+            "end": {
+                "line": token.lineno - 1,
+                "character": token.end_col_offset,
+            },
+        },
+        "expression": expression,
+    }
 
 
-def code_action_others(
+def provide_evaluatable_expression(
     completion_context: ICompletionContext,
-    select_range: Range,
-    only: Set[str],
-) -> Iterable[CodeActionTypedDict]:
-    from robocorp_ls_core.basic import isinstance_name
-
-    if only and "assign.toVar" not in only:
-        return
-
-    if select_range.start != select_range.end:
-        # This one is only done when no range is given.
-        return
+) -> Optional[EvaluatableExpressionTypedDict]:
+    from robotframework_ls.impl import ast_utils
 
-    token_info = completion_context.get_current_token()
-    if not token_info:
-        return
+    var_token_info = completion_context.get_current_variable()
+    if var_token_info is not None:
+        token = var_token_info.token
+        var_identifier = var_token_info.var_info.var_identifier
+        if not var_identifier:
+            var_identifier = "$"
+        return _create_evaluatable_expression_from_token(
+            token, var_identifier + "{" + token.value + "}"
+        )
 
-    if not isinstance_name(token_info.node, "KeywordCall"):
-        return
+    token_info = completion_context.get_current_token()
+    if token_info is not None:
+        keyword_name_token = ast_utils.get_keyword_name_token(
+            token_info.stack, token_info.node, token_info.token
+        )
+        if keyword_name_token is not None:
+            return _create_evaluatable_expression_from_token(
+                keyword_name_token, keyword_name_token.value
+            )
 
-    for keyword_token in token_info.node.tokens:
-        if keyword_token.type == keyword_token.ASSIGN:
-            return
-
-        if keyword_token.type == keyword_token.KEYWORD:
-            # Leave keyword_token in the namespace.
-            break
-    else:
-        return
-
-    from robotframework_ls.robot_config import get_arguments_separator
-
-    sep = get_arguments_separator(completion_context)
-    tok: IRobotToken = keyword_token
-
-    text_edits: List[TextEditTypedDict] = [
-        {
-            "range": {
-                "start": {"line": tok.lineno - 1, "character": tok.col_offset},
-                "end": {"line": tok.lineno - 1, "character": tok.col_offset},
-            },
-            "newText": "${${0:variable}}=%s" % (sep,),
-        }
-    ]
-    yield wrap_edits_in_snippet(
-        completion_context, "Assign to variable", text_edits, "assign.toVar"
-    )
+    return None
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_quickfix.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_quickfix.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_action_refactoring.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_action_refactoring.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_analysis.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,16 @@
     config = initial_completion_context.config
 
     def on_resolved_library(
         completion_context: ICompletionContext,
         library_node: Optional[INode],
         library_doc: ILibraryDoc,
     ):
+        from robotframework_ls.impl.text_utilities import has_deprecated_text
+
         if library_node is None:
             return
 
         from robotframework_ls.impl.robot_lsp_constants import (
             OPTION_ROBOT_LINT_KEYWORD_CALL_ARGUMENTS,
         )
 
@@ -270,14 +272,25 @@
         name_token = library_node.get_token(Token.NAME)
         if name_token is not None:
             for error in keyword_argument_analysis.collect_keyword_usage_errors(
                 UsageInfoForKeywordArgumentAnalysis(library_node, name_token)
             ):
                 errors.append(error)
 
+            if library_doc.doc and has_deprecated_text(library_doc.doc):
+                error = create_error_from_node(
+                    library_node,
+                    f"{library_doc.name} is deprecated.",
+                    tokens=[name_token],
+                )
+                error.severity = DiagnosticSeverity.Hint
+                error.tags = [DiagnosticTag.Deprecated]
+
+                errors.append(error)
+
     def on_unresolved_library(
         completion_context: ICompletionContext,
         library_name: str,
         lineno: int,
         end_lineno: int,
         col_offset: int,
         end_col_offset: int,
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/code_lens.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/collect_keywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/collect_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,35 +153,37 @@
     def __typecheckself__(self) -> None:
         _: IKeywordFound = check_implements(self)
 
 
 class _KeywordFoundFromLibrary(object):
 
     __slots__ = [
+        "_lib_deprecated",
         "_library_doc",
         "_library_alias",
         "_keyword_doc",
         "_keyword_name",
         "_keyword_args",
         "completion_context",
         "completion_item_kind",
         "__instance_cache__",
     ]
 
     def __init__(
         self,
+        lib_deprecated,
         library_doc,
         keyword_doc,
         keyword_name,
         keyword_args: Sequence[IKeywordArg],
         completion_context,
         completion_item_kind,
         library_alias=None,
     ):
-
+        self._lib_deprecated = lib_deprecated
         self._library_doc = library_doc
         self._keyword_doc = keyword_doc
         self._keyword_name = keyword_name
         self._keyword_args = keyword_args
 
         self.completion_context = completion_context
         self.completion_item_kind = completion_item_kind
@@ -209,14 +211,16 @@
 
     @property
     def resource_name(self):
         return None
 
     @instance_cache
     def is_deprecated(self):
+        if self._lib_deprecated:
+            return self._lib_deprecated
         from robotframework_ls.impl import text_utilities
 
         return text_utilities.has_deprecated_text(self._keyword_doc.doc)
 
     @property  # type: ignore
     @instance_cache
     def source(self):
@@ -329,14 +333,15 @@
     completion_context: ICompletionContext,
     library_infos: Iterator[LibraryDependencyInfo],
     collector: IKeywordCollector,
     memo: Dict[Any, Any],
 ):
     from robotframework_ls.impl.libspec_manager import LibspecManager
     from robotframework_ls.impl.protocols import ILibraryDocOrError
+    from robotframework_ls.impl import text_utilities
 
     # Get keywords from libraries
     from robocorp_ls_core.lsp import CompletionItemKind
 
     libspec_manager: LibspecManager = completion_context.workspace.libspec_manager
     tracing = completion_context.tracing
 
@@ -369,14 +374,17 @@
 
             visited = memo.get(key, False)
             if visited:
                 continue
             else:
                 memo[key] = True
 
+            doc = library_doc.doc
+            lib_deprecated = doc and text_utilities.has_deprecated_text(doc)
+
             #: :type keyword: KeywordDoc
             for keyword in library_doc.keywords:
                 keyword_name = keyword.name
                 if collector.accepts(keyword_name):
                     if tracing:
                         log.debug(
                             "Accepted keyword name: %s (libname: %s, libalias: %s)",
@@ -387,14 +395,15 @@
 
                     keyword_args: Sequence[IKeywordArg] = ()
                     if keyword.args:
                         keyword_args = keyword.args
 
                     collector.on_keyword(
                         _KeywordFoundFromLibrary(
+                            lib_deprecated,
                             library_doc,
                             keyword,
                             keyword_name,
                             keyword_args,
                             completion_context,
                             CompletionItemKind.Method,
                             library_alias=library_info.alias,
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/collect_robot_documentation.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/collect_robot_documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context_dependency_graph.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/completion_context_workspace_caches.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/completion_context_workspace_caches.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/dictionary_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/dictionary_completions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/doc_highlight.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/doc_highlight.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/doctree2md.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/doctree2md.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/document_symbol.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/document_symbol.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/filesystem_section_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/filesystem_section_completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,29 +228,29 @@
 def get_requisites(completion_context: ICompletionContext) -> Optional[_Requisites]:
     from robotframework_ls.impl import ast_utils
 
     token_info = completion_context.get_current_token()
     if token_info is not None:
         # Library
         token = ast_utils.get_library_import_name_token(
-            token_info.node, token_info.token
+            token_info.node, token_info.token, generate_empty_on_eol=True
         )
         if token is not None:
             return _Requisites(token, "library")
 
         # Resource
         token = ast_utils.get_resource_import_name_token(
-            token_info.node, token_info.token
+            token_info.node, token_info.token, generate_empty_on_eol=True
         )
         if token is not None:
             return _Requisites(token, "resource")
 
         # Variable
         token = ast_utils.get_variables_import_name_token(
-            token_info.node, token_info.token
+            token_info.node, token_info.token, generate_empty_on_eol=True
         )
         if token is not None:
             return _Requisites(token, "variables")
     return None
 
 
 def complete(completion_context: ICompletionContext) -> List[CompletionItemTypedDict]:
@@ -259,14 +259,27 @@
     """
     try:
 
         requisites = get_requisites(completion_context)
         if requisites is None:
             return []
 
+        return complete_with_requisites(completion_context, requisites)
+
+    except:
+        log.exception()
+
+    return []
+
+
+def complete_with_requisites(
+    completion_context: ICompletionContext, requisites: _Requisites
+) -> List[CompletionItemTypedDict]:
+    try:
+
         if requisites.is_library:
             return _get_library_completions(completion_context, requisites.token)
 
         elif requisites.is_resource:
             return _get_resource_completions(completion_context, requisites.token)
 
         elif requisites.is_variables:
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/find_definition.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/find_definition.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/flow_explorer_model_builder.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/flow_explorer_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,14 +165,49 @@
     suite_name: str,
     parent_body: List[Any],
     memo: dict,
     recursion_stack: _KeywordRecursionStack,
     user_keywords_collector: _UserKeywordCollector,
     parent_node: Optional[Dict] = None,
 ):
+    key = (completion_context.doc.uri, curr_ast.lineno, curr_ast.col_offset)
+    found = memo.get(key)
+    if found is not None:
+        parent_body.extend(found)
+        return
+    temp_parent_body: List[Any] = []
+    memo[key] = temp_parent_body
+
+    ret = __build_hierarchy(
+        completion_context,
+        curr_stack,
+        curr_ast,
+        suite_name,
+        temp_parent_body,
+        memo,
+        recursion_stack,
+        user_keywords_collector,
+        parent_node,
+    )
+
+    parent_body.extend(temp_parent_body)
+    return
+
+
+def __build_hierarchy(
+    completion_context: ICompletionContext,
+    curr_stack: Tuple[INode, ...],
+    curr_ast: Any,
+    suite_name: str,
+    parent_body: List[Any],
+    memo: dict,
+    recursion_stack: _KeywordRecursionStack,
+    user_keywords_collector: _UserKeywordCollector,
+    parent_node: Optional[Dict] = None,
+):
     from robotframework_ls.impl import ast_utils
     from robotframework_ls.impl import ast_utils_keyword_usage
     from robotframework_ls.impl.find_definition import find_keyword_definition
     from robotframework_ls.impl.protocols import TokenInfo
 
     if ast_utils.is_keyword_usage_node(curr_ast):
         keyword_usage_handler = ast_utils_keyword_usage.obtain_keyword_usage_handler(
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/folding_range.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/formatting.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/formatting.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/hover.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/hover.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_argument_analysis.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_argument_analysis.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     AbstractKeywordCollector,
     KeywordUsageInfo,
 )
 from robocorp_ls_core.lsp import (
     TextEditTypedDict,
     CompletionItemTypedDict,
     InsertTextFormat,
+    CompletionItemTag,
 )
 from robotframework_ls.impl.text_utilities import normalize_robot_name
 
 
 log = get_logger(__name__)
 
 
@@ -193,21 +194,24 @@
                     "character": token.col_offset + col_delta,
                 },
                 "end": {"line": selection.line, "character": token.end_col_offset},
             },
             "newText": text,
         }
 
-        return {
+        ret: CompletionItemTypedDict = {
             "label": label,
             "kind": keyword_found.completion_item_kind,
             "textEdit": text_edit,
             "insertText": text_edit["newText"],
             "insertTextFormat": InsertTextFormat.Snippet,
         }
+        if keyword_found.is_deprecated():
+            ret["tags"] = [CompletionItemTag.Deprecated]
+        return ret
 
     def on_keyword(self, keyword_found: IKeywordFound):
         col_delta = 0
 
         if not self._matcher.accepts_keyword_name(keyword_found.keyword_name):
             for matcher in self._scope_matchers:
                 if matcher.accepts_keyword(keyword_found):
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/keyword_parameter_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/keyword_parameter_completions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/keywords_in_args.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/keywords_in_args.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/library_names_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/library_names_completions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_manager.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import threading
 from typing import Optional, Dict, Set, Iterator, Union, Any
 from robocorp_ls_core.protocols import Sentinel, IEndPoint
 from robotframework_ls.impl.protocols import (
     ILibraryDoc,
     ILibraryDocOrError,
     ICompletionContext,
-    ILibraryDocConversions,
 )
 import itertools
 from robocorp_ls_core.watchdog_wrapper import IFSObserver
 from robotframework_ls.impl.robot_lsp_constants import (
     OPTION_ROBOT_LIBRARIES_LIBDOC_NEEDS_ARGS,
 )
 from robotframework_ls.impl.libspec_warmup import (
@@ -494,14 +493,16 @@
             builtin_libspec_dir
             or self.get_internal_builtins_libspec_dir(self._libspec_dir)
         )
         log.info("User libspec dir: %s", self._user_libspec_dir)
         log.info("Builtins libspec dir: %s", self._builtins_libspec_dir)
         log.info("Cache libspec dir: %s", self._cache_libspec_dir)
 
+        self._deprecated_library_name_to_replacement: Dict[str, str] = {}
+
         try:
             os.makedirs(self._user_libspec_dir)
         except:
             # Ignore exception if it's already created.
             pass
         try:
             os.makedirs(self._builtins_libspec_dir)
@@ -624,24 +625,28 @@
 
     @config.setter
     def config(self, config):
         from robotframework_ls.impl.robot_lsp_constants import (
             OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE,
         )
         from robocorp_ls_core.basic import make_unique
+        from robotframework_ls import robot_config
 
         self._check_in_main_thread()
         from robotframework_ls.impl.robot_lsp_constants import OPTION_ROBOT_PYTHONPATH
 
         self._config = config
         existing_entries = set(self._additional_pythonpath_folder_to_folder_info.keys())
         if config is not None:
             pythonpath_entries = set(
                 config.get_setting(OPTION_ROBOT_PYTHONPATH, list, [])
             )
+            pythonpath_entries = set(
+                config.get_setting(OPTION_ROBOT_PYTHONPATH, list, [])
+            )
             for new_pythonpath_entry in pythonpath_entries:
                 new_pythonpath_entry = os.path.abspath(new_pythonpath_entry)
 
                 if new_pythonpath_entry not in existing_entries:
                     self.add_additional_pythonpath_folder(new_pythonpath_entry)
             for old_entry in existing_entries:
                 if old_entry not in pythonpath_entries:
@@ -652,14 +657,18 @@
                 config.get_setting(OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE, list, [])
             )
 
             if self.pre_generate_libspecs:
                 log.debug("Generating user/pythonpath libraries libspec.")
                 self._libspec_warmup.gen_user_libraries(self, make_unique(pre_generate))
 
+        self._deprecated_library_name_to_replacement = (
+            robot_config.get_robot_libraries_deprecated_name_to_replacement(config)
+        )
+
     @property
     def user_libspec_dir(self) -> str:
         return self._user_libspec_dir
 
     @property
     def cache_libspec_dir(self) -> str:
         return self._cache_libspec_dir
@@ -681,16 +690,24 @@
                 libname = cache_key[0]
                 if libname not in spec_file:
                     new[cache_key] = value
             # Always set as a whole (to avoid racing conditions).
             self._libspec_failures_cache = new
 
         # Notify _FolderInfo._on_change_spec
-        if spec_file.lower().endswith(".libspec"):
+        lowername = spec_file.lower()
+        if lowername.endswith(".libspec"):
             folder_info_on_change_spec(spec_file)
+        elif lowername.endswith(".py"):
+            # Note: right now we don't act on .py info.
+            # This means that the caches for libraries will actually be invalid
+            # until someone calls 'libspec_manager.get_library_doc_or_error'
+            # for that library again (at which point it verifies the timestamp
+            # of the library).
+            pass
 
     def add_workspace_folder(self, folder_uri: str):
         self._check_in_main_thread()
         from robocorp_ls_core import uris
 
         if folder_uri not in self._workspace_folder_uri_to_folder_info:
             log.debug("Added workspace folder: %s", folder_uri)
@@ -778,14 +795,55 @@
             yield uris.to_fs_path(uri)
 
         yield from self._pythonpath_folder_to_folder_info.keys()
 
         yield from self._additional_pythonpath_folder_to_folder_info.keys()
 
     def iter_lib_info(self, builtin=False):
+        from robotframework_ls.impl.text_utilities import has_deprecated_text
+
+        blacklist = ()
+        if self.config is not None:
+            from robotframework_ls.impl.robot_generated_lsp_constants import (
+                OPTION_ROBOT_LIBRARIES_BLACKLIST,
+            )
+
+            blacklist = self.config.get_setting(
+                OPTION_ROBOT_LIBRARIES_BLACKLIST, list, ()
+            )
+            if not blacklist:
+                blacklist = ()
+            else:
+                blacklist = set(blacklist)
+
+        deprecated_library_name_to_replacement = (
+            self._deprecated_library_name_to_replacement
+        )
+        for libinfo in self._iter_lib_info(builtin):
+            if libinfo.library_doc.name not in blacklist:
+
+                deprecated = deprecated_library_name_to_replacement.get(
+                    libinfo.library_doc.name
+                )
+                if deprecated is not None:
+                    if not libinfo.library_doc.doc:
+                        libinfo.library_doc = deprecated
+                    elif not has_deprecated_text(libinfo.library_doc.doc):
+                        libinfo.library_doc.__original_doc__ = libinfo.library_doc.doc
+                        libinfo.library_doc.doc = deprecated + libinfo.library_doc.doc
+                else:
+                    if libinfo.library_doc.doc and hasattr(
+                        libinfo.library_doc, "__original_doc__"
+                    ):
+                        libinfo.library_doc.doc = libinfo.library_doc.__original_doc__
+                        delattr(libinfo.library_doc, "__original_doc__")
+
+                yield libinfo
+
+    def _iter_lib_info(self, builtin=False):
         """
         :rtype: generator(_LibInfo)
         """
         # Note: the iteration order is important (first ones are visited earlier
         # and have higher priority).
         iter_in = []
         for (_uri, info) in self._workspace_folder_uri_to_folder_info.items():
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_markdown_conversion.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_markdown_conversion.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/libspec_warmup.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/libspec_warmup.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/on_type_formatting.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/on_type_formatting.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/protocols.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,14 +346,15 @@
     filename: str
     name: str
     source: str
     symbols_cache: Optional["ISymbolsCache"]
     inits: list
     doc_format: str
     keywords: List["IKeywordDoc"]
+    doc: str
 
 
 class ILibraryDocConversions(ILibraryDoc):
     """
     Note: these are actually part of the basic library doc but we
     put it in a different interface because clients usually shouldn't
     use it (it's controlled by the libspec manager).
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/references.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/references.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/rename.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/rename.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_html_formatters.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_html_formatters.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_html_utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_html_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_markuputils.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_markuputils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_formatting/robot_normalizing.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_formatting/robot_normalizing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_generated_lsp_constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_generated_lsp_constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 OPTION_ROBOT_PYTHON_EXECUTABLE = "robot.python.executable"
 OPTION_ROBOT_PYTHON_ENV = "robot.python.env"
 OPTION_ROBOT_VARIABLES = "robot.variables"
 OPTION_ROBOT_LOAD_VARIABLES_FROM_ARGUMENTS_FILE = "robot.loadVariablesFromArgumentsFile"
 OPTION_ROBOT_PYTHONPATH = "robot.pythonpath"
 OPTION_ROBOT_LIBRARIES_LIBDOC_NEEDS_ARGS = "robot.libraries.libdoc.needsArgs"
 OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE = "robot.libraries.libdoc.preGenerate"
+OPTION_ROBOT_LIBRARIES_BLACKLIST = "robot.libraries.blacklist"
+OPTION_ROBOT_LIBRARIES_DEPRECATED = "robot.libraries.deprecated"
 OPTION_ROBOT_CODE_FORMATTER = "robot.codeFormatter"
 OPTION_ROBOT_FLOW_EXPLORER_THEME = "robot.flowExplorerTheme"
 OPTION_ROBOT_LINT_ROBOCOP_ENABLED = "robot.lint.robocop.enabled"
 OPTION_ROBOT_LINT_ENABLED = "robot.lint.enabled"
 OPTION_ROBOT_LINT_UNDEFINED_KEYWORDS = "robot.lint.undefinedKeywords"
 OPTION_ROBOT_LINT_UNDEFINED_LIBRARIES = "robot.lint.undefinedLibraries"
 OPTION_ROBOT_LINT_UNDEFINED_RESOURCES = "robot.lint.undefinedResources"
@@ -58,14 +60,16 @@
         OPTION_ROBOT_PYTHON_EXECUTABLE,
         OPTION_ROBOT_PYTHON_ENV,
         OPTION_ROBOT_VARIABLES,
         OPTION_ROBOT_LOAD_VARIABLES_FROM_ARGUMENTS_FILE,
         OPTION_ROBOT_PYTHONPATH,
         OPTION_ROBOT_LIBRARIES_LIBDOC_NEEDS_ARGS,
         OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE,
+        OPTION_ROBOT_LIBRARIES_BLACKLIST,
+        OPTION_ROBOT_LIBRARIES_DEPRECATED,
         OPTION_ROBOT_CODE_FORMATTER,
         OPTION_ROBOT_FLOW_EXPLORER_THEME,
         OPTION_ROBOT_LINT_ROBOCOP_ENABLED,
         OPTION_ROBOT_LINT_ENABLED,
         OPTION_ROBOT_LINT_UNDEFINED_KEYWORDS,
         OPTION_ROBOT_LINT_UNDEFINED_LIBRARIES,
         OPTION_ROBOT_LINT_UNDEFINED_RESOURCES,
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_localization.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_localization.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_lsp_constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_lsp_constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_specbuilder.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_specbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,16 @@
         self.doc = doc
         self.version = version
         self.specversion = specversion
         self.type = type
         self.scope = scope
         self.named_args = named_args
         self.doc_format = doc_format or "ROBOT"
+        if source and source.startswith("<"):  # Deal with <string>
+            source = None
         self._source = source
         self.lineno = lineno
         self.inits = []
         self.keywords = []
         self.data_types = []
 
         self.symbols_cache: Optional[ISymbolsCache] = None
@@ -479,14 +481,16 @@
     ):
         self._weak_libdoc = weak_libdoc
         self.name = name
         self._args = args
         self.doc = doc
         self.tags = tags
         self._shortdoc = ""
+        if source and source.startswith("<"):
+            source = None
         self._source = source
         self.lineno = lineno
 
     @property
     def shortdoc(self):
         return self._shortdoc or self._doc_to_shortdoc()
 
@@ -504,15 +508,17 @@
 
     @shortdoc.setter  # type: ignore
     def shortdoc(self, shortdoc):
         self._shortdoc = shortdoc
 
     @property
     def deprecated(self) -> bool:
-        return self.doc.startswith("*DEPRECATED") and "*" in self.doc[1:]
+        from robotframework_ls.impl.text_utilities import has_deprecated_text
+
+        return has_deprecated_text(self.doc)
 
     @property  # type: ignore
     @instance_cache
     def args(self) -> Tuple[IKeywordArg, ...]:
         if self._args:
             if isinstance(self._args[0], KeywordArg):
                 return self._args
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_version.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/robot_workspace.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/section_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/section_completions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/section_name_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/section_name_completions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/selection_range.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/semantic_tokens.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/signature_help.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/snippets_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/snippets_completions.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,34 +41,38 @@
             "    $0",
             "END",
         ],
         "description": "Snippet of a FOR IN ZIP loop\n\nA for loop that iterates over two lists and assigns the values from the first list to the first variable and values from the second list to the second variable per iteration.",
     },
     "IF STATEMENT": {
         "prefix": "IF STATEMENT",
-        "body": ["IF<sp>${${1:var1}} == ${${1:var2}}", "    $0", "END"],
+        "body": [
+            "IF<sp>${1:\\$var_in_py_expr1 == \\$var_in_py_expr2}",
+            "    $0",
+            "END",
+        ],
         "description": "Snippet of an IF..END statement.",
     },
     "IF ELSE STATEMENT": {
         "prefix": "IF ELSE STATEMENT",
         "body": [
-            "IF<sp>${${1:var1}} == ${${1:var2}}",
+            "IF<sp>${1:\\$var_in_py_expr1 == \\$var_in_py_expr2}",
             "    ${3:Call Keyword}",
             "ELSE",
             "    $0",
             "END",
         ],
         "description": "Snippet of an IF..ELSE..END statement",
     },
     "Run Keyword If": {
         "prefix": "Run Keyword If",
         "body": [
-            "Run Keyword If<sp>${1:condition}",
+            "Run Keyword If<sp>${1:\\$var_in_py_expr1 == \\$var_in_py_expr2}",
             "...    ${3:Keyword}<sp>${4:@args}",
-            "...  ELSE IF<sp>${2:condition}",
+            "...  ELSE IF<sp>${2:condition_in_py_expr}",
             "...    ${5:Keyword}<sp>${6:@args}",
             "...  ELSE",
             "...    ${7:Keyword}<sp>${8:@args}",
         ],
         "description": "Runs the given keyword with the given arguments, if condition is true.",
     },
     "Run Keywords": {
@@ -105,20 +109,28 @@
     "TRY FINALLY STATEMENT": {
         "prefix": "TRY FINALLY",
         "body": ["TRY", "    $0", "FINALLY", "    ", "END"],
         "description": "Snippet of a TRY..EXCEPT..FINALLY statement",
     },
     "WHILE STATEMENT": {
         "prefix": "WHILE",
-        "body": [r"WHILE<sp>${1:expression}", "    $0", "END"],
+        "body": [
+            "WHILE<sp>${1:\\$var_in_py_expr1 == \\$var_in_py_expr2}",
+            "    $0",
+            "END",
+        ],
         "description": "Snippet of a WHILE statement",
     },
     "WHILE STATEMENT UNLIMITED": {
         "prefix": "WHILE",
-        "body": [r"WHILE<sp>${1:expression}<sp>limit=NONE", "    $0", "END"],
+        "body": [
+            "WHILE<sp>${1:\\$var_in_py_expr1 == \\$var_in_py_expr2}<sp>limit=NONE",
+            "    $0",
+            "END",
+        ],
         "description": "Snippet of a WHILE statement with limit=NONE",
     },
     "CONTINUE": {
         "prefix": "CONTINUE",
         "body": ["CONTINUE"],
         "description": "Snippet for CONTINUE",
     },
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/string_matcher.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/string_matcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/text_utilities.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/text_utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from functools import lru_cache
 from robocorp_ls_core.robotframework_log import get_logger
 import re
 from typing import Sequence
+from robocorp_ls_core.protocols import IDocument
+from robocorp_ls_core.lsp import Range
 
 log = get_logger(__name__)
 
 
-class TextUtilities(object):
-    def __init__(self, text):
+class TextUtilities:
+    def __init__(self, text: str):
         self.text = text
 
     def strip_leading_chars(self, c):
         if len(c) != 1:
             raise AssertionError('Expected "%s" to have size == 1' % (c,))
         text = self.text
         if len(text) == 0 or text[0] != c:
@@ -25,14 +27,21 @@
             # Consumed all chars
             self.text = ""
             return True
 
     def strip(self):
         self.text = self.text.strip()
 
+    def get_indent(self):
+        m = re.match("(\s+)(.*)", self.text)
+        if not m:
+            return ""
+
+        return m.group(1)
+
 
 # Note: this not only makes it faster, but also makes us use less memory as a
 # way to reuse the same 'interned" strings.
 @lru_cache(maxsize=2000)
 def normalize_robot_name(text: str) -> str:
     return text.lower().replace("_", "").replace(" ", "")
 
@@ -200,23 +209,16 @@
                 buf.write(".")
             buf.write(name)
             remainder = ".".join(splitted[i + 1 :])
             head = buf.getvalue()
             yield head, remainder
 
 
-_DEPRECATED_PATTERN = re.compile(r"^\*DEPRECATED(.*)\*(.*)")
-
-
 def has_deprecated_text(docs: str) -> bool:
-    if docs and "DEPRECATED" in docs:
-        matched = _DEPRECATED_PATTERN.match(docs)
-        return bool(matched)
-
-    return False
+    return bool(docs and docs.strip().startswith("*DEPRECATED"))
 
 
 def build_keyword_docs_with_signature(
     keyword_name: str,
     args: Sequence[str],  # tuple(x.original_arg for x in keyword_args)
     docs: str,
     docs_format: str,
@@ -248,7 +250,36 @@
 
 
 @lru_cache(maxsize=300)
 def get_digest_from_string(s: str) -> str:
     import hashlib
 
     return hashlib.sha256(s.encode("utf-8", "replace")).hexdigest()[:8]
+
+
+def set_doc_source_and_get_range_selected(
+    initial_source: str, doc: IDocument, range_char="|"
+) -> Range:
+
+    i = initial_source.find(range_char)
+    j = initial_source.find(range_char, i + 1)
+    if j == -1:
+        # Just position, not a range.
+        source = initial_source[0:i] + initial_source[i + 1 :]
+    else:
+        # Range selected
+        assert i > 0
+        assert j > i
+        source = (
+            initial_source[0:i] + initial_source[i + 1 : j] + initial_source[j + 1 :]
+        )
+
+    doc.source = source
+
+    start = doc.offset_to_line_col(i)
+    if j > 0:
+        end = doc.offset_to_line_col(j - 1)
+    else:
+        end = start
+    select_range = Range(start, end)
+
+    return select_range
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/variable_completions.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/variable_completions.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     IRobotDocument,
     IVariablesCollector,
     IVariableFound,
     IRobotToken,
     TokenInfo,
     AbstractVariablesCollector,
     VariableKind,
-    VarTokenInfo,
     INode,
     AdditionalVarInfo,
 )
 from robotframework_ls.impl.text_utilities import normalize_robot_name
 from robotframework_ls.impl.variable_types import (
     VariableFoundFromToken,
     VariableFoundFromYaml,
@@ -25,21 +24,28 @@
 
 
 log = get_logger(__name__)
 
 
 class _Collector(AbstractVariablesCollector):
     def __init__(
-        self, selection: IDocumentSelection, var_token_info: VarTokenInfo, matcher
+        self,
+        selection: IDocumentSelection,
+        in_expression: bool,
+        tokens_and_matchers,
+        in_assign: bool,
+        add_dollar: bool,
     ):
-        self.matcher = matcher
+
         self.completion_items: List[CompletionItemTypedDict] = []
         self.selection = selection
-        self.token = var_token_info.token
-        self.var_token_info = var_token_info
+        self.in_expression = in_expression
+        self._in_assign = in_assign
+        self._add_dollar = add_dollar
+        self._tokens_and_matchers = tokens_and_matchers
 
     def _create_completion_item_from_variable(
         self,
         variable_found: IVariableFound,
         selection: IDocumentSelection,
         token: IRobotToken,
     ) -> CompletionItemTypedDict:
@@ -50,48 +56,67 @@
             Range,
             TextEdit,
         )
         from robocorp_ls_core.lsp import CompletionItemKind
 
         label = variable_found.variable_name
 
-        if self.var_token_info.var_info.context == AdditionalVarInfo.CONTEXT_EXPRESSION:
+        if self.in_expression:
             # On expressions without '${...}' (just $var_name), we can't use spaces.
             label = label.replace(" ", "_")
 
         text = label
         text = text.replace("$", "\\$")
 
+        if self._add_dollar:
+            label = "$" + label
+            if self.in_expression:
+                text = r"\$" + text
+            else:
+                text = r"\${%s}" % (text,)
+
         text_edit = TextEdit(
             Range(
                 start=Position(selection.line, token.col_offset),
                 end=Position(selection.line, token.end_col_offset),
             ),
             text,
         )
 
         # text_edit = None
         return CompletionItem(
             label,
             kind=CompletionItemKind.Variable,
             text_edit=text_edit,
-            insertText=label,
             documentation=variable_found.variable_value,
             insertTextFormat=InsertTextFormat.Snippet,
         ).to_dict()
 
     def accepts(self, variable_name: str) -> bool:
-        return self.matcher.accepts(variable_name)
+        return True
 
     def on_variable(self, variable_found: IVariableFound):
-        self.completion_items.append(
-            self._create_completion_item_from_variable(
-                variable_found, self.selection, self.token
+        from robotframework_ls.impl.string_matcher import RobotStringMatcher
+
+        matcher: RobotStringMatcher
+        token: IRobotToken
+
+        for token, matcher in self._tokens_and_matchers:
+            if not matcher.accepts(variable_found.variable_name):
+                continue
+
+            if self._in_assign and token.value == variable_found.variable_name:
+                continue
+
+            self.completion_items.append(
+                self._create_completion_item_from_variable(
+                    variable_found, self.selection, token
+                )
             )
-        )
+            break
 
     def __typecheckself__(self) -> None:
         _: IVariablesCollector = check_implements(self)
 
 
 def _collect_variables_from_set_keywords(
     ast,
@@ -480,25 +505,90 @@
     _collect_variables_from_set_keywords(
         stack_node, completion_context, collector, KEYWORD_SET_LOCAL_TO_VAR_KIND
     )
 
 
 def complete(completion_context: ICompletionContext) -> List[CompletionItemTypedDict]:
     from robotframework_ls.impl.string_matcher import RobotStringMatcher
+    from robotframework_ls.impl import ast_utils
+    from robocorp_ls_core.document_selection import word_to_column
 
     var_token_info = completion_context.get_current_variable()
     if var_token_info is not None:
         value = var_token_info.token.value
+        in_assign = var_token_info.token.type == var_token_info.token.ASSIGN
+
+        in_expression = (
+            var_token_info.var_info.context == AdditionalVarInfo.CONTEXT_EXPRESSION
+        )
         collector = _Collector(
-            completion_context.sel, var_token_info, RobotStringMatcher(value)
+            completion_context.sel,
+            in_expression,
+            [(var_token_info.token, RobotStringMatcher(value))],
+            in_assign,
+            add_dollar=False,
         )
         only_current_doc = False
-        if var_token_info.token.type == var_token_info.token.ASSIGN:
+        if in_assign:
             # When assigning to variables we don't want to assign what's not
             # currently in this document (such as builtins).
             only_current_doc = True
 
         collect_variables(
             completion_context, collector, only_current_doc=only_current_doc
         )
         return collector.completion_items
+
+    # Ok, we don't have a variable started, so, let's see if we're in a scope
+    # where we should add the full variable...
+    token_info = completion_context.get_current_token()
+    if token_info and token_info.token:
+        token = token_info.token
+
+        if token.type not in (token.ARGUMENT, token.NAME, token.EOL):
+            return []
+
+        if token.type == token.EOL:
+            token = ast_utils.create_empty_token_name_at_eol(token)
+
+        # It something as:
+        # Log to console    v|
+        # to become:
+        # Log to console    ${variable chosen}
+        #
+        # or
+        #
+        # Log to console    some v| other
+        # to become:
+        # Log to console    some ${variable chosen} other
+        #
+        # or
+        #
+        # Log to console    arg=v|
+        # to become:
+        # Log to console    arg=${variable chosen}
+
+        in_expression = ast_utils.is_node_with_expression_argument(token_info.node)
+        cp = ast_utils.copy_token_with_subpart_up_to_col(
+            token, completion_context.sel.col
+        )
+
+        tokens_and_matchers = [(token, RobotStringMatcher(token.value))]
+
+        word = word_to_column(cp.value)
+        if word != cp.value:
+            cp = ast_utils.copy_token_with_subpart(
+                cp, len(cp.value) - len(word), len(cp.value)
+            )
+            tokens_and_matchers.append((cp, RobotStringMatcher(cp.value)))
+
+        collector = _Collector(
+            completion_context.sel,
+            in_expression,
+            tokens_and_matchers,
+            in_assign=False,
+            add_dollar=True,
+        )
+        collect_variables(completion_context, collector, only_current_doc=False)
+        return collector.completion_items
+
     return []
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/variable_completions_from_py.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/variable_completions_from_py.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/variable_resolve.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/variable_resolve.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/variable_types.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/variable_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/variables_from_arguments_file.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/variables_from_arguments_file.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/impl/workspace_symbols.py` & `robotframework-lsp-1.9.0/robotframework_ls/impl/workspace_symbols.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/ls_timeouts.py` & `robotframework-lsp-1.9.0/robotframework_ls/ls_timeouts.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/rf_interactive_integration.py` & `robotframework-lsp-1.9.0/robotframework_ls/rf_interactive_integration.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/robot_to_markdown.py` & `robotframework-lsp-1.9.0/robotframework_ls/robot_to_markdown.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/robotframework_ls_completion_impl.py` & `robotframework-lsp-1.9.0/robotframework_ls/robotframework_ls_completion_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/robotframework_ls_impl.py` & `robotframework-lsp-1.9.0/robotframework_ls/robotframework_ls_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,14 +494,16 @@
             "codeActionProvider": {
                 "resolveProvider": False,
                 "codeActionKinds": [
                     "quickfix",
                     "refactor",
                     "refactor.extract.local",
                     "assign.toVar",
+                    "surroundWith.tryExcept",
+                    "surroundWith.tryExceptFinally",
                 ],
             },
             "codeLensProvider": {"resolveProvider": True},
             # Docs are lazily computed
             "completionProvider": {"resolveProvider": True},
             "documentFormattingProvider": True,
             "documentHighlightProvider": True,
@@ -911,14 +913,15 @@
         return self.async_api_forward(
             "request_flow_explorer_model",
             "api",
             doc_uri=current_doc_uri,
             uri=current_doc_uri,
             __add_doc_uri_in_args__=False,
             __convert_result__=finish_and_convert_result,
+            __timeout__=999999,  # No timeout for the flow explorer...
         )
 
     @command_dispatcher("robot.listTests")
     def _list_tests(self, *arguments):
         from robotframework_ls.ls_timeouts import get_timeout
         from robotframework_ls.ls_timeouts import TimeoutReason
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/server_api/client.py` & `robotframework-lsp-1.9.0/robotframework_ls/server_api/client.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/server_api/monaco_conversions.py` & `robotframework-lsp-1.9.0/robotframework_ls/server_api/monaco_conversions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/server_api/server.py` & `robotframework-lsp-1.9.0/robotframework_ls/server_api/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,23 @@
     from robotframework_ls.impl.collect_keywords import (
         collect_keyword_name_to_keyword_found,
     )
     from robotframework_ls.impl import ast_utils
 
     ret = section_name_completions.complete(completion_context)
     if not ret:
-        ret.extend(filesystem_section_completions.complete(completion_context))
+        requisites = filesystem_section_completions.get_requisites(completion_context)
+        if requisites:
+            ret.extend(
+                filesystem_section_completions.complete_with_requisites(
+                    completion_context, requisites
+                )
+            )
+            # Variables can also be used on Library/Resource/Variable import names.
+            ret.extend(variable_completions.complete(completion_context))
 
     if not ret:
         token_info = completion_context.get_current_token()
         if token_info is not None:
             token = ast_utils.get_keyword_name_token(
                 token_info.stack, token_info.node, token_info.token
             )
@@ -107,21 +115,19 @@
                     )
                 )
                 ret.extend(library_names_completions.complete(completion_context))
                 return ret
 
     if not ret:
         ret.extend(variable_completions.complete(completion_context))
+        ret.extend(keyword_parameter_completions.complete(completion_context))
 
     if not ret:
         ret.extend(dictionary_completions.complete(completion_context))
 
-    if not ret:
-        ret.extend(keyword_parameter_completions.complete(completion_context))
-
     return ret
 
 
 class RobotFrameworkServerApi(PythonLanguageServer):
     """
     This is a custom server. It uses the same message-format used in the language
     server but with custom messages (i.e.: this is not the language server, but
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/server_api/server__main__.py` & `robotframework-lsp-1.9.0/robotframework_ls/server_api/server__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/server_manager.py` & `robotframework-lsp-1.9.0/robotframework_ls/server_manager.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/README.md` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/basic.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/basic.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/cache.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/cache.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/callbacks.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/callbacks.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/client_base.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/client_base.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/code_units.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/code_units.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/command_dispatcher.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/command_dispatcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/config.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__main__gen_debug_adapter_protocol.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/__main__gen_debug_adapter_protocol.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_base_schema.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_base_schema.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_schema.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/dap/dap_schema.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/debug_adapter_threads.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/debug_adapter_core/debug_adapter_threads.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/document_selection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/document_selection.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from robocorp_ls_core.protocols import IDocumentSelection, IDocument
 
 
 RE_START_WORD = re.compile("[\w]*$")
 RE_END_WORD = re.compile("^[\w]*")
 
 
+def word_to_column(line_to_cursor):
+    m_start = RE_START_WORD.findall(line_to_cursor)
+
+    return m_start[0]
+
+
 class DocumentSelection(object):
     def __init__(self, doc: IDocument, line: int, col: int):
         if line < 0:
             line = 0
 
         if col < 0:
             col = 0
@@ -68,18 +74,15 @@
         m_end = RE_END_WORD.findall(end)
 
         return m_start[0] + m_end[-1]
 
     @property
     def word_to_column(self) -> str:
         line_to_cursor = self.line_to_column
-
-        m_start = RE_START_WORD.findall(line_to_cursor)
-
-        return m_start[0]
+        return word_to_column(line_to_cursor)
 
     @property
     def word_from_column(self) -> str:
         current_line = self.current_line
         if not current_line:
             return ""
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ep_providers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ep_providers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ep_resolve_interpreter.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ep_resolve_interpreter.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/dispatchers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/dispatchers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/endpoint.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/endpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/monitor.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/monitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/streams.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/jsonrpc/streams.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/scandir_vendored.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify/scandir_vendored.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/fsnotify_lib/fsnotify-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_common.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/easter.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/_parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/isoparser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/relativedelta.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/rrule.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_common.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_factories.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/tz.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/win.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/rebuild.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/_identifier.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/async_utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/async_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/bccache.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/compiler.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/debug.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/defaults.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/environment.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/ext.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/filters.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/idtracking.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/lexer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/loaders.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/meta.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nativetypes.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nodes.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/optimizer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/runtime.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/sandbox.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/tests.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/visitor.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_native.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_speedups.c` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/markupsafe/_speedups.c`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__about__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_manylinux.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_musllinux.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_structures.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/markers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/requirements.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/specifiers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/tags.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/version.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/packaging/version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/_meta.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/_meta.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/compat.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/compat.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pathspec.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pathspec.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pattern.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/pattern.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/gitwildmatch.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/patterns/gitwildmatch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_gitwildmatch.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_gitwildmatch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_pathspec.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_pathspec.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec/util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pathspec-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/actions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/common.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/core.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/helpers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/results.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/testing.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/unicode.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pyparsing-3.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/python_dateutil-2.8.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/lazy.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/lazy.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/reference.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/reference.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzfile.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzfile.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzinfo.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/pytz/tzinfo.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/comments.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/documentation.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/duplications.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/errors.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/errors.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/lengths.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/lengths.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/misc.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/naming.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/naming.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/spacing.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/spacing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/tags.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/config.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/files.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/reports.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/reports.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/rules.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/run.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/disablers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/file_types.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/misc.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/run_keywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/robotframework_robocop-2.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/six.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_re.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robocop_lib/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_compat.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_compat.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_termui_impl.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_textwrap.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_winconsole.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/core.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/core.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/decorators.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/formatting.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/formatting.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/globals.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/globals.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/shell_completion.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/termui.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/termui.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/testing.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/testing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/types.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/types.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/click/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__about__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_manylinux.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_musllinux.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_structures.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/markers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/requirements.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/specifiers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/tags.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/version.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/packaging/version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/_meta.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/_meta.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/compat.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/compat.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pathspec.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pathspec.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pattern.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/pattern.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/gitwildmatch.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/patterns/gitwildmatch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_gitwildmatch.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_gitwildmatch.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_pathspec.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_pathspec.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec/util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pathspec-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/actions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/common.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/core.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/helpers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/results.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/testing.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/unicode.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/util.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/pyparsing-3.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotframework_tidy-3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/api.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/app.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/cli.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/config.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/decorators.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/disablers.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/exceptions.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/files.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/skip.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/skip.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AddMissingEnd.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignSettingsSection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignVariablesSection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/DiscardEmptySections.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/IndentNestedKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/InlineIf.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeAssignments.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeNewLines.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSeparators.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSeparators.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSettingName.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeTags.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettings.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettingsSection.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderTags.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameKeywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameTestCases.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceReturns.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SmartSortKeywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SplitTooLongLine.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/aligners_core.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/aligners_core.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/run_keywords.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/utils.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/robotidy/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_re.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/robotidy_lib/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/README.md` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-310-darwin.so` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-38-darwin.so` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-39-darwin.so` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/_watchdog_fsevents.cpython-39-darwin.so`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/events.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/events.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/api.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents2.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/fsevents2.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_buffer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_buffer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_c.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/inotify_c.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/kqueue.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/kqueue.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/polling.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/polling.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/read_directory_changes.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/read_directory_changes.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/winapi.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/observers/winapi.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/tricks/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/bricks.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/bricks.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/delayed_queue.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/delayed_queue.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/dirsnapshot.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/dirsnapshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/echo.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/echo.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/patterns.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/platform.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/platform.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/process_watcher.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/process_watcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/version.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/version.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/watchmedo.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/watchmedo.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog-2.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-5.3.1.dist-info/LICENSE` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-6.0.dist-info/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2020 Ingy döt Net
+Copyright (c) 2017-2021 Ingy döt Net
 Copyright (c) 2006-2016 Kirill Simonov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,59 +4,30 @@
 from .tokens import *
 from .events import *
 from .nodes import *
 
 from .loader import *
 from .dumper import *
 
-__version__ = '5.3.1'
+__version__ = '6.0'
 try:
     from .cyaml import *
     __with_libyaml__ = True
 except ImportError:
     __with_libyaml__ = False
 
 import io
 
 #------------------------------------------------------------------------------
-# Warnings control
+# XXX "Warnings control" is now deprecated. Leaving in the API function to not
+# break code that uses it.
 #------------------------------------------------------------------------------
-
-# 'Global' warnings state:
-_warnings_enabled = {
-    'YAMLLoadWarning': True,
-}
-
-# Get or set global warnings' state
 def warnings(settings=None):
     if settings is None:
-        return _warnings_enabled
-
-    if type(settings) is dict:
-        for key in settings:
-            if key in _warnings_enabled:
-                _warnings_enabled[key] = settings[key]
-
-# Warn when load() is called without Loader=...
-class YAMLLoadWarning(RuntimeWarning):
-    pass
-
-def load_warning(method):
-    if _warnings_enabled['YAMLLoadWarning'] is False:
-        return
-
-    import warnings
-
-    message = (
-        "calling yaml.%s() without Loader=... is deprecated, as the "
-        "default Loader is unsafe. Please read "
-        "https://msg.pyyaml.org/load for full details."
-    ) % method
-
-    warnings.warn(message, YAMLLoadWarning, stacklevel=3)
+        return {}
 
 #------------------------------------------------------------------------------
 def scan(stream, Loader=Loader):
     """
     Scan a YAML stream and produce scanning tokens.
     """
     loader = Loader(stream)
@@ -96,38 +67,30 @@
     loader = Loader(stream)
     try:
         while loader.check_node():
             yield loader.get_node()
     finally:
         loader.dispose()
 
-def load(stream, Loader=None):
+def load(stream, Loader):
     """
     Parse the first YAML document in a stream
     and produce the corresponding Python object.
     """
-    if Loader is None:
-        load_warning('load')
-        Loader = FullLoader
-
     loader = Loader(stream)
     try:
         return loader.get_single_data()
     finally:
         loader.dispose()
 
-def load_all(stream, Loader=None):
+def load_all(stream, Loader):
     """
     Parse all YAML documents in a stream
     and produce corresponding Python objects.
     """
-    if Loader is None:
-        load_warning('load_all')
-        Loader = FullLoader
-
     loader = Loader(stream)
     try:
         while loader.check_data():
             yield loader.get_data()
     finally:
         loader.dispose()
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/composer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/constructor.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -706,26 +706,14 @@
     'tag:yaml.org,2002:python/dict',
     FullConstructor.construct_yaml_map)
 
 FullConstructor.add_multi_constructor(
     'tag:yaml.org,2002:python/name:',
     FullConstructor.construct_python_name)
 
-FullConstructor.add_multi_constructor(
-    'tag:yaml.org,2002:python/module:',
-    FullConstructor.construct_python_module)
-
-FullConstructor.add_multi_constructor(
-    'tag:yaml.org,2002:python/object:',
-    FullConstructor.construct_python_object)
-
-FullConstructor.add_multi_constructor(
-    'tag:yaml.org,2002:python/object/new:',
-    FullConstructor.construct_python_object_new)
-
 class UnsafeConstructor(FullConstructor):
 
     def find_python_module(self, name, mark):
         return super(UnsafeConstructor, self).find_python_module(name, mark, unsafe=True)
 
     def find_python_name(self, name, mark):
         return super(UnsafeConstructor, self).find_python_name(name, mark, unsafe=True)
@@ -735,14 +723,26 @@
             suffix, node, args, kwds, newobj, unsafe=True)
 
     def set_python_instance_state(self, instance, state):
         return super(UnsafeConstructor, self).set_python_instance_state(
             instance, state, unsafe=True)
 
 UnsafeConstructor.add_multi_constructor(
+    'tag:yaml.org,2002:python/module:',
+    UnsafeConstructor.construct_python_module)
+
+UnsafeConstructor.add_multi_constructor(
+    'tag:yaml.org,2002:python/object:',
+    UnsafeConstructor.construct_python_object)
+
+UnsafeConstructor.add_multi_constructor(
+    'tag:yaml.org,2002:python/object/new:',
+    UnsafeConstructor.construct_python_object_new)
+
+UnsafeConstructor.add_multi_constructor(
     'tag:yaml.org,2002:python/object/apply:',
     UnsafeConstructor.construct_python_object_apply)
 
 # Constructor is same as UnsafeConstructor. Need to leave this in place in case
 # people have extended it directly.
 class Constructor(UnsafeConstructor):
     pass
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/cyaml.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/cyaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 __all__ = [
     'CBaseLoader', 'CSafeLoader', 'CFullLoader', 'CUnsafeLoader', 'CLoader',
     'CBaseDumper', 'CSafeDumper', 'CDumper'
 ]
 
-from _yaml import CParser, CEmitter
+from yaml._yaml import CParser, CEmitter
 
 from .constructor import *
 
 from .serializer import *
 from .representer import *
 
 from .resolver import *
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/dumper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/emitter.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/error.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/error.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/events.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/events.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/loader.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/nodes.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/parser.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/reader.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/representer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/representer.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
 Representer.add_representer(complex,
         Representer.represent_complex)
 
 Representer.add_representer(tuple,
         Representer.represent_tuple)
 
-Representer.add_representer(type,
+Representer.add_multi_representer(type,
         Representer.represent_name)
 
 Representer.add_representer(collections.OrderedDict,
         Representer.represent_ordered_dict)
 
 Representer.add_representer(types.FunctionType,
         Representer.represent_name)
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/resolver.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
 
     def resolve(self, kind, value, implicit):
         if kind is ScalarNode and implicit[0]:
             if value == '':
                 resolvers = self.yaml_implicit_resolvers.get('', [])
             else:
                 resolvers = self.yaml_implicit_resolvers.get(value[0], [])
-            resolvers += self.yaml_implicit_resolvers.get(None, [])
-            for tag, regexp in resolvers:
+            wildcard_resolvers = self.yaml_implicit_resolvers.get(None, [])
+            for tag, regexp in resolvers + wildcard_resolvers:
                 if regexp.match(value):
                     return tag
             implicit = implicit[1]
         if self.yaml_path_resolvers:
             exact_paths = self.resolver_exact_paths[-1]
             if kind in exact_paths:
                 return exact_paths[kind]
@@ -173,15 +173,15 @@
                     |true|True|TRUE|false|False|FALSE
                     |on|On|ON|off|Off|OFF)$''', re.X),
         list('yYnNtTfFoO'))
 
 Resolver.add_implicit_resolver(
         'tag:yaml.org,2002:float',
         re.compile(r'''^(?:[-+]?(?:[0-9][0-9_]*)\.[0-9_]*(?:[eE][-+][0-9]+)?
-                    |\.[0-9_]+(?:[eE][-+][0-9]+)?
+                    |\.[0-9][0-9_]*(?:[eE][-+][0-9]+)?
                     |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\.[0-9_]*
                     |[-+]?\.(?:inf|Inf|INF)
                     |\.(?:nan|NaN|NAN))$''', re.X),
         list('-+0123456789.'))
 
 Resolver.add_implicit_resolver(
         'tag:yaml.org,2002:int',
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/scanner.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1207,15 +1207,15 @@
                     self.forward()
                 elif ch in self.ESCAPE_CODES:
                     length = self.ESCAPE_CODES[ch]
                     self.forward()
                     for k in range(length):
                         if self.peek(k) not in '0123456789ABCDEFabcdef':
                             raise ScannerError("while scanning a double-quoted scalar", start_mark,
-                                    "expected escape sequence of %d hexdecimal numbers, but found %r" %
+                                    "expected escape sequence of %d hexadecimal numbers, but found %r" %
                                         (length, self.peek(k)), self.get_mark())
                     code = int(self.prefix(length), 16)
                     chunks.append(chr(code))
                     self.forward(length)
                 elif ch in '\r\n\x85\u2028\u2029':
                     self.scan_line_break()
                     chunks.extend(self.scan_flow_scalar_breaks(double, start_mark))
@@ -1399,15 +1399,15 @@
         codes = []
         mark = self.get_mark()
         while self.peek() == '%':
             self.forward()
             for k in range(2):
                 if self.peek(k) not in '0123456789ABCDEFabcdef':
                     raise ScannerError("while scanning a %s" % name, start_mark,
-                            "expected URI escape sequence of 2 hexdecimal numbers, but found %r"
+                            "expected URI escape sequence of 2 hexadecimal numbers, but found %r"
                             % self.peek(k), self.get_mark())
             codes.append(int(self.prefix(2), 16))
             self.forward(2)
         try:
             value = bytes(codes).decode('utf-8')
         except UnicodeDecodeError as exc:
             raise ScannerError("while scanning a %s" % name, start_mark, str(exc), mark)
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/serializer.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/tokens.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/load_ignored_dirs.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/load_ignored_dirs.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/lsp.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/lsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,22 @@
 
 
 class Position(_Base):
     def __init__(self, line: int = 0, character: int = 0):
         self.line: int = line
         self.character: int = character
 
+    def __getitem__(self, name):
+        # provide tuple-access, not just dict access.
+        if name == 0:
+            return self.line
+        if name == 1:
+            return self.character
+        return getattr(self, name)
+
     def __eq__(self, other):
         return (
             isinstance(other, Position)
             and self.line == other.line
             and self.character == other.character
         )
 
@@ -364,14 +372,17 @@
         start = Position(dct["start"]["line"], dct["start"]["character"])
         end = Position(dct["end"]["line"], dct["end"]["character"])
         return Range(start, end)
 
     def is_inside(self, another_range: "Range") -> bool:
         return self.start >= another_range.start and self.end <= another_range.end
 
+    def get_end_line_col(self):
+        return self.end[0], self.end[1]
+
 
 class TextDocumentContentChangeEvent(_Base):
     def __init__(
         self, range: Optional[RangeTypedDict], rangeLength: Optional[int], text: str
     ):
         """
         :param rangeLength: Deprecated
@@ -1046,14 +1057,17 @@
     path: str
 
 
 class Error(object):
 
     __slots__ = "msg start end severity tags data".split(" ")
 
+    if typing.TYPE_CHECKING:
+        tags: List[int]
+
     def __init__(
         self,
         msg: str,
         start: Tuple[int, int],
         end: Tuple[int, int],
         severity: int = DiagnosticSeverity.Error,
     ):
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/options.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/options.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/ordered_set.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/ordered_set.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/pluginmanager.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/progress_report.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/progress_report.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/protocols.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/protocols.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/python_ls.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/python_ls.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer__main__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer_impl.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/remote_fs_observer_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robocop_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robocop_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robotframework_log.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robotframework_log.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/robotidy_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/robotidy_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/run_and_save_pid.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/run_and_save_pid.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/run_with_env.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/run_with_env.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/subprocess_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/subprocess_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/system_mutex.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/system_mutex.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
             """
             :param check_reentrant:
                 Should only be False if this mutex is expected to be released in
                 a different thread.
             """
             if base_dir is None:
                 base_dir = tempfile.gettempdir()
+            os.makedirs(base_dir, exist_ok=True)
             check_valid_mutex_name(mutex_name)
             self.mutex_name = mutex_name
             self.thread_id = get_tid()
             self.mutex_creation_info = ""
 
             filename = os.path.join(base_dir, mutex_name)
             try:
@@ -198,14 +199,15 @@
             """
             :param check_reentrant:
                 Should only be False if this mutex is expected to be released in
                 a different thread.
             """
             if base_dir is None:
                 base_dir = tempfile.gettempdir()
+            os.makedirs(base_dir, exist_ok=True)
             check_valid_mutex_name(mutex_name)
             self.mutex_name = mutex_name
             self.mutex_creation_info = ""
             self.thread_id = get_tid()
             filename = os.path.join(base_dir, mutex_name)
             try:
                 handle = open(filename, "a+")
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/timeouts.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/timeouts.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/cases_fixture.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/cases_fixture.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/compare.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/compare.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/fixtures.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/fixtures.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/language_server_client.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/language_server_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/monitor.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/unittest_tools/monitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/uris.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/uris.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/watchdog_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/watchdog_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/workspace.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/workspace.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robocorp_ls_core/yaml_wrapper.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robocorp_ls_core/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/_decoder.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/_decoder.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/_impl.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/_impl.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/index.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/index.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robot_out_stream/xml_to_rfstream.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robot_out_stream/xml_to_rfstream.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/__init__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/__main__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/ast_to_code.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/ast_to_code.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/interpreter.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,17 +522,21 @@
                 embedded = isinstance(handler, facade.EmbeddedArgumentsHandler)
                 if not embedded:
                     if handler.name in user_keywords.handlers._normal:
                         del user_keywords.handlers._normal[handler.name]
                 user_keywords.handlers.add(handler, embedded)
 
         # --------------------------------------- Actually run any test content.
+        last_result = None
         for test in new_suite.tests:
             context = EXECUTION_CONTEXTS.current
-            facade.run_test_body(context, test)
+            last_result = facade.run_test_body(context, test, model)
+
+        if len(new_suite.tests) == 1 and last_result is not None:
+            self._stdout.write(f"{last_result}\n")
 
         # Now, update our representation of the document to include what the
         # user just entered.
         for section in model.sections:
             section_name = section.__class__.__name__
             if section.body:
                 if section_name not in self._doc_parts:
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/protocols.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/protocols.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter__main__.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_client.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_generated_lsp_constants.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_generated_lsp_constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 OPTION_ROBOT_PYTHON_EXECUTABLE = "robot.python.executable"
 OPTION_ROBOT_PYTHON_ENV = "robot.python.env"
 OPTION_ROBOT_VARIABLES = "robot.variables"
 OPTION_ROBOT_LOAD_VARIABLES_FROM_ARGUMENTS_FILE = "robot.loadVariablesFromArgumentsFile"
 OPTION_ROBOT_PYTHONPATH = "robot.pythonpath"
 OPTION_ROBOT_LIBRARIES_LIBDOC_NEEDS_ARGS = "robot.libraries.libdoc.needsArgs"
 OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE = "robot.libraries.libdoc.preGenerate"
+OPTION_ROBOT_LIBRARIES_BLACKLIST = "robot.libraries.blacklist"
+OPTION_ROBOT_LIBRARIES_DEPRECATED = "robot.libraries.deprecated"
 OPTION_ROBOT_CODE_FORMATTER = "robot.codeFormatter"
 OPTION_ROBOT_FLOW_EXPLORER_THEME = "robot.flowExplorerTheme"
 OPTION_ROBOT_LINT_ROBOCOP_ENABLED = "robot.lint.robocop.enabled"
 OPTION_ROBOT_LINT_ENABLED = "robot.lint.enabled"
 OPTION_ROBOT_LINT_UNDEFINED_KEYWORDS = "robot.lint.undefinedKeywords"
 OPTION_ROBOT_LINT_UNDEFINED_LIBRARIES = "robot.lint.undefinedLibraries"
 OPTION_ROBOT_LINT_UNDEFINED_RESOURCES = "robot.lint.undefinedResources"
@@ -58,14 +60,16 @@
         OPTION_ROBOT_PYTHON_EXECUTABLE,
         OPTION_ROBOT_PYTHON_ENV,
         OPTION_ROBOT_VARIABLES,
         OPTION_ROBOT_LOAD_VARIABLES_FROM_ARGUMENTS_FILE,
         OPTION_ROBOT_PYTHONPATH,
         OPTION_ROBOT_LIBRARIES_LIBDOC_NEEDS_ARGS,
         OPTION_ROBOT_LIBRARIES_LIBDOC_PRE_GENERATE,
+        OPTION_ROBOT_LIBRARIES_BLACKLIST,
+        OPTION_ROBOT_LIBRARIES_DEPRECATED,
         OPTION_ROBOT_CODE_FORMATTER,
         OPTION_ROBOT_FLOW_EXPLORER_THEME,
         OPTION_ROBOT_LINT_ROBOCOP_ENABLED,
         OPTION_ROBOT_LINT_ENABLED,
         OPTION_ROBOT_LINT_UNDEFINED_KEYWORDS,
         OPTION_ROBOT_LINT_UNDEFINED_LIBRARIES,
         OPTION_ROBOT_LINT_UNDEFINED_RESOURCES,
```

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_api.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_api.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_manager.py` & `robotframework-lsp-1.9.0/robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_server_manager.py`

 * *Files identical despite different names*

### Comparing `robotframework-lsp-1.8.0/robotframework_lsp.egg-info/PKG-INFO` & `robotframework-lsp-1.9.0/robotframework_lsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-lsp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Language Server Protocol implementation for Robot Framework
 Home-page: https://github.com/robocorp/robotframework-lsp
 Author: Fabio Zadrozny
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,27 +49,27 @@
 
 ## Configuration
 
 After having `Robot Framework Language Server` installed, some configurations (such as specifying
 the python executable used for launching the Language Server or Robot Framework)
 may be needed.
 
-See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/config.md) for details.
+See: [Config](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/config.md) for details.
 
-See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
+See: [FAQ](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/faq.md) for common issues encountered while configuring the language server.
 
 ## Contributing
 
-See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
+See: [Contributing](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/contributing.md) for how to help in the development of `Robot Framework Language Server`.
 
 ## Reporting Issues
 
-See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
+See: [Reporting Issue](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/reporting_issues.md) for details on how to report some issue in the `Robot Framework Language Server`.
 
-## Features (1.8.0)
+## Features (1.9.0)
 
 -   Robot Output View:
     -   View current task/test being executed.
     -   Shows Keyword being executed in real time.
 -   Robot Documentation View:
     -   Select a library import for the full library documentation.
     -   Select another element for its docstring.
@@ -92,14 +92,15 @@
     -   Extract variable to variables section.
 -   Quick fixes (VSCode: `Ctrl + .`):
     -   Add import for unresolved keyword.
     -   Create local variable for unresolved variable.
     -   Create argument for unresolved variable.
     -   Creat variable in variables section for unresolved variable.
     -   Assign keyword to variable.
+    -   Surround with Try..Except.
 -   Symbols browser for keywords in workspace (VSCode: `Ctrl + T`).
 -   Document symbols (VSCode: `Ctrl + Shift + O`).
 -   Highlight of keywords and variables.
 -   Syntax highlighting (using `semanticTokens`).
 -   Syntax validation.
 -   Signature Help (VSCode: `Ctrl + Shift + Space`).
 -   Code Formatting (see: [Editor Settings](https://code.visualstudio.com/docs/getstarted/settings#_language-specific-editor-settings) for details on how to toggle code formatting just for `robotframework`).
@@ -113,10 +114,10 @@
     -   Pause at breakpoints to inspect the stack and see variables
     -   Breakpoint condition/hitCondition/logMessage
     -   Step in
     -   Step over
     -   Step return
     -   Continue
 
-See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.8.0/robotframework-ls/docs/changelog.md) for details.
+See: [Changelog](https://github.com/robocorp/robotframework-lsp/tree/robotframework-lsp-1.9.0/robotframework-ls/docs/changelog.md) for details.
 
 ## License: Apache 2.0
```

### Comparing `robotframework-lsp-1.8.0/robotframework_lsp.egg-info/SOURCES.txt` & `robotframework-lsp-1.9.0/robotframework_lsp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -994,15 +994,16 @@
 robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/dirsnapshot.py
 robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/echo.py
 robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/patterns.py
 robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/platform.py
 robotframework_ls/vendored/robocorp_ls_core/libs/watchdog_lib/watchdog/utils/process_watcher.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/README.md
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/__init__.py
-robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-5.3.1.dist-info/LICENSE
+robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/PyYAML-6.0.dist-info/LICENSE
+robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/_yaml/__init__.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/__init__.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/composer.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/constructor.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/cyaml.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/dumper.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/emitter.py
 robotframework_ls/vendored/robocorp_ls_core/libs/yaml_lib/yaml/error.py
@@ -1032,14 +1033,15 @@
 robotframework_ls/vendored/robotframework_interactive/__main__.py
 robotframework_ls/vendored/robotframework_interactive/ast_to_code.py
 robotframework_ls/vendored/robotframework_interactive/callbacks.py
 robotframework_ls/vendored/robotframework_interactive/interpreter.py
 robotframework_ls/vendored/robotframework_interactive/main_loop.py
 robotframework_ls/vendored/robotframework_interactive/protocols.py
 robotframework_ls/vendored/robotframework_interactive/robot_interactive_console.robot
+robotframework_ls/vendored/robotframework_interactive/robot_version.py
 robotframework_ls/vendored/robotframework_interactive/robotfacade.py
 robotframework_ls/vendored/robotframework_interactive/server/__init__.py
 robotframework_ls/vendored/robotframework_interactive/server/options.py
 robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter__main__.py
 robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_client.py
 robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_generated_lsp_constants.py
 robotframework_ls/vendored/robotframework_interactive/server/rf_interpreter_ls_config.py
```

### Comparing `robotframework-lsp-1.8.0/setup.py` & `robotframework-lsp-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     assert len(ret) > 20, "Did not collect vendored files properly. Found: %s" % (ret,)
     return ret
 
 
 setup(
     name="robotframework-lsp",
-    version="1.8.0",
+    version="1.9.0",
     description="Language Server Protocol implementation for Robot Framework",
     long_description=_readme.read_text(),
     url="https://github.com/robocorp/robotframework-lsp",
     author="Fabio Zadrozny",
     license="Apache-2.0",
     copyright="Robocorp Technologies, Inc.",
     packages=find_packages(),
```

