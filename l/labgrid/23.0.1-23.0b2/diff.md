# Comparing `tmp/labgrid-23.0.1.tar.gz` & `tmp/labgrid-23.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgrid-23.0.1.tar", last modified: Wed Apr 26 14:21:18 2023, max compression
+gzip compressed data, was "labgrid-23.0b2.tar", last modified: Tue Feb 28 13:17:28 2023, max compression
```

## Comparing `labgrid-23.0.1.tar` & `labgrid-23.0b2.tar`

### file list

```diff
@@ -1,428 +1,418 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.669779 labgrid-23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 14:21:05.000000 labgrid-23.0.1/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-26 14:21:05.000000 labgrid-23.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/.crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 14:21:05.000000 labgrid-23.0.1/.crossbar/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 14:21:05.000000 labgrid-23.0.1/.crossbar/config-anonymous.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-26 14:21:05.000000 labgrid-23.0.1/.crossbar/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 14:21:05.000000 labgrid-23.0.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 14:21:05.000000 labgrid-23.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/build-and-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/push-pr-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/reusable-unit-tests-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/reusable-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 14:21:05.000000 labgrid-23.0.1/.github/workflows/scheduled-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-26 14:21:05.000000 labgrid-23.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 14:21:05.000000 labgrid-23.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-04-26 14:21:05.000000 labgrid-23.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 14:21:05.000000 labgrid-23.0.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-04-26 14:21:05.000000 labgrid-23.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 14:21:05.000000 labgrid-23.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-26 14:21:18.665779 labgrid-23.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-26 14:21:05.000000 labgrid-23.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/contrib/completion/
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/completion/labgrid-client.bash
--rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/coordinator-statsd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/sync-places.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/contrib/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/systemd/labgrid-coordinator.service
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/systemd/labgrid-exporter.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/contrib/systemd/sysusers.d/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/systemd/sysusers.d/labgrid.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.629779 labgrid-23.0.1/contrib/systemd/tmpfiles.d/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 14:21:05.000000 labgrid-23.0.1/contrib/systemd/tmpfiles.d/labgrid.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid-client
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid-exporter
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid-pytest
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid-suggest
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid.install
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid.manpages
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid.tmpfile
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid.triggers
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/labgrid.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-04-26 14:21:05.000000 labgrid-23.0.1/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    88737 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/design_decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/images/labgrid_logo_outline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/doc/man/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/man/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/man/device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/man/exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/man.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/doc/res/
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/res/config_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/res/graphstrategy-via-nand.png
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/res/graphstrategy-via-nfs.png
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-04-26 14:21:05.000000 labgrid-23.0.1/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/exporter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/exporter/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/staging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.625779 labgrid-23.0.1/dockerfiles/staging/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/staging/client/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/client/.ssh/id_rsa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/staging/client/simple-test/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/client/simple-test/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/client/simple-test/remote_shell_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.633779 labgrid-23.0.1/dockerfiles/staging/crossbar/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/crossbar/places_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/dockerfiles/staging/dut/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/dut/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/dut/authorized_keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/dockerfiles/staging/exporter-conf/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 14:21:05.000000 labgrid-23.0.1/dockerfiles/staging/exporter-conf/exporter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/examples/barebox/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/local-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/test_barebox.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/test_bootchooser.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/test_sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/barebox/test_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/examples/deditec-relais8/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/deditec-relais8/deditec.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/deditec-relais8/deditec_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/deditec-relais8/export-didicontrol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/deditec-relais8/import-dedicontrol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.637779 labgrid-23.0.1/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/docker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/docker/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/docker/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/docker/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/library/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/library/phytec.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/library/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/modbusrtu/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/modbusrtu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/modbusrtu/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/modbusrtu/test_modbusrtu_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/networkmanager/nm.env
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/networkmanager/nm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/power/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/power/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/power/power_example.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/pyvisa/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/pyvisa/env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/pyvisa/pyvisa_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/qemu-networking/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/qemu-networking/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/qemu-networking/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/qemu-networking/qemunetworkstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/qemu-networking/test_qemu_networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/remote/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/remote/test_barebox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/test_hwclock.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/test_rt.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/shell/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/strategy/bareboxrebootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/strategy/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/strategy/quartusstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/strategy/test_barebox_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/strategy/test_uboot_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/sysfsgpio/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/sysfsgpio/export-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/sysfsgpio/import-gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/sysfsgpio/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/sysfsgpio/sysfsgpio_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.641779 labgrid-23.0.1/examples/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usb/mass-storage-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usb/mxs-usb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usb/test_usb_mxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usb/test_usb_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/examples/usbpower/
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/examplestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/exports.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/remote.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbpower/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/examples/usbsdmux/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbsdmux/local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-26 14:21:05.000000 labgrid-23.0.1/examples/usbsdmux/test_sdmux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-04-26 14:21:05.000000 labgrid-23.0.1/helpers/labgrid-bound-connect
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/labgrid/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/labgrid/autoinstall/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/autoinstall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/autoinstall/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/consoleloggingreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.649779 labgrid-23.0.1/labgrid/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/commandmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/consoleexpectmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/dediprogflashdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/deditecrelaisdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/dfudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/dockerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/fastbootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/flashromdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/flashscriptdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/gpiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/httpvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/lxaiobusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/lxausbmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/modbusdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/networkinterfacedriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/onewiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/openocddriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.653779 labgrid-23.0.1/labgrid/driver/power/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/apc.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/digipower.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/digitalloggers_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/eaton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/eg_pms2_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/gude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/gude24.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/gude8031.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/gude8225.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/gude8316.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/netio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/netio_kshell.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/shelly_gen1.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/siglent.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/simplerest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/power/tplink.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/pyvisadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/quartushpsdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/resetdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/serialdigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/sigrokdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/smallubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbaudiodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbhidrelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbsdmuxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbsdwiredriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbstoragedriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.653779 labgrid-23.0.1/labgrid/driver/usbtmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbtmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbtmc/keysight_dsox2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbtmc/tektronix_tds2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbtmcdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/usbvideodriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/driver/xenadriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.653779 labgrid-23.0.1/labgrid/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/bootstrapprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/commandprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/consoleprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/digitaloutputprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/filesystemprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/filetransferprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/infoprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/linuxbootprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/mmioprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/powerprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/resetprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/protocol/videoprotocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.653779 labgrid-23.0.1/labgrid/pytestplugin/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/pytestplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/pytestplugin/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/pytestplugin/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/pytestplugin/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.657779 labgrid-23.0.1/labgrid/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/authenticator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81608 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32314 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/remote/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.657779 labgrid-23.0.1/labgrid/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/fastboot.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/httpvideostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/modbusrtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/networkservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/onewireport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/udev.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/xenamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/resource/ykushpowerport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/stepreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.657779 labgrid-23.0.1/labgrid/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/bareboxstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/dockerstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/shellstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/strategy/ubootstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.661779 labgrid-23.0.1/labgrid/util/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.661779 labgrid-23.0.1/labgrid/util/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/deditec_relais8.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/sysfsgpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agents/usb_hid_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/agentwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/expect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/managedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/qmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.645779 labgrid-23.0.1/labgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 14:21:18.000000 labgrid-23.0.1/labgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-26 14:21:05.000000 labgrid-23.0.1/labgrid_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.661779 labgrid-23.0.1/man/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-client.1
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-device-config.5
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-device-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-exporter.1
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-exporter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-pytest.7
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-pytest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-suggest.1
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-26 14:21:05.000000 labgrid-23.0.1/man/labgrid-suggest.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:21:05.000000 labgrid-23.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-26 14:21:05.000000 labgrid-23.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:21:18.669779 labgrid-23.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:21:18.665779 labgrid-23.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_autoinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_bareboxdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_crossbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_dediprogflasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_ethernetport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_externalconsoledriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_filedigitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_flashrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_flashscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_graphstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_httpvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_lxaiobus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_manualswitchdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_modbusrtudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_onewire.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_openocd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_powerdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_processwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_pyvisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_qemudriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_sched.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_serialdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_serialport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_shelldriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_sigrok.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_sispm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_sshdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_stepreporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_sysfsgpioagent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_tasmota.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_ubootdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_usbtmc.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_usbvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-26 14:21:05.000000 labgrid-23.0.1/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.314658 labgrid-23.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-28 13:17:18.000000 labgrid-23.0b2/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-28 13:17:18.000000 labgrid-23.0b2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/.crossbar/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-28 13:17:18.000000 labgrid-23.0b2/.crossbar/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-28 13:17:18.000000 labgrid-23.0b2/.crossbar/config-anonymous.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-28 13:17:18.000000 labgrid-23.0b2/.crossbar/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-28 13:17:18.000000 labgrid-23.0b2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-28 13:17:18.000000 labgrid-23.0b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/build-and-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/push-pr-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/reusable-unit-tests-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/reusable-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-28 13:17:18.000000 labgrid-23.0b2/.github/workflows/scheduled-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-28 13:17:18.000000 labgrid-23.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-28 13:17:18.000000 labgrid-23.0b2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-02-28 13:17:18.000000 labgrid-23.0b2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-28 13:17:18.000000 labgrid-23.0b2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-02-28 13:17:18.000000 labgrid-23.0b2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-28 13:17:18.000000 labgrid-23.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-02-28 13:17:28.314658 labgrid-23.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-28 13:17:18.000000 labgrid-23.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/contrib/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/completion/labgrid-client.bash
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6195 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/coordinator-statsd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/sync-places.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/contrib/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/systemd/labgrid-coordinator.service
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/systemd/labgrid-exporter.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/contrib/systemd/sysusers.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/systemd/sysusers.d/labgrid.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.274657 labgrid-23.0b2/contrib/systemd/tmpfiles.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-28 13:17:18.000000 labgrid-23.0b2/contrib/systemd/tmpfiles.d/labgrid.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid-client
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid-exporter
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid-pytest
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid-suggest
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid.install
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid.manpages
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid.tmpfile
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid.triggers
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/labgrid.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-02-28 13:17:18.000000 labgrid-23.0b2/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86673 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/design_decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24657 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/images/labgrid_logo_outline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/doc/man/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/man/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/man/device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/man/exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/man.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/doc/res/
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/res/config_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/res/graphstrategy-via-nand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/res/graphstrategy-via-nfs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-02-28 13:17:18.000000 labgrid-23.0b2/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.278657 labgrid-23.0b2/dockerfiles/exporter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/exporter/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.270657 labgrid-23.0b2/dockerfiles/staging/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/client/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/client/.ssh/id_rsa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/client/simple-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/client/simple-test/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/client/simple-test/remote_shell_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/crossbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/crossbar/places_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/dut/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/dut/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/dut/authorized_keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/dockerfiles/staging/exporter-conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-28 13:17:18.000000 labgrid-23.0b2/dockerfiles/staging/exporter-conf/exporter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/barebox/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/local-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/test_barebox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/test_bootchooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/test_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/barebox/test_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/deditec-relais8/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/deditec-relais8/deditec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/deditec-relais8/deditec_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/deditec-relais8/export-didicontrol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/deditec-relais8/import-dedicontrol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/docker/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/docker/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/docker/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/library/phytec.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/library/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/modbusrtu/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/modbusrtu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/modbusrtu/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/modbusrtu/test_modbusrtu_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/networkmanager/nm.env
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/networkmanager/nm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/power/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/power/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/power/power_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.282657 labgrid-23.0b2/examples/pyvisa/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/pyvisa/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/pyvisa/pyvisa_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/remote/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/remote/test_barebox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/test_hwclock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/test_rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/shell/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/strategy/bareboxrebootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/strategy/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/strategy/quartusstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/strategy/test_barebox_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/strategy/test_uboot_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/sysfsgpio/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/sysfsgpio/export-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/sysfsgpio/import-gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/sysfsgpio/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/sysfsgpio/sysfsgpio_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usb/mass-storage-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usb/mxs-usb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usb/test_usb_mxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usb/test_usb_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/usbpower/
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/examplestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/exports.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/remote.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbpower/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/examples/usbsdmux/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbsdmux/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-28 13:17:18.000000 labgrid-23.0b2/examples/usbsdmux/test_sdmux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.286657 labgrid-23.0b2/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-02-28 13:17:18.000000 labgrid-23.0b2/helpers/labgrid-bound-connect
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.290657 labgrid-23.0b2/labgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.290657 labgrid-23.0b2/labgrid/autoinstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/autoinstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/autoinstall/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/consoleloggingreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.294657 labgrid-23.0b2/labgrid/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/commandmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/consoleexpectmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/deditecrelaisdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/dfudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/dockerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/fastbootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/flashromdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/flashscriptdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/gpiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/httpvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/lxaiobusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/lxausbmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/modbusdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/networkinterfacedriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/onewiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/openocddriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.298657 labgrid-23.0b2/labgrid/driver/power/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/apc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/digipower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/eaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/eg_pms2_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/gude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/gude24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/gude8031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/gude8225.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/gude8316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/netio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/netio_kshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/siglent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/simplerest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/power/tplink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/pyvisadriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/quartushpsdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/resetdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/serialdigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/sigrokdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/smallubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbaudiodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbhidrelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbsdmuxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbsdwiredriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbstoragedriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.298657 labgrid-23.0b2/labgrid/driver/usbtmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbtmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbtmc/keysight_dsox2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbtmc/tektronix_tds2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbtmcdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/usbvideodriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/driver/xenadriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.298657 labgrid-23.0b2/labgrid/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/bootstrapprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/commandprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/consoleprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/digitaloutputprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/filesystemprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/filetransferprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/infoprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/linuxbootprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/mmioprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/powerprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/resetprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/protocol/videoprotocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.298657 labgrid-23.0b2/labgrid/pytestplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/pytestplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/pytestplugin/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/pytestplugin/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/pytestplugin/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.302657 labgrid-23.0b2/labgrid/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/authenticator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77349 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32235 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/remote/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.302657 labgrid-23.0b2/labgrid/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/fastboot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/httpvideostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/modbusrtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/networkservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/onewireport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/serialport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/xenamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/resource/ykushpowerport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/stepreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.302657 labgrid-23.0b2/labgrid/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/bareboxstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/dockerstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/shellstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/strategy/ubootstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.306657 labgrid-23.0b2/labgrid/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.306657 labgrid-23.0b2/labgrid/util/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/deditec_relais8.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/sysfsgpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agents/usb_hid_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/agentwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/expect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/managedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/qmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.290657 labgrid-23.0b2/labgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 13:17:28.000000 labgrid-23.0b2/labgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-02-28 13:17:18.000000 labgrid-23.0b2/labgrid_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.306657 labgrid-23.0b2/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-client.1
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-device-config.5
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-device-config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-exporter.1
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-exporter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-pytest.7
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-pytest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-suggest.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-28 13:17:18.000000 labgrid-23.0b2/man/labgrid-suggest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-28 13:17:18.000000 labgrid-23.0b2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-28 13:17:18.000000 labgrid-23.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 13:17:28.314658 labgrid-23.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:17:28.314658 labgrid-23.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_autoinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_bareboxdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16487 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_crossbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_ethernetport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_externalconsoledriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_filedigitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_flashrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_flashscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_graphstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_httpvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_lxaiobus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_manualswitchdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_modbusrtudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_onewire.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_openocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_powerdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_processwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_pyvisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_qemudriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_sched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_serialdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_serialport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_shelldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_sigrok.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_sispm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_sshdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_stepreporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_sysfsgpioagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_tasmota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_ubootdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_usbtmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_usbvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-28 13:17:18.000000 labgrid-23.0b2/tests/test_yaml.py
```

### Comparing `labgrid-23.0.1/.crossbar/config-anonymous.yaml` & `labgrid-23.0b2/.crossbar/config-anonymous.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/.crossbar/config.yaml` & `labgrid-23.0b2/.crossbar/config.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/.github/pull_request_template.md` & `labgrid-23.0b2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/.github/workflows/build-and-release.yml` & `labgrid-23.0b2/.github/workflows/build-and-release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
       with:
         python-version: "3.11"
     - name: Install python dependencies
       run: |
         python -m pip install --upgrade pip build
     - name: Build sdist
       run: |
-        python -m build
+        python -m build -s
     - name: Publish distribution 📦 to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       if: startsWith(github.ref, 'refs/tags') != true
       with:
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-        repository-url: https://test.pypi.org/legacy/
+        repository_url: https://test.pypi.org/legacy/
     - name: Publish distribution 📦 to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `labgrid-23.0.1/.github/workflows/docker.yml` & `labgrid-23.0b2/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/.github/workflows/push-pr-unit-tests.yml` & `labgrid-23.0b2/.github/workflows/push-pr-unit-tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -14,10 +14,10 @@
       python-version: ${{ matrix.python-version }}
   push-pr-unit-tests-docker:
     name: Docker Unit Tests
     uses: ./.github/workflows/reusable-unit-tests-docker.yml
   build-and-release:
     name: Release to Pypi
     needs: push-pr-unit-tests
-    if: github.event_name == 'push' && github.repository == 'labgrid-project/labgrid'
+    if: github.event_name == 'push'
     uses: ./.github/workflows/build-and-release.yml
     secrets: inherit
```

### Comparing `labgrid-23.0.1/.github/workflows/reusable-unit-tests-docker.yml` & `labgrid-23.0b2/.github/workflows/reusable-unit-tests-docker.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/.github/workflows/reusable-unit-tests.yml` & `labgrid-23.0b2/.github/workflows/reusable-unit-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         chmod 755 ~
         ssh-keygen -f ~/.ssh/id_ed25519.local -t ed25519 -N ""
         cat ~/.ssh/id_ed25519.local.pub >> ~/.ssh/authorized_keys
         echo -e "Host localhost ip6-localhost\n  Hostname 127.0.0.1\n  IdentityFile ~/.ssh/id_ed25519.local\n  UserKnownHostsFile ~/.ssh/known_hosts.local" >> ~/.ssh/config
         ssh -o StrictHostKeyChecking=no localhost echo OK
     - name: Install python dependencies
       run: |
-        python -m pip install --upgrade pip
+        python -m pip install --upgrade pip codecov coveralls
     - name: Install labgrid
       run: |
         pip install -e ".[dev]"
     - name: Lint with pylint
       run: |
         pylint --list-msgs-enabled
         pylint labgrid
```

### Comparing `labgrid-23.0.1/.github/workflows/scheduled-unit-tests.yml` & `labgrid-23.0b2/.github/workflows/scheduled-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/CHANGES.rst` & `labgrid-23.0b2/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,147 +1,70 @@
-Release 23.0.1 (Released Apr 26, 2023)
---------------------------------------
-
-Bug fixes in 23.0.1
-~~~~~~~~~~~~~~~~~~~
-- The pypi release now uses the labgrid pyserial fork in the form of the 
-  pyserial-labgrid package. This fixes installation with newer versions
-  of pip.
-- Several tests have gained an importorskip() call to skip them if the
-  module is not available.
-- The build-and-release workflow supports building wheels.
-- The markers now are restricted to patterns which won't match WARN,
-  ERROR, INFO and similar log notifiers.
-- Fix named SSH lookups in conjunction with an environment file in
-  labgrid-client.
-  
-
-Release 23.0 (Released Apr 24, 2023)
-------------------------------------
+Release 23.0 (unreleased)
+-------------------------
 
 New Features in 23.0
 ~~~~~~~~~~~~~~~~~~~~
-- Python 3.6 support has been dropped.
 - Exporter config templates now have access to the following new variables:
   isolated (all resource accesses must be tunneled True/False),
   hostname (of the exporter host), name (of the exporter).
 - ModbusRTU driver for instruments
-- Support for Eaton ePDU and TP-Link power strips added, either can be used as
-  a NetworkPowerPort.
-- The example strategies now wait for complete system startup using systemctl.
+- Support for Eaton ePDU and TP-Link power strips added, either can be used as a NetworkPowerPort.
 - Consider a combination of multiple "lg_feature" markers instead of
   considering only the closest marker.
-- There is a new ``get_strategy`` helper function which returns the strategy of
-  the target.
-- labgrid-client now supports an ``export`` command which exposes the resource
-  information as environment variables.
-- Newer C920 webcams are now supported.
-- The pytestplugin now correctly combines feature markers instead of replacing
-  them.
-- The ConsoleLoggingReporter is now exported for library usage.
-- The HD 2MP Webcam is now supported by the video-driver.
-- TP-Link power strips are supported by the NetworkPowerDriver.
-- A ModbusRTUResource and Driver has been added to control RS485 equipment.
-- The strategies within labgrid learned the force() function.
 - The labgrid client SSH command is now able to instantiate the SSHDriver when
   there are multiple NetworkService resources available.
 - eg_pms2_network power port driver supports controlling the Energenie power
-  management series with devices like the EG_PMS2_LAN & EG_PMS2_WLAN.
-- The client and coordinator learned of a new "release-from" operation that
-  only releases a place if it acquired by a specific user. This can be used to
-  prevent race conditions when attempting to automate the cleanup of unused
-  places (e.g. in CI jobs).
+  management series with devices like the EG_PMS2_LAN & EG_PMS2_WLAN
+- The client and coordinator learned of a new "release-from" operation that only releases a place
+  if it acquired by a specific user. This can be used to prevent race conditions when attempting to
+  automate the cleanup of unused places (e.g. in CI jobs)
 - ModbusTCPCoil driver supports writing using multiple coils write method
-  in order to make driver usable with Papouch Quido I/O modules.
-- If supported, ser2net started by the exporter now allows multiple connections.
+  in order to make driver usable with Papouch Quido I/O modules
 - SmallUBootDriver driver now supports wide range of Ralink/mt7621 devices
   which expects ``boot_secret`` without new line with new ``boot_secret_nolf``
   boolean config option.
-- More USBVideo devices have been added.
-- labgrid now uses a custom yaml loader/dumper.
 - labgrid-client add-match/add-named-match check for duplicate matches
 - `DFUDriver` has been added to communicate with a `DFUDevice`, a device in DFU
   (Device Firmware Upgrade) mode.
-- ``labgrid-client dfu`` added to allow communication with devices in DFU mode.
+- ``labgrid-client dfu`` added to allow communcation with devices in DFU mode.
 - Support for QEMU Q35 machine added.
 - `UBootDriver` now handles idle console, allowing driver activation on
-  an interrupted U-Boot.
-- Support for the STLINK-V3 has been added to the USBDebugger resource.
-- labgrid-suggest can now suggest matches for a USBPowerPort used by power
-  switchable USB hubs.
-- AndroidFastboot is now deprecated and was replaced by AndroidUSBFastboot. This
-  is more consistent with the AndroidNetFastboot support.
-- In case multiple matches are found for a driver, labgrid-client now outputs
-  the available names.
+  an interupted U-Boot.
 - ProcessWrapper now supports an "input" argument to check_output() that allows
-  a string to be passed to stdin of the process.
+  a string to be passed to stdin of the process
 - The ``NetworkInterfaceDriver`` now supports local and remote SSH port
   forwarding to/from the exporter.
-- labgrid was switched over to use pyproject.toml.
-- A contrib script was added to export coordinator metrics to stasd.
 - The SSH connection timeout can now be globally controlled using the
   ``LG_SSH_CONNECT_TIMEOUT`` environment variable.
 - The `QEMUDriver` now supports a ``display`` option which can specify if an
   display device should be created. ``none`` (the default) will not create a
   display device, ``fb-headless`` will create a headless framebuffer device
   for software rendering, and ``egl-headless`` will create a headless GPU
-  device for accelerated rendering (but requires host support).
-- The `AndroidFastbootDriver` now supports interaction with network devices in
-  fastboot state.
-- Add bash completion for labgrid-client.
-- The `QEMUDriver` now support a ``nic`` property that can be used to create a
-  network interface when booting.
-- The SSHDriver now correctly uses the processwrapper for rsync.
-- The `QEMUDriver` now supports API to add port-forwarding from localhost.
-- The get() method for sdwire has been added.
-- If there are multiple named resources for a target, one of them can be named
-  "default" to select it automatically if no explicit other name is given.
-- labgrid-client has been extended with --name/-n for most commands. This allows
-  attaching multiple power sources/usb-muxes and switching them individually
-  from the command line.
-- Add DediprogFlashDriver and DediprogFlasher resource.
-- Add support for Digital Loggers PDU.
-- Add support for Shelly power switches.
-- Make labgrid-client use crossbar_url and crossbar_realm from ennvironment
-  config.
+  device for accelerated rendering (but requires host support)
 
 Bug fixes in 23.0
 ~~~~~~~~~~~~~~~~~
 
 - The exporter now exports sysfsgpios during place acquire/release, fixing a
   race in the sysfspgio agent interface.
 - Fixed a bug where using ``labgrid-client io get`` always returned ``low``
   when reading a ``sysfsgpio``.
 - Fix labgrid-client exit code on keyboard interrupt.
 - Fixed ``labgrid-client forward --remote``/``-R``, which used either the LOCAL
   part of ``--local``/``-L`` accidentally (if specified) or raised an
   UnboundLocalError.
-- Fix udev matching by attributes.
-- Stop Exporter's event loop when register calls fail.
-- Fix exit codes for various subcommands.
-- Omit role and place output for ``labgrid-client reserve`` to fix shell
-  evaluation.
+- Fix udev matching by attributes
 
 Breaking changes in 23.0
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 - ``Config``'s ``get_option()``/``get_target_option()`` convert non-string
   options no longer to strings.
 - `UBootDriver`'s ``boot_expression`` attribute is deprecated, it will no
   longer check for the string during U-Boot boot. This allows activating the
   driver on an already running U-Boot.
-- The uuu command handling was fixed for the UUUDriver.
-- `UBootDriver` boot() method was fixed.
-- Fix proxying of dynamic port power backends with URL in host parameter and
-  authentication credentials.
-- The coordinator was switched over to anonymous static authentication. You'll
-  have to use the legacy crossbar configuration to support older
-  clients/exporters. The 23.1 release will remove support for the legacy ticket
-  authentication.
-- AndroidFastboot has been deprecated. Please replace it with the more specific
-  AndroidUSBFastboot with the same semantics.
 
 Known issues in 23.0
 ~~~~~~~~~~~~~~~~~~~~
 
 Release 0.4.0 (Released Sep 22, 2021)
 -------------------------------------
```

### Comparing `labgrid-23.0.1/COPYING` & `labgrid-23.0b2/COPYING`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/LICENSE` & `labgrid-23.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/PKG-INFO` & `labgrid-23.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labgrid
-Version: 23.0.1
+Version: 23.0b2
 Summary: embedded systems control library for development, testing and installation
 Author-email: Rouven Czerwinski <entwicklung@pengutronix.de>, Jan Luebbe <entwicklung@pengutronix.de>
 License: Copyright (C) 2016-2017 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
         Copyright (C) 2016-2017 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
         
         This library is free software; you can redistribute it and/or
         modify it under the terms of the GNU Lesser General Public
@@ -44,15 +44,14 @@
 Provides-Extra: pyvisa
 Provides-Extra: snmp
 Provides-Extra: vxi11
 Provides-Extra: xena
 Provides-Extra: deb
 Provides-Extra: dev
 License-File: LICENSE
-License-File: COPYING
 
 .. image:: labgrid_logo.png
    :alt: labgrid logo
    :align: center
 
 Welcome to labgrid
 ==================
@@ -171,10 +170,10 @@
     :alt: documentation status
     :target: https://labgrid.readthedocs.io/en/latest/?badge=latest
 
 .. |chat| image:: https://matrix.to/img/matrix-badge.svg
     :alt: chat
     :target: https://app.element.io/#/room/#labgrid:matrix.org
 
-.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.%5BMICRO%5D-22bfda.svg
+.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg 
     :alt: chat
     :target: https://calver.org/
```

### Comparing `labgrid-23.0.1/README.rst` & `labgrid-23.0b2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -119,10 +119,10 @@
     :alt: documentation status
     :target: https://labgrid.readthedocs.io/en/latest/?badge=latest
 
 .. |chat| image:: https://matrix.to/img/matrix-badge.svg
     :alt: chat
     :target: https://app.element.io/#/room/#labgrid:matrix.org
 
-.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.%5BMICRO%5D-22bfda.svg
+.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg 
     :alt: chat
     :target: https://calver.org/
```

### Comparing `labgrid-23.0.1/contrib/completion/labgrid-client.bash` & `labgrid-23.0b2/contrib/completion/labgrid-client.bash`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # labgrid-client(1) completion                                                 -*- shell-script -*-
 
 # options top level and subcommands support
 _labgrid_shared_options="--help"
-_labgrid_main_opts_with_value="@(-x|--crossbar|-c|--config|-p|--place|-s|--state|-i|--initial-state|-P|--proxy)"
+_labgrid_main_opts_with_value="@(-x|--crossbar|-c|--config|-p|--place|-s|--state|-P|--proxy)"
 
 # Parses labgrid-client arguments
 # Sets arg to subcommand, excluding options and their values.
 # Sets last_arg_opt_with_value to true if the last argument is an option requiring a value, else
 # false.
 # Sets base_cmd to the labgrid-client base command up to subcommand and removes trailing
 # option requiring a value - useful to call 'labgrid-client complete' with place/crossbar/proxy set
@@ -287,23 +287,19 @@
     local cur prev words cword
     _init_completion || return
 
     case "$prev" in
     -t|--delay)
         return
         ;;
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
     esac
 
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--delay --name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "--delay $_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
         _labgrid_count_args "@(-t|--delay)" || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
@@ -326,22 +322,17 @@
     -*)
         COMPREPLY=( $(compgen -W "$_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
         _labgrid_count_args || return
         # only complete second argument
-        case "$args" in
-        2)
-            COMPREPLY=( $(compgen -W "high low get" -- "$cur") )
-            ;;
-        3)
-            _labgrid_complete match-names "$cur"
-            ;;
-        esac
+        [ "$args" -ne 2 ] && return
+
+        COMPREPLY=( $(compgen -W "high low get" -- "$cur") )
         ;;
     esac
 }
 
 _labgrid_client_console()
 {
     local cur prev words cword
@@ -381,79 +372,48 @@
     case "$prev" in
     --wait)
         return
         ;;
     download|detach|list)
         _filedir
         ;;
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
     esac
 
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--wait --name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "--wait $_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
-        _labgrid_count_args "@(--wait|-n|--name)" || return
+        _labgrid_count_args "@(--wait)" || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         COMPREPLY=( $(compgen -W "download detach list" -- "$cur") )
         ;;
     esac
 }
 
 _labgrid_client_fastboot()
 {
-    local cur prev words cword
-    _init_completion || return
-
-    case "$prev" in
-    --wait)
-        return
-        ;;
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
-    case "$cur" in
-    -*)
-        COMPREPLY=( $(compgen -W "--wait --name $_labgrid_shared_options" -- "$cur") )
-        ;;
-    *)
-        _filedir
-        ;;
-    esac
+    _labgrid_client_generic_subcommand "--wait"
 }
 
 _labgrid_client_flashscript()
 {
     local cur prev words cword
     _init_completion || return
 
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "$_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
-        _labgrid_count_args "@(-n|--name)" || return
+        _labgrid_count_args || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         _filedir
         ;;
     esac
 }
@@ -463,81 +423,63 @@
     local cur prev words cword
     _init_completion || return
 
     case "$prev" in
     -w|--wait)
         return
         ;;
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
     esac
 
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--wait --name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "--wait $_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
-        _labgrid_count_args "@(-w|--wait|-n|--name)" || return
+        _labgrid_count_args "@(-w|--wait)" || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         _filedir
         ;;
     esac
 }
 
 _labgrid_client_sd_mux()
 {
     local cur prev words cword
     _init_completion || return
 
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "$_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args
-        _labgrid_count_args "@(-n|--name)" || return
+        _labgrid_count_args || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         COMPREPLY=( $(compgen -W "dut host off client get" -- "$cur") )
         ;;
     esac
 }
 
 _labgrid_client_usb_mux()
 {
     local cur prev words cword
     _init_completion || return
 
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "$_labgrid_shared_options" -- "$cur") )
         ;;
     *)
         local args actions
-        _labgrid_count_args "@(-n|--name)" || return
+        _labgrid_count_args || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         actions="off \
                  dut-device \
                  host-dut \
                  host-device \
@@ -644,70 +586,30 @@
         COMPREPLY=( $(compgen -W "--name --local --remote $_labgrid_shared_options" -- "$cur") )
         ;;
     esac
 }
 
 _labgrid_client_video()
 {
-    local cur prev words cword
-    _init_completion || return
-
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
-    case "$cur" in
-    -*)
-        COMPREPLY=( $(compgen -W "--quality --controls --name $_labgrid_shared_options" -- "$cur") )
-        ;;
-    esac
-}
-
-_labgrid_client_audio()
-{
-    local cur prev words cword
-    _init_completion || return
-
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
-    case "$cur" in
-    -*)
-        COMPREPLY=( $(compgen -W "--name $_labgrid_shared_options" -- "$cur") )
-        ;;
-    esac
+    _labgrid_client_generic_subcommand "--quality --controls"
 }
 
 _labgrid_client_tmc()
 {
     local args cur prev words cword
     _init_completion || return
 
-    case "$prev" in
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
-    esac
-
     case "$cur" in
     -*)
-        COMPREPLY=( $(compgen -W "--name $_labgrid_shared_options" -- "$cur") )
+        COMPREPLY=( $(compgen -W "$_labgrid_shared_options" -- "$cur") )
         return
         ;;
     *)
         local args
-        _labgrid_count_args "@(-n|--name)" || return
+        _labgrid_count_args || return
         # only complete second argument
         if [ "$args" -eq 2 ]; then
             COMPREPLY=( $(compgen -W "cmd query screen channel" -- "$cur") )
             return
         fi
         ;;
     esac
@@ -743,28 +645,24 @@
     --seek)
         return
         ;;
     --mode)
         COMPREPLY=( $( compgen -W "dd bmaptool" -- "$cur") )
         return
         ;;
-    -n|--name)
-        _labgrid_complete match-names "$cur"
-        return
-        ;;
     esac
 
     case "$cur" in
     -*)
-        local options="--wait --partition --skip --seek --mode --name $_labgrid_shared_options"
+        local options="--wait --partition --skip --seek --mode $_labgrid_shared_options"
         COMPREPLY=( $(compgen -W "$options" -- "$cur") )
         ;;
     *)
         local args
-        _labgrid_count_args "@(-w|--wait|-p|--partition|--skip|--seek|--mode|-n|--name)" || return
+        _labgrid_count_args "@(-w|--wait|-p|--partition|--skip|--seek|--mode)" || return
         # only complete second argument
         [ "$args" -ne 2 ] && return
 
         _filedir
         ;;
     esac
 }
@@ -833,15 +731,14 @@
         case "$cur" in
         --*)
             # top level args completion
             local options="--crossbar \
                            --config \
                            --place \
                            --state \
-                           --initial-state \
                            --debug \
                            --verbose \
                            --proxy \
                            $_labgrid_shared_options"
 
             COMPREPLY=( $(compgen -W "$options" -- "$cur" ) )
             return
```

### Comparing `labgrid-23.0.1/contrib/coordinator-statsd.py` & `labgrid-23.0b2/contrib/coordinator-statsd.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/contrib/sync-places.py` & `labgrid-23.0b2/contrib/sync-places.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/debian/changelog` & `labgrid-23.0b2/debian/changelog`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/debian/control` & `labgrid-23.0b2/debian/control`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/debian/copyright` & `labgrid-23.0b2/debian/copyright`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/Makefile` & `labgrid-23.0b2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/RELEASE.rst` & `labgrid-23.0b2/doc/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/conf.py` & `labgrid-23.0b2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/configuration.rst` & `labgrid-23.0b2/doc/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -156,28 +156,17 @@
 
 ``apc``
   Controls an APU PDU via SNMP.
 
 ``digipower``
   Controls a DigiPower PDU via a simple HTTP API.
 
-``digitalloggers_http``
-  Control a Digital Loggers PDU that use the legacy HTTP API. Note that
-  host argument must include the protocol, such as
-  ``http://192.168.0.3`` or ``http://admin:pass@192.168.0.4``.
-
 ``eaton``
   Controls Eaton ePDUs via SNMP.
 
-``eg_pms2_network``
-  Controls the EG_PMS2_LAN & EG_PMS2_WLAN devices, through simple HTTP POST and
-  GET requests.  The device requires a password for logging into the control
-  interface, this module deliberately uses the standard password '1' and is
-  not compatible with a different password.
-
 ``gude``
   Controls a Gude PDU via a simple HTTP API.
 
 ``gude24``
   Controls a Gude Expert Power Control 8008 PDU via a simple HTTP API.
 
 ``gude8031``
@@ -202,20 +191,14 @@
   <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/rest.py>`__
   for details.
 
 ``sentry``
   Controls a Sentry PDU via SNMP using Sentry3-MIB.
   It was tested on CW-24VDD and 4805-XLS-16.
 
-``shelly_gen1``
-  Controls relays of Shelly devices using the Gen 1 Device API.
-  See the `docstring in the module
-  <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/shelly_gen1.py>`__
-  for details.
-
 ``siglent``
   Controls Siglent SPD3000X series modules via the `vxi11 Python module
   <https://pypi.org/project/python-vxi11/>`_.
 
 ``simplerest``
   This is a generic backend for PDU implementations which can be controlled via
   HTTP GET requests (both set and get).
@@ -223,14 +206,20 @@
   <https://github.com/labgrid-project/labgrid/blob/master/labgrid/driver/power/simplerest.py>`__
   for details.
 
 ``tplink``
   Controls TP-Link power strips via `python-kasa
   <https://github.com/python-kasa/python-kasa>`_.
 
+``eg_pms2_network``
+  Controls the EG_PMS2_LAN & EG_PMS2_WLAN devices, through simple HTTP POST and
+  GET requests.  The device requires a password for logging into the control
+  interface, this module deliberately uses the standard password '1' and is
+  not compatible with a different password.
+
 Used by:
   - `NetworkPowerDriver`_
 
 PDUDaemonPort
 +++++++++++++
 A PDUDaemonPort describes a PDU port accessible via `PDUDaemon
 <https://github.com/pdudaemon/pdudaemon>`_.
@@ -1032,43 +1021,14 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 A :any:`NetworkUSBFlashableDevice` resource describes a :any:`USBFlashableDevice`
 resource available on a remote computer
 
 Used by:
   - `FlashScriptDriver`_
 
-DediprogFlasher
-~~~~~~~~~~~~~~~
-A DediprogFlasher resource is used to configure the parameters to a locally installed
-dpmcd instance. It is assumed that dpcmd is installed on the host and the
-executable can be configured via:
-
-.. code-block:: yaml
-
-  tools:
-    dpcmd: '/usr/sbin/dpcmd'
-
-Arguments:
-  - vcc (str): '3.5V', '2.5V' or '1.8V'.
-
-For instance, to flash using 3.5V vcc:
-
-.. code-block:: yaml
-
-  DediprogFlasher:
-    vcc: '3.5V'
-
-
-Used by:
-  - `DediprogFlashDriver`_
-
-NetworkDediprogFlasher
-~~~~~~~~~~~~~~~~~~~~~~
-A NetworkDediprogFlasher describes a `DediprogFlasher`_ available on a remote computer.
-
 XenaManager
 ~~~~~~~~~~~
 A XenaManager resource describes a Xena Manager instance which is the instance the
 `XenaDriver`_ must connect to in order to configure a Xena chassis.
 
 .. code-block:: yaml
 
@@ -1524,19 +1484,17 @@
    SSHDriver:
      keyfile: example.key
 
 Arguments:
   - keyfile (str): optional, filename of private key to login into the remote system
     (has precedence over `NetworkService`'s password)
   - stderr_merge (bool, default=False): set to True to make `run()` return stderr merged with
-    stdout, and an empty list as second element.
+      stdout, and an empty list as second element.
   - connection_timeout (float, default=30.0): timeout when trying to establish connection to
-    target.
-  - explicit_sftp_mode (bool, default=False): if set to True, `put()` and `get()` will
-    explicitly use the SFTP protocol for file transfers instead of scp's default protocol
+      target.
 
 UBootDriver
 ~~~~~~~~~~~
 A UBootDriver interfaces with a U-Boot bootloader via a `ConsoleProtocol`.
 
 Binds to:
   console:
@@ -2252,15 +2210,15 @@
 
    images:
      mybootloaderkey: path/to/mybootloader.img
 
 Arguments:
   - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
     of an image to bootstrap onto the target
-  - script (str): run built-in script with "uuu -b", called with image as arg0
+  - cmd (str, default="spl"): single command used for mfgtool
 
 USBStorageDriver
 ~~~~~~~~~~~~~~~~
 A USBStorageDriver allows access to a USB stick or similar local or
 remote device.
 
 Binds to:
@@ -2349,15 +2307,14 @@
      cpu: cortex-a9
      memory: 512M
      boot_args: "root=/dev/root console=ttyAMA0,115200"
      extra_args: ""
      kernel: kernel
      rootfs: rootfs
      dtb: dtb
-     nic: user
 
 .. code-block:: yaml
 
    tools:
      qemu_arm: /bin/qemu-system-arm
    paths:
      rootfs: ../images/root
@@ -2383,15 +2340,14 @@
   - rootfs (str): optional, reference to the paths key for use as the virtio-9p filesystem
   - dtb (str): optional, reference to the image key for the device tree
   - bios (str): optional, reference to the image key for the bios image
   - display (str, default="none"): optional, display output to enable; must be one of:
     - none: Do not create a display device
     - fb-headless: Create a headless framebuffer device
     - egl-headless: Create a headless GPU-backed graphics card. Requires host support
-  - nic (str): optional, configuration string to pass to QEMU to create a network interface
 
 The QEMUDriver also requires the specification of:
 
 - a tool key, this contains the path to the QEMU binary
 - an image key, the path to the kernel image and optionally the dtb key to
   specify the build device tree
 - a path key, this is the path to the rootfs
@@ -2660,38 +2616,14 @@
 ``file``   The :any:`ManagedFile` used to track the flashable script
 ========== =========================================================
 
 Properties of these keys can be selected using the Python format string syntax,
 e.g. ``{device.devnode}`` to select the device node path of
 :any:`USBFlashableDevice`
 
-DediprogFlashDriver
-~~~~~~~~~~~~~~~~~~~
-The :any:`DediprogFlashDriver` is used to flash an SPI device using DediprogFlasher dpcmd.
-
-.. code-block:: yaml
-
-   DediprogFlashDriver:
-     image: 'foo'
-   images:
-     foo: ../images/image_to_load.raw
-
-Binds to:
-  DediprogFlasher_resource:
-    - `DediprogFlasher`_
-    - `NetworkDediprogFlasher`_
-
-Arguments:
-  - image (str): optional, key in :ref:`images <labgrid-device-config-images>` containing the path
-    of an image to flash onto the target
-
-The DediprogFlashDriver allows using DediprogFlasher dpcmd to flash or erase SPI
-devices. It is assumed that the device flashing is an exporter wired, via
-DediprogFlasher SF100 for instance, to the device being flashed.
-
 XenaDriver
 ~~~~~~~~~~
 The XenaDriver allows to use Xena networking test equipment.
 Using the `xenavalkyrie` library a full API to control the tester is available.
 
 Binds to:
   xena_manager:
```

### Comparing `labgrid-23.0.1/doc/design_decisions.rst` & `labgrid-23.0b2/doc/design_decisions.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/development.rst` & `labgrid-23.0b2/doc/development.rst`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
   $ tail -F logdir/console_main # for the 'main' target
 
 For getting information about timing, the ``annotate-output`` command turned
 out to be quite helpful.
 On Debian it comes with the ``devscripts`` package and you can install it
 with::
 
-  $ sudo apt install devscripts
+  $ apt-get install devscripts
 
 To use it, run::
 
   $ annotate-output tail -F logdir/console_main
 
 This will print your system time before each line, allowing you to both see
 relative delays between steps in your tests as well as absolute timing of
```

### Comparing `labgrid-23.0.1/doc/getting_started.rst` & `labgrid-23.0b2/doc/getting_started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 labgrid, running your first test and setting up the distributed infrastructure.
 For an overview about the basic design and components of `labgrid`, read the
 :ref:`overview` first.
 
 Installation
 ------------
 
-Depending on your distribution you need some dependencies. On Debian these
-usually are:
+Depending on your distribution you need some dependencies. On Debian stretch
+and buster these usually are:
 
 .. code-block:: bash
 
-   $ sudo apt install python3 python3-virtualenv python3-pip python3-setuptools virtualenv microcom
+   $ apt-get install python3 python3-virtualenv python3-pip python3-setuptools virtualenv
 
 
 In many cases, the easiest way is to install labgrid into a virtualenv:
 
 .. code-block:: bash
 
     $ virtualenv -p python3 labgrid-venv
@@ -204,21 +204,15 @@
          ID_SERIAL_SHORT: ID23421JLK
 
 .. note:: See the :ref:`udev matching section <udev-matching>` on how to
           match ManagedResources and the
           :ref:`resources sections <overview-resources>` for a description of
           different resource types.
 
-The exporter requires additional dependencies:
-
-.. code-block:: bash
-
-    $ sudo apt install ser2net
-
-It can now be started by running:
+The exporter can now be started by running:
 
 .. code-block:: bash
 
     labgrid-venv $ labgrid-exporter configuration.yaml
 
 Additional groups and resources can be added:
```

### Comparing `labgrid-23.0.1/doc/images/favicon.png` & `labgrid-23.0b2/doc/images/favicon.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/images/labgrid_logo_outline.svg` & `labgrid-23.0b2/doc/images/labgrid_logo_outline.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/index.rst` & `labgrid-23.0b2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/overview.rst` & `labgrid-23.0b2/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/res/config_graph.svg` & `labgrid-23.0b2/doc/res/config_graph.svg`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/res/graphstrategy-via-nand.png` & `labgrid-23.0b2/doc/res/graphstrategy-via-nand.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/res/graphstrategy-via-nfs.png` & `labgrid-23.0b2/doc/res/graphstrategy-via-nfs.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/doc/usage.rst` & `labgrid-23.0b2/doc/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -862,29 +862,7 @@
 Command-Line
 ------------
 
 labgrid contains some command line tools which are used for remote access to
 resources.
 See :doc:`man/client`, :doc:`man/device-config` and :doc:`man/exporter` for
 more information.
-
-Advanced CLI features
-~~~~~~~~~~~~~~~~~~~~~
-
-This section of the manual describes advanced features that are supported by the
-labgrid client CLI.
-
-Sharing a place with a co-worker
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Labgrid client allows multiple people to access the same shared place,
-even though locks can only be acquired by one person. To allow a coworker to use
-a place use the ``allow`` command of labgrid client in conjunction with the
-coworkers ``user`` and ``hostname``. As an example, with a places named
-``example``, a user name ``john`` and a host named ``sirius``, the command looks
-like this:
-
-.. code-block:: bash
-
-  $ labgrid-client -p example allow sirius/john
-
-To remove the allow it is currently necessary to unlock and lock the place.
```

### Comparing `labgrid-23.0.1/dockerfiles/Dockerfile` & `labgrid-23.0b2/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/dockerfiles/README.rst` & `labgrid-23.0b2/dockerfiles/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/dockerfiles/build.sh` & `labgrid-23.0b2/dockerfiles/build.sh`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/dockerfiles/staging/client/.ssh/id_rsa` & `labgrid-23.0b2/dockerfiles/staging/client/.ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/dockerfiles/staging/docker-compose.yml` & `labgrid-23.0b2/dockerfiles/staging/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/dockerfiles/staging/dut/Dockerfile` & `labgrid-23.0b2/dockerfiles/staging/dut/Dockerfile`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/barebox/test_sleep.py` & `labgrid-23.0b2/examples/barebox/test_sleep.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/deditec-relais8/deditec.py` & `labgrid-23.0b2/examples/deditec-relais8/deditec.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 t = labgrid.Target('main')
 r = labgrid.resource.udev.DeditecRelais8(t, name=None, index=1)
 d = DeditecRelaisDriver(t, name=None)
 
 p = t.get_driver("DigitalOutputProtocol")
 print(t.resources)
```

### Comparing `labgrid-23.0.1/examples/deditec-relais8/deditec_remote.py` & `labgrid-23.0b2/examples/deditec-relais8/deditec_remote.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 e = labgrid.Environment('import-dedicontrol.yaml')
 t = e.get_target()
 
 p = t.get_driver("DigitalOutputProtocol")
 print(t.resources)
 p.set(True)
```

### Comparing `labgrid-23.0.1/examples/docker/README.md` & `labgrid-23.0b2/examples/docker/README.md`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/library/test.py` & `labgrid-23.0b2/examples/library/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 def run_once(target):
     s = target.get_driver('BareboxStrategy')
     s.status = Status.unknown  # force a power-cycle
     s.transition('barebox')
     cmd = target['CommandProtocol']
     cmd.run_check('test -e /dev/nand0')
```

### Comparing `labgrid-23.0.1/examples/networkmanager/nm.py` & `labgrid-23.0b2/examples/networkmanager/nm.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 
 e = Environment('nm.env')
 t = e.get_target()
 d = t.get_driver('NetworkInterfaceDriver')
 
 # based on https://developer.gnome.org/NetworkManager/stable/ch01.html, but adapted to python dicts
```

### Comparing `labgrid-23.0.1/examples/shell/test_hwclock.py` & `labgrid-23.0b2/examples/shell/test_hwclock.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/shell/test_memory.py` & `labgrid-23.0b2/examples/shell/test_memory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/shell/test_rt.py` & `labgrid-23.0b2/examples/shell/test_rt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/strategy/bareboxrebootstrategy.py` & `labgrid-23.0b2/examples/strategy/bareboxrebootstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/strategy/quartusstrategy.py` & `labgrid-23.0b2/examples/strategy/quartusstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/strategy/test_barebox_strategy.py` & `labgrid-23.0b2/examples/strategy/test_barebox_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/strategy/test_uboot_strategy.py` & `labgrid-23.0b2/examples/strategy/test_uboot_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/sysfsgpio/sysfsgpio.py` & `labgrid-23.0b2/examples/sysfsgpio/sysfsgpio.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 t = labgrid.Target('main')
 r = labgrid.resource.base.SysfsGPIO(t, name=None, index=60)
 d = GpioDigitalOutputDriver(t, name=None)
 
 p = t.get_driver("DigitalOutputProtocol")
 print(t.resources)
```

### Comparing `labgrid-23.0.1/examples/sysfsgpio/sysfsgpio_remote.py` & `labgrid-23.0b2/examples/sysfsgpio/sysfsgpio_remote.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)7s: %(message)s',
     stream=sys.stderr,
 )
 
 # show labgrid steps on the console
-StepReporter.start()
+StepReporter()
 
 e = labgrid.Environment('import-gpio.yaml')
 t = e.get_target()
 
 p = t.get_driver("DigitalOutputProtocol")
 print(t.resources)
 p.set(True)
```

### Comparing `labgrid-23.0.1/examples/usb/mxs-usb.yaml` & `labgrid-23.0b2/examples/usb/mxs-usb.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/README.rst` & `labgrid-23.0b2/examples/usbpower/README.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/cycle.py` & `labgrid-23.0b2/examples/usbpower/cycle.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/examplestrategy.py` & `labgrid-23.0b2/examples/usbpower/examplestrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/exports.yaml` & `labgrid-23.0b2/examples/usbpower/exports.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/local.yaml` & `labgrid-23.0b2/examples/usbpower/local.yaml`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/examples/usbpower/test_example.py` & `labgrid-23.0b2/examples/usbpower/test_example.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/helpers/labgrid-bound-connect` & `labgrid-23.0b2/helpers/labgrid-bound-connect`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/autoinstall/main.py` & `labgrid-23.0b2/labgrid/autoinstall/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     args = parser.parse_args()
 
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
 
     env = Environment(config_file=args.config)
 
-    StepReporter.start()
+    StepReporter()
 
     manager = Manager(env, args)
     if not manager.configure():
         exit(1)
     manager.start()
     manager.join()
```

### Comparing `labgrid-23.0.1/labgrid/binding.py` & `labgrid-23.0b2/labgrid/binding.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/config.py` & `labgrid-23.0b2/labgrid/config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/consoleloggingreporter.py` & `labgrid-23.0b2/labgrid/consoleloggingreporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/__init__.py` & `labgrid-23.0b2/labgrid/driver/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 from .dfudriver import DFUDriver
 from .openocddriver import OpenOCDDriver
 from .quartushpsdriver import QuartusHPSDriver
 from .flashromdriver import FlashromDriver
 from .onewiredriver import OneWirePIODriver
 from .powerdriver import ManualPowerDriver, ExternalPowerDriver, \
                          DigitalOutputPowerDriver, YKUSHPowerDriver, \
-                         USBPowerDriver, SiSPMPowerDriver, NetworkPowerDriver, \
-                         PDUDaemonDriver
-from .usbloader import MXSUSBDriver, IMXUSBDriver, BDIMXUSBDriver, RKUSBDriver, UUUDriver
+                         USBPowerDriver, SiSPMPowerDriver
+from .usbloader import MXSUSBDriver, IMXUSBDriver, RKUSBDriver, UUUDriver
 from .usbsdmuxdriver import USBSDMuxDriver
 from .usbsdwiredriver import USBSDWireDriver
 from .common import Driver
 from .qemudriver import QEMUDriver
 from .modbusdriver import ModbusCoilDriver
 from .modbusrtudriver import ModbusRTUDriver
-from .sigrokdriver import SigrokDriver, SigrokPowerDriver
+from .sigrokdriver import SigrokDriver
 from .usbstoragedriver import USBStorageDriver, NetworkUSBStorageDriver, Mode
 from .resetdriver import DigitalOutputResetDriver
 from .gpiodriver import GpioDigitalOutputDriver
 from .filedigitaloutput import FileDigitalOutputDriver
 from .serialdigitaloutput import SerialPortDigitalOutputDriver
 from .xenadriver import XenaDriver
 from .dockerdriver import DockerDriver
@@ -36,13 +35,12 @@
 from .pyvisadriver import PyVISADriver
 from .usbhidrelay import HIDRelayDriver
 from .flashscriptdriver import FlashScriptDriver
 from .usbaudiodriver import USBAudioInputDriver
 from .usbvideodriver import USBVideoDriver
 from .httpvideodriver import HTTPVideoDriver
 from .networkinterfacedriver import NetworkInterfaceDriver
-from .provider import HTTPProviderDriver, NFSPProviderDriver, TFTPProviderDriver
+from .provider import TFTPProviderDriver
 from .mqtt import TasmotaPowerDriver
 from .manualswitchdriver import ManualSwitchDriver
 from .usbtmcdriver import USBTMCDriver
 from .deditecrelaisdriver import DeditecRelaisDriver
-from .dediprogflashdriver import DediprogFlashDriver
```

### Comparing `labgrid-23.0.1/labgrid/driver/bareboxdriver.py` & `labgrid-23.0b2/labgrid/driver/bareboxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/commandmixin.py` & `labgrid-23.0b2/labgrid/driver/commandmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/common.py` & `labgrid-23.0b2/labgrid/driver/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/consoleexpectmixin.py` & `labgrid-23.0b2/labgrid/driver/consoleexpectmixin.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/dediprogflashdriver.py` & `labgrid-23.0b2/labgrid/driver/flashromdriver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 import os.path
 import logging
 import attr
 
-from ..resource import NetworkDediprogFlasher
+from ..resource import NetworkFlashrom
 from ..factory import target_factory
 from ..step import step
+from ..protocol import BootstrapProtocol
 from .common import Driver, check_file
 from ..util.managedfile import ManagedFile
 from ..util.helper import processwrapper
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
-class DediprogFlashDriver(Driver):
-    """ The DediprogFlashDriver uses the dediprog utility to write an image
-    to a raw rom. The driver is a pure wrapper of the dpcmd utility"""
+class FlashromDriver(Driver, BootstrapProtocol):
+    """ The Flashrom driver used the flashrom utility to write an image to a raw rom.
+    The driver is a pure wrapper of the flashrom utility"""
     bindings = {
-        'flasher': {"DediprogFlasher", NetworkDediprogFlasher},
+        'flashrom_resource': {"Flashrom", NetworkFlashrom},
     }
 
-    image = attr.ib(validator=attr.validators.optional(attr.validators.instance_of(str)),
-                    default=None)
+    image = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self.logger = logging.getLogger(f'{self}')
         if self.target.env:
-            self.tool = self.target.env.config.get_tool('dpcmd')
+            self.tool = self.target.env.config.get_tool('flashrom')
         else:
-            self.tool = 'dpcmd'
+            self.tool = 'flashrom'
+        self.logger.debug('Tool %s', self.tool)
 
-    def _get_dediprog_prefix(self):
-        return self.flasher.command_prefix + [self.tool]
+    def _get_flashrom_prefix(self):
+        return self.flashrom_resource.command_prefix+[
+            self.tool
+        ]
 
     def on_activate(self):
         pass
 
     def on_deactivate(self):
         pass
 
-    def map_vcc(self):
-        vcc_map = {'3.5V': '0', '2.5V': '1', '1.8V': '2'}
-        return vcc_map[self.flasher.vcc]
-
     @Driver.check_active
     @step(title='call', args=['args'])
     def __call__(self, *args):
-        vcc = self.map_vcc()
         arg_list = list(args)
-        arg_list.append('--vcc')
-        arg_list.append(vcc)
-        arg_list.append('--silent')
-        processwrapper.check_output(self._get_dediprog_prefix() + arg_list)
+        arg_list.append('-p')
+        arg_list.append(f'{self.flashrom_resource.programmer}')
+        processwrapper.check_output(self._get_flashrom_prefix() + arg_list)
 
     @Driver.check_active
     @step(args=['filename'])
-    def flash(self, filename=None):
+    def load(self, filename=None):
         if filename is None and self.image is not None:
             filename = self.target.env.config.get_image_path(self.image)
         filename = os.path.abspath(filename)
         check_file(filename)
-        mf = ManagedFile(filename, self.flasher)
+        mf = ManagedFile(filename, self.flashrom_resource)
         mf.sync_to_resource()
-
-        self('--auto', mf.get_remote_path(), '--verify', '-x', 'ff')
-
-    @Driver.check_active
-    def erase(self):
-        self('--erase')
+        self.logger.debug('Local File %s synced to remote path %s', filename, mf.get_remote_path())
+        self('-w', mf.get_remote_path())
```

### Comparing `labgrid-23.0.1/labgrid/driver/deditecrelaisdriver.py` & `labgrid-23.0b2/labgrid/driver/deditecrelaisdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/dfudriver.py` & `labgrid-23.0b2/labgrid/driver/dfudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/dockerdriver.py` & `labgrid-23.0b2/labgrid/driver/dockerdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/externalconsoledriver.py` & `labgrid-23.0b2/labgrid/driver/externalconsoledriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/fake.py` & `labgrid-23.0b2/labgrid/driver/fake.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/fastbootdriver.py` & `labgrid-23.0b2/labgrid/driver/fastbootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/filedigitaloutput.py` & `labgrid-23.0b2/labgrid/driver/filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/flashscriptdriver.py` & `labgrid-23.0b2/labgrid/driver/flashscriptdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/gpiodriver.py` & `labgrid-23.0b2/labgrid/driver/gpiodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/httpvideodriver.py` & `labgrid-23.0b2/labgrid/driver/httpvideodriver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import subprocess
-import sys
 from urllib.parse import urlsplit
 
 import attr
 
 from .common import Driver
 from ..factory import target_factory
 from ..util.proxy import proxymanager
@@ -24,15 +23,15 @@
     def stream(self, quality_hint=None):
         s = urlsplit(self.video.url)
         if s.scheme == "http":
             default_port = 80
         elif s.scheme == "https":
             default_port = 443
         else:
-            print(f"Unknown scheme: {s.scheme}", file=sys.stderr)
+            print(f"Unknown scheme: {s.scheme}")
             return
 
         url = proxymanager.get_url(self.video.url, default_port=default_port)
         pipeline = [
             "gst-launch-1.0",
             "souphttpsrc",
             f"location={url}",
@@ -41,9 +40,8 @@
             "!",
             "autovideoconvert",
             "!",
             "autovideosink",
             "sync=false",
         ]
 
-        sub = subprocess.run(pipeline)
-        return sub.returncode
+        subprocess.run(pipeline)
```

### Comparing `labgrid-23.0.1/labgrid/driver/lxaiobusdriver.py` & `labgrid-23.0b2/labgrid/driver/lxaiobusdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/lxausbmuxdriver.py` & `labgrid-23.0b2/labgrid/driver/lxausbmuxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/manualswitchdriver.py` & `labgrid-23.0b2/labgrid/driver/manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/modbusdriver.py` & `labgrid-23.0b2/labgrid/driver/modbusdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/modbusrtudriver.py` & `labgrid-23.0b2/labgrid/driver/modbusrtudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/mqtt.py` & `labgrid-23.0b2/labgrid/driver/mqtt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/networkinterfacedriver.py` & `labgrid-23.0b2/labgrid/driver/networkinterfacedriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/onewiredriver.py` & `labgrid-23.0b2/labgrid/driver/onewiredriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/openocddriver.py` & `labgrid-23.0b2/labgrid/driver/openocddriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/apc.py` & `labgrid-23.0b2/labgrid/driver/power/apc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/digipower.py` & `labgrid-23.0b2/labgrid/driver/power/digipower.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/eaton.py` & `labgrid-23.0b2/labgrid/driver/power/eaton.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/eg_pms2_network.py` & `labgrid-23.0b2/labgrid/driver/power/eg_pms2_network.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/gude.py` & `labgrid-23.0b2/labgrid/driver/power/gude.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/gude24.py` & `labgrid-23.0b2/labgrid/driver/power/gude24.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/gude8031.py` & `labgrid-23.0b2/labgrid/driver/power/gude8031.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/gude8225.py` & `labgrid-23.0b2/labgrid/driver/power/gude8225.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/gude8316.py` & `labgrid-23.0b2/labgrid/driver/power/gude8316.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/netio.py` & `labgrid-23.0b2/labgrid/driver/power/netio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/netio_kshell.py` & `labgrid-23.0b2/labgrid/driver/power/netio_kshell.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/rest.py` & `labgrid-23.0b2/labgrid/driver/power/rest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/sentry.py` & `labgrid-23.0b2/labgrid/driver/power/sentry.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/siglent.py` & `labgrid-23.0b2/labgrid/driver/power/siglent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/simplerest.py` & `labgrid-23.0b2/labgrid/driver/power/simplerest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/power/tplink.py` & `labgrid-23.0b2/labgrid/driver/power/tplink.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/powerdriver.py` & `labgrid-23.0b2/labgrid/driver/powerdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import shlex
 import time
 import math
+from urllib.parse import urlparse
 from importlib import import_module
 
 import attr
 
 from ..factory import target_factory
 from ..protocol import PowerProtocol, DigitalOutputProtocol, ResetProtocol
 from ..resource import NetworkPowerPort
@@ -179,16 +180,14 @@
 
     def set_proxy_from_url(self):
         """
         Some power backends (e.g. rest, simplerest) expect a URL in the host parameter. Try to
         handle the host parameter as a URL, extract the power backend port from it and set new
         proxied host parameter.
         """
-        from urllib.parse import urlparse
-
         url = urlparse(self.port.host)
         if not url.hostname:
             return False
 
         if url.port:
             backend_port = url.port
         elif url.scheme == 'http':
@@ -200,17 +199,15 @@
             return False
 
         self._host, self._port = proxymanager.get_host_and_port(
             self.port, force_port=backend_port
         )
 
         # construct proxied host parameter
-        query = f'?{url.query}' if url.query else ''
-        user_pass = f'{url.netloc.split("@")[0]}@' if '@' in url.netloc else ''
-        self._host = f'{url.scheme}://{user_pass}{self._host}:{self._port}{url.path}{query}'
+        self._host = f'{url.scheme}://{self._host}:{self._port}{url.path}'
         self._port = None
 
         return True
 
     @Driver.check_active
     @step()
     def on(self):
```

### Comparing `labgrid-23.0.1/labgrid/driver/provider.py` & `labgrid-23.0b2/labgrid/driver/provider.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/pyvisadriver.py` & `labgrid-23.0b2/labgrid/driver/pyvisadriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/qemudriver.py` & `labgrid-23.0b2/labgrid/driver/qemudriver.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         rootfs (str): optional, reference to the paths key for use as the virtio-9p filesystem
         dtb (str): optional, reference to the image key for the device tree
         bios (str): optional, reference to the image key for the bios image
         display (str, default="none"): optional, display output to enable; must be one of:
             none: Do not create a display device
             fb-headless: Create a headless framebuffer device
             egl-headless: Create a headless GPU-backed graphics card. Requires host support
-        nic (str): optional, configuration string to pass to QEMU to create a network interface
     """
     qemu_bin = attr.ib(validator=attr.validators.instance_of(str))
     machine = attr.ib(validator=attr.validators.instance_of(str))
     cpu = attr.ib(validator=attr.validators.instance_of(str))
     memory = attr.ib(validator=attr.validators.instance_of(str))
     extra_args = attr.ib(validator=attr.validators.instance_of(str))
     boot_args = attr.ib(
@@ -78,28 +77,24 @@
     display = attr.ib(
         default="none",
         validator=attr.validators.optional(attr.validators.and_(
             attr.validators.instance_of(str),
             attr.validators.in_(["none", "fb-headless", "egl-headless"]),
         ))
     )
-    nic = attr.ib(
-        default=None,
-        validator=attr.validators.optional(attr.validators.instance_of(str)))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self.logger = logging.getLogger(f"{self}:")
         self.status = 0
         self.txdelay = None
         self._child = None
         self._tempdir = None
         self._socket = None
         self._clientsocket = None
-        self._forwarded_ports = {}
         atexit.register(self._atexit)
 
     def _atexit(self):
         if not self._child:
             return
         self._child.terminate()
         try:
@@ -198,18 +193,14 @@
             raise ExecutionError(f"Unknown display '{self.display}'")
 
         self._cmd.append("-chardev")
         self._cmd.append(f"socket,id=serialsocket,path={sockpath}")
         self._cmd.append("-serial")
         self._cmd.append("chardev:serialsocket")
 
-        if self.nic:
-            self._cmd.append("-nic")
-            self._cmd.append(self.nic)
-
         if self.boot_args is not None:
             boot_args.append(self.boot_args)
         if self.kernel is not None and boot_args:
             self._cmd.append("-append")
             self._cmd.append(" ".join(boot_args))
 
     def on_deactivate(self):
@@ -244,19 +235,14 @@
                 self._child.communicate()
                 raise IOError(
                     f"QEMU process terminated with exit code {self._child.returncode}"
                 ) from exc
             raise
 
         self.status = 1
-
-        # Restore port forwards
-        for v in self._forwarded_ports.values():
-            self._add_port_forward(*v)
-
         self.monitor_command("cont")
 
     @step()
     def off(self):
         """Stop the emulator using a monitor command and await the exitcode"""
         if not self.status:
             return
@@ -268,38 +254,21 @@
         self.status = 0
 
     def cycle(self):
         """Cycle the emulator by restarting it"""
         self.off()
         self.on()
 
-    @step(result=True, args=['command', 'arguments'])
-    def monitor_command(self, command, arguments={}):
+    @step(args=['command'])
+    def monitor_command(self, command):
         """Execute a monitor_command via the QMP"""
         if not self.status:
             raise ExecutionError(
                 "Can't use monitor command on non-running target")
-        return self.qmp.execute(command, arguments)
-
-    def _add_port_forward(self, proto, local_address, local_port, remote_address, remote_port):
-        self.monitor_command(
-            "human-monitor-command",
-            {"command-line": f"hostfwd_add {proto}:{local_address}:{local_port}-{remote_address}:{remote_port}"},
-        )
-
-    def add_port_forward(self, proto, local_address, local_port, remote_address, remote_port):
-        self._add_port_forward(proto, local_address, local_port, remote_address, remote_port)
-        self._forwarded_ports[(proto, local_address, local_port)] = (proto, local_address, local_port, remote_address, remote_port)
-
-    def remove_port_forward(self, proto, local_address, local_port):
-        del self._forwarded_ports[(proto, local_address, local_port)]
-        self.monitor_command(
-            "human-monitor-command",
-            {"command-line": f"hostfwd_remove {proto}:{local_address}:{local_port}"},
-        )
+        return self.qmp.execute(command)
 
     def _read(self, size=1, timeout=10, max_size=None):
         ready, _, _ = select.select([self._clientsocket], [], [], timeout)
         if ready:
             # Collect some more data
             time.sleep(0.01)
             # Always read a page, regardless of size
```

### Comparing `labgrid-23.0.1/labgrid/driver/quartushpsdriver.py` & `labgrid-23.0b2/labgrid/driver/quartushpsdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/resetdriver.py` & `labgrid-23.0b2/labgrid/driver/resetdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/serialdigitaloutput.py` & `labgrid-23.0b2/labgrid/driver/serialdigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/serialdriver.py` & `labgrid-23.0b2/labgrid/driver/serialdriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import warnings
 
 import attr
 from packaging import version
 from pexpect import TIMEOUT
 import serial
 import serial.rfc2217
 
@@ -22,14 +23,20 @@
     """
     # pyserial 3.2.1 does not support RFC2217 under Python 3
     # https://github.com/pyserial/pyserial/pull/183
     if version.parse(serial.__version__) <= version.Version('3.2.1'):
         bindings = {"port": "SerialPort", }
     else:
         bindings = {"port": {"SerialPort", "NetworkSerialPort"}, }
+    if version.parse(serial.__version__) != version.Version('3.4.0.1'):
+        message = ("The installed pyserial version does not contain important RFC2217 fixes.\n"
+                   "You can install the labgrid fork via:\n"
+                   "pip uninstall pyserial\n"
+                   "pip install https://github.com/labgrid-project/pyserial/archive/v3.4.0.1.zip#egg=pyserial\n")
+        warnings.warn(message)
 
     txdelay = attr.ib(default=0.0, validator=attr.validators.instance_of(float))
     timeout = attr.ib(default=3.0, validator=attr.validators.instance_of(float))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self.logger = logging.getLogger(f"{self}({self.target})")
```

### Comparing `labgrid-23.0.1/labgrid/driver/shelldriver.py` & `labgrid-23.0b2/labgrid/driver/shelldriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/sigrokdriver.py` & `labgrid-23.0b2/labgrid/driver/sigrokdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/smallubootdriver.py` & `labgrid-23.0b2/labgrid/driver/smallubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/sshdriver.py` & `labgrid-23.0b2/labgrid/driver/sshdriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """The SSHDriver uses SSH as a transport to implement CommandProtocol and FileTransferProtocol"""
 import contextlib
 import logging
 import os
-import re
 import stat
 import shlex
 import shutil
 import subprocess
 import tempfile
 import time
 
@@ -29,15 +28,14 @@
 class SSHDriver(CommandMixin, Driver, CommandProtocol, FileTransferProtocol):
     """SSHDriver - Driver to execute commands via SSH"""
     bindings = {"networkservice": "NetworkService", }
     priorities = {CommandProtocol: 10, FileTransferProtocol: 10}
     keyfile = attr.ib(default="", validator=attr.validators.instance_of(str))
     stderr_merge = attr.ib(default=False, validator=attr.validators.instance_of(bool))
     connection_timeout = attr.ib(default=float(get_ssh_connect_timeout()), validator=attr.validators.instance_of(float))
-    explicit_sftp_mode = attr.ib(default=False, validator=attr.validators.instance_of(bool))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         self.logger = logging.getLogger(f"{self}({self.target})")
         self._keepalive = None
 
     def on_activate(self):
@@ -395,36 +393,20 @@
 
         sub.wait()
 
     def get_status(self):
         """The SSHDriver is always connected, return 1"""
         return 1
 
-    def _scp_supports_explicit_sftp_mode(self):
-        version = subprocess.run(["ssh", "-V"], capture_output=True, text=True)
-        version = re.match(r"^OpenSSH_(\d+)\.(\d+)", version.stderr)
-        major, minor = map(int, version.groups())
-
-        # OpenSSH >= 8.6 supports explicitly using the SFTP protocol via -s
-        if major == 8 and minor >= 6:
-            return True
-        # OpenSSH >= 9.0 default to the SFTP protocol
-        if major >= 9:
-            return False
-        raise Exception(f"OpenSSH version {major}.{minor} does not support explicit SFTP mode")
-
     @Driver.check_active
     @step(args=['filename', 'remotepath'])
     def put(self, filename, remotepath=''):
-        ssh_prefix = self.ssh_prefix
-        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
-            ssh_prefix.append("-s")
         transfer_cmd = [
             "scp",
-            *ssh_prefix,
+            *self.ssh_prefix,
             "-P", str(self.networkservice.port),
             "-r",
             filename,
             f"{self.networkservice.username}@{self.networkservice.address}:{remotepath}"
             ]
 
         try:
@@ -439,20 +421,17 @@
             raise ExecutionError(
                 f"error executing command: {transfer_cmd}"
             )
 
     @Driver.check_active
     @step(args=['filename', 'destination'])
     def get(self, filename, destination="."):
-        ssh_prefix = self.ssh_prefix
-        if self.explicit_sftp_mode and self._scp_supports_explicit_sftp_mode():
-            ssh_prefix.append("-s")
         transfer_cmd = [
             "scp",
-            *ssh_prefix,
+            *self.ssh_prefix,
             "-P", str(self.networkservice.port),
             "-r",
             f"{self.networkservice.username}@{self.networkservice.address}:{filename}",
             destination
             ]
 
         try:
```

### Comparing `labgrid-23.0.1/labgrid/driver/ubootdriver.py` & `labgrid-23.0b2/labgrid/driver/ubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbaudiodriver.py` & `labgrid-23.0b2/labgrid/driver/usbaudiodriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,9 +200,7 @@
                 pass
 
         rx.terminate()
         tx.terminate()
 
         rx.communicate()
         tx.communicate()
-
-        return tx.returncode or rx.returncode
```

### Comparing `labgrid-23.0.1/labgrid/driver/usbhidrelay.py` & `labgrid-23.0b2/labgrid/driver/usbhidrelay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbloader.py` & `labgrid-23.0b2/labgrid/driver/usbloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 @attr.s(eq=False)
 class UUUDriver(Driver, BootstrapProtocol):
     bindings = {
         "loader": {"IMXUSBLoader", "NetworkIMXUSBLoader", "MXSUSBLoader", "NetworkMXSUSBLoader"},
     }
 
     image = attr.ib(default=None)
-    script = attr.ib(default='', validator=attr.validators.instance_of(str))
+    cmd = attr.ib(default='spl', validator=attr.validators.instance_of(str))
 
     def __attrs_post_init__(self):
         super().__attrs_post_init__()
         # FIXME make sure we always have an environment or config
         if self.target.env:
             self.tool = self.target.env.config.get_tool('uuu-loader') or 'uuu-loader'
         else:
@@ -173,18 +173,16 @@
     @step(args=['filename'])
     def load(self, filename=None):
         if filename is None and self.image is not None:
             filename = self.target.env.config.get_image_path(self.image)
         mf = ManagedFile(filename, self.loader)
         mf.sync_to_resource()
 
-        cmd = ['-b', self.script] if self.script else []
-
         processwrapper.check_output(
-            self.loader.command_prefix + [self.tool] + cmd + [mf.get_remote_path()]
+            self.loader.command_prefix + [self.tool, mf.get_remote_path(), self.cmd]
         )
 
 
 @target_factory.reg_driver
 @attr.s(eq=False)
 class BDIMXUSBDriver(Driver, BootstrapProtocol):
     """
```

### Comparing `labgrid-23.0.1/labgrid/driver/usbsdmuxdriver.py` & `labgrid-23.0b2/labgrid/driver/usbsdmuxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbsdwiredriver.py` & `labgrid-23.0b2/labgrid/driver/usbsdwiredriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,7 @@
         cmd = self.mux.command_prefix + [
             self.tool,
             '--dut' if mode.lower() == "dut" else "--ts",
             "-e",
             self.mux.control_serial,
         ]
         processwrapper.check_output(cmd)
-
-    @Driver.check_active
-    @step(title='sdmux_get')
-    def get_mode(self):
-        cmd = self.mux.command_prefix + [
-            self.tool,
-            "-e",
-            self.mux.control_serial,
-            "-u",
-        ]
-        result = processwrapper.check_output(cmd)
-        return result.split(b": ", maxsplit=1)[1].strip().decode()
```

### Comparing `labgrid-23.0.1/labgrid/driver/usbstoragedriver.py` & `labgrid-23.0b2/labgrid/driver/usbstoragedriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbtmc/keysight_dsox2000.py` & `labgrid-23.0b2/labgrid/driver/usbtmc/keysight_dsox2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbtmc/tektronix_tds2000.py` & `labgrid-23.0b2/labgrid/driver/usbtmc/tektronix_tds2000.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbtmcdriver.py` & `labgrid-23.0b2/labgrid/driver/usbtmcdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/usbvideodriver.py` & `labgrid-23.0b2/labgrid/driver/usbvideodriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/driver/xenadriver.py` & `labgrid-23.0b2/labgrid/driver/xenadriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/environment.py` & `labgrid-23.0b2/labgrid/environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/exceptions.py` & `labgrid-23.0b2/labgrid/exceptions.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/factory.py` & `labgrid-23.0b2/labgrid/factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/protocol/__init__.py` & `labgrid-23.0b2/labgrid/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/protocol/commandprotocol.py` & `labgrid-23.0b2/labgrid/protocol/commandprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/protocol/consoleprotocol.py` & `labgrid-23.0b2/labgrid/protocol/consoleprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/protocol/infoprotocol.py` & `labgrid-23.0b2/labgrid/protocol/infoprotocol.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/pytestplugin/fixtures.py` & `labgrid-23.0b2/labgrid/pytestplugin/fixtures.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/pytestplugin/hooks.py` & `labgrid-23.0b2/labgrid/pytestplugin/hooks.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/pytestplugin/reporter.py` & `labgrid-23.0b2/labgrid/pytestplugin/reporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/remote/authenticator.py` & `labgrid-23.0b2/labgrid/remote/authenticator.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/remote/client.py` & `labgrid-23.0b2/labgrid/remote/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,14 @@
     pass
 
 
 class ServerError(Error):
     pass
 
 
-class InteractiveCommandError(Error):
-    pass
-
-
 class ClientSession(ApplicationSession):
     """The ClientSession encapsulates all the actions a Client can Invoke on
     the coordinator."""
 
     def gethostname(self):
         return os.environ.get('LG_HOSTNAME', gethostname())
 
@@ -488,15 +484,15 @@
             raise UserError(f"can not change acquired place {place.name}")
         for pattern in self.args.patterns:
             if not 2 <= pattern.count("/") <= 3:
                 raise UserError(
                     f"invalid pattern format '{pattern}' (use 'exporter/group/cls/name')"
                 )
             if place.hasmatch(pattern.split("/")):
-                print(f"pattern '{pattern}' exists, skipping", file=sys.stderr)
+                print(f"pattern '{pattern}' exists, skipping")
                 continue
             res = await self.call('org.labgrid.coordinator.add_place_match', place.name, pattern)
             if not res:
                 raise ServerError(f"failed to add match {pattern} for place {place.name}")
 
     async def del_match(self):
         """Delete a match for a place"""
@@ -505,15 +501,15 @@
             raise UserError(f"can not change acquired place {place.name}")
         for pattern in self.args.patterns:
             if not 2 <= pattern.count("/") <= 3:
                 raise UserError(
                     f"invalid pattern format '{pattern}' (use 'exporter/group/cls/name')"
                 )
             if not place.hasmatch(pattern.split("/")):
-                print(f"pattern '{pattern}' not found, skipping", file=sys.stderr)
+                print(f"pattern '{pattern}' not found, skipping")
             res = await self.call('org.labgrid.coordinator.del_place_match', place.name, pattern)
             if not res:
                 raise ServerError(f"failed to delete match {pattern} for place {place.name}")
 
     async def add_named_match(self):
         """Add a named match for a place.
 
@@ -657,42 +653,35 @@
         manager.session = self
         manager.loop = self.loop
 
     def _get_target(self, place):
         self._prepare_manager()
         target = None
         if self.env:
-            if self.role is None:
-                self.role = find_role_by_place(self.env.config.get_targets(), place.name)
-                if self.role is not None:
-                    print(f"Selected role {self.role} from configuration file")
             target = self.env.get_target(self.role)
         if target:
             if self.args.state:
                 if self.args.verbose >= 2:
                     from .. import StepReporter
-                    StepReporter.start()
+                    StepReporter()
                 strategy = target.get_driver("Strategy")
-                if self.args.initial_state:
-                    print(f"Setting initial state to {self.args.initial_state}")
-                    strategy.force(self.args.initial_state)
                 print(f"Transitioning into state {self.args.state}")
                 strategy.transition(self.args.state)
                 # deactivate console drivers so we are able to connect with microcom later
                 try:
                     con = target.get_active_driver("ConsoleProtocol")
                     target.deactivate(con)
                 except NoDriverFoundError:
                     pass
         else:
             target = Target(place.name, env=self.env)
             RemotePlace(target, name=place.name)
         return target
 
-    def _get_driver_or_new(self, target, cls, *, name=None, activate=True):
+    def _get_driver_or_new(self, target, cls, *, name=None, activate=True, binding_map=None):
         """
         Helper function trying to get an active driver. If no such driver
         exists, instanciates a new driver.
         Driver instanciation works only for drivers without special kwargs.
 
         Arguments:
         target -- target to operate on
@@ -701,97 +690,96 @@
         activate -- activate the driver (default True)
         """
         try:
             return target.get_driver(cls, name=name, activate=activate)
         except NoDriverFoundError:
             if isinstance(cls, str):
                 cls = target_factory.class_from_string(cls)
-
-            if name is not None:
-                # set name in binding map for unique bindings
-                try:
-                    [unique_binding_key] = cls.bindings
-                    target.set_binding_map({unique_binding_key: name})
-                except ValueError:
-                    raise NotImplementedError("Multiple bindings not implemented for named resources")
+            if binding_map:
+                target.set_binding_map(binding_map)
 
             drv = cls(target, name=name)
             if activate:
                 target.activate(drv)
             return drv
 
     def power(self):
         place = self.get_acquired_place()
         action = self.args.action
         delay = self.args.delay
-        name = self.args.name
         target = self._get_target(place)
         from ..resource.power import NetworkPowerPort, PDUDaemonPort
         from ..resource.remote import NetworkUSBPowerPort, NetworkSiSPMPowerPort
         from ..resource import TasmotaPowerPort
 
         drv = None
         try:
-            drv = target.get_driver("PowerProtocol", name=name)
+            drv = target.get_driver("PowerProtocol")
         except NoDriverFoundError:
             for resource in target.resources:
                 if isinstance(resource, NetworkPowerPort):
-                    drv = self._get_driver_or_new(target, "NetworkPowerDriver", name=name)
+                    drv = self._get_driver_or_new(target, "NetworkPowerDriver")
                 elif isinstance(resource, NetworkUSBPowerPort):
-                    drv = self._get_driver_or_new(target, "USBPowerDriver", name=name)
+                    drv = self._get_driver_or_new(target, "USBPowerDriver")
                 elif isinstance(resource, NetworkSiSPMPowerPort):
-                    drv = self._get_driver_or_new(target, "SiSPMPowerDriver", name=name)
+                    drv = self._get_driver_or_new(target, "SiSPMPowerDriver")
                 elif isinstance(resource, PDUDaemonPort):
-                    drv = self._get_driver_or_new(target, "PDUDaemonDriver", name=name)
+                    drv = self._get_driver_or_new(target, "PDUDaemonDriver")
                 elif isinstance(resource, TasmotaPowerPort):
-                    drv = self._get_driver_or_new(target, "TasmotaPowerDriver", name=name)
+                    drv = self._get_driver_or_new(target, "TasmotaPowerDriver")
                 if drv:
                     break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         if delay is not None:
             drv.delay = delay
         res = getattr(drv, action)()
         if action == 'get':
-            print(f"power{' ' + name if name else ''} for place {place.name} is {'on' if res else 'off'}")
+            print(f"power for place {place.name} is {'on' if res else 'off'}")
 
     def digital_io(self):
         place = self.get_acquired_place()
         action = self.args.action
         name = self.args.name
         target = self._get_target(place)
         from ..resource import ModbusTCPCoil, OneWirePIO
         from ..resource.remote import (NetworkDeditecRelais8, NetworkSysfsGPIO, NetworkLXAIOBusPIO,
                                        NetworkHIDRelay)
 
         drv = None
         try:
-            drv = target.get_driver("DigitalOutputProtocol", name=name)
+            drv = target.get_driver("DigitalOutputProtocol")
         except NoDriverFoundError:
             for resource in target.resources:
                 if isinstance(resource, ModbusTCPCoil):
-                    drv = self._get_driver_or_new(target, "ModbusCoilDriver", name=name)
+                    drv = self._get_driver_or_new(target, "ModbusCoilDriver", name=name,
+                                                  binding_map={"coil": name})
                 elif isinstance(resource, OneWirePIO):
-                    drv = self._get_driver_or_new(target, "OneWirePIODriver", name=name)
+                    drv = self._get_driver_or_new(target, "OneWirePIODriver", name=name,
+                                                  binding_map={"port": name})
                 elif isinstance(resource, NetworkDeditecRelais8):
-                    drv = self._get_driver_or_new(target, "DeditecRelaisDriver", name=name)
+                    drv = self._get_driver_or_new(target, "DeditecRelaisDriver", name=name,
+                                                  binding_map={"relais": name})
                 elif isinstance(resource, NetworkSysfsGPIO):
-                    drv = self._get_driver_or_new(target, "GpioDigitalOutputDriver", name=name)
+                    drv = self._get_driver_or_new(target, "GpioDigitalOutputDriver", name=name,
+                                                  binding_map={"gpio": name})
                 elif isinstance(resource, NetworkLXAIOBusPIO):
-                    drv = self._get_driver_or_new(target, "LXAIOBusPIODriver", name=name)
+                    drv = self._get_driver_or_new(target, "LXAIOBusPIODriver", name=name,
+                                                  binding_map={"pio": name})
                 elif isinstance(resource, NetworkHIDRelay):
-                    drv = self._get_driver_or_new(target, "HIDRelayDriver", name=name)
+                    drv = self._get_driver_or_new(target, "HIDRelayDriver", name=name,
+                                                  binding_map={"relay": name})
                 if drv:
                     break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         if action == 'get':
-            print(f"digital IO{' ' + name if name else ''} for place {place.name} is {'high' if drv.get() else 'low'}")
+            print(f"digital IO {name} for place {place.name} is {'high' if drv.get() else 'low'}")
         elif action == 'high':
             drv.set(True)
         elif action == 'low':
             drv.set(False)
 
     async def _console(self, place, target, timeout, *, logfile=None, loop=False, listen_only=False):
         name = self.args.name
@@ -841,54 +829,49 @@
                     await asyncio.wait_for(p.wait(), 1.0)
                 except asyncio.TimeoutError:
                     # try harder
                     p.kill()
                     await asyncio.wait_for(p.wait(), 1.0)
                 raise
         if p.returncode:
-            print("connection lost", file=sys.stderr)
-        return p.returncode
+            print("connection lost")
+            return False
+        return True
 
     async def console(self, place, target):
         while True:
             res = await self._console(place, target, 10.0, logfile=self.args.logfile,
                                       loop=self.args.loop, listen_only=self.args.listenonly)
-            if res:
-                exc = InteractiveCommandError("microcom error")
-                exc.exitcode = res
-                raise exc
-            if not self.args.loop:
+            if res or not self.args.loop:
                 break
             await asyncio.sleep(1.0)
     console.needs_target = True
 
     def dfu(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
         if self.args.action == 'download' and not self.args.filename:
             raise UserError('not enough arguments for dfu download')
-        drv = self._get_driver_or_new(target, "DFUDriver", activate=False, name=name)
+        drv = self._get_driver_or_new(target, "DFUDriver", activate=False)
         drv.dfu.timeout = self.args.wait
         target.activate(drv)
 
         if self.args.action == 'download':
             drv.download(self.args.altsetting, os.path.abspath(self.args.filename))
         if self.args.action == 'detach':
             drv.detach(self.args.altsetting)
         if self.args.action == 'list':
             drv.list()
 
     def fastboot(self):
         place = self.get_acquired_place()
         args = self.args.fastboot_args
         target = self._get_target(place)
-        name = self.args.name
 
-        drv = self._get_driver_or_new(target, "AndroidFastbootDriver", activate=False, name=name)
+        drv = self._get_driver_or_new(target, "AndroidFastbootDriver", activate=False)
         drv.fastboot.timeout = self.args.wait
         target.activate(drv)
 
         try:
             action = args[0]
             if action == 'flash':
                 drv.flash(args[1], os.path.abspath(args[2]))
@@ -903,70 +886,65 @@
             raise UserError('not enough arguments for fastboot action')
         except subprocess.CalledProcessError as e:
             raise UserError(str(e))
 
     def flashscript(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
 
-        drv = self._get_driver_or_new(target, "FlashScriptDriver", name=name)
+        drv = self._get_driver_or_new(target, "FlashScriptDriver")
         drv.flash(script=self.args.script, args=self.args.script_args)
 
     def bootstrap(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
         from ..resource.remote import (NetworkMXSUSBLoader, NetworkIMXUSBLoader, NetworkRKUSBLoader,
                                        NetworkAlteraUSBBlaster)
         from ..driver import OpenOCDDriver
         drv = None
         try:
-            drv = target.get_driver("BootstrapProtocol", name=name)
+            drv = target.get_driver("BootstrapProtocol")
         except NoDriverFoundError:
             for resource in target.resources:
                 if isinstance(resource, NetworkIMXUSBLoader):
-                    drv = self._get_driver_or_new(target, "IMXUSBDriver", activate=False,
-                                                  name=name)
+                    drv = self._get_driver_or_new(target, "IMXUSBDriver", activate=False)
                     drv.loader.timeout = self.args.wait
                 elif isinstance(resource, NetworkMXSUSBLoader):
-                    drv = self._get_driver_or_new(target, "MXSUSBDriver", activate=False,
-                                                  name=name)
+                    drv = self._get_driver_or_new(target, "MXSUSBDriver", activate=False)
                     drv.loader.timeout = self.args.wait
                 elif isinstance(resource, NetworkAlteraUSBBlaster):
                     args = dict(arg.split('=', 1) for arg in self.args.bootstrap_args)
                     try:
-                        drv = target.get_driver("OpenOCDDriver", activate=False, name=name)
+                        drv = target.get_driver("OpenOCDDriver", activate=False)
                     except NoDriverFoundError:
-                        drv = OpenOCDDriver(target, name=name, **args)
+                        drv = OpenOCDDriver(target, name=None, **args)
                     drv.interface.timeout = self.args.wait
                 elif isinstance(resource, NetworkRKUSBLoader):
-                    drv = self._get_driver_or_new(target, "RKUSBDriver", activate=False, name=name)
+                    drv = self._get_driver_or_new(target, "RKUSBDriver", activate=False)
                     drv.loader.timeout = self.args.wait
                 if drv:
                     break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         target.activate(drv)
         drv.load(self.args.filename)
 
     def sd_mux(self):
         place = self.get_acquired_place()
         action = self.args.action
         target = self._get_target(place)
-        name = self.args.name
         from ..resource.remote import NetworkUSBSDMuxDevice, NetworkUSBSDWireDevice
 
         drv = None
         for resource in target.resources:
             if isinstance(resource, NetworkUSBSDMuxDevice):
-                drv = self._get_driver_or_new(target, "USBSDMuxDriver", name=name)
+                drv = self._get_driver_or_new(target, "USBSDMuxDriver")
             elif isinstance(resource, NetworkUSBSDWireDevice):
-                drv = self._get_driver_or_new(target, "USBSDWireDriver", name=name)
+                drv = self._get_driver_or_new(target, "USBSDWireDriver")
             if drv:
                 break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         if action == 'get':
             print(drv.get_mode())
@@ -974,29 +952,28 @@
             try:
                 drv.set_mode(action)
             except ExecutionError as e:
                 raise UserError(str(e))
 
     def usb_mux(self):
         place = self.get_acquired_place()
-        name = self.args.name
         links = self.args.links
         if links == 'off':
             links = []
         elif links == 'host-dut+host-device':
             links = ['host-dut', 'host-device']
         else:
             links = [links]
         target = self._get_target(place)
         from ..resource.remote import NetworkLXAUSBMux
 
         drv = None
         for resource in target.resources:
             if isinstance(resource, NetworkLXAUSBMux):
-                drv = self._get_driver_or_new(target, "LXAUSBMuxDriver", name=name)
+                drv = self._get_driver_or_new(target, "LXAUSBMuxDriver")
                 break
 
         if not drv:
             raise UserError("target has no compatible resource available")
         drv.set_links(links)
 
     def _get_ip(self, place):
@@ -1012,73 +989,62 @@
             ips = details.get('ips', [])
             if not ips:
                 continue
             matches.append((details['timestamp'], ips))
         matches.sort()
         newest = matches[-1][1]
         if len(ips) > 1:
-            print(f"multiple IPs found: {ips}", file=sys.stderr)
+            print(f"multiple IPs found: {ips}")
             return None
         return newest[0]
 
     def _get_ssh(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
 
+        from ..resource import NetworkService
         try:
-            drv = target.get_driver("SSHDriver", name=self.args.name)
-            return drv
-        except NoDriverFoundError:
-            from ..resource import NetworkService
-            try:
-                resource = target.get_resource(NetworkService, name=self.args.name)
-            except NoResourceFoundError:
-                ip = self._get_ip(place)
-                if not ip:
-                    return
-                resource = NetworkService(target, address=str(ip), username='root')
-
-            drv = self._get_driver_or_new(target, "SSHDriver", name=resource.name)
-            return drv
+            resource = target.get_resource(NetworkService, name=self.args.name)
+        except NoResourceFoundError:
+            ip = self._get_ip(place)
+            if not ip:
+                return
+            resource = NetworkService(target, address=str(ip), username='root')
+
+        drv = self._get_driver_or_new(target, "SSHDriver", name=resource.name,
+                                      binding_map={"networkservice": resource.name})
+        return drv
 
     def ssh(self):
         drv = self._get_ssh()
 
         res = drv.interact(self.args.leftover)
-        if res:
-            exc = InteractiveCommandError("ssh error")
-            exc.exitcode = res
-            raise exc
+        if res == 255:
+            print("connection lost (SSH error)")
+        elif res:
+            print(f"connection lost (remote exit code {res})")
 
     def scp(self):
         drv = self._get_ssh()
 
-        res = drv.scp(src=self.args.src, dst=self.args.dst)
-        if res:
-            exc = InteractiveCommandError("scp error")
-            exc.exitcode = res
-            raise exc
+        drv.scp(src=self.args.src, dst=self.args.dst)
 
     def rsync(self):
         drv = self._get_ssh()
 
-        res = drv.rsync(src=self.args.src, dst=self.args.dst, extra=self.args.leftover)
-        if res:
-            exc = InteractiveCommandError("rsync error")
-            exc.exitcode = res
-            raise exc
+        drv.rsync(src=self.args.src, dst=self.args.dst, extra=self.args.leftover)
 
     def sshfs(self):
         drv = self._get_ssh()
 
         drv.sshfs(path=self.args.path, mountpoint=self.args.mountpoint)
 
     def forward(self):
         if not self.args.local and not self.args.remote:
-            print("Nothing to forward", file=sys.stderr)
+            print("Nothing to forward")
             return
 
         drv = self._get_ssh()
 
         with contextlib.ExitStack() as stack:
             for local, remote in self.args.local:
                 localport = stack.enter_context(drv.forward_local_port(remote, localport=local))
@@ -1099,70 +1065,57 @@
         place = self.get_acquired_place()
         ip = self._get_ip(place)
         if not ip:
             return
         args = ['telnet', str(ip)]
         res = subprocess.call(args)
         if res:
-            exc = InteractiveCommandError("telnet error")
-            exc.exitcode = res
-            raise exc
+            print("connection lost")
 
     def video(self):
         place = self.get_acquired_place()
         quality = self.args.quality
         controls = self.args.controls
         target = self._get_target(place)
-        name = self.args.name
         from ..resource.httpvideostream import HTTPVideoStream
         from ..resource.udev import USBVideo
         from ..resource.remote import NetworkUSBVideo
         drv = None
         try:
-            drv = target.get_driver("VideoProtocol", name=name)
+            drv = target.get_driver("VideoProtocol")
         except NoDriverFoundError:
             for resource in target.resources:
                 if isinstance(resource, (USBVideo, NetworkUSBVideo)):
-                    drv = self._get_driver_or_new(target, "USBVideoDriver", name=name)
+                    drv = self._get_driver_or_new(target, "USBVideoDriver")
                 elif isinstance(resource, HTTPVideoStream):
-                    drv = self._get_driver_or_new(target, "HTTPVideoDriver", name=name)
+                    drv = self._get_driver_or_new(target, "HTTPVideoDriver")
                 if drv:
                     break
         if not drv:
             raise UserError("target has no compatible resource available")
 
         if quality == 'list':
             default, variants = drv.get_qualities()
             for name, caps in variants:
                 mark = '*' if default == name else ' '
                 print(f"{mark} {name:<10s} {caps:s}")
         else:
-            res = drv.stream(quality, controls=controls)
-            if res:
-                exc = InteractiveCommandError("gst-launch-1.0 error")
-                exc.exitcode = res
-                raise exc
+            drv.stream(quality, controls=controls)
 
     def audio(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
-        drv = self._get_driver_or_new(target, "USBAudioInputDriver", name=name)
-        res = drv.play()
-        if res:
-            exc = InteractiveCommandError("gst-launch-1.0 error")
-            exc.exitcode = res
-            raise exc
+        drv = self._get_driver_or_new(target, "USBAudioInputDriver")
+        drv.play()
 
     def _get_tmc(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
 
-        return self._get_driver_or_new(target, "USBTMCDriver", name=name)
+        return self._get_driver_or_new(target, "USBTMCDriver")
 
     def tmc_command(self):
         drv = self._get_tmc()
         command = ' '.join(self.args.command)
         if not command:
             raise UserError("no command given")
         if '?' in command:
@@ -1201,16 +1154,15 @@
             data = drv.get_channel_values(channel)
         for k, v in sorted(data.items()):
             print(f"{k:<16s} {str(v):<10s}")
 
     def write_image(self):
         place = self.get_acquired_place()
         target = self._get_target(place)
-        name = self.args.name
-        drv = self._get_driver_or_new(target, "USBStorageDriver", activate=False, name=name)
+        drv = self._get_driver_or_new(target, "USBStorageDriver", activate=False)
         drv.storage.timeout = self.args.wait
         target.activate(drv)
 
         try:
             drv.write_image(self.args.filename, partition=self.args.partition, skip=self.args.skip,
                             seek=self.args.seek, mode=self.args.write_mode)
         except subprocess.CalledProcessError as e:
@@ -1410,24 +1362,24 @@
     )
 
     # Support both legacy variables and properly namespaced ones
     place = os.environ.get('PLACE', None)
     place = os.environ.get('LG_PLACE', place)
     state = os.environ.get('STATE', None)
     state = os.environ.get('LG_STATE', state)
-    initial_state = os.environ.get('LG_INITIAL_STATE', None)
     token = os.environ.get('LG_TOKEN', None)
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '-x',
         '--crossbar',
         metavar='URL',
         type=str,
-        help="crossbar websocket URL (default: value from env variable LG_CROSSBAR, otherwise ws://127.0.0.1:20408/ws)"
+        default=os.environ.get("LG_CROSSBAR", "ws://127.0.0.1:20408/ws"),
+        help="crossbar websocket URL (default: %(default)s)"
     )
     parser.add_argument(
         '-c',
         '--config',
         type=str,
         default=os.environ.get("LG_ENV"),
         help="config file"
@@ -1443,21 +1395,14 @@
         '-s',
         '--state',
         type=str,
         default=state,
         help="strategy state to switch into before command"
     )
     parser.add_argument(
-        '-i',
-        '--initial-state',
-        type=str,
-        default=initial_state,
-        help="strategy state to force into before switching to desired state"
-    )
-    parser.add_argument(
         '-d',
         '--debug',
         action='store_true',
         default=False,
         help="enable debug mode (show python tracebacks)"
     )
     parser.add_argument(
@@ -1588,15 +1533,14 @@
 
     subparser = subparsers.add_parser('power',
                                       aliases=('pw',),
                                       help="change (or get) a place's power status")
     subparser.add_argument('action', choices=['on', 'off', 'cycle', 'get'])
     subparser.add_argument('-t', '--delay', type=float, default=None,
                            help='wait time in seconds between off and on during cycle')
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.power)
 
     subparser = subparsers.add_parser('io',
                                       help="change (or get) a digital IO status")
     subparser.add_argument('action', choices=['high', 'low', 'get'], help="action")
     subparser.add_argument('name', help="optional resource name", nargs='?')
     subparser.set_defaults(func=ClientSession.digital_io)
@@ -1615,52 +1559,46 @@
     subparser = subparsers.add_parser('dfu',
                                       help="communicate with device in DFU mode")
     subparser.add_argument('action', choices=['download', 'detach', 'list'], help='action')
     subparser.add_argument('altsetting', help='altsetting name or number (download, detach only)',
                            nargs='?')
     subparser.add_argument('filename', help='file to write into device (download only)', nargs='?')
     subparser.add_argument('--wait', type=float, default=10.0)
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.dfu)
 
     subparser = subparsers.add_parser('fastboot',
                                       help="run fastboot")
     subparser.add_argument('fastboot_args', metavar='ARG', nargs=argparse.REMAINDER,
                            help='fastboot arguments')
     subparser.add_argument('--wait', type=float, default=10.0)
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.fastboot)
 
     subparser = subparsers.add_parser('flashscript',
                                       help="run flash script")
     subparser.add_argument('script', help="Flashing script")
     subparser.add_argument('script_args', metavar='ARG', nargs=argparse.REMAINDER,
                            help='script arguments')
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.flashscript)
 
     subparser = subparsers.add_parser('bootstrap',
                                       help="start a bootloader")
     subparser.add_argument('-w', '--wait', type=float, default=10.0)
     subparser.add_argument('filename', help='filename to boot on the target')
     subparser.add_argument('bootstrap_args', metavar='ARG', nargs=argparse.REMAINDER,
                            help='extra bootstrap arguments')
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.bootstrap)
 
     subparser = subparsers.add_parser('sd-mux',
                                       help="switch USB SD Muxer or get current mode")
     subparser.add_argument('action', choices=['dut', 'host', 'off', 'client', 'get'])
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.sd_mux)
 
     subparser = subparsers.add_parser('usb-mux',
                                       help="switch USB Muxer")
     subparser.add_argument('links', choices=['off', 'dut-device', 'host-dut', 'host-device', 'host-dut+host-device'])
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.usb_mux)
 
     subparser = subparsers.add_parser('ssh',
                                       help="connect via ssh (with optional arguments)",
                                       epilog="Additional arguments are passed to the ssh subprocess.")
     subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.ssh)
@@ -1704,24 +1642,21 @@
 
     subparser = subparsers.add_parser('video',
                                       help="start a video stream")
     subparser.add_argument('-q', '--quality', type=str,
                            help="select a video quality (use 'list' to show options)")
     subparser.add_argument('-c', '--controls', type=str,
                            help="configure v4l controls (such as 'focus_auto=0,focus_absolute=40')")
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.video)
 
     subparser = subparsers.add_parser('audio', help="start a audio stream")
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.set_defaults(func=ClientSession.audio)
 
     tmc_parser = subparsers.add_parser('tmc', help="control a USB TMC device")
-    tmc_parser.add_argument('--name', '-n', help="optional resource name")
-    tmc_parser.set_defaults(func=lambda _: tmc_parser.print_help(file=sys.stderr))
+    tmc_parser.set_defaults(func=lambda _: tmc_parser.print_help())
     tmc_subparsers = tmc_parser.add_subparsers(
         dest='subcommand',
         title='available subcommands',
         metavar="SUBCOMMAND",
     )
 
     tmc_subparser = tmc_subparsers.add_parser('cmd',
@@ -1751,15 +1686,14 @@
     subparser.add_argument('--skip', type=int, default=0,
                            help="skip n 512-sized blocks at start of input")
     subparser.add_argument('--seek', type=int, default=0,
                            help="skip n 512-sized blocks at start of output")
     subparser.add_argument('--mode', dest='write_mode',
                            type=Mode, choices=Mode, default=Mode.DD,
                            help="Choose tool for writing images (default: %(default)s)")
-    subparser.add_argument('--name', '-n', help="optional resource name")
     subparser.add_argument('filename', help='filename to boot on the target')
     subparser.set_defaults(func=ClientSession.write_image)
 
     subparser = subparsers.add_parser('reserve', help="create a reservation")
     subparser.add_argument('--wait', action='store_true',
                            help="wait until the reservation is allocated")
     subparser.add_argument('--shell', action='store_true',
@@ -1796,37 +1730,33 @@
         args.leftover = leftover
 
     if args.verbose:
         logging.getLogger().setLevel(logging.INFO)
     if args.debug or args.verbose > 1:
         logging.getLogger().setLevel(logging.DEBUG)
 
-    if not args.config and (args.state or args.initial_state):
-        print("Setting the state requires a configuration file", file=sys.stderr)
-        exit(1)
-    if args.initial_state and not args.state:
-        print("Setting the initial state requires a desired state", file=sys.stderr)
+    if not args.config and args.state:
+        print("Setting the state requires a configuration file")
         exit(1)
 
     if args.proxy:
         proxymanager.force_proxy(args.proxy)
 
     env = None
     if args.config:
         env = Environment(config_file=args.config)
 
     role = None
-    if args.command != 'reserve' and env and env.config.get_targets():
+    if env and env.config.get_targets():
         if args.place:
-            if not args.place.startswith('+'):
-                role = find_role_by_place(env.config.get_targets(), args.place)
-                if not role:
-                    print(f"RemotePlace {args.place} not found in configuration file", file=sys.stderr)
-                    exit(1)
-                print(f"Selected role {role} from configuration file")
+            role = find_role_by_place(env.config.get_targets(), args.place)
+            if not role:
+                print(f"RemotePlace {args.place} not found in configuration file", file=sys.stderr)
+                exit(1)
+            print(f"Selected role {role} from configuration file")
         else:
             role, args.place = find_any_role_with_place(env.config.get_targets())
             if not role:
                 print("No RemotePlace found in configuration file", file=sys.stderr)
                 exit(1)
             print(f"Selected role {role} and place {args.place} from configuration file")
 
@@ -1838,30 +1768,16 @@
     }
 
     if args.command and args.command != 'help':
         exitcode = 0
         try:
             signal.signal(signal.SIGTERM, lambda *_: sys.exit(0))
 
-            try:
-                crossbar_url = args.crossbar or env.config.get_option('crossbar_url')
-            except (AttributeError, KeyError):
-                # in case of no env or not set, use LG_CROSSBAR env variable or default
-                crossbar_url = os.environ.get("LG_CROSSBAR", "ws://127.0.0.1:20408/ws")
-
-            try:
-                crossbar_realm = env.config.get_option('crossbar_realm')
-            except (AttributeError, KeyError):
-                # in case of no env, use LG_CROSSBAR_REALM env variable or default
-                crossbar_realm = os.environ.get("LG_CROSSBAR_REALM", "realm1")
-
-            logging.debug('Starting session with "%s", realm: "%s"', crossbar_url,
-                    crossbar_realm)
-
-            session = start_session(crossbar_url, crossbar_realm, extra)
+            session = start_session(args.crossbar, os.environ.get("LG_CROSSBAR_REALM", "realm1"),
+                                    extra)
             try:
                 if asyncio.iscoroutinefunction(args.func):
                     if getattr(args.func, 'needs_target', False):
                         place = session.get_acquired_place()
                         target = session._get_target(place)
                         coro = args.func(session, place, target)
                     else:
@@ -1869,49 +1785,45 @@
                     session.loop.run_until_complete(coro)
                 else:
                     args.func(session)
             finally:
                 session.loop.close()
         except (NoResourceFoundError, NoDriverFoundError, InvalidConfigError) as e:
             if args.debug:
-                traceback.print_exc(file=sys.stderr)
+                traceback.print_exc()
             else:
                 print(f"{parser.prog}: error: {e}", file=sys.stderr)
 
             if isinstance(e, NoResourceFoundError):
                 if e.found:
-                    print("Found multiple resources but no name was given, available names:", file=sys.stderr)
+                    print("Found multiple resources but no name was given, available names:")
                     for res in e.found:
-                        print(f"{res.name}", file=sys.stderr)
+                        print(f"{res.name}")
                 else:
                     print("This may be caused by disconnected exporter or wrong match entries.\nYou can use the 'show' command to review all matching resources.", file=sys.stderr)  # pylint: disable=line-too-long
             elif isinstance(e, NoDriverFoundError):
                 print("This is likely caused by an error or missing driver in the environment configuration.", file=sys.stderr)  # pylint: disable=line-too-long
             elif isinstance(e, InvalidConfigError):
                 print("This is likely caused by an error in the environment configuration or invalid\nresource information provided by the coordinator.", file=sys.stderr)  # pylint: disable=line-too-long
 
             exitcode = 1
         except ConnectionError as e:
-            print(f"Could not connect to coordinator: {e}", file=sys.stderr)
+            print(f"Could not connect to coordinator: {e}")
             exitcode = 1
-        except InteractiveCommandError as e:
-            if args.debug:
-                traceback.print_exc(file=sys.stderr)
-            exitcode = e.exitcode
         except Error as e:
             if args.debug:
-                traceback.print_exc(file=sys.stderr)
+                traceback.print_exc()
             else:
                 print(f"{parser.prog}: error: {e}", file=sys.stderr)
             exitcode = 1
         except KeyboardInterrupt:
             exitcode = 1
         except Exception:  # pylint: disable=broad-except
-            traceback.print_exc(file=sys.stderr)
+            traceback.print_exc()
             exitcode = 2
         exit(exitcode)
     else:
-        parser.print_help(file=sys.stderr)
+        parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `labgrid-23.0.1/labgrid/remote/common.py` & `labgrid-23.0b2/labgrid/remote/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/remote/config.py` & `labgrid-23.0b2/labgrid/remote/config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/remote/coordinator.py` & `labgrid-23.0b2/labgrid/remote/coordinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """The coordinator module coordinates exported resources and clients accessing them."""
 # pylint: disable=no-member,unused-argument
 import asyncio
-import sys
 import traceback
 from collections import defaultdict
 from os import environ
 from pprint import pprint
 from enum import Enum
 from functools import wraps
 
@@ -589,15 +588,15 @@
             for resource in resources:
                 # this triggers an update from the exporter which is published
                 # to the clients
                 await self.call(f'org.labgrid.exporter.{resource.path[0]}.acquire',
                                 resource.path[1], resource.path[3], place.name)
                 acquired.append(resource)
         except:
-            print(f"failed to acquire {resource}", file=sys.stderr)
+            print(f"failed to acquire {resource}")
             # cleanup
             await self._release_resources(place, acquired)
             return False
 
         for resource in resources:
             place.acquired_resources.append(resource)
 
@@ -616,15 +615,15 @@
             try:
                 # this triggers an update from the exporter which is published
                 # to the clients
                 if callback:
                     await self.call(f'org.labgrid.exporter.{resource.path[0]}.release',
                                     resource.path[1], resource.path[3])
             except:
-                print(f"failed to release {resource}", file=sys.stderr)
+                print(f"failed to release {resource}")
                 # at leaset try to notify the clients
                 try:
                     self._publish_resource(resource)
                 except:
                     pass
 
     @locked
```

### Comparing `labgrid-23.0.1/labgrid/remote/exporter.py` & `labgrid-23.0b2/labgrid/remote/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,29 +764,29 @@
                     # this may call back to acquire the resource immediately
                     await self.add_resource(
                         group_name, resource_name, cls, params
                     )
                     self.checkpoint = time.monotonic()
 
         except Exception:  # pylint: disable=broad-except
-            traceback.print_exc(file=sys.stderr)
+            traceback.print_exc()
             self.loop.stop()
             return
 
         self.poll_task = self.loop.create_task(self.poll())
 
     async def onLeave(self, details):
         """Cleanup after leaving the coordinator connection"""
         if self.poll_task:
             self.poll_task.cancel()
             await asyncio.wait([self.poll_task])
         super().onLeave(details)
 
     async def onDisconnect(self):
-        print("connection lost", file=sys.stderr)
+        print("connection lost")
         global reexec
         reexec = True
         if self.poll_task:
             self.poll_task.cancel()
             await asyncio.wait([self.poll_task])
             await asyncio.sleep(0.5) # give others a chance to clean up
         self.loop.stop()
@@ -814,15 +814,15 @@
             for resource_name, resource in group.items():
                 if not isinstance(resource, ResourceExport):
                     continue
                 try:
                     changed = resource.poll()
                 except Exception:  # pylint: disable=broad-except
                     print(f"Exception while polling {resource}", file=sys.stderr)
-                    traceback.print_exc(file=sys.stderr)
+                    traceback.print_exc()
                     continue
                 if changed:
                     await self.update_resource(group_name, resource_name)
                 else:
                     # let other tasks run, see https://github.com/python/asyncio/issues/284
                     await asyncio.sleep(0)
 
@@ -830,18 +830,18 @@
         while True:
             try:
                 await asyncio.sleep(0.25)
                 await self._poll_step()
             except asyncio.CancelledError:
                 break
             except Exception:  # pylint: disable=broad-except
-                traceback.print_exc(file=sys.stderr)
+                traceback.print_exc()
             age = time.monotonic() - self.checkpoint
             if age > 300:
-                print(f"missed checkpoint, exiting (last was {age} seconds ago)", file=sys.stderr)
+                print(f"missed checkpoint, exiting (last was {age} seconds ago)")
                 self.disconnect()
 
     async def add_resource(self, group_name, resource_name, cls, params):
         """Add a resource to the exporter and update status on the coordinator"""
         print(
             f"add resource {group_name}/{resource_name}: {cls}/{params}"
         )
```

### Comparing `labgrid-23.0.1/labgrid/remote/scheduler.py` & `labgrid-23.0b2/labgrid/remote/scheduler.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/__init__.py` & `labgrid-23.0b2/labgrid/resource/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,8 +18,7 @@
 from .flashrom import Flashrom, NetworkFlashrom
 from .docker import DockerManager, DockerDaemon, DockerConstants
 from .lxaiobus import LXAIOBusPIO
 from .pyvisa import PyVISADevice
 from .provider import TFTPProvider
 from .mqtt import TasmotaPowerPort
 from .httpvideostream import HTTPVideoStream
-from .dediprogflasher import DediprogFlasher, NetworkDediprogFlasher
```

### Comparing `labgrid-23.0.1/labgrid/resource/base.py` & `labgrid-23.0b2/labgrid/resource/base.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/common.py` & `labgrid-23.0b2/labgrid/resource/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/docker.py` & `labgrid-23.0b2/labgrid/resource/docker.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/ethernetport.py` & `labgrid-23.0b2/labgrid/resource/ethernetport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import subprocess
-import sys
 from time import time
 import attr
 
 from ..factory import target_factory
 from .common import ManagedResource, ResourceManager
 
 @attr.s
@@ -243,15 +242,15 @@
                 try:
                     await asyncio.sleep(1.0)
                     await handler(self)
                 except asyncio.CancelledError:
                     break
                 except Exception:  # pylint: disable=broad-except
                     import traceback
-                    traceback.print_exc(file=sys.stderr)
+                    traceback.print_exc()
 
         self.loop = asyncio.get_event_loop()
         self.poll_tasks.append(self.loop.create_task(poll(self, poll_neighbour)))
         self.poll_tasks.append(self.loop.create_task(poll(self, poll_switches)))
 
     @staticmethod
     def _get_neigh():
```

### Comparing `labgrid-23.0.1/labgrid/resource/lxaiobus.py` & `labgrid-23.0b2/labgrid/resource/lxaiobus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/modbus.py` & `labgrid-23.0b2/labgrid/resource/modbus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/modbusrtu.py` & `labgrid-23.0b2/labgrid/resource/modbusrtu.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/mqtt.py` & `labgrid-23.0b2/labgrid/resource/mqtt.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/onewireport.py` & `labgrid-23.0b2/labgrid/resource/onewireport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/power.py` & `labgrid-23.0b2/labgrid/resource/power.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/provider.py` & `labgrid-23.0b2/labgrid/resource/provider.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/pyvisa.py` & `labgrid-23.0b2/labgrid/resource/pyvisa.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/remote.py` & `labgrid-23.0b2/labgrid/resource/remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/serialport.py` & `labgrid-23.0b2/labgrid/resource/serialport.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/sigrok.py` & `labgrid-23.0b2/labgrid/resource/sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/suggest.py` & `labgrid-23.0b2/labgrid/resource/suggest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/resource/udev.py` & `labgrid-23.0b2/labgrid/resource/udev.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/step.py` & `labgrid-23.0b2/labgrid/step.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/stepreporter.py` & `labgrid-23.0b2/labgrid/stepreporter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 from .step import steps
 
 
 class StepReporter:
-    _started = False
-
-    def __init__(self):
-        from warnings import warn
-
-        warn(
-            "StepReporter should not be instantiated, use StepReporter.start()/.stop() instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
+    instance = None
 
     @classmethod
     def start(cls):
         """starts the StepReporter"""
-        assert not cls._started
-        steps.subscribe(cls.notify)
-        cls._started = True
+        assert cls.instance is None
+        cls.instance = cls()
 
     @classmethod
     def stop(cls):
         """stops the StepReporter"""
-        assert cls._started
+        assert cls.instance is not None
         steps.unsubscribe(cls.notify)
-        cls._started = False
+        cls.instance = None
+
+    def __init__(self):
+        steps.subscribe(StepReporter.notify)
 
     @staticmethod
     def notify(event):
         # ignore tagged events
         if event.step.tag:
             return
```

### Comparing `labgrid-23.0.1/labgrid/strategy/bareboxstrategy.py` & `labgrid-23.0b2/labgrid/strategy/bareboxstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/strategy/common.py` & `labgrid-23.0b2/labgrid/strategy/common.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/strategy/dockerstrategy.py` & `labgrid-23.0b2/labgrid/strategy/dockerstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/strategy/graphstrategy.py` & `labgrid-23.0b2/labgrid/strategy/graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/strategy/shellstrategy.py` & `labgrid-23.0b2/labgrid/strategy/shellstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/strategy/ubootstrategy.py` & `labgrid-23.0b2/labgrid/strategy/ubootstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/target.py` & `labgrid-23.0b2/labgrid/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import abc
 import atexit
 import logging
-import sys
 from time import monotonic, sleep
 
 import attr
 
 from .binding import BindingError, BindingState
 from .driver import Driver
 from .exceptions import NoSupplierFoundError, NoDriverFoundError, NoResourceFoundError, NoStrategyFoundError
@@ -113,33 +112,24 @@
         Arguments:
         cls -- resource-class to return as a resource
         name -- optional name to use as a filter
         wait_avail -- wait for the resource to become available (default True)
         """
         found = []
         other_names = []
-        default = None
         if isinstance(cls, str):
             cls = target_factory.class_from_string(cls)
 
         for res in self.resources:
             if not isinstance(res, cls):
                 continue
-            if res.name == "default":
-                default = res
             if name and res.name != name:
                 other_names.append(res.name)
                 continue
             found.append(res)
-
-        # if no explicit resource name is requested and a "default" resource was saved and
-        # multiple resources were found, use the default resource
-        if not name and default and len(found) != 1:
-            found = [default]
-
         if not found:
             name_msg = f" named '{name}'" if name else ""
             if other_names:
                 raise NoResourceFoundError(
                     f"no {cls} resource{name_msg} found in {self}, matching resources with other names: {other_names}"  # pylint: disable=line-too-long
                 )
 
@@ -505,18 +495,18 @@
             self.deactivate(drv)
 
     def _atexit_cleanup(self):
         try:
             self.cleanup()
         except Exception as e:
             print("An exception occured during cleanup, call the cleanup() "
-                  "method on targets yourself to handle exceptions explictly.", file=sys.stderr)
-            print(f"Error: {e}", file=sys.stderr)
+                  "method on targets yourself to handle exceptions explictly.")
+            print(f"Error: {e}")
             import traceback
-            traceback.print_exc(file=sys.stderr)
+            traceback.print_exc()
 
     def export(self):
         """
         Export information from drivers.
 
         All drivers are deactivated before being exported, unless their
         skip_deactivate_on_export property is true.
```

### Comparing `labgrid-23.0.1/labgrid/util/agent.py` & `labgrid-23.0b2/labgrid/util/agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/agents/deditec_relais8.py` & `labgrid-23.0b2/labgrid/util/agents/deditec_relais8.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/agents/network_interface.py` & `labgrid-23.0b2/labgrid/util/agents/network_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         super().__init__(daemon=True)
 
     def run(self):
         try:
             GLib.MainLoop(None).run()
         except Exception:
             import traceback
-            traceback.print_exc(file=sys.stderr)
+            traceback.print_exc()
             sys.exit(1)
 
     def block_on(self, func, *args, **kwargs):
         done = threading.Event()
         result = [None]
 
         def cb(data):
```

### Comparing `labgrid-23.0.1/labgrid/util/agents/sysfsgpio.py` & `labgrid-23.0b2/labgrid/util/agents/sysfsgpio.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/agents/usb_hid_relay.py` & `labgrid-23.0b2/labgrid/util/agents/usb_hid_relay.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/agentwrapper.py` & `labgrid-23.0b2/labgrid/util/agentwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/dict.py` & `labgrid-23.0b2/labgrid/util/dict.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/expect.py` & `labgrid-23.0b2/labgrid/util/expect.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/helper.py` & `labgrid-23.0b2/labgrid/util/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,29 @@
 
 @attr.s
 class ProcessWrapper:
     callbacks = attr.ib(default=attr.Factory(list))
     loglevel = logging.INFO
 
     @step(args=['command'], result=True, tag='process')
-    def check_output(self, command, *, print_on_silent_log=False, input=None, stdin=None): # pylint: disable=redefined-builtin
+    def check_output(self, command, *, print_on_silent_log=False, input=None): # pylint: disable=redefined-builtin
         """Run a command and supply the output to callback functions"""
         logger = logging.getLogger("Process")
         res = []
         mfd, sfd = pty.openpty()
         set_nonblocking(mfd)
 
         kwargs = {}
 
         stdin_r = None
         stdin_w = None
         if input is not None:
             stdin_r, stdin_w = os.pipe()
             kwargs['stdin'] = stdin_r
             set_nonblocking(stdin_w)
-        elif stdin is not None:
-            kwargs['stdin'] = stdin
 
         process = subprocess.Popen(command, stderr=sfd,
                                    stdout=sfd, bufsize=0, **kwargs)
 
         logger.log(ProcessWrapper.loglevel, "[%d] command: %s", process.pid, " ".join(command))
 
         # do not register/unregister already registered print_callback
```

### Comparing `labgrid-23.0.1/labgrid/util/managedfile.py` & `labgrid-23.0b2/labgrid/util/managedfile.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/proxy.py` & `labgrid-23.0b2/labgrid/util/proxy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/qmp.py` & `labgrid-23.0b2/labgrid/util/qmp.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     def _read_parse_json(self):
         line = self.monitor_out.readline().decode('utf-8')
         self.logger.debug("Received line: %s", line.rstrip("\r\n"))
         if not line:
             raise QMPError("Received empty response")
         return json.loads(line)
 
-    def execute(self, command, arguments={}):
-        json_command = {"execute": command, "arguments": arguments}
+    def execute(self, command):
+        json_command = {"execute": command}
 
         self.monitor_in.write(json.dumps(json_command).encode("utf-8"))
         self.monitor_in.write("\n".encode("utf-8"))
         self.monitor_in.flush()
 
         answer = self._read_parse_json()
         # skip all asynchronous events
```

### Comparing `labgrid-23.0.1/labgrid/util/ssh.py` & `labgrid-23.0b2/labgrid/util/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from select import select
 from functools import wraps
 from typing import Dict
 
 import attr
 from ..driver.exception import ExecutionError
 
-from .helper import get_free_port, processwrapper
+from .helper import get_free_port
 
 __all__ = ['sshmanager', 'SSHConnection', 'ForwardError']
 
 def get_ssh_connect_timeout():
     return int(os.environ.get("LG_SSH_CONNECT_TIMEOUT", 30))
 
 
@@ -325,18 +325,17 @@
         complete_cmd = ["rsync", "--compress", "--sparse", "--copy-links", "--verbose", "--progress", "--times", "-e",
                         " ".join(['ssh'] + self._get_ssh_args())]
         complete_cmd += [
             f"{local_file}",
             f"{self.host}:{remote_path}"
         ]
         self._logger.debug("Running command: %s", complete_cmd)
-        processwrapper.check_output(
+        subprocess.check_call(
             complete_cmd,
             stdin=subprocess.DEVNULL,
-            print_on_silent_log=True
         )
 
     @_check_connected
     def add_port_forward(self, remote_host, remote_port, local_port=None):
         """forward command"""
         if local_port is None:
             local_port = get_free_port()
```

### Comparing `labgrid-23.0.1/labgrid/util/timeout.py` & `labgrid-23.0b2/labgrid/util/timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid/util/yaml.py` & `labgrid-23.0b2/labgrid/util/yaml.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/labgrid.egg-info/PKG-INFO` & `labgrid-23.0b2/labgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labgrid
-Version: 23.0.1
+Version: 23.0b2
 Summary: embedded systems control library for development, testing and installation
 Author-email: Rouven Czerwinski <entwicklung@pengutronix.de>, Jan Luebbe <entwicklung@pengutronix.de>
 License: Copyright (C) 2016-2017 Pengutronix, Jan Luebbe <entwicklung@pengutronix.de>
         Copyright (C) 2016-2017 Pengutronix, Rouven Czerwinski <entwicklung@pengutronix.de>
         
         This library is free software; you can redistribute it and/or
         modify it under the terms of the GNU Lesser General Public
@@ -44,15 +44,14 @@
 Provides-Extra: pyvisa
 Provides-Extra: snmp
 Provides-Extra: vxi11
 Provides-Extra: xena
 Provides-Extra: deb
 Provides-Extra: dev
 License-File: LICENSE
-License-File: COPYING
 
 .. image:: labgrid_logo.png
    :alt: labgrid logo
    :align: center
 
 Welcome to labgrid
 ==================
@@ -171,10 +170,10 @@
     :alt: documentation status
     :target: https://labgrid.readthedocs.io/en/latest/?badge=latest
 
 .. |chat| image:: https://matrix.to/img/matrix-badge.svg
     :alt: chat
     :target: https://app.element.io/#/room/#labgrid:matrix.org
 
-.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.%5BMICRO%5D-22bfda.svg
+.. |calver| image:: https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg 
     :alt: chat
     :target: https://calver.org/
```

### Comparing `labgrid-23.0.1/labgrid.egg-info/SOURCES.txt` & `labgrid-23.0b2/labgrid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,14 @@
 examples/modbusrtu/test_modbusrtu_example.py
 examples/networkmanager/nm.env
 examples/networkmanager/nm.py
 examples/power/env.yaml
 examples/power/power_example.py
 examples/pyvisa/env.yaml
 examples/pyvisa/pyvisa_example.py
-examples/qemu-networking/conftest.py
-examples/qemu-networking/local.yaml
-examples/qemu-networking/qemunetworkstrategy.py
-examples/qemu-networking/test_qemu_networking.py
 examples/remote/remote.yaml
 examples/remote/test_barebox.py
 examples/shell/conftest.py
 examples/shell/local.yaml
 examples/shell/test_hwclock.py
 examples/shell/test_memory.py
 examples/shell/test_rt.py
@@ -157,15 +153,14 @@
 labgrid/autoinstall/__init__.py
 labgrid/autoinstall/main.py
 labgrid/driver/__init__.py
 labgrid/driver/bareboxdriver.py
 labgrid/driver/commandmixin.py
 labgrid/driver/common.py
 labgrid/driver/consoleexpectmixin.py
-labgrid/driver/dediprogflashdriver.py
 labgrid/driver/deditecrelaisdriver.py
 labgrid/driver/dfudriver.py
 labgrid/driver/dockerdriver.py
 labgrid/driver/exception.py
 labgrid/driver/externalconsoledriver.py
 labgrid/driver/fake.py
 labgrid/driver/fastbootdriver.py
@@ -204,27 +199,25 @@
 labgrid/driver/usbstoragedriver.py
 labgrid/driver/usbtmcdriver.py
 labgrid/driver/usbvideodriver.py
 labgrid/driver/xenadriver.py
 labgrid/driver/power/__init__.py
 labgrid/driver/power/apc.py
 labgrid/driver/power/digipower.py
-labgrid/driver/power/digitalloggers_http.py
 labgrid/driver/power/eaton.py
 labgrid/driver/power/eg_pms2_network.py
 labgrid/driver/power/gude.py
 labgrid/driver/power/gude24.py
 labgrid/driver/power/gude8031.py
 labgrid/driver/power/gude8225.py
 labgrid/driver/power/gude8316.py
 labgrid/driver/power/netio.py
 labgrid/driver/power/netio_kshell.py
 labgrid/driver/power/rest.py
 labgrid/driver/power/sentry.py
-labgrid/driver/power/shelly_gen1.py
 labgrid/driver/power/siglent.py
 labgrid/driver/power/simplerest.py
 labgrid/driver/power/tplink.py
 labgrid/driver/usbtmc/__init__.py
 labgrid/driver/usbtmc/keysight_dsox2000.py
 labgrid/driver/usbtmc/tektronix_tds2000.py
 labgrid/protocol/__init__.py
@@ -251,15 +244,14 @@
 labgrid/remote/config.py
 labgrid/remote/coordinator.py
 labgrid/remote/exporter.py
 labgrid/remote/scheduler.py
 labgrid/resource/__init__.py
 labgrid/resource/base.py
 labgrid/resource/common.py
-labgrid/resource/dediprogflasher.py
 labgrid/resource/docker.py
 labgrid/resource/ethernetport.py
 labgrid/resource/fastboot.py
 labgrid/resource/flashrom.py
 labgrid/resource/httpvideostream.py
 labgrid/resource/lxaiobus.py
 labgrid/resource/modbus.py
@@ -318,15 +310,14 @@
 man/labgrid-suggest.rst
 tests/conftest.py
 tests/test_agent.py
 tests/test_autoinstall.py
 tests/test_bareboxdriver.py
 tests/test_config.py
 tests/test_crossbar.py
-tests/test_dediprogflasher.py
 tests/test_docker.py
 tests/test_environment.py
 tests/test_ethernetport.py
 tests/test_export.py
 tests/test_externalconsoledriver.py
 tests/test_factory.py
 tests/test_filedigitaloutput.py
```

### Comparing `labgrid-23.0.1/labgrid.egg-info/requires.txt` & `labgrid-23.0b2/labgrid.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ansicolors==1.1.8
 attrs==21.4.0
 autobahn==21.3.1
 jinja2==3.0.2
 packaging==21.0
 pexpect==4.8.0
-pyserial-labgrid>=3.4.0.1
-pytest==7.2.2
+pyserial@ git+https://github.com/labgrid-project/pyserial.git@v3.4.0.1
+pytest==6.2.5
 pyudev==0.22.0
 pyusb==1.2.1
 PyYAML==5.4.1
 requests==2.26.0
 xmodem==0.4.6
 
 [crossbar]
```

### Comparing `labgrid-23.0.1/labgrid_logo.png` & `labgrid-23.0b2/labgrid_logo.png`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-client.1` & `labgrid-23.0b2/man/labgrid-client.1`

 * *Files 11% similar despite different names*

```diff
@@ -57,18 +57,14 @@
 .BI \-c \ CONFIG\fR,\fB \ \-\-config \ CONFIG
 set the configuration file
 .TP
 .BI \-s \ STATE\fR,\fB \ \-\-state \ STATE
 set an initial state before executing a command, requires a configuration
 file and strategy
 .TP
-.BI \-i \ INITIAL_STATE\fR,\fB \ \-\-initial\-state \ INITIAL_STATE
-strategy state to force into before switching to desired state, requires a
-desired state (\fB\-s\fP/\fB\-\-state\fP/\fBLG_STATE\fP)
-.TP
 .B  \-d\fP,\fB  \-\-debug
 enable debugging
 .TP
 .B  \-v\fP,\fB  \-\-verbose
 increase verbosity
 .TP
 .BI \-P \ PROXY\fR,\fB \ \-\-proxy \ PROXY
@@ -88,21 +84,14 @@
 This variable can be used to specify a reservation for the \fBwait\fP command and
 for the \fB+\fP place expansion.
 .SS LG_STATE
 .sp
 This variable can be used to specify a state which the device transitions into
 before executing a command. Requires a configuration file and a Strategy
 specified for the device.
-.SS LG_INITIAL_STATE
-.sp
-This variable can be used to specify an initial state the device is known to
-be in.
-This is useful during development. The Strategy used must implement the
-\fBforce()\fP method.
-A desired state must be set using \fBLG_STATE\fP or \fB\-s\fP/\fB\-\-state\fP\&.
 .SS LG_ENV
 .sp
 This variable can be used to specify the configuration file to use without
 using the \fB\-\-config\fP option, the \fB\-\-config\fP option overrides it.
 .SS LG_CROSSBAR
 .sp
 This variable can be used to set the default crossbar URL (instead of using the
@@ -234,17 +223,14 @@
 .sp
 If a target contains multiple Resources of the same type, named matches need to
 be used to address the individual resources. In addition to the \fImatch\fP taken by
 \fIadd\-match\fP, \fIadd\-named\-match\fP also takes a name for the resource. The other
 client commands support the name as an optional parameter and will inform the
 user that a name is required if multiple resources are found, but no name is
 given.
-.sp
-If one of the resources should be used by default when no resource name is
-explicitly specified, it can be named \fBdefault\fP\&.
 .SH EXAMPLES
 .sp
 To retrieve a list of places run:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
```

### Comparing `labgrid-23.0.1/man/labgrid-client.rst` & `labgrid-23.0b2/man/labgrid-client.rst`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,14 @@
 -x URL, --crossbar URL
     the crossbar url of the coordinator, defaults to ``ws://127.0.0.1:20408/ws``
 -c CONFIG, --config CONFIG
     set the configuration file
 -s STATE, --state STATE
     set an initial state before executing a command, requires a configuration
     file and strategy
--i INITIAL_STATE, --initial-state INITIAL_STATE
-    strategy state to force into before switching to desired state, requires a
-    desired state (``-s``/``--state``/``LG_STATE``)
 -d, --debug
     enable debugging
 -v, --verbose
     increase verbosity
 -P PROXY, --proxy PROXY
     proxy connections over ssh
 
@@ -74,22 +71,14 @@
 
 LG_STATE
 ~~~~~~~~
 This variable can be used to specify a state which the device transitions into
 before executing a command. Requires a configuration file and a Strategy
 specified for the device.
 
-LG_INITIAL_STATE
-~~~~~~~~~~~~~~~~
-This variable can be used to specify an initial state the device is known to
-be in.
-This is useful during development. The Strategy used must implement the
-``force()`` method.
-A desired state must be set using ``LG_STATE`` or ``-s``/``--state``.
-
 LG_ENV
 ~~~~~~
 This variable can be used to specify the configuration file to use without
 using the ``--config`` option, the ``--config`` option overrides it.
 
 LG_CROSSBAR
 ~~~~~~~~~~~
@@ -228,17 +217,14 @@
 If a target contains multiple Resources of the same type, named matches need to
 be used to address the individual resources. In addition to the `match` taken by
 `add-match`, `add-named-match` also takes a name for the resource. The other
 client commands support the name as an optional parameter and will inform the
 user that a name is required if multiple resources are found, but no name is
 given.
 
-If one of the resources should be used by default when no resource name is
-explicitly specified, it can be named ``default``.
-
 EXAMPLES
 --------
 
 To retrieve a list of places run:
 
 .. code-block:: bash
```

### Comparing `labgrid-23.0.1/man/labgrid-exporter.1` & `labgrid-23.0b2/man/labgrid-exporter.1`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-exporter.rst` & `labgrid-23.0b2/man/labgrid-exporter.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-pytest.7` & `labgrid-23.0b2/man/labgrid-pytest.7`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-pytest.rst` & `labgrid-23.0b2/man/labgrid-pytest.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-suggest.1` & `labgrid-23.0b2/man/labgrid-suggest.1`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/man/labgrid-suggest.rst` & `labgrid-23.0b2/man/labgrid-suggest.rst`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/pyproject.toml` & `labgrid-23.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 dependencies = [
     "ansicolors==1.1.8",
     "attrs==21.4.0",
     "autobahn==21.3.1",
     "jinja2==3.0.2",
     "packaging==21.0",
     "pexpect==4.8.0",
-    "pyserial-labgrid>=3.4.0.1",
-    "pytest==7.2.2",
+    "pyserial @ git+https://github.com/labgrid-project/pyserial.git@v3.4.0.1",
+    "pytest==6.2.5",
     "pyudev==0.22.0",
     "pyusb==1.2.1",
     "PyYAML==5.4.1",
     "requests==2.26.0",
     "xmodem==0.4.6",
 ]
 dynamic = ["version"]  # via setuptools_scm
```

### Comparing `labgrid-23.0.1/tests/conftest.py` & `labgrid-23.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_agent.py` & `labgrid-23.0b2/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_autoinstall.py` & `labgrid-23.0b2/tests/test_autoinstall.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_bareboxdriver.py` & `labgrid-23.0b2/tests/test_bareboxdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_config.py` & `labgrid-23.0b2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_crossbar.py` & `labgrid-23.0b2/tests/test_crossbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,44 +426,7 @@
     assert not exporter.isalive()
     assert exporter.exitstatus == 100
 
     with pexpect.spawn('python -m labgrid.remote.client -p test release') as spawn:
         spawn.expect(pexpect.EOF)
         spawn.close()
         assert spawn.exitstatus == 0, spawn.before.strip()
-
-def test_reservation_custom_config(place, exporter, tmpdir):
-    p = tmpdir.join("config.yaml")
-    p.write(
-    """
-    targets:
-      test1:
-        role: foo
-        resources:
-          RemotePlace:
-            name: test
-    """
-    )
-    with pexpect.spawn(f'python -m labgrid.remote.client -c {p} reserve --wait --shell board=bar name=test') as spawn:
-        spawn.expect(pexpect.EOF)
-        spawn.close()
-        assert spawn.exitstatus == 0, spawn.before.strip()
-        m = re.search(rb"^export LG_TOKEN=(\S+)$", spawn.before.replace(b'\r\n', b'\n'), re.MULTILINE)
-        s = re.search(rb"^Selected role$", spawn.before.replace(b'\r\n', b'\n'), re.MULTILINE)
-        assert m is not None, spawn.before.strip()
-        assert s is None, spawn.before.strip()
-        token = m.group(1)
-
-    env = os.environ.copy()
-    env['LG_TOKEN'] = token.decode('ASCII')
-
-    with pexpect.spawn(f'python -m labgrid.remote.client -c {p} -p + lock', env=env) as spawn:
-        spawn.expect("acquired place test")
-        spawn.expect(pexpect.EOF)
-        spawn.close()
-        assert spawn.exitstatus == 0, spawn.before.strip()
-
-    with pexpect.spawn(f'python -m labgrid.remote.client -c {p} -p + release', env=env) as spawn:
-        spawn.expect("released place test")
-        spawn.expect(pexpect.EOF)
-        spawn.close()
-        assert spawn.exitstatus == 0, spawn.before.strip()
```

### Comparing `labgrid-23.0.1/tests/test_docker.py` & `labgrid-23.0b2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_environment.py` & `labgrid-23.0b2/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_export.py` & `labgrid-23.0b2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_externalconsoledriver.py` & `labgrid-23.0b2/tests/test_externalconsoledriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_factory.py` & `labgrid-23.0b2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_filedigitaloutput.py` & `labgrid-23.0b2/tests/test_filedigitaloutput.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_fixtures.py` & `labgrid-23.0b2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_flags.py` & `labgrid-23.0b2/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_flashrom.py` & `labgrid-23.0b2/tests/test_flashrom.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_flashscript.py` & `labgrid-23.0b2/tests/test_flashscript.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_graphstrategy.py` & `labgrid-23.0b2/tests/test_graphstrategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_lxaiobus.py` & `labgrid-23.0b2/tests/test_lxaiobus.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_manualswitchdriver.py` & `labgrid-23.0b2/tests/test_manualswitchdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_modbusrtudriver.py` & `labgrid-23.0b2/tests/test_modbusrtudriver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from labgrid.resource.modbusrtu import ModbusRTU
 from labgrid.driver.modbusrtudriver import ModbusRTUDriver
 
 import pytest
 
+
 def test_resource_with_minimum_argument(target):
     dut = ModbusRTU(target, name=None, port="/dev/tty1", address=10)
 
     assert dut.port == "/dev/tty1"
     assert dut.address == 10
     assert dut.speed == 115200
     assert dut.timeout == 0.25
@@ -19,15 +20,14 @@
     assert dut.port == "/dev/tty1"
     assert dut.address == 10
     assert dut.speed == 9600
     assert dut.timeout == 0.5
 
 
 def test_driver(target, mocker):
-    pytest.importorskip("minimalmodbus")
     ModbusRTU(target, name=None, port="/dev/tty0", address=10)
     driver = ModbusRTUDriver(target, name=None)
 
     # Ensure pyserial will not try to open the port
     driver.resource.port = None
 
     target.activate(driver)
```

### Comparing `labgrid-23.0.1/tests/test_onewire.py` & `labgrid-23.0b2/tests/test_onewire.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_openocd.py` & `labgrid-23.0b2/tests/test_openocd.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_powerdriver.py` & `labgrid-23.0b2/tests/test_powerdriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -177,16 +177,14 @@
     @pytest.mark.parametrize(
         'host',
         (
             'http://example.com/{index}',
             'https://example.com/{index}',
             'http://example.com:1234/{index}',
             'https://example.com:1234/{index}',
-            'http://user:pass@example.com:1234/{index}',
-            'https://user:pass@example.com:1234/{index}',
         )
     )
     def test_create_backend_with_url_in_host(self, target, mocker, backend, host):
         get = mocker.patch('requests.get')
         get.return_value.text = '1'
         mocker.patch('requests.put')
 
@@ -199,68 +197,30 @@
         d.cycle()
         assert d.get() is True
 
         # the called URL should be similar to the one configured in the resource, but with
         # index and explicit port
         expected_host = host.format(index=index)
         url = urlparse(expected_host)
-        if url.port is None:
-            implicit_port = 443 if url.scheme == 'https' else 80
-            expected_host = expected_host.replace(url.netloc, f'{url.netloc}:{implicit_port}')
-
-        get.assert_called_with(expected_host)
-
-    @pytest.mark.parametrize(
-        'host',
-        (
-            'http://example.com',
-            'https://example.com',
-        )
-    )
-    def test_create_shelly_gen1_backend_with_url_in_host(self, target, mocker, host):
-        get = mocker.patch('requests.get')
-        get.return_value.text = '{"ison": true}'
-        mocker.patch('requests.post')
-
-        index = '0'
-        NetworkPowerPort(target, 'power', model='shelly_gen1', host=host, index=index)
-        d = NetworkPowerDriver(target, 'power')
-        target.activate(d)
-
-        d.cycle()
-        assert d.get() is True
-
-        # the called URL should be similar to the one configured in the resource, but with
-        # index and explicit port
-        expected_host = f"{host}/relay/{index}"
-        url = urlparse(expected_host)
-        if url.port is None:
+        if ':' not in url.netloc:
             implicit_port = 443 if url.scheme == 'https' else 80
             expected_host = expected_host.replace(url.netloc, f'{url.netloc}:{implicit_port}')
 
         get.assert_called_with(expected_host)
 
     def test_import_backends(self):
         import labgrid.driver.power
         import labgrid.driver.power.apc
+        import labgrid.driver.power.eaton
         import labgrid.driver.power.digipower
-        import labgrid.driver.power.digitalloggers_http
         import labgrid.driver.power.gude
         import labgrid.driver.power.gude24
+        import labgrid.driver.power.tplink
         import labgrid.driver.power.netio
         import labgrid.driver.power.netio_kshell
         import labgrid.driver.power.rest
         import labgrid.driver.power.sentry
         import labgrid.driver.power.eg_pms2_network
-        import labgrid.driver.power.shelly_gen1
-
-    def test_import_backend_eaton(self):
-        pytest.importorskip("pysnmp")
-        import labgrid.driver.power.eaton
-
-    def test_import_backend_tplink(self):
-        pytest.importorskip("kasa")
-        import labgrid.driver.power.tplink
 
     def test_import_backend_siglent(self):
         pytest.importorskip("vxi11")
         import labgrid.driver.power.siglent
```

### Comparing `labgrid-23.0.1/tests/test_processwrapper.py` & `labgrid-23.0b2/tests/test_processwrapper.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_qemudriver.py` & `labgrid-23.0b2/tests/test_qemudriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_remote.py` & `labgrid-23.0b2/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_reporter.py` & `labgrid-23.0b2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_resource.py` & `labgrid-23.0b2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_sched.py` & `labgrid-23.0b2/tests/test_sched.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_serialdriver.py` & `labgrid-23.0b2/tests/test_serialdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_shelldriver.py` & `labgrid-23.0b2/tests/test_shelldriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_sigrok.py` & `labgrid-23.0b2/tests/test_sigrok.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_sshdriver.py` & `labgrid-23.0b2/tests/test_sshdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_step.py` & `labgrid-23.0b2/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_stepreporter.py` & `labgrid-23.0b2/tests/test_stepreporter.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_strategy.py` & `labgrid-23.0b2/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_sysfsgpioagent.py` & `labgrid-23.0b2/tests/test_sysfsgpioagent.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_target.py` & `labgrid-23.0b2/tests/test_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,14 @@
         pass
 
     a = A(target, "aresource")
     assert isinstance(target.get_resource(A), A)
     assert target.get_resource(A) is a
     assert target.get_resource(A, name="aresource") is a
 
-    # make sure resources named "default" are prioritized
-    b = A(target, "default")
-    assert target.get_resource(A) is b
-    assert target.get_resource(A, name="aresource") is a
-
-def test_get_resource_multiple_no_default(target):
-    class A(Resource):
-        pass
-
-    a = A(target, "aresource")
-    b = A(target, "default")
-    with pytest.raises(NoResourceFoundError) as excinfo:
-        target.get_resource(A, name="nosuchresource")
 
 def test_get_driver(target):
     class A(Driver):
         pass
 
     a = A(target, "adriver")
     assert isinstance(target.get_driver(A), A)
```

### Comparing `labgrid-23.0.1/tests/test_tasmota.py` & `labgrid-23.0b2/tests/test_tasmota.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_timeout.py` & `labgrid-23.0b2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_ubootdriver.py` & `labgrid-23.0b2/tests/test_ubootdriver.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_usbtmc.py` & `labgrid-23.0b2/tests/test_usbtmc.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_util.py` & `labgrid-23.0b2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `labgrid-23.0.1/tests/test_yaml.py` & `labgrid-23.0b2/tests/test_yaml.py`

 * *Files identical despite different names*

