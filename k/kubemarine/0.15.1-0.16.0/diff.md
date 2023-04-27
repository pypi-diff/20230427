# Comparing `tmp/kubemarine-0.15.1.tar.gz` & `tmp/kubemarine-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.15.1.tar", last modified: Mon Apr  3 08:37:20 2023, max compression
+gzip compressed data, was "kubemarine-0.16.0.tar", last modified: Wed Apr 26 09:35:28 2023, max compression
```

## Comparing `kubemarine-0.15.1.tar` & `kubemarine-0.16.0.tar`

### file list

```diff
@@ -1,228 +1,235 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.896131 kubemarine-0.15.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-03 08:37:05.000000 kubemarine-0.15.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-03 08:37:05.000000 kubemarine-0.15.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12361 2023-04-03 08:37:20.896131 kubemarine-0.15.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-03 08:37:05.000000 kubemarine-0.15.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.872131 kubemarine-0.15.1/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-04-03 08:37:05.000000 kubemarine-0.15.1/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-04-03 08:37:05.000000 kubemarine-0.15.1/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.872131 kubemarine-0.15.1/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8380 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    44365 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.876131 kubemarine-0.15.1/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15402 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    24852 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     4563 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    15921 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    17948 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    40219 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    12557 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8408 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    17548 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     6769 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.876131 kubemarine-0.15.1/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    19878 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10879 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11275 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.880131 kubemarine-0.15.1/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    63662 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    19658 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.880131 kubemarine-0.15.1/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/patches/p1_reinstall_calico.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.880131 kubemarine-0.15.1/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    38375 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    15343 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     5157 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     6080 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    15117 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    18362 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.880131 kubemarine-0.15.1/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222145 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/calico-v3.22.2.yaml.original
--rw-r--r--   0 root         (0) root         (0)   239958 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/calico-v3.24.2.yaml.original
--rw-r--r--   0 root         (0) root         (0)     7725 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7725 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3053 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3053 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15440 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15907 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4910 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20599 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2620 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50473 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    73488 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5053 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26777 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1760 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1658 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    15470 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2371 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6679 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13644 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13169 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/configurations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27197 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    20794 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.868131 kubemarine-0.15.1/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/etalons/patches/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.884131 kubemarine-0.15.1/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.888131 kubemarine-0.15.1/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.888131 kubemarine-0.15.1/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.888131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.888131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.892131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.892131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)      672 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)      456 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     1376 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1620 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3096 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.892131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.892131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9465 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4857 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      503 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.892131 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4092 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5128 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1619 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2826 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.896131 kubemarine-0.15.1/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    30932 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.896131 kubemarine-0.15.1/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.896131 kubemarine-0.15.1/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.896131 kubemarine-0.15.1/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    10441 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    11252 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-04-03 08:37:05.000000 kubemarine-0.15.1/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:37:20.876131 kubemarine-0.15.1/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12361 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8387 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-03 08:37:20.000000 kubemarine-0.15.1/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2553 2023-04-03 08:37:05.000000 kubemarine-0.15.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 08:37:20.896131 kubemarine-0.15.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-03 08:37:05.000000 kubemarine-0.15.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.509318 kubemarine-0.16.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-26 09:35:14.000000 kubemarine-0.16.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-26 09:35:14.000000 kubemarine-0.16.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-04-26 09:35:28.509318 kubemarine-0.16.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-26 09:35:14.000000 kubemarine-0.16.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.485318 kubemarine-0.16.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-04-26 09:35:14.000000 kubemarine-0.16.0/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-04-26 09:35:14.000000 kubemarine-0.16.0/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.489318 kubemarine-0.16.0/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8380 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    44652 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15402 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23933 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    15921 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    17948 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    39980 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    12720 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8220 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    20046 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     6769 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6492 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3784 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    19878 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10879 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11275 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    63972 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    19658 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/patches/p1_helm_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.493318 kubemarine-0.16.0/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    38251 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14938 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    18029 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4910 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20629 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2620 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50542 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    74051 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5053 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26777 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1760 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1658 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    15470 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2371 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6679 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    13644 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    13192 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     5199 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    27019 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     9376 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.497318 kubemarine-0.16.0/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.485318 kubemarine-0.16.0/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/etalons/patches/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      615 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.501318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9465 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    32103 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.505318 kubemarine-0.16.0/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.509318 kubemarine-0.16.0/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    10441 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    13898 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-04-26 09:35:14.000000 kubemarine-0.16.0/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:35:28.489318 kubemarine-0.16.0/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8783 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-26 09:35:28.000000 kubemarine-0.16.0/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-04-26 09:35:14.000000 kubemarine-0.16.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 09:35:28.509318 kubemarine-0.16.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-04-26 09:35:14.000000 kubemarine-0.16.0/setup.py
```

### Comparing `kubemarine-0.15.1/LICENSE` & `kubemarine-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/PKG-INFO` & `kubemarine-0.16.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.15.1
+Version: 0.16.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
 Keywords: kubernetes,devops,administration,helm
@@ -32,36 +32,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -79,15 +79,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -98,15 +98,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.15.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -127,24 +127,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.15.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.16.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -172,42 +172,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.15.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.15.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.16.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.15.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.16.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.15.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.16.0/LICENSE)
```

### Comparing `kubemarine-0.15.1/README.md` & `kubemarine-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/bin/kubemarine` & `kubemarine-0.16.0/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/bin/kubemarine.cmd` & `kubemarine-0.16.0/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/__init__.py` & `kubemarine-0.16.0/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/__main__.py` & `kubemarine-0.16.0/kubemarine/__main__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/admission.py` & `kubemarine-0.16.0/kubemarine/admission.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,14 +602,21 @@
         for item in procedure_config["namespaces_defaults"]:
             if item.endswith("version"):
                 verify_version(item, procedure_config["namespaces_defaults"][item], minor_version)
 
     return inventory
 
 
+def enrich_default_admission(inventory, _):
+    minor_version = int(inventory["services"]["kubeadm"]["kubernetesVersion"].split('.')[1])
+    if not inventory["rbac"].get("admission"):
+        inventory["rbac"]["admission"] = "psp" if minor_version < 25 else "pss"
+    return inventory
+
+
 def manage_enrichment(inventory, cluster):
     admission_impl = inventory['rbac']['admission']
     if admission_impl == "psp":
         return manage_psp_enrichment(inventory, cluster)
     elif admission_impl == "pss":
         return manage_pss_enrichment(inventory, cluster)
```

### Comparing `kubemarine-0.15.1/kubemarine/apparmor.py` & `kubemarine-0.16.0/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/apt.py` & `kubemarine-0.16.0/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/audit.py` & `kubemarine-0.16.0/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/controlplane.py` & `kubemarine-0.16.0/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/__init__.py` & `kubemarine-0.16.0/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/action.py` & `kubemarine-0.16.0/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/annotations.py` & `kubemarine-0.16.0/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/cluster.py` & `kubemarine-0.16.0/kubemarine/core/cluster.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/connections.py` & `kubemarine-0.16.0/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/defaults.py` & `kubemarine-0.16.0/kubemarine/core/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from kubemarine.core.yaml_merger import default_merger
 
 # All enrichment procedures should not connect to any node.
 # The information about nodes should be collected within KubernetesCluster#detect_nodes_context().
 DEFAULT_ENRICHMENT_FNS = [
     "kubemarine.core.schema.verify_inventory",
     "kubemarine.core.defaults.merge_defaults",
+    "kubemarine.admission.enrich_default_admission",
     "kubemarine.kubernetes.add_node_enrichment",
     "kubemarine.kubernetes.remove_node_enrichment",
     "kubemarine.controlplane.controlplane_node_enrichment",
     "kubemarine.core.defaults.append_controlplain",
     "kubemarine.kubernetes.enrich_upgrade_inventory",
     "kubemarine.plugins.enrich_upgrade_inventory",
     "kubemarine.packages.enrich_inventory_associations",
@@ -62,15 +63,16 @@
     "kubemarine.packages.enrich_inventory_include_all",
     "kubemarine.audit.verify_inventory",
     "kubemarine.plugins.enrich_inventory",
     "kubemarine.plugins.verify_inventory",
     "kubemarine.plugins.builtin.verify_inventory",
     "kubemarine.coredns.enrich_add_hosts_config",
     "kubemarine.k8s_certs.renew_verify",
-    "kubemarine.cri.enrich_inventory"
+    "kubemarine.cri.enrich_inventory",
+    "kubemarine.system.enrich_kernel_modules"
 ]
 
 supported_defaults = {
     'rbac': {
         'account_defaults': 'accounts'
     },
     'node_defaults': 'nodes',
@@ -178,59 +180,48 @@
         registry_mirrors = inventory['services']['cri']['dockerConfig']["registry-mirrors"]
         registry_mirrors.append(f"{protocol}://{registry_mirror_address}")
         inventory['services']['cri']['dockerConfig']["registry-mirrors"] = list(set(registry_mirrors))
 
     elif cri_impl == "containerd":
         registry_section = f'plugins."io.containerd.grpc.v1.cri".registry.mirrors."{registry_mirror_address}"'
 
-        if not inventory['services']['cri']['containerdConfig'].get(registry_section):
+        containerd_config = inventory['services']['cri']['containerdConfig']
+        if not containerd_config.get(registry_section):
             if not containerd_endpoints:
                 containerd_endpoints = ["%s://%s" % (protocol, registry_mirror_address)]
 
-            inventory['services']['cri']['containerdConfig'][registry_section] = {
+            containerd_config[registry_section] = {
                 'endpoint': containerd_endpoints
             }
 
-        effective_kubernetes_version = ".".join(inventory['services']['kubeadm']['kubernetesVersion'].split('.')[0:2])
-        pause_version = cluster.globals['compatibility_map']['software']['pause'][effective_kubernetes_version]['version']
-        if not inventory['services']['cri']['containerdConfig'].get('plugins."io.containerd.grpc.v1.cri"'):
-            inventory['services']['cri']['containerdConfig']['plugins."io.containerd.grpc.v1.cri"'] = {}
-        if not inventory['services']['cri']['containerdConfig']['plugins."io.containerd.grpc.v1.cri"'].get('sandbox_image'):
-            inventory['services']['cri']['containerdConfig']['plugins."io.containerd.grpc.v1.cri"']['sandbox_image'] = \
+        path = 'plugins."io.containerd.grpc.v1.cri"'
+        if not containerd_config.get(path):
+            containerd_config[path] = {}
+        if not containerd_config[path].get('sandbox_image'):
+            kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
+            pause_mapping = cluster.globals['compatibility_map']['software']['pause']
+            if kubernetes_version not in pause_mapping:
+                raise Exception(f"Failed to detect pause version for Kubernetes {kubernetes_version}. "
+                                f"Please explicitly specify services.cri.containerdConfig.{path}.sandbox_image section.")
+            pause_version = pause_mapping[kubernetes_version]['version']
+            containerd_config[path]['sandbox_image'] = \
                 f"{inventory['services']['kubeadm']['imageRepository']}/pause:{pause_version}"
 
-    if inventory['services'].get('thirdparties', []) and thirdparties_address:
-        for destination, config in inventory['services']['thirdparties'].items():
+    from kubemarine import thirdparties
 
-            if isinstance(config, str):
-                new_source = inventory['services']['thirdparties'][destination]
-            elif config.get('source') is not None:
-                new_source = inventory['services']['thirdparties'][destination]['source']
-            else:
+    if thirdparties_address:
+        for destination, config in inventory['services']['thirdparties'].items():
+            if not thirdparties.is_default_thirdparty(destination) or isinstance(config, str) or 'source' in config:
                 continue
 
-            for binary in ['kubeadm', 'kubelet', 'kubectl']:
-                if destination == '/usr/bin/' + binary:
-                    new_source = new_source.replace('https://storage.googleapis.com/kubernetes-release/release',
-                                                    '%s/kubernetes/%s'
-                                                    % (thirdparties_address, binary))
-
-            if '/usr/bin/calicoctl' == destination:
-                new_source = new_source.replace('https://github.com/projectcalico/calico/releases/download',
-                                                '%s/projectcalico/calico'
-                                                % thirdparties_address)
-
-            if '/usr/bin/crictl.tar.gz' == destination:
-                new_source = new_source.replace('https://github.com/kubernetes-sigs/cri-tools/releases/download',
-                                                '%s/kubernetes-sigs/cri-tools'
-                                                % thirdparties_address)
-            if isinstance(config, str):
-                inventory['services']['thirdparties'][destination] = new_source
-            else:
-                inventory['services']['thirdparties'][destination]['source'] = new_source
+            source, sha1 = thirdparties.get_default_thirdparty_identity(cluster.inventory, destination, in_public=False)
+            source = source.format(registry=thirdparties_address)
+            config['source'] = source
+            if 'sha1' not in config:
+                config['sha1'] = sha1
 
     return inventory
 
 
 def apply_registry_endpoints(inventory, cluster):
 
     if not inventory['registry'].get('mirror_registry'):
```

### Comparing `kubemarine-0.15.1/kubemarine/core/environment.py` & `kubemarine-0.16.0/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/errors.py` & `kubemarine-0.16.0/kubemarine/core/errors.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/executor.py` & `kubemarine-0.16.0/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/flow.py` & `kubemarine-0.16.0/kubemarine/core/flow.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/group.py` & `kubemarine-0.16.0/kubemarine/core/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import hashlib
 import io
 import os
 import random
 import re
 import time
 import uuid
 from datetime import datetime
 from typing import Callable, Dict, List, Union, IO
 
 import fabric
 import invoke
 from invoke import UnexpectedExit
 
+from kubemarine.core import utils
 from kubemarine.core.connections import Connections
 from kubemarine.core.executor import RemoteExecutor
 
 _GenericResult = Union[Exception, fabric.runners.Result, fabric.transfer.Result]
 _HostToResult = Dict[str, _GenericResult]
 
 
@@ -730,28 +730,18 @@
     def is_allowed_kubernetes_exception(self, exception_message):
         for known_exception_message in self.cluster.globals['kubernetes']['temporary_exceptions']:
             if known_exception_message in exception_message:
                 return True
 
         return False
 
-    def get_local_file_sha1(self, filename):
-        sha1 = hashlib.sha1()
+    def get_local_file_sha1(self, filename: str) -> str:
+        return utils.get_local_file_sha1(filename)
 
-        # Read local file by chunks of 2^16 bytes (65536) and calculate aggregated SHA1
-        with open(filename, 'rb') as f:
-            while True:
-                data = f.read(2 ** 16)
-                if not data:
-                    break
-                sha1.update(data)
-
-        return sha1.hexdigest()
-
-    def get_remote_file_sha1(self, filename):
+    def get_remote_file_sha1(self, filename: str) -> Dict[str, str]:
         results = self._do_with_wa("sudo", "openssl sha1 %s" % filename, warn=True)
         self._make_result_or_fail(results, lambda h, r: isinstance(r, Exception))
 
         return {host: result.stdout.split("= ")[1].strip() if result.stdout else None
                 for host, result in results.items()}
 
     def get_ordered_members_list(self, provide_node_configs=False, apply_filter=None) \
```

### Comparing `kubemarine-0.15.1/kubemarine/core/log.py` & `kubemarine-0.16.0/kubemarine/core/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import sys
+from abc import ABC, abstractmethod
+
 from pygelf import gelf, GelfTcpHandler, GelfUdpHandler, GelfTlsHandler, GelfHttpHandler
 
 from copy import deepcopy
 from typing import List, Optional
 
 VERBOSE = 5
 gelf.LEVELS.update({VERBOSE: 8})
@@ -74,15 +76,21 @@
     logging.INFO: 'info',
     logging.WARNING: 'warning',
     logging.ERROR: 'error',
     logging.CRITICAL: 'critical'
 }
 
 
-class EnhancedLogger(logging.Logger):
+class VerboseLogger(ABC):
+    @abstractmethod
+    def verbose(self, msg: str, *args, **kwargs):
+        pass
+
+
+class EnhancedLogger(logging.Logger, VerboseLogger):
     def __init__(self, name, level=logging.NOTSET):
         super().__init__(name, level)
         logging.addLevelName(VERBOSE, 'VERBOSE')
 
     def verbose(self, msg, *args, **kwargs):
         if self.isEnabledFor(VERBOSE):
             self._log(VERBOSE, msg, args, **kwargs)
```

### Comparing `kubemarine-0.15.1/kubemarine/core/patch.py` & `kubemarine-0.16.0/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/resources.py` & `kubemarine-0.16.0/kubemarine/core/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 print(msg)
             else:
                 logger.info(msg)
         try:
             data = utils.read_external(self.inventory_filepath)
             self._raw_inventory = yaml.safe_load(data)
             # load inventory as ruamel.yaml to save original structure
-            self._formatted_inventory = _yaml_structure_preserver().load(data)
+            self._formatted_inventory = utils.yaml_structure_preserver().load(data)
         except (yaml.YAMLError, ruamel.yaml.YAMLError) as exc:
             utils.do_fail("Failed to load inventory file", exc, log=logger)
 
     def make_final_inventory(self):
         self._formatted_inventory = utils.get_final_inventory(self.cluster(), initial_inventory=self.formatted_inventory())
 
     def recreate_inventory(self):
@@ -106,15 +106,15 @@
         and post processing of actions may work incorrectly.
         """
         if self._formatted_inventory is None:
             return
 
         # replace initial inventory file with changed inventory
         with utils.open_external(self.inventory_filepath, "w+") as stream:
-            _yaml_structure_preserver().dump(self.formatted_inventory(), stream)
+            utils.yaml_structure_preserver().dump(self.formatted_inventory(), stream)
 
         self._raw_inventory = None
         self._formatted_inventory = None
         # no need to clear _nodes_context as it should not change after cluster is reinitialized.
         # should not clear working_context as it can be inspected after execution.
         self._cluster = None
 
@@ -191,18 +191,11 @@
                                 procedure_inventory=self.procedure_inventory(),
                                 logger=self.logger())
 
     def _create_logger(self):
         return log.init_log_from_context_args(static.GLOBALS, self.context, self.raw_inventory()).logger
 
 
-def _yaml_structure_preserver():
-    """YAML loader and dumper which saves original structure"""
-    ruamel_yaml = ruamel.yaml.YAML()
-    ruamel_yaml.preserve_quotes = True
-    return ruamel_yaml
-
-
 def _provide_cluster(*args, **kw):
     from kubemarine.core import flow
     return flow.DEFAULT_CLUSTER_OBJ(*args, **kw) if flow.DEFAULT_CLUSTER_OBJ is not None \
         else c.KubernetesCluster(*args, **kw)
```

### Comparing `kubemarine-0.15.1/kubemarine/core/schema.py` & `kubemarine-0.16.0/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/summary.py` & `kubemarine-0.16.0/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/core/utils.py` & `kubemarine-0.16.0/kubemarine/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import hashlib
 import io
 import json
 import os
 import shutil
 import sys
 import time
 import tarfile
 
 from typing import Union, Tuple
 
 import yaml
+import ruamel.yaml
 from copy import deepcopy
 from datetime import datetime
 from collections import OrderedDict
 
+from ruamel.yaml import CommentedMap
+
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.errors import pretty_print_error
 
 
 def do_fail(message='', reason: Union[str, Exception] = '', hint='', log=None):
 
     if log:
@@ -301,14 +305,88 @@
     if os.path.isdir(patched_definition):
         return patched_definition, False
 
     raise Exception(
         'Requested resource directory %s is not exists at %s or %s' % (path, initial_definition, patched_definition))
 
 
+def get_local_file_sha1(filename: str) -> str:
+    sha1 = hashlib.sha1()
+
+    # Read local file by chunks of 2^16 bytes (65536) and calculate aggregated SHA1
+    with open(filename, 'rb') as f:
+        while True:
+            data = f.read(2 ** 16)
+            if not data:
+                break
+            sha1.update(data)
+
+    return sha1.hexdigest()
+
+
+def yaml_structure_preserver() -> ruamel.yaml.YAML:
+    """YAML loader and dumper which saves original structure"""
+    ruamel_yaml = ruamel.yaml.YAML()
+    ruamel_yaml.preserve_quotes = True
+    return ruamel_yaml
+
+
+def is_sorted(l: list, key: callable = None) -> bool:
+    """
+    Check that the specified list is sorted.
+
+    :param l: list to check
+    :param key: custom key function to customize the sort order
+    :return: boolean flag if the list is sorted
+    """
+    if key is None:
+        key = lambda x: x
+    return all(key(l[i]) <= key(l[i + 1]) for i in range(len(l) - 1))
+
+
+def map_sorted(map_: CommentedMap, key: callable = None) -> CommentedMap:
+    """
+    Check that the specified CommentedMap is sorted, or create new sorted map from it otherwise.
+
+    :param map_: CommentedMap instance to check
+    :param key: custom key function to customize the sort order of the map keys
+    :return: the same or new sorted instance of the map
+    """
+    if key is None:
+        key = lambda x: x
+    map_keys = list(map_)
+    if not is_sorted(map_keys, key=key):
+        map_ = CommentedMap(sorted(map_.items(), key=lambda item: key(item[0])))
+
+    return map_
+
+def insert_map_sorted(map_: CommentedMap, k, v, key: callable = None) -> None:
+    """
+    Insert new item to the CommentedMap or update the value for the existing key.
+    The map should be already sorted.
+
+    :param map_: sorted CommentedMap instance
+    :param k: new key
+    :param v: new value
+    :param key: custom key function to customize the sort order of the map keys
+    """
+    if k in map_:
+        map_[k] = v
+        return
+
+    if key is None:
+        key = lambda x: x
+    # Find position to insert new item maintaining the order
+    pos = max((mi + 1 for mi, mv in enumerate(map_)
+               if key(mv) < key(k)),
+              default=0)
+
+    map_.insert(pos, k, v)
+
+
 def load_yaml(filepath) -> dict:
     try:
         with open_utf8(filepath, 'r') as stream:
             return yaml.safe_load(stream)
     except yaml.YAMLError as exc:
         do_fail(f"Failed to load {filepath}", exc)
 
@@ -339,21 +417,28 @@
 def minor_version(version: str) -> str:
     """
     Converts vN.N.N to vN.N
     """
     return ".".join(version.split(".")[0:2])
 
 
-def version_key(version: str):
+def version_key(version: str) -> tuple:
     """
-    Converts vN.N.N to (N, N, N) that can be used in comparisons.
+    Converts vN.N.N to (N, N, N) or vN.N to (N, N) that can be used in comparisons.
     """
     return tuple(map(int, version[1:].split('.')))
 
 
+def minor_version_key(version: str) -> tuple:
+    """
+    Converts vN.N.N to (N, N) that can be used in comparisons.
+    """
+    return version_key(minor_version(version))
+
+
 class ClusterStorage:
     """
     File preservation:
     1- Create folder where dumps are stored
     2- Rotating dumps in the storage folder
     3- Uploading dumps to nodes
     4- Copying dumps to new nodes
```

### Comparing `kubemarine-0.15.1/kubemarine/core/yaml_merger.py` & `kubemarine-0.16.0/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/coredns.py` & `kubemarine-0.16.0/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/cri/__init__.py` & `kubemarine-0.16.0/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/cri/containerd.py` & `kubemarine-0.16.0/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/cri/docker.py` & `kubemarine-0.16.0/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/demo.py` & `kubemarine-0.16.0/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/etcd.py` & `kubemarine-0.16.0/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/haproxy.py` & `kubemarine-0.16.0/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/jinja.py` & `kubemarine-0.16.0/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/k8s_certs.py` & `kubemarine-0.16.0/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/keepalived.py` & `kubemarine-0.16.0/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/__init__.py` & `kubemarine-0.16.0/kubemarine/kubernetes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,16 +597,16 @@
     plugins.expect_pods(cluster, [
         'kube-apiserver',
         'kube-controller-manager',
         'kube-proxy',
         'kube-scheduler',
         'etcd'
     ], node=connection, apply_filter=apply_filter,
-                        timeout=cluster.globals['pods']['expect']['kubernetes']['timeout'],
-                        retries=cluster.globals['pods']['expect']['kubernetes']['retries'])
+                        timeout=cluster.inventory['globals']['expect']['pods']['kubernetes']['timeout'],
+                        retries=cluster.inventory['globals']['expect']['pods']['kubernetes']['retries'])
 
 
 def wait_for_nodes(group: NodeGroup):
     log = group.cluster.log
 
     first_control_plane = group.cluster.nodes["control-plane"].get_first_member()
     node_names = group.get_nodes_names()
@@ -979,18 +979,18 @@
 
 
 def verify_target_version(target_version):
     test_version(target_version)
 
     pos = target_version.rfind(".")
     target_version = target_version[:pos]
-    globals_yml = static.GLOBALS
-    if target_version not in globals_yml["kubernetes_versions"]:
+    supported_versions = static.SUPPORTED_VERSIONS
+    if target_version not in supported_versions:
         raise Exception("ERROR! Specified target Kubernetes version '%s' - cannot be installed!" % target_version)
-    if not globals_yml["kubernetes_versions"].get(target_version, {}).get("supported", False):
+    if not supported_versions.get(target_version, {}).get("supported", False):
         message = "\033[91mWarning! Specified target Kubernetes version '%s' - is not supported!\033[0m" % target_version
         print(message)
         return message
     return ""
 
 
 def expect_kubernetes_version(cluster, version, timeout=None, retries=None, node=None, apply_filter=None):
@@ -1226,14 +1226,22 @@
     """
     Prepull kubeadm images on group.
     :param group: NodeGroup where prepull should be performed.
     :return: NodeGroupResult from all nodes in presented group.
     """
 
     config = get_kubeadm_config(group.cluster.inventory)
+    kubeadm_init: dict = {
+        'apiVersion': group.cluster.inventory["services"]["kubeadm"]['apiVersion'],
+        'kind': 'InitConfiguration',
+    }
+
+    configure_container_runtime(group.cluster, kubeadm_init)
+    config = f'{config}---\n{yaml.dump(kubeadm_init, default_flow_style=False)}'
+
     group.put(io.StringIO(config), '/etc/kubernetes/prepull-config.yaml', sudo=True)
 
     return group.sudo("kubeadm config images pull --config=/etc/kubernetes/prepull-config.yaml")
 
 
 def schedule_running_nodes_report(cluster: KubernetesCluster):
     summary.schedule_delayed_report(cluster, exec_running_nodes_report)
```

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.16.0/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/deployment.py` & `kubemarine-0.16.0/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/object.py` & `kubemarine-0.16.0/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.16.0/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.16.0/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/kubernetes_accounts.py` & `kubemarine-0.16.0/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/packages.py` & `kubemarine-0.16.0/kubemarine/packages.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/patches/__init__.py` & `kubemarine-0.16.0/kubemarine/patches/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
-from kubemarine.patches.p1_reinstall_calico import CalicoFixes
+from kubemarine.patches.p1_helm_values import HelmValues
 
 patches: List[Patch] = [
-    CalicoFixes(),
+    HelmValues(),
 ]
 """List of patches which can be executed strictly in the declared order"""
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/__init__.py` & `kubemarine-0.16.0/kubemarine/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,17 @@
     :param node: Node where daemonsets should be detected
     :return: None
     """
 
     log = cluster.log
 
     if timeout is None:
-        timeout = cluster.globals['deployments']['expect']['timeout']
+        timeout = cluster.inventory['globals']['expect']['deployments']['timeout']
     if retries is None:
-        retries = cluster.globals['deployments']['expect']['retries']
+        retries = cluster.inventory['globals']['expect']['deployments']['retries']
 
     log.debug(f"Expecting the following DaemonSets to be up to date: {daemonsets_names}")
     log.verbose("Max expectation time: %ss" % (timeout * retries))
 
     log.debug("Waiting for DaemonSets...")
 
     daemonsets = []
@@ -215,17 +215,17 @@
     :param node: Node where replicasests should be detected
     :return: None
     """
 
     log = cluster.log
 
     if timeout is None:
-        timeout = cluster.globals['deployments']['expect']['timeout']
+        timeout = cluster.inventory['globals']['expect']['deployments']['timeout']
     if retries is None:
-        retries = cluster.globals['deployments']['expect']['retries']
+        retries = cluster.inventory['globals']['expect']['deployments']['retries']
 
     log.debug(f"Expecting the following ReplicaSets to be up to date: {replicasets_names}")
     log.verbose("Max expectation time: %ss" % (timeout * retries))
 
     log.debug("Waiting for ReplicaSets...")
 
     replicasets = []
@@ -267,17 +267,17 @@
     :param node: Node where statefulsets should be detected
     :return: None
     """
 
     log = cluster.log
 
     if timeout is None:
-        timeout = cluster.globals['deployments']['expect']['timeout']
+        timeout = cluster.inventory['globals']['expect']['deployments']['timeout']
     if retries is None:
-        retries = cluster.globals['deployments']['expect']['retries']
+        retries = cluster.inventory['globals']['expect']['deployments']['retries']
 
     log.debug(f"Expecting the following StatefulSets to be up to date: {statefulsets_names}")
     log.verbose("Max expectation time: %ss" % (timeout * retries))
 
     log.debug("Waiting for StatefulSets...")
 
     statefulsets = []
@@ -319,17 +319,17 @@
     :param node: Node where deployments should be detected
     :return: None
     """
 
     log = cluster.log
 
     if timeout is None:
-        timeout = cluster.globals['deployments']['expect']['timeout']
+        timeout = cluster.inventory['globals']['expect']['deployments']['timeout']
     if retries is None:
-        retries = cluster.globals['deployments']['expect']['retries']
+        retries = cluster.inventory['globals']['expect']['deployments']['retries']
 
     log.debug(f"Expecting the following Deployments to be up to date: {deployments_names}")
     log.verbose("Max expectation time: %ss" % (timeout * retries))
 
     log.debug("Waiting for Deployments...")
 
     deployments = []
@@ -360,17 +360,17 @@
                 node=None, apply_filter=None):
 
     if isinstance(cluster, NodeGroup):
         # when instead of cluster there was received a group
         cluster = cluster.cluster
 
     if timeout is None:
-        timeout = cluster.globals['pods']['expect']['plugins']['timeout']
+        timeout = cluster.inventory['globals']['expect']['pods']['plugins']['timeout']
     if retries is None:
-        retries = cluster.globals['pods']['expect']['plugins']['retries']
+        retries = cluster.inventory['globals']['expect']['pods']['plugins']['retries']
 
     cluster.log.debug("Expecting the following pods to be ready: %s" % pods)
     cluster.log.verbose("Max expectation time: %ss" % (timeout * retries))
 
     cluster.log.debug("Waiting for pods...")
 
     failures = 0
@@ -738,35 +738,35 @@
     cluster.log.debug(output.decode('utf-8'))
 
     return output
 
 
 def process_chart_values(config, local_chart_path):
     config_values = config.get("values")
+    file_values = None
     config_values_file = config.get("values_file")
-
-    if config_values is not None:
-        with utils.open_external(os.path.join(local_chart_path, 'values.yaml'), 'r+') as stream:
-            original_values = yaml.safe_load(stream)
-            stream.seek(0)
-            merged_values = default_merger.merge(original_values, config_values)
-            stream.write(yaml.dump(merged_values))
-            stream.truncate()
-    else:
-        if config_values_file is not None:
-            with utils.open_external(os.path.join(local_chart_path, 'values.yaml'), 'r+') as stream:
-                with utils.open_external(config_values_file, 'r+') as additional_stream:
-                    original_values = yaml.safe_load(stream)
-                    additional_values = yaml.safe_load(additional_stream)
-                    if additional_values is None:
-                        return
-                    stream.seek(0)
-                    merged_values = default_merger.merge(original_values, additional_values)
-                    stream.write(yaml.dump(merged_values))
-                    stream.truncate()
+    if config_values_file is not None:
+        with utils.open_external(config_values_file) as stream:
+            file_values = yaml.safe_load(stream)
+
+    if config_values is None and file_values is None:
+        return
+
+    with utils.open_external(os.path.join(local_chart_path, 'values.yaml'), 'r+') as stream:
+        merged_values = yaml.safe_load(stream)
+
+        if file_values is not None:
+            merged_values = default_merger.merge(merged_values, file_values)
+        # Values from 'values' section have priority over values in 'values_file' section
+        if config_values is not None:
+            merged_values = default_merger.merge(merged_values, config_values)
+
+        stream.seek(0)
+        stream.write(yaml.dump(merged_values))
+        stream.truncate()
 
 
 def get_local_chart_path(log, config):
     chart_path = config.get('chart_path')
 
     is_curl = chart_path[:4] == 'http' and '://' in chart_path[4:8]
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/builtin.py` & `kubemarine-0.16.0/kubemarine/plugins/builtin.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict
 
+from kubemarine.core import log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.plugins import manifest
 from kubemarine.plugins.calico import CalicoManifestProcessor
 from kubemarine.plugins.kubernetes_dashboard import get_dashboard_manifest_processor
 from kubemarine.plugins.local_path_provisioner import LocalPathProvisionerManifestProcessor
 from kubemarine.plugins.nginx_ingress import get_ingress_nginx_manifest_processor
 
@@ -51,25 +52,32 @@
 
             expected_args = {'plugin_name', 'original_yaml_path', 'destination_name'}
             declared_args = set(arguments.keys())
             if not declared_args.issubset(expected_args):
                 raise Exception(f"Unexpected python method arguments {list(declared_args.difference(expected_args))} "
                                 f"in {plugin_name!r} installation step {i}.")
 
-            processor_provider(cluster, inventory, **arguments).validate_inventory()
+            processor_provider(cluster.log, inventory, **arguments).validate_inventory()
             break
         else:
             cluster.log.warning(f"Invocation of plugins.builtin.apply_yaml is not found for {plugin_name!r} plugin. "
                                 f"Such configuration is obsolete, and support for it may be stopped in future releases.")
 
     return inventory
 
 
-def apply_yaml(cluster: KubernetesCluster, **arguments):
-    arguments = dict(arguments)
-    plugin_name = arguments.pop('plugin_name')
+def get_manifest_processor(logger: log.VerboseLogger, inventory: dict, plugin_name: str, **arguments):
     if plugin_name not in MANIFEST_PROCESSOR_PROVIDERS:
         raise Exception(f"Manifest processor is not registered for {plugin_name!r} plugin.")
 
     processor_provider = MANIFEST_PROCESSOR_PROVIDERS[plugin_name]
-    processor = processor_provider(cluster, cluster.inventory, **arguments)
-    processor.apply()
+    return processor_provider(logger, inventory, **arguments)
+
+
+def apply_yaml(cluster: KubernetesCluster, **arguments):
+    arguments = dict(arguments)
+    plugin_name = arguments.pop('plugin_name')
+
+    processor = get_manifest_processor(cluster.log, cluster.inventory, plugin_name, **arguments)
+
+    manifest = processor.enrich()
+    processor.apply(cluster, manifest)
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/calico.py` & `kubemarine-0.16.0/kubemarine/plugins/calico.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,88 +12,82 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import ipaddress
 from typing import Optional, List
 
 import os
 
-from kubemarine.core import utils
+from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
 # DEPRECATED
 def apply_calico_yaml(cluster: KubernetesCluster, calico_original_yaml: str, calico_yaml: str):
     """
     The method implements full processing for Calico plugin
     :param calico_original_yaml: path to original Calico manifest
     :param calico_yaml: file name of the resulting Calico manifest
     :param cluster: Cluster object
     """
 
     calico_yaml = os.path.basename(calico_yaml)
-    processor = CalicoManifestProcessor(cluster, cluster.inventory,
+    processor = CalicoManifestProcessor(cluster.log, cluster.inventory,
                                         original_yaml_path=calico_original_yaml,
                                         destination_name=calico_yaml)
-    processor.apply()
+    manifest = processor.enrich()
+    processor.apply(cluster, manifest)
 
 
 class CalicoManifestProcessor(Processor):
-    def __init__(self, cluster: KubernetesCluster, inventory: dict,
+    def __init__(self, logger: log.VerboseLogger, inventory: dict,
                  original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
-        plugin_name = 'calico'
-        version = inventory['plugins'][plugin_name]['version']
-        if original_yaml_path is None:
-            original_yaml_path = f"plugins/yaml/calico-{version}.yaml.original"
-        if destination_name is None:
-            destination_name = f"calico-{version}.yaml"
-        super().__init__(cluster, inventory, plugin_name, original_yaml_path, destination_name)
+        super().__init__(logger, inventory, 'calico', original_yaml_path, destination_name)
 
     def exclude_typha_objects_if_disabled(self, manifest: Manifest) -> None:
         # enrich 'calico-typha' objects only if it's enabled in 'cluster.yaml'
         # in other case those objects must be excluded
         str_value = utils.true_or_false(self.inventory['plugins']['calico']['typha']['enabled'])
         if str_value == 'false':
             for key in ("Deployment_calico-typha", "Service_calico-typha", "PodDisruptionBudget_calico-typha"):
-                manifest.exclude(key)
+                self.exclude(manifest, key)
         elif str_value == 'true':
             return
         else:
             raise Exception(f"plugins.calico.typha.enabled must be set in 'True' or 'False' "
                             f"as string or boolean value")
 
     def enrich_configmap_calico_config(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico ConfigMap
         :param manifest: Container to operate with manifest objects
         """
 
         key = "ConfigMap_calico-config"
         source_yaml = manifest.get_obj(key, patch=True)
-        cluster = self.cluster
-        val = cluster.inventory['plugins']['calico']['mtu']
+        val = self.inventory['plugins']['calico']['mtu']
         source_yaml['data']['veth_mtu'] = str(val)
-        cluster.log.verbose(f"The {key} has been patched in 'data.veth_mtu' with '{val}'")
-        str_value = utils.true_or_false(cluster.inventory['plugins']['calico']['typha']['enabled'])
+        self.log.verbose(f"The {key} has been patched in 'data.veth_mtu' with '{val}'")
+        str_value = utils.true_or_false(self.inventory['plugins']['calico']['typha']['enabled'])
         if str_value == "true":
             val = "calico-typha"
         elif str_value == "false":
             val = "none"
         source_yaml['data']['typha_service_name'] = val
-        cluster.log.verbose(f"The {key} has been patched in 'data.typha_service_name' with '{val}'")
+        self.log.verbose(f"The {key} has been patched in 'data.typha_service_name' with '{val}'")
         string_part = source_yaml['data']['cni_network_config']
-        ip = cluster.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
+        ip = self.inventory['services']['kubeadm']['networking']['podSubnet'].split('/')[0]
         if type(ipaddress.ip_address(ip)) is ipaddress.IPv4Address:
-            val = cluster.inventory['plugins']['calico']['cni']['ipam']['ipv4']
+            val = self.inventory['plugins']['calico']['cni']['ipam']['ipv4']
         else:
-            val = cluster.inventory['plugins']['calico']['cni']['ipam']['ipv6']
+            val = self.inventory['plugins']['calico']['cni']['ipam']['ipv6']
         new_string_part = string_part.replace('"type": "calico-ipam"', str(val)[:-1][1:].replace("'", "\""))
         source_yaml['data']['cni_network_config'] = new_string_part
         log_str = new_string_part.replace("\n", "")
-        cluster.log.verbose(f"The {key} has been patched in 'data.cni_network_config' with '{log_str}'")
+        self.log.verbose(f"The {key} has been patched in 'data.cni_network_config' with '{log_str}'")
 
     def enrich_deployment_calico_kube_controllers(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico controller Deployment
         :param manifest: Container to operate with manifest objects
         """
 
@@ -186,59 +180,56 @@
         """
         The method implements the enrichment procedure for Typha Deployment
         :param manifest: Container to operate with manifest objects
         """
 
         key = "Deployment_calico-typha"
         source_yaml = manifest.get_obj(key, patch=True, allow_absent=True)
-        cluster = self.cluster
         if source_yaml is None:
             return
 
         default_tolerations = [{'key': 'node.kubernetes.io/network-unavailable', 'effect': 'NoSchedule'},
                                {'key': 'node.kubernetes.io/network-unavailable', 'effect': 'NoExecute'}]
 
-        val = cluster.inventory['plugins']['calico']['typha']['replicas']
+        val = self.inventory['plugins']['calico']['typha']['replicas']
         source_yaml['spec']['replicas'] = int(val)
-        cluster.log.verbose(f"The {key} has been patched in 'spec.replicas' with '{val}'")
+        self.log.verbose(f"The {key} has been patched in 'spec.replicas' with '{val}'")
 
         self.enrich_node_selector(manifest, key, plugin_service='typha')
         self.enrich_tolerations(manifest, key, plugin_service='typha', extra_tolerations=default_tolerations)
         self.enrich_image_for_container(manifest, key,
             plugin_service='typha', container_name='calico-typha', is_init_container=False)
 
     def enrich_clusterrole_calico_kube_controllers(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico controller ClusterRole
         :param manifest: Container to operate with manifest objects
         """
 
         key = "ClusterRole_calico-kube-controllers"
-        cluster = self.cluster
-        if cluster.inventory['rbac']['admission'] == "psp" and \
-                cluster.inventory['rbac']['psp']['pod-security'] == "enabled":
+        if self.inventory['rbac']['admission'] == "psp" and \
+                self.inventory['rbac']['psp']['pod-security'] == "enabled":
             source_yaml = manifest.get_obj(key, patch=True)
             api_list = source_yaml['rules']
             api_list.append(psp_calico_kube_controllers)
-            cluster.log.verbose(f"The {key} has been patched in 'rules' with '{psp_calico_kube_controllers}'")
+            self.log.verbose(f"The {key} has been patched in 'rules' with '{psp_calico_kube_controllers}'")
 
     def enrich_clusterrole_calico_node(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico node ClusterRole
         :param manifest: Container to operate with manifest objects
         """
 
         key = "ClusterRole_calico-node"
-        cluster = self.cluster
-        if cluster.inventory['rbac']['admission'] == "psp" and \
-                cluster.inventory['rbac']['psp']['pod-security'] == "enabled":
+        if self.inventory['rbac']['admission'] == "psp" and \
+                self.inventory['rbac']['psp']['pod-security'] == "enabled":
             source_yaml = manifest.get_obj(key, patch=True)
             api_list = source_yaml['rules']
             api_list.append(psp_calico_node)
-            cluster.log.verbose(f"The {key} has been patched in 'rules' with '{psp_calico_node}'")
+            self.log.verbose(f"The {key} has been patched in 'rules' with '{psp_calico_node}'")
 
     def enrich_crd_felix_configuration(self, manifest: Manifest) -> None:
         """
         The method implements the enrichment procedure for Calico CRD Felixconfigurations
         :param cluster: Cluster object
         :param obj_list: list of objects for enrichment
         """
@@ -251,16 +242,16 @@
             'prometheusMetricsEnabled']
         api_list["default"] = True
         source_yaml['spec']['versions'][0]['schema']['openAPIV3Schema']['properties']['spec']['properties'][
             'prometheusMetricsEnabled'] = api_list
 
         sz = len(manifest.all_obj_keys())
         import ruamel.yaml
-        manifest.include(sz, ruamel.yaml.safe_load(utils.read_internal('templates/plugins/calico-kube-controllers-metrics.yaml')))
-        manifest.include(sz, ruamel.yaml.safe_load(utils.read_internal('templates/plugins/calico-metrics.yaml')))
+        self.include(manifest, sz, ruamel.yaml.safe_load(utils.read_internal('templates/plugins/calico-kube-controllers-metrics.yaml')))
+        self.include(manifest, sz, ruamel.yaml.safe_load(utils.read_internal('templates/plugins/calico-metrics.yaml')))
 
     def get_known_objects(self) -> List[str]:
         return [
             "ConfigMap_calico-config",
             "CustomResourceDefinition_bgpconfigurations.crd.projectcalico.org",
             "CustomResourceDefinition_bgppeers.crd.projectcalico.org",
             "CustomResourceDefinition_blockaffinities.crd.projectcalico.org",
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.16.0/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
-from kubemarine.core import summary, utils
+from kubemarine.core import summary, utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
 def schedule_summary_report(cluster: KubernetesCluster):
     plugin_item = cluster.inventory['plugins']['kubernetes-dashboard']
     hostname = plugin_item['hostname']
     # Currently we declare that Dashboard UI is available only via HTTPS
     summary.schedule_report(cluster.context, summary.SummaryItem.DASHBOARD_URL, f'https://{hostname}')
 
 
 class DashboardManifestProcessor(Processor):
-    def __init__(self, cluster: KubernetesCluster, inventory: dict,
+    def __init__(self, logger: log.VerboseLogger, inventory: dict,
                  original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
-        plugin_name = 'kubernetes-dashboard'
-        version = inventory['plugins'][plugin_name]['version']
-        if original_yaml_path is None:
-            original_yaml_path = f"plugins/yaml/dashboard-{version}-original.yaml"
-        if destination_name is None:
-            destination_name = f"dashboard-{version}.yaml"
-        super().__init__(cluster, inventory, plugin_name, original_yaml_path, destination_name)
+        super().__init__(logger, inventory, 'kubernetes-dashboard', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_kubernetes-dashboard",
             "ServiceAccount_kubernetes-dashboard",
             "Service_kubernetes-dashboard",
             "Secret_kubernetes-dashboard-certs",
@@ -94,13 +88,13 @@
         source_yaml = manifest.get_obj(key, patch=True)
         template_spec: dict = source_yaml['spec']['template']['spec']
         del template_spec['securityContext']
         self.log.verbose(f"The 'securityContext' property has been removed from 'spec.template.spec' in the {key}")
         super().enrich_deployment_dashboard_metrics_scraper(manifest)
 
 
-def get_dashboard_manifest_processor(cluster: KubernetesCluster, inventory: dict, **kwargs):
+def get_dashboard_manifest_processor(logger: log.VerboseLogger, inventory: dict, **kwargs):
     version: str = inventory['plugins']['kubernetes-dashboard']['version']
     if utils.minor_version(version) == 'v2.5':
-        return V2_5_X_DashboardManifestProcessor(cluster, inventory, **kwargs)
+        return V2_5_X_DashboardManifestProcessor(logger, inventory, **kwargs)
 
-    return DashboardManifestProcessor(cluster, inventory, **kwargs)
+    return DashboardManifestProcessor(logger, inventory, **kwargs)
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.16.0/kubemarine/plugins/local_path_provisioner.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,21 @@
 # limitations under the License.
 
 from textwrap import dedent
 from typing import List, Optional
 
 import yaml
 
-from kubemarine.core.cluster import KubernetesCluster
+from kubemarine.core import log
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 class LocalPathProvisionerManifestProcessor(Processor):
-    def __init__(self, cluster: KubernetesCluster, inventory: dict,
+    def __init__(self, logger: log.VerboseLogger, inventory: dict,
                  original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
-        plugin_name = 'local-path-provisioner'
-        version = inventory['plugins'][plugin_name]['version']
-        if original_yaml_path is None:
-            original_yaml_path = f"plugins/yaml/local-path-provisioner-{version}-original.yaml"
-        if destination_name is None:
-            destination_name = f"local-path-provisioner-{version}.yaml"
-        super().__init__(cluster, inventory, plugin_name, original_yaml_path, destination_name)
+        super().__init__(logger, inventory, 'local-path-provisioner', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_local-path-storage",
             "ServiceAccount_local-path-provisioner-service-account",
             "ClusterRole_local-path-provisioner-role",
             "ClusterRoleBinding_local-path-provisioner-bind",
@@ -60,15 +54,15 @@
 
     def add_clusterrolebinding_local_path_provisioner_privileged_psp(self, manifest: Manifest):
         # TODO add only if psp is enabled?
         new_yaml = yaml.safe_load(clusterrolebinding_local_path_provisioner_privileged_psp)
         # Insert new ClusterRoleBinding after all existing resources of this kind
         max_crb_idx = max(i for i, key in enumerate(manifest.all_obj_keys())
                           if key.startswith("ClusterRoleBinding_"))
-        manifest.include(max_crb_idx + 1, new_yaml)
+        self.include(manifest, max_crb_idx + 1, new_yaml)
 
     def enrich_deployment_local_path_provisioner(self, manifest: Manifest):
         key = "Deployment_local-path-provisioner"
         self.enrich_image_for_container(manifest, key,
             container_name='local-path-provisioner', is_init_container=False)
 
         self.enrich_tolerations(manifest, key)
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/manifest.py` & `kubemarine-0.16.0/kubemarine/plugins/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,21 @@
 from kubemarine import plugins
 from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 
 ERROR_MANIFEST_NOT_FOUND = "Cannot find original manifest %s for '%s' plugin"
 
 
+def get_default_manifest_path(plugin_name: str, version: str):
+    resource = f"plugins/yaml/{plugin_name}-{version}-original.yaml"
+    return utils.get_internal_resource_path(resource)
+
+
 class Manifest:
-    def __init__(self, logger: log.EnhancedLogger, stream: IO):
-        self.logger = logger
+    def __init__(self, stream: IO):
         self._patched = OrderedSet()
         self._excluded = OrderedSet()
         self._included = OrderedSet()
         self._obj_list = self._load(stream)
 
     def obj_key(self, obj: dict) -> str:
         return f"{obj['kind']}_{obj['metadata']['name']}"
@@ -71,20 +75,18 @@
             raise ValueError(f"{key} not found")
         return None
 
     def include(self, index: int, obj: dict):
         self._obj_list.insert(index, obj)
         key = self.obj_key(obj)
         self._included.add(key)
-        self.logger.verbose(f"The {key} has been added")
 
     def exclude(self, key: str):
         del self._obj_list[self.key_index(key)]
         self._excluded.add(key)
-        self.logger.verbose(f"The {key} has been excluded from result")
 
     @property
     def patched(self) -> List[str]:
         return list(self._patched)
 
     @property
     def included(self) -> List[str]:
@@ -102,18 +104,31 @@
 
         with io.StringIO() as stream:
             yaml.dump_all(self._obj_list, stream)
             result = stream.getvalue()
 
         return result
 
+    def get_all_container_images(self) -> List[str]:
+        images = []
+        for key in self.all_obj_keys():
+            obj = self.get_obj(key, patch=False)
+            for spec_section in ('containers', 'initContainers'):
+                containers = obj.get('spec', {}).get('template', {}).get('spec', {}).get(spec_section, [])
+                for container in containers:
+                    image = container['image']
+                    if image not in images:
+                        images.append(image)
+
+        return images
+
     def _load(self, stream: IO) -> List[dict]:
         """
         The method implements the parse YAML file that includes several YAMLs inside
-        :param filepath: Path to file that should be parsed
+        :param stream: stream with manifest content that should be parsed
         :return: list of original objects to enrich in YAML format.
         """
         yaml = ruamel.yaml.YAML()
         obj_list = []
         source_yamls = yaml.load_all(stream)
         yaml_keys = set()
         for source_yaml in source_yamls:
@@ -131,53 +146,60 @@
         return obj_list
 
 
 EnrichmentFunction = Callable[[Manifest], None]
 
 
 class Processor(ABC):
-    def __init__(self, cluster: KubernetesCluster, inventory: dict,
-                 plugin_name: str, original_yaml_path: str, destination_name: str):
+    def __init__(self, logger: log.VerboseLogger, inventory: dict, plugin_name: str,
+                 original_yaml_path: Optional[str], destination_name: Optional[str]):
         """
-        :param cluster: cluster object
+        :param logger: VerboseLogger instance
         :param inventory: inventory of the cluster
         :param plugin_name: name of plugin-owner
-        :param original_yaml_path: path to original manifest
-        :param destination_name: destination manifest file name
+        :param original_yaml_path: path to custom manifest
+        :param destination_name: custom destination manifest file name
         """
-        self.cluster = cluster
-        self.log: log.EnhancedLogger = cluster.log
+        self.log: log.VerboseLogger = logger
         self.inventory = inventory
         self.plugin_name = plugin_name
-        self.original_yaml_path = original_yaml_path
-        self.destination_name = destination_name
+        self.manifest_path = self._get_manifest_path(original_yaml_path)
+        self.destination_name = self._get_destination(destination_name)
 
     def get_known_objects(self) -> List[str]:
         """
         :return: list with the 'kind' and 'name' of expected objects in original manifest
         """
         return []
 
     @abstractmethod
     def get_enrichment_functions(self) -> List[EnrichmentFunction]:
         """
         :return: list of enrichment methods
         """
         pass
 
+    def get_version(self) -> str:
+        return self.inventory['plugins'][self.plugin_name]['version']
+
+    def include(self, manifest: Manifest, index: int, obj: dict):
+        key = manifest.obj_key(obj)
+        manifest.include(index, obj)
+        self.log.verbose(f"The {key} has been added")
+
+    def exclude(self, manifest: Manifest, key: str):
+        manifest.exclude(key)
+        self.log.verbose(f"The {key} has been excluded from result")
+
     def validate_inventory(self) -> None:
         """
         # Check if original YAML exists
         """
-        config = {
-            "source": self.original_yaml_path
-        }
-        original_yaml_path, _ = plugins.get_source_absolute_pattern(config)
-        if not os.path.isfile(original_yaml_path):
-            raise Exception(ERROR_MANIFEST_NOT_FOUND % (original_yaml_path, self.plugin_name))
+        if not os.path.isfile(self.manifest_path):
+            raise Exception(ERROR_MANIFEST_NOT_FOUND % (self.manifest_path, self.plugin_name))
 
     def validate_original(self, manifest: Manifest) -> None:
         """
         The method implements default validations for manifest objects
 
         :param manifest: container to operate with manifest objects
         """
@@ -190,34 +212,25 @@
 
         # check if known objects were excluded
         for key in known_objects:
             if manifest.get_obj(key, patch=False, allow_absent=True) is None:
                 self.log.verbose(f"The current version of original yaml does not include "
                                  f"the following object: {key}")
 
-    def apply(self):
+    def enrich(self) -> Manifest:
         """
         The method implements full processing for the plugin main manifest.
         """
-        destination = '/etc/kubernetes/%s' % self.destination_name
-
-        # create config for plugin module
-        config = {
-            "source": self.original_yaml_path,
-            "destination": destination,
-            "do_render": False
-        }
 
         # get original YAML and parse it into list of objects
-        original_yaml_path, _ = plugins.get_source_absolute_pattern(config)
         try:
-            with utils.open_utf8(original_yaml_path, 'r') as stream:
-                manifest = Manifest(self.log, stream)
+            with utils.open_utf8(self.manifest_path, 'r') as stream:
+                manifest = Manifest(stream)
         except Exception as exc:
-            raise Exception(f"Failed to load {original_yaml_path} for {self.plugin_name!r} plugin") from exc
+            raise Exception(f"Failed to load {self.manifest_path} for {self.plugin_name!r} plugin") from exc
 
         self.validate_original(manifest)
 
         # call enrichment functions one by one
         enrichment_functions = self.get_enrichment_functions()
         for fn in enrichment_functions:
             fn(manifest)
@@ -225,22 +238,49 @@
         self.log.verbose(f"The total number of patched objects is {len(manifest.patched)} "
                          f"the objects are the following: {manifest.patched}")
         self.log.verbose(f"The total number of added objects is {len(manifest.included)} "
                          f"the objects are the following: {manifest.included}")
         self.log.verbose(f"The total number of excluded objects is {len(manifest.excluded)} "
                          f"the objects are the following: {manifest.excluded}")
 
+        return manifest
+
+    def apply(self, cluster: KubernetesCluster, manifest: Manifest):
+        logger = cluster.log
         enriched_manifest = manifest.dump()
-        utils.dump_file(self.cluster, enriched_manifest, self.destination_name)
-        config['source'] = io.StringIO(enriched_manifest)
+        utils.dump_file(cluster, enriched_manifest, self.destination_name)
+
+        destination = '/etc/kubernetes/%s' % self.destination_name
+
+        # create config for plugin module
+        config = {
+            "source": io.StringIO(enriched_manifest),
+            "destination": destination,
+            "do_render": False
+        }
+
+        logger.debug(f"Uploading manifest enriched from {self.manifest_path} for {self.plugin_name!r} plugin...")
+        logger.debug("\tDestination: %s" % destination)
+
+        plugins.apply_source(cluster, config)
+
+    def _get_manifest_path(self, custom_manifest_path: Optional[str]) -> str:
+        if custom_manifest_path is not None:
+            config = {"source": custom_manifest_path}
+            manifest_path, _ = plugins.get_source_absolute_pattern(config)
+        else:
+            manifest_path = get_default_manifest_path(self.plugin_name, self.get_version())
+
+        return manifest_path
 
-        self.log.debug(f"Uploading manifest enriched from {original_yaml_path} for {self.plugin_name!r} plugin...")
-        self.log.debug("\tDestination: %s" % destination)
+    def _get_destination(self, custom_destination_name) -> str:
+        if custom_destination_name is not None:
+            return custom_destination_name
 
-        plugins.apply_source(self.cluster, config)
+        return f'{self.plugin_name}-{self.get_version()}.yaml'
 
     def assign_default_pss_labels(self, manifest: Manifest, key: str, profile: str):
         source_yaml = manifest.get_obj(key, patch=True)
         labels: dict = source_yaml['metadata'].setdefault('labels', {})
         labels.update({
             'pod-security.kubernetes.io/enforce': profile,
             'pod-security.kubernetes.io/enforce-version': 'latest',
@@ -351,8 +391,8 @@
         tolerations.extend(plugin_service_section.get('tolerations', []))
 
         for val in tolerations:
             template_spec.setdefault('tolerations', []).append(val)
             self.log.verbose(f"The {key} has been patched in 'spec.template.spec.tolerations' with '{val}'")
 
 
-PROCESSOR_PROVIDER = Callable[[KubernetesCluster, dict, str, str], Processor]
+PROCESSOR_PROVIDER = Callable[[log.VerboseLogger, dict, str, str], Processor]
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.16.0/kubemarine/plugins/nginx_ingress.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 from typing import Optional, List
 
-from kubemarine.core import utils
+from kubemarine.core import utils, log
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroup
 from kubemarine.plugins.manifest import Processor, EnrichmentFunction, Manifest
 
 
 def enrich_inventory(inventory, _):
     if not inventory["plugins"]["nginx-ingress-controller"]["install"]:
@@ -131,23 +131,17 @@
 
 def create_tls_secret(first_control_plane, crt_path, key_path, name, namespace):
     first_control_plane.sudo(f"kubectl create secret tls {name} --key {key_path} --cert {crt_path} -n {namespace} "
                       f"--dry-run -o yaml | sudo kubectl apply -f -", timeout=300)
 
 
 class IngressNginxManifestProcessor(Processor):
-    def __init__(self, cluster: KubernetesCluster, inventory: dict,
+    def __init__(self, logger: log.VerboseLogger, inventory: dict,
                  original_yaml_path: Optional[str] = None, destination_name: Optional[str] = None):
-        plugin_name = 'nginx-ingress-controller'
-        version = inventory['plugins'][plugin_name]['version']
-        if original_yaml_path is None:
-            original_yaml_path = f"plugins/yaml/nginx-ingress-controller-{version}-original.yaml"
-        if destination_name is None:
-            destination_name = f"nginx-ingress-controller-{version}.yaml"
-        super().__init__(cluster, inventory, plugin_name, original_yaml_path, destination_name)
+        super().__init__(logger, inventory, 'nginx-ingress-controller', original_yaml_path, destination_name)
 
     def get_known_objects(self) -> List[str]:
         return [
             "Namespace_ingress-nginx",
             "ServiceAccount_ingress-nginx",
             "ServiceAccount_ingress-nginx-admission",
             "Role_ingress-nginx",
@@ -199,15 +193,15 @@
     def add_configmap_ingress_nginx_controller(self, manifest: Manifest):
         custom_headers = self.inventory['plugins']['nginx-ingress-controller'].get('custom_headers')
         if custom_headers:
             custom_headers_cm = dict(CUSTOM_HEADERS_CM)
             custom_headers_cm['data'] = custom_headers
             # Insert custom-headers ConfigMap before ingress-nginx-controller ConfigMap
             ingres_nginx_cm = manifest.key_index("ConfigMap_ingress-nginx-controller")
-            manifest.include(ingres_nginx_cm, custom_headers_cm)
+            self.include(manifest, ingres_nginx_cm, custom_headers_cm)
             self.log.verbose(f"The {manifest.obj_key(custom_headers_cm)} has been patched in 'data' "
                              f"with the data from 'plugins.nginx-ingress-controller.custom_headers'")
 
     def enrich_deployment_ingress_nginx_controller(self, manifest: Manifest):
         key = "Deployment_ingress-nginx-controller"
         source_yaml = manifest.get_obj(key, patch=True)
 
@@ -342,31 +336,31 @@
             "ClusterRoleBinding_ingress-nginx-admission",
             "Service_ingress-nginx-controller-admission",
             "Job_ingress-nginx-admission-create",
             "Job_ingress-nginx-admission-patch",
             "ValidatingWebhookConfiguration_ingress-nginx-admission",
         ]
         for key in webhook_resources:
-            manifest.exclude(key)
+            self.exclude(manifest, key)
 
     def enrich_role_ingress_nginx(self, manifest: Manifest):
         key = "Role_ingress-nginx"
         source_yaml = manifest.get_obj(key, patch=True)
         # TODO patch only if psp is enabled?
         api_list = source_yaml['rules']
         api_list.append(psp_ingress_nginx)
         self.log.verbose(f"The {key} has been patched in 'rules' with {psp_ingress_nginx}")
 
 
-def get_ingress_nginx_manifest_processor(cluster: KubernetesCluster, inventory: dict, **kwargs):
+def get_ingress_nginx_manifest_processor(logger: log.VerboseLogger, inventory: dict, **kwargs):
     version: str = inventory['plugins']['nginx-ingress-controller']['version']
     if utils.minor_version(version) == 'v1.2':
-        return V1_2_X_IngressNginxManifestProcessor(cluster, inventory, **kwargs)
+        return V1_2_X_IngressNginxManifestProcessor(logger, inventory, **kwargs)
 
-    return IngressNginxManifestProcessor(cluster, inventory, **kwargs)
+    return IngressNginxManifestProcessor(logger, inventory, **kwargs)
 
 
 CUSTOM_HEADERS_CM = {
     "apiVersion": "v1",
     "kind": "ConfigMap",
     "metadata": {
         "name": "custom-headers",
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/calico-v3.22.2.yaml.original` & `kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://github.com/projectcalico/calico/releases/download/v3.22.2/release-v3.22.2.tgz
-# manifests/calico-typha.yaml
 ---
 # Source: calico/templates/calico-config.yaml
 # This ConfigMap is used to configure a self-hosted Calico installation.
 kind: ConfigMap
 apiVersion: v1
 metadata:
   name: calico-config
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/calico-v3.24.2.yaml.original` & `kubemarine-0.16.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Source: https://raw.githubusercontent.com/projectcalico/calico/v3.24.2/manifests/calico-typha.yaml
 ---
 # Source: calico/templates/calico-kube-controllers.yaml
 # This manifest creates a Pod Disruption Budget for Controller to allow K8s Cluster Autoscaler to evict
 
 apiVersion: policy/v1
 kind: PodDisruptionBudget
 metadata:
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/dashboard-v2.5.1-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.1/aio/deploy/recommended.yaml
----
 # Copyright 2017 The Kubernetes Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/dashboard-v2.7.0-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/kubernetes/dashboard/v2.7.0/aio/deploy/recommended.yaml
----
 # Copyright 2017 The Kubernetes Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/rancher/local-path-provisioner/v0.0.22/deploy/local-path-storage.yaml
----
 apiVersion: v1
 kind: Namespace
 metadata:
   name: local-path-storage
 
 ---
 apiVersion: v1
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/rancher/local-path-provisioner/v0.0.23/deploy/local-path-storage.yaml
----
 apiVersion: v1
 kind: Namespace
 metadata:
   name: local-path-storage
 
 ---
 apiVersion: v1
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.0/deploy/static/provider/do/deploy.yaml
----
 apiVersion: v1
 kind: Namespace
 metadata:
   labels:
     app.kubernetes.io/instance: ingress-nginx
     app.kubernetes.io/name: ingress-nginx
   name: ingress-nginx
```

### Comparing `kubemarine-0.15.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.16.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Source: https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.4.0/deploy/static/provider/cloud/deploy.yaml
----
 apiVersion: v1
 kind: Namespace
 metadata:
   labels:
     app.kubernetes.io/instance: ingress-nginx
     app.kubernetes.io/name: ingress-nginx
   name: ingress-nginx
```

### Comparing `kubemarine-0.15.1/kubemarine/procedures/__init__.py` & `kubemarine-0.16.0/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/add_node.py` & `kubemarine-0.16.0/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/backup.py` & `kubemarine-0.16.0/kubemarine/procedures/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "/etc/audit/rules.d/",
         "/etc/haproxy/haproxy.cfg",
         f"/etc/systemd/system/{haproxy_service}.service.d/{haproxy_service}.conf",
         "/etc/keepalived/keepalived.conf",
         f"/etc/systemd/system/{keepalived_service}.service.d/{keepalived_service}.conf",
         "/usr/local/bin/check_haproxy.sh",
         "/etc/kubernetes",
+        "/root/.kube/config",
         "/etc/systemd/system/kubelet.service"
     ]
 
     cri_impl = cluster.inventory['services']['cri']['containerRuntime']
     if cri_impl == "docker":
         backup_files_list.append("/etc/docker/daemon.json")
     elif cri_impl == "containerd":
```

### Comparing `kubemarine-0.15.1/kubemarine/procedures/cert_renew.py` & `kubemarine-0.16.0/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/check_iaas.py` & `kubemarine-0.16.0/kubemarine/procedures/check_iaas.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,15 +859,16 @@
         cluster.log.warning(f"Nodes without python: {nodes_without_python.keys()}")
         raise TestWarn(f"Cannot perform check on {list(nodes_without_python.keys())}: python doesn't exist.")
 
 
 def check_tcp_ports(cluster):
     with TestCase(cluster.context['testsuite'], '011', 'Network', 'TCPPorts', default_results='Connected'),\
             suspend_firewalld(cluster):
-        tcp_ports = ["80", "443", "6443", "2379", "2380", "10250", "10251", "10252", "30001", "30002"]
+        tcp_ports = ["80", "443", "179", "5473", "6443", "8443", "2379", "2380", "9091", "9094", "10250", "10254",
+                     "10257", "10259", "30001", "30002"]
         nodes = {node["connect_to"]: node
                  for node in cluster.nodes['all'].get_ordered_members_list(provide_node_configs=True)}
         host_to_ip = {host: node['internal_address'] for host, node in nodes.items()}
         with install_tcp_listener(cluster, nodes, tcp_ports):
             failed_nodes = check_tcp_connect_between_all_nodes(cluster, list(nodes.values()), tcp_ports, host_to_ip)
 
             if failed_nodes:
```

### Comparing `kubemarine-0.15.1/kubemarine/procedures/check_paas.py` & `kubemarine-0.16.0/kubemarine/procedures/check_paas.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,17 +117,17 @@
     if k8s_version not in compatibility["kubeadm"]:
         raise TestWarn(f"Using not recommended k8s version: {k8s_version}")
 
     # Mapping "system_package_alias -> expected_packages_names -> expected_versions"
     # We assume that system packages have word "haproxy"/"keepalived"/"docker"/"containerd"/"podman" in their name,
     # if not - then we may miss such package
     if pckg_alias == "haproxy":
-        expected_system_packages = {"haproxy": compatibility["haproxy"][k8s_version][version_key]}
+        expected_system_packages = {"haproxy": compatibility["haproxy"][version_key]}
     elif pckg_alias == "keepalived":
-        expected_system_packages = {"keepalived": compatibility["keepalived"][k8s_version][version_key]}
+        expected_system_packages = {"keepalived": compatibility["keepalived"][version_key]}
     elif pckg_alias == "containerd":
         expected_system_packages = {"podman": compatibility["podman"][k8s_version][version_key]}
         if version_key in ["version_rhel", "version_rhel8"]:
             expected_system_packages["containerd.io"] = compatibility["containerdio"][k8s_version][version_key]
         else:
             expected_system_packages["containerd"] = compatibility["containerd"][k8s_version][version_key]
     elif pckg_alias == "docker":
@@ -378,20 +378,28 @@
                 broken.append(f'expected sha {expected_sha} is not equal to actual sha {actual_sha} for {path}')
                 continue
 
             successful.append(path)
             # SHA is correct, now check if it is an archive and if it does, then also check SHA for archive content
             if 'unpack' in config:
                 unpack_dir = config['unpack']
-                # TODO support zip
-                res = group.sudo('tar tf %s | grep -vw "./" | while read file_name; do '  # for each file in archive
+                extension = path.split('.')[-1]
+                if extension == 'zip': 
+                    res = group.sudo(' unzip -qq -l %s | awk \'NF > 3 { print $4 }\' | while read file_name; do '  # for each file in archive
+                                 '  echo ${file_name} '  # print   1) filename
+                                 '    $(sudo unzip -p %s ${file_name} | openssl sha1 | cut -d\\  -f2) '  # 2) sha archive
+                                 '    $(sudo openssl sha1 %s/${file_name} | cut -d\\  -f2); '  # 3) sha unpacked
+                                 'done' % (path, path, unpack_dir)) 
+                else :
+                    res = group.sudo('tar tf %s | grep -vw "./" | while read file_name; do '  # for each file in archive
                                  '  echo ${file_name} '  # print   1) filename
                                  '    $(sudo tar xfO %s ${file_name} | openssl sha1 | cut -d\\  -f2) '  # 2) sha archive
                                  '    $(sudo openssl sha1 %s/${file_name} | cut -d\\  -f2); '  # 3) sha unpacked
                                  'done' % (path, path, unpack_dir))
+                
                 # for each file on each host, verify that SHA in archive is equal to SHA for unpacked
                 for host, result in res.items():
                     if result.failed:
                         broken.append(f'can not verify files SHA for archive {path} '
                                       f'on host {host.host}, unpacked to {unpack_dir}')
                         continue
                     files_results = result.stdout.strip().split('\n')
@@ -837,16 +845,16 @@
 
             result = dict()
             result['name'] = control_plane['name']
             version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
 
             for static_pod in static_pods_content:
                 result[static_pod['metadata']['name']] = dict()
-                if version in static_pod["spec"]["containers"][0].get("image", ""):
-                    result[static_pod['metadata']['name']]['correct_version'] = True
+                result[static_pod['metadata']['name']]['correct_version'] = \
+                    version in static_pod["spec"]["containers"][0].get("image", "")
                 result[static_pod['metadata']['name']]['correct_properties'] = \
                     check_extra_args(cluster, static_pod, control_plane)
                 result[static_pod['metadata']['name']]['correct_volumes'] = check_extra_volumes(cluster, static_pod)
             results.append(result)
 
         message = ""
         for result in results:
@@ -961,15 +969,15 @@
         coredns_result = ddiff.to_dict().get('values_changed', {}).get("root['Corefile']", {}).get('diff')
 
         message = ""
         if coredns_result:
             message += f"CoreDNS config is outdated: \n {coredns_result} \n"
 
         coredns_version = first_control_plane.sudo("kubeadm config images list | grep coredns").get_simple_out().split(":")[1].rstrip()
-        version = ".".join(cluster.inventory['services']['kubeadm']['kubernetesVersion'].split('.')[0:2])
+        version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
         entities_to_check = {"kube-system": [{"DaemonSet": [{"calico-node": {"version": cluster.globals["compatibility_map"]["software"]["calico"][version]["version"]}},
                                                             {"kube-proxy": {"version": cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]}}]},
                                              {"Deployment": [{"calico-kube-controllers": {"version": cluster.globals["compatibility_map"]["software"]["calico"][version]["version"]}},
                                                              {"coredns": {"version": coredns_version}}]}],
                              "ingress-nginx": [{"DaemonSet": [{"ingress-nginx-controller": {"version": cluster.globals["compatibility_map"]["software"]["nginx-ingress-controller"][version]["version"]}}]}]}
 
         results = dict()
```

### Comparing `kubemarine-0.15.1/kubemarine/procedures/do.py` & `kubemarine-0.16.0/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/install.py` & `kubemarine-0.16.0/kubemarine/procedures/install.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/manage_psp.py` & `kubemarine-0.16.0/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/manage_pss.py` & `kubemarine-0.16.0/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.16.0/kubemarine/procedures/migrate_cri.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.16.0/kubemarine/procedures/migrate_kubemarine.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/reboot.py` & `kubemarine-0.16.0/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/remove_node.py` & `kubemarine-0.16.0/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/restore.py` & `kubemarine-0.16.0/kubemarine/procedures/restore.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/procedures/upgrade.py` & `kubemarine-0.16.0/kubemarine/procedures/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,22 @@
     """
 
 
     cri = cluster.inventory["services"]["cri"]['containerRuntime']
     if cri == 'containerd':
         path = 'plugins."io.containerd.grpc.v1.cri"'
         target_kubernetes_version = cluster.context["upgrade_version"]
-        index_pos = target_kubernetes_version.rfind(".")
-        target_kubernetes_version = target_kubernetes_version[:index_pos]
-        pause_version = cluster.globals['compatibility_map']['software']['pause'][target_kubernetes_version]['version']
+        pause_mapping = cluster.globals['compatibility_map']['software']['pause']
+        if target_kubernetes_version not in pause_mapping:
+            raise Exception(f"Upgrade to {target_kubernetes_version} is not supported")
+        pause_version = pause_mapping[target_kubernetes_version]['version']
         if not cluster.inventory["services"]["cri"]['containerdConfig'].get(path, False):
             return
         last_pause_version = cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"].split(":")[2]
-        if last_pause_version != pause_version:
+        if True:
             sandbox = cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"]
             param_begin_pos = sandbox.rfind(":")
             sandbox = sandbox[:param_begin_pos] + ":" + str(pause_version)
             cluster.inventory["services"]["cri"]['containerdConfig'][path]["sandbox_image"] = sandbox
             config_string = ""
             containerd_config = cluster.inventory["services"]["cri"]['containerdConfig']
             runc_options_path = 'plugins."io.containerd.grpc.v1.cri".containerd.runtimes.runc.options'
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.16.0/kubemarine/resources/configurations/defaults.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 vrrp_ips: []
 
 globals: 
+  expect:
+    deployments:
+      timeout: 5
+      retries: 45
+    pods:
+      kubernetes:
+        timeout: 5
+        retries: 30
+      plugins:
+        timeout: 5
+        retries: 150
   nodes:
     ready:
       timeout: 5
       retries: 15
     boot:
      timeout: 600
   timeout_download:
@@ -17,24 +28,25 @@
 public_cluster_ip: '{{ control_plain.external }}'
 
 services:
   kubeadm_kubelet:
     apiVersion: kubelet.config.k8s.io/v1beta1
     kind: KubeletConfiguration
     readOnlyPort: 0
+    enableDebuggingHandlers: true
     protectKernelDefaults: true
     podPidsLimit: 4096
     cgroupDriver: systemd
   kubeadm_flags:
     ignorePreflightErrors: Port-6443,CoreDNSUnsupportedPlugins
   kubeadm:
     # for patches functionality we need v1beta3 which is available since k8s v1.22 only
     apiVersion: '{% if "v1.21" in services["kubeadm"]["kubernetesVersion"] %}kubeadm.k8s.io/v1beta2{% else %}kubeadm.k8s.io/v1beta3{% endif %}'
     kind: ClusterConfiguration
-    kubernetesVersion: v1.24.11
+    kubernetesVersion: v1.26.3
     controlPlaneEndpoint: '{{ cluster_name }}:6443'
     networking:
       podSubnet: '{% if nodes[0]["internal_address"]|isipv4 %}10.128.0.0/14{% else %}fd02::/48{% endif %}'
       serviceSubnet: '{% if nodes[0]["internal_address"]|isipv4 %}172.30.0.0/16{% else %}fd03::/112{% endif %}'
     apiServer:
       certSANs: []
       extraArgs:
@@ -86,31 +98,28 @@
       state: enforcing
       policy: targeted
       permissive:
         - haproxy_t
         - container_t
         - keepalived_t
 
+  # Default "source" is enriched from "thirdparties" section of globals.yaml
+  # Default "sha1" is enriched from kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
   thirdparties:
     /usr/bin/etcdctl:
       source: 'resources/scripts/etcdctl.sh'
       group: control-plane
-    /usr/bin/kubeadm:
-      source: 'https://storage.googleapis.com/kubernetes-release/release/{{ services.kubeadm.kubernetesVersion }}/bin/linux/amd64/kubeadm'
-    /usr/bin/kubelet:
-      source: 'https://storage.googleapis.com/kubernetes-release/release/{{ services.kubeadm.kubernetesVersion }}/bin/linux/amd64/kubelet'
+    /usr/bin/kubeadm: {}
+    /usr/bin/kubelet: {}
     /usr/bin/kubectl:
-      source: 'https://storage.googleapis.com/kubernetes-release/release/{{ services.kubeadm.kubernetesVersion }}/bin/linux/amd64/kubectl'
       group: control-plane
     /usr/bin/calicoctl:
-      source: 'https://github.com/projectcalico/calico/releases/download/{{ plugins.calico.version }}/calicoctl-linux-amd64'
       group: control-plane
     # "crictl" is installed by default ONLY if "containerRuntime != docker", otherwise it is removed programmatically
     /usr/bin/crictl.tar.gz:
-      source: 'https://github.com/kubernetes-sigs/cri-tools/releases/download/{{ globals.compatibility_map.software.crictl[services.kubeadm.kubernetesVersion].version }}/crictl-{{ globals.compatibility_map.software.crictl[services.kubeadm.kubernetesVersion].version }}-linux-amd64.tar.gz'
       unpack: /usr/bin/
 
   cri:
     containerRuntime: containerd
     containerdConfig:
       version: 2
       plugins."io.containerd.grpc.v1.cri".containerd.runtimes.runc:
@@ -126,20 +135,35 @@
       exec-opts:
         - native.cgroupdriver=systemd
       icc: False
       live-restore: True
       userland-proxy: False
 
   modprobe:
-    - br_netfilter
-    - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
-    - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_conntrack_ipv6{% endif %}'
-    - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat_masquerade_ipv6{% endif %}'
-    - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
-    - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
+    rhel:
+      - br_netfilter
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_conntrack_ipv6{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat_masquerade_ipv6{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
+    rhel8:
+      - br_netfilter
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_conntrack{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
+    debian:
+      - br_netfilter
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}ip6table_filter{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_conntrack{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_nat{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_reject_ipv6{% endif %}'
+      - '{% if not nodes[0]["internal_address"]|isipv4 %}nf_defrag_ipv6{% endif %}'
 
   sysctl:
     net.bridge.bridge-nf-call-iptables: 1
     net.ipv4.ip_forward: 1
     net.ipv4.ip_nonlocal_bind: 1
     net.ipv4.conf.all.route_localnet: 1
     net.bridge.bridge-nf-call-ip6tables: '{% if not nodes[0]["internal_address"]|isipv4 %}1{% endif %}'
@@ -348,18 +372,18 @@
             - 'containerd.io={{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_debian }}'
         containerd:
           package_name:
             - 'containerd={{ globals.compatibility_map.software.containerd[services.kubeadm.kubernetesVersion].version_debian }}'
             - 'podman={{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_debian }}'
         haproxy:
           executable_name: 'haproxy'
-          package_name: 'haproxy={{ globals.compatibility_map.software.haproxy[services.kubeadm.kubernetesVersion].version_debian }}'
+          package_name: 'haproxy={{ globals.compatibility_map.software.haproxy.version_debian }}'
           service_name: 'haproxy'
         keepalived:
-          package_name: 'keepalived={{ globals.compatibility_map.software.keepalived[services.kubeadm.kubernetesVersion].version_debian }}'
+          package_name: 'keepalived={{ globals.compatibility_map.software.keepalived.version_debian }}'
         audit:
           package_name: 'auditd'
         conntrack:
           package_name: 'conntrack'
       rhel:
         docker:
           package_name:
@@ -368,18 +392,18 @@
             - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel }}'
         containerd:
           package_name:
             - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel }}'
             - 'podman-{{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_rhel }}'
         haproxy:
           executable_name: '/opt/rh/rh-haproxy18/root/usr/sbin/haproxy'
-          package_name: 'rh-haproxy18-haproxy-{{ globals.compatibility_map.software.haproxy[services.kubeadm.kubernetesVersion].version_rhel }}'
+          package_name: 'rh-haproxy18-haproxy-{{ globals.compatibility_map.software.haproxy.version_rhel }}'
           service_name: 'rh-haproxy18-haproxy'
         keepalived:
-          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived[services.kubeadm.kubernetesVersion].version_rhel }}'
+          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived.version_rhel }}'
         audit:
           package_name: 'audit'
         conntrack:
           package_name: 'conntrack-tools'
         semanage:
           package_name: 'policycoreutils-python'
       rhel8:
@@ -390,32 +414,32 @@
             - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel8 }}'
         containerd:
           package_name:
             - 'containerd.io-{{ globals.compatibility_map.software.containerdio[services.kubeadm.kubernetesVersion].version_rhel8 }}'
             - 'podman-{{ globals.compatibility_map.software.podman[services.kubeadm.kubernetesVersion].version_rhel8 }}'
         haproxy:
           executable_name: '/usr/sbin/haproxy'
-          package_name: 'haproxy-{{ globals.compatibility_map.software.haproxy[services.kubeadm.kubernetesVersion].version_rhel8 }}'
+          package_name: 'haproxy-{{ globals.compatibility_map.software.haproxy.version_rhel8 }}'
           service_name: 'haproxy'
         keepalived:
-          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived[services.kubeadm.kubernetesVersion].version_rhel8 }}'
+          package_name: 'keepalived-{{ globals.compatibility_map.software.keepalived.version_rhel8 }}'
         audit:
           package_name: 'audit'
         conntrack:
           package_name: 'conntrack-tools'
         semanage:
           package_name: 'policycoreutils-python-utils'
 
 plugin_defaults:
   installation: {}
 
 plugins:
 
   calico:
-    version: '{{ globals.compatibility_map.software["calico"][services.kubeadm.kubernetesVersion|minorversion].version }}'
+    version: '{{ globals.compatibility_map.software["calico"][services.kubeadm.kubernetesVersion].version }}'
     install: true
     installation:
       priority: 0
       procedures:
         - python:
             module: plugins/builtin.py
             method: apply_yaml
@@ -427,16 +451,14 @@
             deployments:
               - calico-kube-controllers
             pods:
               list:
                 - coredns
                 - calico-kube-controllers
                 - calico-node
-              timeout: 5
-              retries: 150
         - thirdparty: /usr/bin/calicoctl
         - shell:
             command: mkdir -p /etc/calico
             groups: ['control-plane']
             sudo: true
         - template:
             source: templates/plugins/calicoctl.cfg.j2
@@ -525,15 +547,15 @@
       image: 'calico/kube-controllers:{{ plugins.calico.version }}'
       nodeSelector:
         kubernetes.io/os: linux
     flexvol:
       image: 'calico/pod2daemon-flexvol:{{ plugins.calico.version }}'
 
   nginx-ingress-controller:
-    version: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|minorversion].version }}'
+    version: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion].version }}'
     install: true
     installation:
       registry: k8s.gcr.io
       priority: 1
       procedures:
         - python:
             module: plugins/nginx_ingress.py
@@ -544,19 +566,19 @@
             arguments:
               plugin_name: nginx-ingress-controller
         - expect:
             daemonsets:
               - name: ingress-nginx-controller
                 namespace: ingress-nginx
             pods:
-              - '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|minorversion]["pod-name"] }}'
+              - ingress-nginx-controller
     webhook:
-      image: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|minorversion]["webhook-image-name"] }}:{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|minorversion]["webhook-version"] }}'
+      image: 'ingress-nginx/kube-webhook-certgen:{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion]["webhook-version"] }}'
     controller:
-      image: '{{ globals.compatibility_map.software["nginx-ingress-controller"][services.kubeadm.kubernetesVersion|minorversion]["image-name"] }}:{{ plugins["nginx-ingress-controller"].version }}'
+      image: 'ingress-nginx/controller:{{ plugins["nginx-ingress-controller"].version }}'
       ssl:
         enableSslPassthrough: false
       nodeSelector:
         kubernetes.io/os: linux
     ports:
       - name: http
         containerPort: 80
@@ -570,15 +592,15 @@
         containerPort: 10254
         protocol: TCP
       - name: webhook
         containerPort: 8443
         protocol: TCP
 
   kubernetes-dashboard:
-    version: '{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion|minorversion].version }}'
+    version: '{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion].version }}'
     install: false
     installation:
       priority: 2
       procedures:
         - python:
             module: plugins/builtin.py
             method: apply_yaml
@@ -599,15 +621,15 @@
             method: schedule_summary_report
     hostname: 'dashboard.{{ cluster_name }}'
     dashboard:
       image: 'kubernetesui/dashboard:{{ plugins["kubernetes-dashboard"].version }}'
       nodeSelector:
         kubernetes.io/os: linux
     metrics-scraper:
-      image: 'kubernetesui/metrics-scraper:{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion|minorversion]["metrics-scraper-version"] }}'
+      image: 'kubernetesui/metrics-scraper:{{ globals.compatibility_map.software["kubernetes-dashboard"][services.kubeadm.kubernetesVersion]["metrics-scraper-version"] }}'
       nodeSelector:
         kubernetes.io/os: linux
     ingress:
       metadata:
         name: kubernetes-dashboard
         namespace: kubernetes-dashboard
         annotations:
@@ -632,15 +654,15 @@
                   backend:
                     service:
                       name: kubernetes-dashboard
                       port:
                         number: 443
 
   local-path-provisioner:
-    version: '{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion|minorversion].version }}'
+    version: '{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion].version }}'
     install: false
     installation:
       priority: 2
       procedures:
       - python:
           module: plugins/builtin.py
           method: apply_yaml
@@ -650,15 +672,15 @@
           pods:
             - local-path-provisioner
     storage-class:
       name: local-path
       is-default: "false"
     volume-dir: /opt/local-path-provisioner
     image: 'rancher/local-path-provisioner:{{ plugins["local-path-provisioner"].version }}'
-    helper-pod-image: 'library/busybox:{{ globals.compatibility_map.software["busybox"][services.kubeadm.kubernetesVersion|minorversion].version }}'
+    helper-pod-image: 'library/busybox:{{ globals.compatibility_map.software["local-path-provisioner"][services.kubeadm.kubernetesVersion]["busybox-version"] }}'
 
 rbac:
   account_defaults:
     namespace: kube-system
     configs:
       - apiVersion: v1
         kind: ServiceAccount
@@ -674,15 +696,14 @@
           - kind: ServiceAccount
       - apiVersion: v1
         kind: Secret
         metadata:
           annotations: {}
         type: kubernetes.io/service-account-token
 
-  admission: psp
   psp:
     pod-security: enabled
     oob-policies:
       default: enabled
       host-network: enabled
       anyuid: enabled
     custom-policies:
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/psp/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.16.0/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/psp/default.yaml` & `kubemarine-0.16.0/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.16.0/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.16.0/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/reports/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/reports/check_report.css` & `kubemarine-0.16.0/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/backup.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'description'": "'Configure settings of different services'",*

 * * "'properties'": "{replace: OrderedDict([('kubeadm_kubelet', OrderedDict([('$ref', "*

 * *                 "'services/kubeadm_kubelet.json')])), ('kubeadm_patches', OrderedDict([('$ref', "*

 * *                 "'services/kubeadm_patches.json')])), ('kubeadm_flags', OrderedDict([('type', "*

 * *                 "'object'), ('description', 'Flags for kubeadm command line tool'), "*

 * *                 "('properties', OrderedDict([('ignorePreflightErrors', OrderedD […]*

```diff
@@ -1,57 +1,66 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
-    "definitions": {
-        "Nodes": {
+    "description": "Configure settings of different services",
+    "properties": {
+        "audit": {
+            "$ref": "services/audit.json"
+        },
+        "coredns": {
+            "$ref": "services/coredns.json"
+        },
+        "cri": {
+            "$ref": "services/cri.json"
+        },
+        "etc_hosts": {
+            "$ref": "services/etc_hosts.json"
+        },
+        "kernel_security": {
+            "$ref": "services/kernel_security.json"
+        },
+        "kubeadm": {
+            "$ref": "services/kubeadm.json"
+        },
+        "kubeadm_flags": {
             "additionalProperties": false,
-            "description": "Section to hold mostly timeout-related settings, global for nodes",
+            "description": "Flags for kubeadm command line tool",
             "properties": {
-                "boot": {
-                    "additionalProperties": false,
-                    "description": "Nodes boot settings",
-                    "properties": {
-                        "timeout": {
-                            "default": 600,
-                            "description": "Timeout for node reboot in seconds",
-                            "minimal": 1,
-                            "type": "integer"
-                        }
-                    },
-                    "type": "object"
-                },
-                "ready": {
-                    "additionalProperties": false,
-                    "description": "Settings for Kubernetes nodes readiness check",
-                    "properties": {
-                        "retries": {
-                            "default": 30,
-                            "description": "Number of retries for node readiness check",
-                            "minimal": 1,
-                            "type": "integer"
-                        },
-                        "timeout": {
-                            "default": 5,
-                            "description": "Timeout for node readiness check in seconds",
-                            "minimal": 1,
-                            "type": "integer"
-                        }
-                    },
-                    "type": "object"
+                "ignorePreflightErrors": {
+                    "default": "Port-6443,CoreDNSUnsupportedPlugins",
+                    "description": "Kubeadm preflight errors to be ignored for a successful deploy or upgrade",
+                    "type": "string"
                 }
             },
             "type": "object"
-        }
-    },
-    "description": "Section to hold the parameters which override global settings",
-    "properties": {
-        "nodes": {
-            "$ref": "#/definitions/Nodes"
         },
-        "timeout_download": {
-            "default": 60,
-            "description": "Timeout for the thirdparties download on nodes.",
-            "type": "integer"
+        "kubeadm_kubelet": {
+            "$ref": "services/kubeadm_kubelet.json"
+        },
+        "kubeadm_patches": {
+            "$ref": "services/kubeadm_patches.json"
+        },
+        "loadbalancer": {
+            "$ref": "services/loadbalancer.json"
+        },
+        "modprobe": {
+            "$ref": "services/modprobe.json"
+        },
+        "ntp": {
+            "$ref": "services/ntp.json"
+        },
+        "packages": {
+            "$ref": "services/packages.json"
+        },
+        "resolv.conf": {
+            "$ref": "services/resolv.conf.json"
+        },
+        "sysctl": {
+            "$ref": "services/sysctl.json"
+        },
+        "thirdparties": {
+            "$ref": "services/thirdparties.json"
         }
     },
+    "required": [],
     "type": "object"
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6652777777777777%*

 * *Differences: {"'description'": "'An alias for template that allows you not to render the contents of the files'",*

 * * "'oneOf'": "{1: {'properties': {'do_render': {'description': 'Allows you not to render the "*

 * *            "contents of the file'}}}}"}*

```diff
@@ -1,22 +1,24 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
+    "description": "An alias for template that allows you not to render the contents of the files",
     "oneOf": [
         {
             "type": "string"
         },
         {
             "allOf": [
                 {
                     "$ref": "template.json#/definitions/Properties"
                 }
             ],
             "properties": {
                 "do_render": {
                     "default": true,
+                    "description": "Allows you not to render the contents of the file",
                     "type": "boolean"
                 }
             },
             "propertyNames": {
                 "anyOf": [
                     {
                         "$ref": "template.json#/definitions/PropertyNames"
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/restore.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('ThirdParty', OrderedDict([('type', 'object'), "*

 * *                  "('description', 'The absolute destination path of the 3rd-party on the host "*

 * *                  "system of the cluster'), ('allOf', [OrderedDict([('$ref', "*

 * *                  "'definitions/services/thirdparties.json#/definitions/MinimalThirdPartyProperties')])]), "*

 * *                  "('required', ['source']), ('propertyNames', OrderedDict([('$ref', "*

 * *                  "'definitions/services/thirdpa […]*

```diff
@@ -1,143 +1,107 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "definitions": {
-        "CommonResourceProperties": {
-            "properties": {
-                "retries": {
-                    "default": 30,
-                    "type": "integer"
-                },
-                "timeout": {
-                    "default": 5,
-                    "type": "integer"
-                }
-            }
-        },
-        "CommonResourcePropertyNames": {
-            "enum": [
-                "timeout",
-                "retries"
-            ]
-        },
-        "GenericResource": {
-            "oneOf": [
+        "ThirdParty": {
+            "allOf": [
                 {
-                    "$ref": "#/definitions/ResourcesList"
-                },
-                {
-                    "allOf": [
-                        {
-                            "$ref": "#/definitions/CommonResourceProperties"
-                        }
-                    ],
+                    "$ref": "definitions/services/thirdparties.json#/definitions/MinimalThirdPartyProperties"
+                }
+            ],
+            "description": "The absolute destination path of the 3rd-party on the host system of the cluster",
+            "propertyNames": {
+                "$ref": "definitions/services/thirdparties.json#/definitions/MinimalThirdPartyPropertyNames"
+            },
+            "required": [
+                "source"
+            ],
+            "type": "object"
+        }
+    },
+    "properties": {
+        "backup_location": {
+            "description": "Path to the file with the backup from which the recovery is performed",
+            "type": "string"
+        },
+        "restore_plan": {
+            "additionalProperties": false,
+            "description": "Restore procedure configuration",
+            "properties": {
+                "etcd": {
+                    "additionalProperties": false,
+                    "description": "Additional parameters for ETCD restore",
                     "properties": {
-                        "list": {
-                            "$ref": "#/definitions/ResourcesList"
-                        }
-                    },
-                    "propertyNames": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/CommonResourcePropertyNames"
+                        "certificates": {
+                            "additionalProperties": false,
+                            "description": "ETCD certificates for etcdctl connection to ETCD API. You can specify some certificates, or specify them all. Certificates should be presented on all nodes.",
+                            "properties": {
+                                "cacert": {
+                                    "default": "/etc/kubernetes/pki/etcd/ca.crt",
+                                    "type": "string"
+                                },
+                                "cert": {
+                                    "default": "/etc/kubernetes/pki/etcd/server.crt",
+                                    "type": "string"
+                                },
+                                "key": {
+                                    "default": "/etc/kubernetes/pki/etcd/server.key",
+                                    "type": "string"
+                                },
+                                "peer_cacert": {
+                                    "default": "/etc/kubernetes/pki/etcd/ca.crt",
+                                    "type": "string"
+                                },
+                                "peer_cert": {
+                                    "default": "/etc/kubernetes/pki/etcd/peer.crt",
+                                    "type": "string"
+                                },
+                                "peer_key": {
+                                    "default": "/etc/kubernetes/pki/etcd/peer.key",
+                                    "type": "string"
+                                }
                             },
-                            {
-                                "enum": [
-                                    "list"
-                                ]
-                            }
-                        ]
+                            "type": "object"
+                        },
+                        "image": {
+                            "description": "Full name of the ETCD image, including the registry address. On its basis, the restoration is performed.",
+                            "type": "string"
+                        }
                     },
-                    "required": [
-                        "list"
-                    ],
                     "type": "object"
-                }
-            ]
-        },
-        "Pods": {
-            "oneOf": [
-                {
-                    "$ref": "#/definitions/PodsList"
                 },
-                {
-                    "allOf": [
-                        {
-                            "$ref": "#/definitions/CommonResourceProperties"
-                        }
-                    ],
+                "thirdparties": {
+                    "additionalProperties": {
+                        "$ref": "#/definitions/ThirdParty"
+                    },
+                    "description": "Specify sources of the 3rd-parties to restore in case the corresponding sources in cluster.yaml are outdated",
                     "properties": {
-                        "list": {
-                            "$ref": "#/definitions/PodsList"
+                        "/usr/bin/calicoctl": {
+                            "$ref": "#/definitions/ThirdParty"
                         },
-                        "namespace": {
-                            "type": "string"
+                        "/usr/bin/crictl.tar.gz": {
+                            "$ref": "#/definitions/ThirdParty"
+                        },
+                        "/usr/bin/etcdctl": {
+                            "$ref": "#/definitions/ThirdParty"
+                        },
+                        "/usr/bin/kubeadm": {
+                            "$ref": "#/definitions/ThirdParty"
+                        },
+                        "/usr/bin/kubectl": {
+                            "$ref": "#/definitions/ThirdParty"
+                        },
+                        "/usr/bin/kubelet": {
+                            "$ref": "#/definitions/ThirdParty"
                         }
                     },
-                    "propertyNames": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/CommonResourcePropertyNames"
-                            },
-                            {
-                                "enum": [
-                                    "list",
-                                    "namespace"
-                                ]
-                            }
-                        ]
-                    },
-                    "required": [
-                        "list"
-                    ],
                     "type": "object"
                 }
-            ]
-        },
-        "PodsList": {
-            "$ref": "../../common/utils.json#/definitions/SetOfStrings"
-        },
-        "ResourcesList": {
-            "items": {
-                "oneOf": [
-                    {
-                        "type": "string"
-                    },
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "name": {
-                                "type": "string"
-                            },
-                            "namespace": {
-                                "default": "kube-system",
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
-                    }
-                ]
             },
-            "type": "array"
-        }
-    },
-    "minProperties": 1,
-    "properties": {
-        "daemonsets": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "deployments": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "pods": {
-            "$ref": "#/definitions/Pods"
-        },
-        "replicasets": {
-            "$ref": "#/definitions/GenericResource"
-        },
-        "statefulsets": {
-            "$ref": "#/definitions/GenericResource"
+            "type": "object"
         }
     },
+    "required": [
+        "backup_location"
+    ],
     "type": "object"
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14285714285714285%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'definitions'": "OrderedDict([('control-plane-pod-patch', OrderedDict([('type', 'array'), "*

 * *                  "('description', 'Patches for control-plane pods'), ('minItems', 0), ('items', "*

 * *                  "OrderedDict([('anyOf', [OrderedDict([('type', 'object'), "*

 * *                  "('additionalProperties', False), ('properties', OrderedDict([('groups', "*

 * *                  "OrderedDict([('type', 'array'), ('items', OrderedDict([('enum', "*

 * *                  "['contro […]*

```diff
@@ -1,80 +1,132 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "oneOf": [
-        {
-            "minLength": 1,
-            "type": "string"
-        },
-        {
-            "additionalProperties": false,
-            "properties": {
-                "command": {
-                    "oneOf": [
-                        {
-                            "minLength": 1,
-                            "type": "string"
+    "additionalProperties": false,
+    "definitions": {
+        "control-plane-pod-patch": {
+            "description": "Patches for control-plane pods",
+            "items": {
+                "anyOf": [
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "groups": {
+                                "items": {
+                                    "enum": [
+                                        "control-plane"
+                                    ]
+                                },
+                                "type": "array"
+                            },
+                            "patch": {
+                                "properties": {
+                                    "additionalProperties": {
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
                         },
-                        {
-                            "items": {
-                                "minLength": 1,
-                                "type": "string"
+                        "type": "object"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "nodes": {
+                                "items": [
+                                    {
+                                        "type": "string"
+                                    }
+                                ],
+                                "type": "array"
                             },
-                            "minItems": 1,
-                            "type": "array"
-                        }
-                    ]
-                },
-                "groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles"
-                },
-                "in_vars": {
-                    "items": {
+                            "patch": {
+                                "properties": {
+                                    "additionalProperties": {
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        },
+                        "type": "object"
+                    }
+                ]
+            },
+            "minItems": 0,
+            "type": "array"
+        },
+        "kubelet-patch": {
+            "description": "Patches for kubelet",
+            "items": {
+                "anyOf": [
+                    {
                         "additionalProperties": false,
                         "properties": {
-                            "name": {
-                                "type": "string"
+                            "groups": {
+                                "items": {
+                                    "enum": [
+                                        "control-plane",
+                                        "worker"
+                                    ]
+                                },
+                                "type": "array"
                             },
-                            "value": {
-                                "type": "string"
+                            "patch": {
+                                "properties": {
+                                    "additionalProperties": {
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
                             }
                         },
-                        "required": [
-                            "name"
-                        ],
                         "type": "object"
                     },
-                    "type": "array"
-                },
-                "nodes": {
-                    "$ref": "../../common/node_ref.json#/definitions/Names"
-                },
-                "out_vars": {
-                    "items": {
+                    {
                         "additionalProperties": false,
                         "properties": {
-                            "name": {
-                                "type": "string"
+                            "nodes": {
+                                "items": [
+                                    {
+                                        "type": "string"
+                                    }
+                                ],
+                                "type": "array"
                             },
-                            "save_as": {
-                                "type": "string"
+                            "patch": {
+                                "properties": {
+                                    "additionalProperties": {
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
                             }
                         },
-                        "required": [
-                            "name"
-                        ],
                         "type": "object"
-                    },
-                    "type": "array"
-                },
-                "sudo": {
-                    "default": false,
-                    "type": "boolean"
-                }
+                    }
+                ]
             },
-            "required": [
-                "command"
-            ],
-            "type": "object"
+            "minItems": 0,
+            "type": "array"
+        }
+    },
+    "description": "Override the original settings for patches of control-plane pods and kubelet",
+    "properties": {
+        "apiServer": {
+            "$ref": "#/definitions/control-plane-pod-patch"
+        },
+        "controllerManager": {
+            "$ref": "#/definitions/control-plane-pod-patch"
+        },
+        "etcd": {
+            "$ref": "#/definitions/control-plane-pod-patch"
+        },
+        "kubelet": {
+            "$ref": "#/definitions/kubelet-patch"
+        },
+        "scheduler": {
+            "$ref": "#/definitions/control-plane-pod-patch"
         }
-    ]
+    },
+    "type": "object"
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2357142857142857%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '#/definitions/Properties')])]",*

 * * "'definitions'": "{'Properties': {'properties': {replace: OrderedDict([('pod-security', "*

 * *                  "OrderedDict([('enum', ['enabled', 'disabled']), ('default', 'enabled'), "*

 * *                  "('description', 'Specify if PSS should be enabled/disabled')])), ('defaults', "*

 * *                  'OrderedDict([(\'$ref\', \'#/definitions/Profiles\'), (\'description\', "Default '*

 * *                  "profiles that are passed to 'defaults' s […]*

```diff
@@ -1,70 +1,111 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
+    "allOf": [
+        {
+            "$ref": "#/definitions/Properties"
+        }
+    ],
     "definitions": {
-        "Properties": {
+        "Profile": {
+            "default": "baseline",
+            "enum": [
+                "privileged",
+                "baseline",
+                "restricted"
+            ]
+        },
+        "ProfileVersion": {
+            "default": "latest",
+            "type": [
+                "string"
+            ]
+        },
+        "Profiles": {
+            "additionalProperties": false,
             "properties": {
-                "apply_command": {
-                    "type": "string"
-                },
-                "apply_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles"
-                },
-                "apply_nodes": {
-                    "$ref": "../../common/node_ref.json#/definitions/Names"
+                "audit": {
+                    "$ref": "#/definitions/Profile"
                 },
-                "apply_required": {
-                    "default": true,
-                    "type": "boolean"
+                "audit-version": {
+                    "$ref": "#/definitions/ProfileVersion"
                 },
-                "destination": {
-                    "type": "string"
+                "enforce": {
+                    "$ref": "#/definitions/Profile"
                 },
-                "destination_groups": {
-                    "$ref": "../../common/node_ref.json#/definitions/Roles"
+                "enforce-version": {
+                    "$ref": "#/definitions/ProfileVersion"
                 },
-                "destination_nodes": {
-                    "$ref": "../../common/node_ref.json#/definitions/Names"
+                "warn": {
+                    "$ref": "#/definitions/Profile"
                 },
-                "source": {
-                    "type": "string"
-                },
-                "sudo": {
-                    "default": true,
-                    "type": "boolean"
+                "warn-version": {
+                    "$ref": "#/definitions/ProfileVersion"
+                }
+            },
+            "type": "object"
+        },
+        "Properties": {
+            "properties": {
+                "defaults": {
+                    "$ref": "#/definitions/Profiles",
+                    "description": "Default profiles that are passed to 'defaults' section of PodSecurityConfiguration"
+                },
+                "exemptions": {
+                    "additionalProperties": false,
+                    "description": "The section describes objects that are not enforced by the policy",
+                    "properties": {
+                        "namespaces": {
+                            "description": "List of namespaces to not enforce the policy",
+                            "items": {
+                                "anyOf": [
+                                    {
+                                        "enum": [
+                                            "kube-system"
+                                        ],
+                                        "type": "string"
+                                    },
+                                    {
+                                        "type": "string"
+                                    },
+                                    {
+                                        "$ref": "../common/utils.json#/definitions/ListMergingSymbol"
+                                    }
+                                ]
+                            },
+                            "type": "array",
+                            "uniqueItems": true
+                        },
+                        "runtimeClasses": {
+                            "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings"
+                        },
+                        "usernames": {
+                            "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
+                            "description": "List of User or ServiceAccount names"
+                        }
+                    },
+                    "type": "object"
+                },
+                "pod-security": {
+                    "default": "enabled",
+                    "description": "Specify if PSS should be enabled/disabled",
+                    "enum": [
+                        "enabled",
+                        "disabled"
+                    ]
                 }
             }
         },
         "PropertyNames": {
             "enum": [
-                "source",
-                "destination",
-                "apply_required",
-                "apply_command",
-                "sudo",
-                "destination_groups",
-                "destination_nodes",
-                "apply_groups",
-                "apply_nodes"
+                "pod-security",
+                "defaults",
+                "exemptions"
             ]
         }
     },
-    "oneOf": [
-        {
-            "type": "string"
-        },
-        {
-            "allOf": [
-                {
-                    "$ref": "#/definitions/Properties"
-                }
-            ],
-            "propertyNames": {
-                "$ref": "#/definitions/PropertyNames"
-            },
-            "required": [
-                "source"
-            ],
-            "type": "object"
-        }
-    ]
+    "description": "PSS configuration section",
+    "propertyNames": {
+        "$ref": "#/definitions/PropertyNames"
+    },
+    "type": "object"
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999909577546297%*

 * *Differences: {"'properties'": "{'procedures': {'items': {'properties': {'thirdparty': {'description': 'Trigger "*

 * *                 'specific thirdparty installation. This thirdparty must be configured in the '*

 * *                 "thirdparties section.'}}}}}"}*

```diff
@@ -52,14 +52,15 @@
                     "shell": {
                         "$ref": "installation/shell.json"
                     },
                     "template": {
                         "$ref": "installation/template.json"
                     },
                     "thirdparty": {
+                        "description": "Trigger specific thirdparty installation. This thirdparty must be configured in the thirdparties section.",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
             "minItems": 1,
             "type": "array"
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.21428571428571427%*

 * *Differences: {"'description'": "'Execute shell code on remote hosts. Can be either a command string or a "*

 * *                  "dictionary with the extra parameters.'",*

 * * "'oneOf'": "[OrderedDict([('type', 'string'), ('minLength', 1)]), OrderedDict([('type', "*

 * *            "'object'), ('properties', OrderedDict([('command', OrderedDict([('description', "*

 * *            '"A shell command(s) to be executed on remote hosts. If the list of commands is '*

 * *            'provided, they will be joint with \'&&\'."), (\'oneOf\', [Ordered […]*

```diff
@@ -1,111 +1,87 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "allOf": [
+    "description": "Execute shell code on remote hosts. Can be either a command string or a dictionary with the extra parameters.",
+    "oneOf": [
         {
-            "$ref": "#/definitions/Properties"
-        }
-    ],
-    "definitions": {
-        "Profile": {
-            "default": "baseline",
-            "enum": [
-                "privileged",
-                "baseline",
-                "restricted"
-            ]
-        },
-        "ProfileVersion": {
-            "default": "latest",
-            "type": [
-                "string"
-            ]
+            "minLength": 1,
+            "type": "string"
         },
-        "Profiles": {
+        {
             "additionalProperties": false,
             "properties": {
-                "audit": {
-                    "$ref": "#/definitions/Profile"
-                },
-                "audit-version": {
-                    "$ref": "#/definitions/ProfileVersion"
-                },
-                "enforce": {
-                    "$ref": "#/definitions/Profile"
-                },
-                "enforce-version": {
-                    "$ref": "#/definitions/ProfileVersion"
-                },
-                "warn": {
-                    "$ref": "#/definitions/Profile"
-                },
-                "warn-version": {
-                    "$ref": "#/definitions/ProfileVersion"
-                }
-            },
-            "type": "object"
-        },
-        "Properties": {
-            "properties": {
-                "defaults": {
-                    "$ref": "#/definitions/Profiles",
-                    "description": "Default profiles that are passed to 'defaults' section of PodSecurityConfiguration"
-                },
-                "exemptions": {
-                    "additionalProperties": false,
-                    "description": "The section describes objects that are not enforced by the policy",
-                    "properties": {
-                        "namespaces": {
-                            "description": "List of namespaces to not enforce the policy",
+                "command": {
+                    "description": "A shell command(s) to be executed on remote hosts. If the list of commands is provided, they will be joint with '&&'.",
+                    "oneOf": [
+                        {
+                            "minLength": 1,
+                            "type": "string"
+                        },
+                        {
                             "items": {
-                                "anyOf": [
-                                    {
-                                        "enum": [
-                                            "kube-system"
-                                        ],
-                                        "type": "string"
-                                    },
-                                    {
-                                        "type": "string"
-                                    },
-                                    {
-                                        "$ref": "../common/utils.json#/definitions/ListMergingSymbol"
-                                    }
-                                ]
+                                "minLength": 1,
+                                "type": "string"
                             },
-                            "type": "array",
-                            "uniqueItems": true
+                            "minItems": 1,
+                            "type": "array"
+                        }
+                    ]
+                },
+                "groups": {
+                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "description": "List of groups on which the shell command should be executed"
+                },
+                "in_vars": {
+                    "description": "List of ENV variables to import before command execution",
+                    "items": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "name": {
+                                "type": "string"
+                            },
+                            "value": {
+                                "type": "string"
+                            }
                         },
-                        "runtimeClasses": {
-                            "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings"
+                        "required": [
+                            "name"
+                        ],
+                        "type": "object"
+                    },
+                    "type": "array"
+                },
+                "nodes": {
+                    "$ref": "../../common/node_ref.json#/definitions/Names",
+                    "description": "List of nodes on which the shell command should be executed"
+                },
+                "out_vars": {
+                    "description": "List of ENV variables to export and save for later use",
+                    "items": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "name": {
+                                "type": "string"
+                            },
+                            "save_as": {
+                                "type": "string"
+                            }
                         },
-                        "usernames": {
-                            "$ref": "../common/utils.json#/definitions/MergeableSetOfStrings",
-                            "description": "List of User or ServiceAccount names"
-                        }
+                        "required": [
+                            "name"
+                        ],
+                        "type": "object"
                     },
-                    "type": "object"
+                    "type": "array"
                 },
-                "pod-security": {
-                    "default": "enabled",
-                    "description": "Specify if PSS should be enabled/disabled",
-                    "enum": [
-                        "enabled",
-                        "disabled"
-                    ]
+                "sudo": {
+                    "default": false,
+                    "description": "Switch for the command execution from the sudoer",
+                    "type": "boolean"
                 }
-            }
-        },
-        "PropertyNames": {
-            "enum": [
-                "pod-security",
-                "defaults",
-                "exemptions"
-            ]
+            },
+            "required": [
+                "command"
+            ],
+            "type": "object"
         }
-    },
-    "description": "PSS configuration section",
-    "propertyNames": {
-        "$ref": "#/definitions/PropertyNames"
-    },
-    "type": "object"
+    ]
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'properties'": "{'kubernetesVersion': {'default': 'v1.26.3'}}"}*

```diff
@@ -206,15 +206,15 @@
         "kind": {
             "default": "ClusterConfiguration",
             "enum": [
                 "ClusterConfiguration"
             ]
         },
         "kubernetesVersion": {
-            "default": "v1.24.11",
+            "default": "v1.26.3",
             "description": "Specify the version to install and maintain. This version applies into all the dependent parameters - images, binaries, rpms, configurations.",
             "type": "string"
         },
         "networking": {
             "properties": {
                 "podSubnet": {
                     "type": "string"
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.21428571428571427%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('ExtendedVRRP', OrderedDict([('type', 'object'), "*

 * *                  "('properties', OrderedDict([('ip', OrderedDict([('type', 'string'), "*

 * *                  "('description', 'The IP address for virtual IP')])), ('floating_ip', "*

 * *                  "OrderedDict([('type', 'string'), ('description', 'The floating IP address for "*

 * *                  "virtual IP')])), ('hosts', OrderedDict([('type', 'array'), ('description', "*

 * *                  "'List of hosts on which t […]*

```diff
@@ -1,132 +1,103 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": false,
     "definitions": {
-        "control-plane-pod-patch": {
-            "description": "Patches for control-plane pods",
-            "items": {
-                "anyOf": [
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "groups": {
-                                "items": {
-                                    "enum": [
-                                        "control-plane"
-                                    ]
-                                },
-                                "type": "array"
-                            },
-                            "patch": {
-                                "properties": {
-                                    "additionalProperties": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "type": "object"
+        "ExtendedVRRP": {
+            "additionalProperties": false,
+            "properties": {
+                "control_endpoint": {
+                    "default": false,
+                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
+                    "type": "boolean"
+                },
+                "floating_ip": {
+                    "description": "The floating IP address for virtual IP",
+                    "type": "string"
+                },
+                "hosts": {
+                    "description": "List of hosts on which the VRRP IP should be set. Each item can be either a name of the balancer node, or a dictionary with the balancer name and additional parameters.",
+                    "items": {
+                        "$ref": "#/definitions/HostToApplyVRRP"
                     },
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "nodes": {
-                                "items": [
-                                    {
-                                        "type": "string"
-                                    }
-                                ],
-                                "type": "array"
-                            },
-                            "patch": {
-                                "properties": {
-                                    "additionalProperties": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "type": "object"
-                    }
-                ]
+                    "type": "array"
+                },
+                "id": {
+                    "description": "The ID of the VRRP IP. It must be unique for each VRRP IP.",
+                    "type": "string"
+                },
+                "interface": {
+                    "default": "auto",
+                    "description": "The interface on which the address must be listened. The value of this property is propagated to the corresponding hosts[i].interface property, if the latter is not explicitly defined.",
+                    "type": "string"
+                },
+                "ip": {
+                    "description": "The IP address for virtual IP",
+                    "type": "string"
+                },
+                "params": {
+                    "additionalProperties": false,
+                    "description": "Additional params for other non-keepalived services",
+                    "properties": {
+                        "maintenance-type": {
+                            "description": "Label for IPs that describes what type of traffic should be received in maintenance mode",
+                            "enum": [
+                                "not bind"
+                            ]
+                        }
+                    },
+                    "type": "object"
+                },
+                "password": {
+                    "description": "Password for VRRP IP set. It must be unique for every VRRP IP ID.",
+                    "type": "string"
+                },
+                "router_id": {
+                    "description": "The router ID of the VRRP IP. Must be unique for each VRRP IP ID and have maximum 3-character size.",
+                    "type": "string"
+                }
             },
-            "minItems": 0,
-            "type": "array"
+            "required": [
+                "ip"
+            ],
+            "type": "object"
         },
-        "kubelet-patch": {
-            "description": "Patches for kubelet",
-            "items": {
-                "anyOf": [
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "groups": {
-                                "items": {
-                                    "enum": [
-                                        "control-plane",
-                                        "worker"
-                                    ]
-                                },
-                                "type": "array"
-                            },
-                            "patch": {
-                                "properties": {
-                                    "additionalProperties": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
+        "HostToApplyVRRP": {
+            "oneOf": [
+                {
+                    "type": "string"
+                },
+                {
+                    "additionalProperties": false,
+                    "properties": {
+                        "interface": {
+                            "default": "auto",
+                            "description": "The interface on which the address must be listened for the particular host",
+                            "type": "string"
                         },
-                        "type": "object"
-                    },
-                    {
-                        "additionalProperties": false,
-                        "properties": {
-                            "nodes": {
-                                "items": [
-                                    {
-                                        "type": "string"
-                                    }
-                                ],
-                                "type": "array"
-                            },
-                            "patch": {
-                                "properties": {
-                                    "additionalProperties": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
+                        "name": {
+                            "description": "The name of the node. It must match the name in the nodes list.",
+                            "type": "string"
                         },
-                        "type": "object"
-                    }
-                ]
-            },
-            "minItems": 0,
-            "type": "array"
+                        "priority": {
+                            "description": "The priority of the VRRP IP host",
+                            "maximum": 255,
+                            "minimum": 0,
+                            "type": "integer"
+                        }
+                    },
+                    "required": [
+                        "name"
+                    ],
+                    "type": "object"
+                }
+            ]
         }
     },
-    "description": "Override the original settings for patches of control-plane pods and kubelet",
-    "properties": {
-        "apiServer": {
-            "$ref": "#/definitions/control-plane-pod-patch"
-        },
-        "controllerManager": {
-            "$ref": "#/definitions/control-plane-pod-patch"
-        },
-        "etcd": {
-            "$ref": "#/definitions/control-plane-pod-patch"
+    "oneOf": [
+        {
+            "type": "string"
         },
-        "kubelet": {
-            "$ref": "#/definitions/kubelet-patch"
-        },
-        "scheduler": {
-            "$ref": "#/definitions/control-plane-pod-patch"
+        {
+            "$ref": "#/definitions/ExtendedVRRP"
         }
-    },
-    "type": "object"
+    ]
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5416666666666666%*

 * *Differences: {"'definitions'": "{replace: OrderedDict([('Properties', OrderedDict([('properties', "*

 * *                  "OrderedDict([('source', OrderedDict([('type', 'string'), ('description', 'The "*

 * *                  'local path to the source Jinja2 template file. It is compiled before uploading '*

 * *                  "to hosts.')])), ('destination', OrderedDict([('type', 'string'), "*

 * *                  "('description', 'The absolute path on the hosts where the compiled template "*

 * *                  "needs to be uploaded')]) […]*

```diff
@@ -1,103 +1,80 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
-        "ExtendedVRRP": {
-            "additionalProperties": false,
+        "Properties": {
             "properties": {
-                "control_endpoint": {
-                    "default": false,
-                    "description": "Parameter to help the algorithm in choosing which address to take as the control_plain",
-                    "type": "boolean"
-                },
-                "floating_ip": {
-                    "description": "The floating IP address for virtual IP",
+                "apply_command": {
+                    "description": "The command to apply the template on remote hosts after uploading it. It is called only if the switch apply_required is on.",
                     "type": "string"
                 },
-                "hosts": {
-                    "description": "List of hosts on which the VRRP IP should be set. Each item can be either a name of the balancer node, or a dictionary with the balancer name and additional parameters.",
-                    "items": {
-                        "$ref": "#/definitions/HostToApplyVRRP"
-                    },
-                    "type": "array"
+                "apply_groups": {
+                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "description": "List of groups on which the template apply command needs to be executed"
                 },
-                "id": {
-                    "description": "The ID of the VRRP IP. It must be unique for each VRRP IP.",
-                    "type": "string"
+                "apply_nodes": {
+                    "$ref": "../../common/node_ref.json#/definitions/Names",
+                    "description": "List of nodes on which the template apply command needs to be executed"
                 },
-                "interface": {
-                    "default": "auto",
-                    "description": "The interface on which the address must be listened. The value of this property is propagated to the corresponding hosts[i].interface property, if the latter is not explicitly defined.",
-                    "type": "string"
+                "apply_required": {
+                    "default": true,
+                    "description": "A switch to call the command to apply the uploaded template on remote hosts",
+                    "type": "boolean"
                 },
-                "ip": {
-                    "description": "The IP address for virtual IP",
+                "destination": {
+                    "description": "The absolute path on the hosts where the compiled template needs to be uploaded",
                     "type": "string"
                 },
-                "params": {
-                    "additionalProperties": false,
-                    "description": "Additional params for other non-keepalived services",
-                    "properties": {
-                        "maintenance-type": {
-                            "description": "Label for IPs that describes what type of traffic should be received in maintenance mode",
-                            "enum": [
-                                "not bind"
-                            ]
-                        }
-                    },
-                    "type": "object"
+                "destination_groups": {
+                    "$ref": "../../common/node_ref.json#/definitions/Roles",
+                    "description": "List of groups on which the compiled template needs to be uploaded"
                 },
-                "password": {
-                    "description": "Password for VRRP IP set. It must be unique for every VRRP IP ID.",
-                    "type": "string"
+                "destination_nodes": {
+                    "$ref": "../../common/node_ref.json#/definitions/Names",
+                    "description": "List of nodes on which the compiled template needs to be uploaded"
                 },
-                "router_id": {
-                    "description": "The router ID of the VRRP IP. Must be unique for each VRRP IP ID and have maximum 3-character size.",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "ip"
-            ],
-            "type": "object"
-        },
-        "HostToApplyVRRP": {
-            "oneOf": [
-                {
+                "source": {
+                    "description": "The local path to the source Jinja2 template file. It is compiled before uploading to hosts.",
                     "type": "string"
                 },
-                {
-                    "additionalProperties": false,
-                    "properties": {
-                        "interface": {
-                            "default": "auto",
-                            "description": "The interface on which the address must be listened for the particular host",
-                            "type": "string"
-                        },
-                        "name": {
-                            "description": "The name of the node. It must match the name in the nodes list.",
-                            "type": "string"
-                        },
-                        "priority": {
-                            "description": "The priority of the VRRP IP host",
-                            "maximum": 255,
-                            "minimum": 0,
-                            "type": "integer"
-                        }
-                    },
-                    "required": [
-                        "name"
-                    ],
-                    "type": "object"
+                "sudo": {
+                    "default": true,
+                    "description": "A switch for the command execution from the sudoer",
+                    "type": "boolean"
                 }
+            }
+        },
+        "PropertyNames": {
+            "enum": [
+                "source",
+                "destination",
+                "apply_required",
+                "apply_command",
+                "sudo",
+                "destination_groups",
+                "destination_nodes",
+                "apply_groups",
+                "apply_nodes"
             ]
         }
     },
+    "description": "Compile the Jinja2 template file, upload to remote hosts, and apply it. Can be either a local path to file or a dictionary with the extra parameters.",
     "oneOf": [
         {
             "type": "string"
         },
         {
-            "$ref": "#/definitions/ExtendedVRRP"
+            "allOf": [
+                {
+                    "$ref": "#/definitions/Properties"
+                }
+            ],
+            "propertyNames": {
+                "$ref": "#/definitions/PropertyNames"
+            },
+            "required": [
+                "source"
+            ],
+            "type": "object"
         }
     ]
 }
```

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.16.0/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.16.0/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.16.0/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.16.0/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.16.0/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/selinux.py` & `kubemarine-0.16.0/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/sysctl.py` & `kubemarine-0.16.0/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/system.py` & `kubemarine-0.16.0/kubemarine/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.executor import RemoteExecutor
 from kubemarine.core.group import NodeGroupResult, NodeGroup
 from kubemarine.core.yaml_merger import default_merger
 from kubemarine.core.annotations import restrict_empty_group
 
+ERROR_UNSUPPORTED_KERNEL_MODULES_VERSIONS_DETECTED = \
+        "Kernel modules are not available for the current OS family"
 
 def verify_inventory(inventory, cluster):
 
     if cluster.inventory['services']['ntp'].get('chrony', {}).get('servers') \
         and (cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('NTP') or
              cluster.inventory['services']['ntp'].get('timesyncd', {}).get('Time', {}).get('FallbackNTP')):
         raise Exception('chrony and timesyncd configured both at the same time')
@@ -123,14 +125,36 @@
         default_merger.merge(inventory["services"]["packages"].setdefault(_type, {}), packages)
 
     # merge remained packages section
     default_merger.merge(inventory["services"]["packages"], packages_section)
 
     return inventory
 
+def enrich_kernel_modules(inventory: dict, cluster: KubernetesCluster):
+    """
+    The method enrich the list of kernel modules ('services.modprobe') according to OS family
+    """
+    
+    os_family = cluster.get_os_family()
+    if os_family in ["unknown", "unsupported"]:
+        raise Exception(ERROR_UNSUPPORTED_KERNEL_MODULES_VERSIONS_DETECTED)
+    elif os_family in ["debian", "rhel", "rhel8"]:
+        modprobe = {}
+        modprobe[os_family] = inventory["services"]["modprobe"][os_family]
+        inventory["services"]["modprobe"] = modprobe
+    elif os_family == "multiple":
+        modprobe = {}
+        os_families = set()
+        for node in cluster.nodes['all'].get_final_nodes().get_hosts():
+            os_families.add(cluster.get_os_family_for_node(node))
+        for item in os_families:
+            modprobe[item] = inventory["services"]["modprobe"][item]
+        inventory["services"]["modprobe"] = modprobe
+
+    return inventory
 
 def get_system_packages_for_upgrade(cluster):
     upgrade_ver = cluster.context["upgrade_version"]
     previous_ver = cluster.context["initial_kubernetes_version"]
     compatibility = cluster.globals["compatibility_map"]["software"]
 
     # handle special cases in which upgrade is not required for particular package
@@ -551,28 +575,29 @@
 
     raise Exception("Time not synced, but timeout is reached")
 
 
 def setup_modprobe(group):
     log = group.cluster.log
 
+    os_family = group.get_nodes_os()
     if group.cluster.inventory['services'].get('modprobe') is None \
             or not group.cluster.inventory['services']['modprobe']:
         log.debug('Skipped - no modprobe configs in inventory')
         return
 
     is_valid, result = is_modprobe_valid(group)
 
     if is_valid:
         log.debug("Skipped - all necessary kernel modules are presented")
         return result
 
     config = ''
     raw_config = ''
-    for module_name in group.cluster.inventory['services']['modprobe']:
+    for module_name in group.cluster.inventory['services']['modprobe'][os_family]:
         module_name = module_name.strip()
         if module_name is not None and module_name != '':
             config += module_name + "\n"
             raw_config += module_name + " "
 
     log.debug("Uploading config...")
     utils.dump_file(group.cluster, config, 'modprobe_predefined.conf')
@@ -585,15 +610,16 @@
 
 def is_modprobe_valid(group):
     log = group.cluster.log
 
     verify_results = group.sudo("lsmod", warn=True)
     is_valid = True
 
-    for module_name in group.cluster.inventory['services']['modprobe']:
+    os_family = group.get_nodes_os()
+    for module_name in group.cluster.inventory['services']['modprobe'][os_family]:
         for conn, result in verify_results.items():
             if module_name not in result.stdout:
                 log.debug('Kernel module %s not found at %s' % (module_name, conn.host))
                 is_valid = False
 
     return is_valid, verify_results
```

### Comparing `kubemarine-0.15.1/kubemarine/templates/__init__.py` & `kubemarine-0.16.0/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.16.0/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.16.0/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.16.0/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.16.0/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.16.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/testsuite.py` & `kubemarine-0.16.0/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine/thirdparties.py` & `kubemarine-0.16.0/kubemarine/thirdparties.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,105 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 from copy import deepcopy
+from typing import Tuple, Optional, Dict, List
 
 from kubemarine.core import utils, static
 from kubemarine.core.cluster import KubernetesCluster
 from kubemarine.core.group import NodeGroupResult, NodeGroup
 
 
+def is_default_thirdparty(destination: str):
+    return destination in static.GLOBALS['thirdparties']
+
+
+def get_default_thirdparties() -> List[str]:
+    return list(static.GLOBALS['thirdparties'])
+
+
+def get_default_thirdparty_version(kubernetes_version: str, destination: str) -> str:
+    """
+    :param kubernetes_version: Kubernetes version
+    :param destination: absolute path of default third-party
+    :return: version of third-party from compatibility map
+    """
+    software_settings = _get_software_settings_for_thirdparty(kubernetes_version, destination)
+
+    if 'version' in software_settings:
+        return software_settings['version']
+    else:
+        # kubeadm, kubelet, kubectl
+        return kubernetes_version
+
+
+def get_default_thirdparty_source(destination: str, version: str, in_public: bool):
+    """
+    :param destination: absolute path of default third-party
+    :param version: version of third-party
+    :param in_public: flag whether to return third-party URL in public resources.
+    :return: URL of the third-party source.
+    """
+    if not is_default_thirdparty(destination):
+        raise Exception(f"{destination} is not a default 3rd-party")
+
+    thirdparty_settings = static.GLOBALS['thirdparties'][destination]
+    if in_public:
+        source_prefix = thirdparty_settings['source_prefix']['public']
+    else:
+        source_prefix = thirdparty_settings['source_prefix']['private']
+
+    relative_path = thirdparty_settings['relative_path'].format(version=version)
+    return f"{source_prefix}/{relative_path}"
+
+
+def get_default_thirdparty_identity(inventory: dict,
+                                    destination: str, in_public: bool) -> Tuple[str, str]:
+    """
+    :param inventory: inventory of the cluster
+    :param destination: absolute path of default third-party
+    :param in_public: flag whether to return third-party URL in public resources.
+    :return: a pair of the third-party URL and sha1
+    """
+    kubernetes_version = inventory['services']['kubeadm']['kubernetesVersion']
+
+    software_settings = _get_software_settings_for_thirdparty(kubernetes_version, destination)
+    sha1 = software_settings['sha1']
+
+    version = get_default_thirdparty_version(kubernetes_version, destination)
+    source = get_default_thirdparty_source(destination, version, in_public)
+
+    return source, sha1
+
+
+def _get_software_settings_for_thirdparty(kubernetes_version: str, destination: str) -> dict:
+    if not is_default_thirdparty(destination):
+        raise Exception(f"{destination} is not a default 3rd-party")
+
+    thirdparty_settings = static.GLOBALS['thirdparties'][destination]
+    software_name = thirdparty_settings['software_name']
+    return static.GLOBALS['compatibility_map']['software'][software_name][kubernetes_version]
+
+
+def get_thirdparty_recommended_sha(destination: str, cluster: KubernetesCluster) -> Optional[str]:
+    if not is_default_thirdparty(destination):
+        # 3rd-party is not managed by Kubemarine
+        return None
+
+    cluster.log.verbose("Calculate recommended sha for thirdparty %s..." % destination)
+    _, recommended_sha = get_default_thirdparty_identity(cluster.inventory,
+                                                         destination, in_public=True)
+    cluster.log.verbose(f"Recommended sha for thirdparty {destination} was calculated: {recommended_sha}")
+
+    return recommended_sha
+
+
 def enrich_inventory_apply_upgrade_defaults(inventory, cluster):
     if cluster.context.get('initial_procedure') == 'upgrade':
         upgrade_version = cluster.context["upgrade_version"]
         upgrade_thirdparties = cluster.procedure_inventory.get(upgrade_version, {}).get('thirdparties')
         if upgrade_thirdparties:
             upgrade_thirdparties = deepcopy(upgrade_thirdparties)
             default_thirdparties = static.DEFAULTS['services']['thirdparties']
@@ -35,44 +120,21 @@
 
             inventory['services']['thirdparties'] = upgrade_thirdparties
         else:
             cluster.log.warning('New thirdparties for upgrade procedure is not set in procedure config - default will be used')
     return inventory
 
 
-def get_thirdparty_recommended_sha(destination, cluster):
-    cluster.log.verbose("Calculate recommended sha for thirdparty %s..." % destination)
-    # Get kubeadm version
-    kubernetes_version = cluster.inventory['services']['kubeadm']['kubernetesVersion']
-    effective_kubernetes_version = ".".join(kubernetes_version.split('.')[0:2])
-
-    # Get software versions map
-    software_name = cluster.globals['thirdparties'].get(destination, {}).get('software_name', None)
-    software_versions = cluster.globals['compatibility_map']['software'].get(software_name, {})
-
-    # Return sha1 related to used kubernetes version
-    recommended_sha = software_versions[kubernetes_version].get('sha1', None) \
-        if kubernetes_version in software_versions else \
-        software_versions.get(effective_kubernetes_version, {}).get('sha1', None)
-
-    if recommended_sha is not None:
-        cluster.log.verbose(f"Recommended sha for thirdparty {destination} was calculated: {recommended_sha}")
-    else:
-        cluster.log.verbose(f"Recommended sha for thirdparty {destination} doesn't exist")
-
-    return recommended_sha
-
-
-def enrich_inventory_apply_defaults(inventory, cluster):
+def enrich_inventory_apply_defaults(inventory: dict, cluster: KubernetesCluster) -> dict:
+    thirdparties: Dict[str, dict] = inventory['services'].get('thirdparties', {})
     # if thirdparties is empty, then nothing to do
-    if not inventory['services'].get('thirdparties', {}):
+    if not thirdparties:
         return inventory
-    raw_inventory = cluster.raw_inventory
 
-    for destination, config in inventory['services']['thirdparties'].items():
+    for destination, config in thirdparties.items():
 
         if isinstance(config, str):
             config = {
                 'source': config
             }
 
         if config.get('mode') is None:
@@ -96,28 +158,28 @@
             all_nodes_names = cluster.nodes['all'].get_nodes_names()
             for node_name in config['nodes']:
                 if node_name not in all_nodes_names:
                     raise Exception('Unknown node name provided for thirdparty %s. '
                                     'Expected any of %s, but \'%s\' found.'
                                     % (destination, all_nodes_names, node_name))
 
-        raw_config = raw_inventory.get('services', {}).get('thirdparties', {}).get(destination, {})
-        recommended_sha = get_thirdparty_recommended_sha(destination, cluster)
-        if 'source' not in raw_config and 'sha1' not in raw_config and recommended_sha is not None:
-            config['sha1'] = get_thirdparty_recommended_sha(destination, cluster)
+        if is_default_thirdparty(destination) and 'source' not in config:
+            source, sha1 = get_default_thirdparty_identity(cluster.inventory, destination, in_public=True)
+            config['source'] = source
+            if 'sha1' not in config:
+                config['sha1'] = sha1
 
-        inventory['services']['thirdparties'][destination] = config
+        thirdparties[destination] = config
 
     # remove "crictl" from thirdparties when docker is used, but ONLY IF it is NOT explicitly specified in cluster.yaml
     cri_name = inventory['services']['cri']['containerRuntime']
     crictl_key = '/usr/bin/crictl.tar.gz'
     if cri_name == "docker" and \
-            crictl_key not in cluster.raw_inventory.get('services', {}).get('thirdparties', {}) and \
-            crictl_key in inventory['services']['thirdparties']:
-        del(inventory['services']['thirdparties'][crictl_key])
+            crictl_key not in cluster.raw_inventory.get('services', {}).get('thirdparties', {}):
+        del(thirdparties[crictl_key])
 
     return inventory
 
 
 def get_install_group(cluster: KubernetesCluster, config: dict):
     return cluster.create_group_from_groups_nodes_names(
         config.get('groups', []), config.get('nodes', []))
@@ -196,26 +258,32 @@
         cluster.log.verbose('Unpack request detected')
 
         remote_commands += ' && sudo mkdir -p %s' % config['unpack']
 
         extension = destination.split('.')[-1]
         if extension == 'zip':
             cluster.log.verbose('Unzip will be used for unpacking')
-            # TODO re-installation waits forever
-            remote_commands += ' && sudo unzip %s -d %s' % (destination, config['unpack'])
+            remote_commands += ' && sudo unzip -o %s -d %s' % (destination, config['unpack'])
+            
+            remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo chmod %s %s/FILE' \
+                   % (destination, config['mode'], config['unpack'])
+            remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo chown -R %s %s/FILE' \
+                   % (destination, config['owner'], config['unpack'])
+            remote_commands += ' && sudo unzip -qq -l %s | awk \'NF > 3 { print $4 }\'| xargs -I FILE sudo ls -la %s/FILE' % (destination, config['unpack'])
+            
         else:
             cluster.log.verbose('Tar will be used for unpacking')
             remote_commands += ' && sudo tar -zxf %s -C %s' % (destination, config['unpack'])
-
-        # TODO access rights do not work for zip
-        remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo chmod %s %s/FILE' \
+            
+            remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo chmod %s %s/FILE' \
                            % (destination, config['mode'], config['unpack'])
-        remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo chown %s %s/FILE' \
+            remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo chown %s %s/FILE' \
                            % (destination, config['owner'], config['unpack'])
-        remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo ls -la %s/FILE' % (destination, config['unpack'])
+            remote_commands += ' && sudo tar -tf %s | xargs -I FILE sudo ls -la %s/FILE' % (destination, config['unpack'])
+
 
     return common_group.sudo(remote_commands)
 
 
 def install_all_thirparties(group):
     cluster = group.cluster
     log = cluster.log
```

### Comparing `kubemarine-0.15.1/kubemarine/yum.py` & `kubemarine-0.16.0/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.15.1/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.16.0/kubemarine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.15.1
+Version: 0.16.0
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
 Keywords: kubernetes,devops,administration,helm
@@ -32,36 +32,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -79,15 +79,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -98,15 +98,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.15.1/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -127,24 +127,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.15.1/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.16.0/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -172,42 +172,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.15.1/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.16.0/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.15.1/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.16.0/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.15.1/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.16.0/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.15.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.16.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.15.1/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.16.0/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.15.1/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.16.0/LICENSE)
```

### Comparing `kubemarine-0.15.1/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.16.0/kubemarine.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,26 @@
 kubemarine/kubernetes/__init__.py
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
-kubemarine/patches/p1_reinstall_calico.py
+kubemarine/patches/p1_helm_values.py
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
-kubemarine/plugins/yaml/calico-v3.22.2.yaml.original
-kubemarine/plugins/yaml/calico-v3.24.2.yaml.original
-kubemarine/plugins/yaml/dashboard-v2.5.1-original.yaml
-kubemarine/plugins/yaml/dashboard-v2.7.0-original.yaml
+kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
 kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
 kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
 kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
 kubemarine/procedures/__init__.py
 kubemarine/procedures/add_node.py
 kubemarine/procedures/backup.py
@@ -95,14 +95,19 @@
 kubemarine/procedures/remove_node.py
 kubemarine/procedures/restore.py
 kubemarine/procedures/upgrade.py
 kubemarine/resources/__init__.py
 kubemarine/resources/configurations/__init__.py
 kubemarine/resources/configurations/defaults.yaml
 kubemarine/resources/configurations/globals.yaml
+kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+kubemarine/resources/configurations/compatibility/internal/packages.yaml
+kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
 kubemarine/resources/drop_ins/__init__.py
 kubemarine/resources/drop_ins/haproxy.conf
 kubemarine/resources/drop_ins/keepalived.conf
 kubemarine/resources/etalons/patches/__init__.py
 kubemarine/resources/psp/__init__.py
 kubemarine/resources/psp/anyuid.yaml
 kubemarine/resources/psp/default.yaml
```

### Comparing `kubemarine-0.15.1/pyproject.toml` & `kubemarine-0.16.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "cryptography==39.0.*",
     "paramiko==2.11.*",
     "jsonschema==4.17.*",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-ansible = ["ansible==6.7.*"]
+ansible = ["ansible==7.0.*"]
 
 # Auxiliary executable roughly equivalent to python -m kubemarine
 # Allows to not worry about exact path to python executable on the client machine
 # Should still no be called directly as it does not ensure necessary environment variables.
 # Real executables are installed by setup.py
 [project.scripts]
 _kubemarine = "kubemarine.__main__:main"
@@ -60,15 +60,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "0.15.1"
+current_version = "0.16.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.15.1/setup.py` & `kubemarine-0.16.0/setup.py`

 * *Files identical despite different names*

