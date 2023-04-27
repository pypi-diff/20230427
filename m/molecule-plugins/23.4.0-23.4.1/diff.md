# Comparing `tmp/molecule-plugins-23.4.0.tar.gz` & `tmp/molecule-plugins-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-plugins-23.4.0.tar", last modified: Thu Apr 20 13:37:02 2023, max compression
+gzip compressed data, was "molecule-plugins-23.4.1.tar", last modified: Thu Apr 27 17:49:56 2023, max compression
```

## Comparing `molecule-plugins-23.4.0.tar` & `molecule-plugins-23.4.1.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/doc/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/ec2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/ec2/platforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.124648 molecule-plugins-23.4.0/doc/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/doc/vagrant/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.128649 molecule-plugins-23.4.0/molecule/test-podman/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/molecule/test-podman/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:37:02.204650 molecule-plugins-23.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.080648 molecule-plugins-23.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.128649 molecule-plugins-23.4.0/src/molecule_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 13:37:01.000000 molecule-plugins-23.4.0/src/molecule_plugins/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/azure/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/containers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.084648 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.136649 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.140649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.088648 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/ec2/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.088648 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.144649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.092648 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.148649 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.096648 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.152649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24577 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/vagrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.132649 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 13:37:02.000000 molecule-plugins-23.4.0/src/molecule_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/functional/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.096648 molecule-plugins-23.4.0/test/azure/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.156649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/azure/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.160649 molecule-plugins-23.4.0/test/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/containers/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/functional/test_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.100648 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/containers/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.164649 molecule-plugins-23.4.0/test/docker/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/with-context/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.104648 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/FOO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/scenarios/with-context/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/docker/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.168649 molecule-plugins-23.4.0/test/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/functional/test_ec2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.108648 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.172649 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/ec2/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.176649 molecule-plugins-23.4.0/test/gce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.176649 molecule-plugins-23.4.0/test/gce/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/gce/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.180649 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/linux/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/files/windows_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.184649 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/scenarios/windows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/gce/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/podman/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/podman/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/vagrant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.188649 molecule-plugins-23.4.0/test/vagrant/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/functional/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.112648 molecule-plugins-23.4.0/test/vagrant/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.116648 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.192649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/invalid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.196649 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/network/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/test/vagrant/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:37:02.200650 molecule-plugins-23.4.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/Vagrantfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/create_testbox.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tools/test-setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-20 13:36:43.000000 molecule-plugins-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.798894 molecule-plugins-23.4.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/doc/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/ec2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/ec2/platforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/doc/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/doc/vagrant/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.798894 molecule-plugins-23.4.1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.850895 molecule-plugins-23.4.1/molecule/test-podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/molecule/test-podman/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:49:56.922895 molecule-plugins-23.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.802894 molecule-plugins-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.802894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/azure/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.806894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/containers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.806894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.858894 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/create_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/delete_network.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.862894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.810894 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/ec2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.814894 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.866895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.818894 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.870895 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.818894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/vagrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.854894 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 17:49:56.000000 molecule-plugins-23.4.1/src/molecule_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.838894 molecule-plugins-23.4.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.874894 molecule-plugins-23.4.1/test/azure/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/functional/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.822894 molecule-plugins-23.4.1/test/azure/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.822894 molecule-plugins-23.4.1/test/azure/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.826894 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.826894 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/azure/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.878895 molecule-plugins-23.4.1/test/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/containers/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/functional/test_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.830894 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/scenarios/driver/containers/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/containers/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.882895 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/env-substitution/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/with-context/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/FOO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/scenarios/with-context/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/docker/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/functional/test_ec2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.834894 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.886895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/prepare.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/ec2/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/gce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.890895 molecule-plugins-23.4.1/test/gce/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.838894 molecule-plugins-23.4.1/test/gce/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.894895 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/linux/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/files/windows_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_linux_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_windows_instance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/scenarios/windows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/gce/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/podman/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.898895 molecule-plugins-23.4.1/test/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/functional/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.842894 molecule-plugins-23.4.1/test/vagrant/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.842894 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.902895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.906895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/invalid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.910895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.914895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/network/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.914895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/provider_config_options/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.918895 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/test/vagrant/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:49:56.918895 molecule-plugins-23.4.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/Vagrantfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/create_testbox.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6414 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tools/test-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-27 17:49:31.000000 molecule-plugins-23.4.1/tox.ini
```

### Comparing `molecule-plugins-23.4.0/.github/workflows/release.yml` & `molecule-plugins-23.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/.github/workflows/tox.yml` & `molecule-plugins-23.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/.gitignore` & `molecule-plugins-23.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/.pre-commit-config.yaml` & `molecule-plugins-23.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/LICENSE` & `molecule-plugins-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/PKG-INFO` & `molecule-plugins-23.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.4.0
+Version: 23.4.1
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
@@ -33,14 +33,15 @@
 Provides-Extra: test
 Provides-Extra: azure
 Provides-Extra: docker
 Provides-Extra: ec2
 Provides-Extra: gce
 Provides-Extra: podman
 Provides-Extra: selinux
+Provides-Extra: vagrant
 License-File: LICENSE
 
 # molecule-plugins
 
 This repository contains the following molecule plugins:
 
 - azure
```

### Comparing `molecule-plugins-23.4.0/README.md` & `molecule-plugins-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/bindep.txt` & `molecule-plugins-23.4.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/conftest.py` & `molecule-plugins-23.4.1/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/doc/ec2/README.rst` & `molecule-plugins-23.4.1/doc/ec2/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/doc/ec2/platforms.rst` & `molecule-plugins-23.4.1/doc/ec2/platforms.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/doc/vagrant/README.rst` & `molecule-plugins-23.4.1/doc/vagrant/README.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/pyproject.toml` & `molecule-plugins-23.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     # that do have selinux enabled and where code is running inside of an
     # isolated (default) virtualenv. It does not avoid need to install the
     # system selinux libraries but it will provide a clear message when user
     # has to do that.
     'selinux; sys_platform=="linux2"',
     'selinux; sys_platform=="linux"',
 ]
+vagrant = [
+    "python-vagrant",
+]
 
 [tool.ruff]
 ignore = [
   "E501", # we use black
   # we deliberately ignore these:
   "EM102",
   # temporary disabled until we either fix them or decide to ignore them:
```

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/azure/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/azure/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/azure/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/containers/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/containers/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/Dockerfile.j2` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/filter_plugins/get_docker_networks.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/tasks/create_network.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/tasks/create_network.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/docker/playbooks/validate-dockerfile.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/ec2/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/ec2/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/ec2/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/files/windows_auth.py` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/handlers/main.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_linux_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/gce/playbooks/tasks/create_windows_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/podman/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/podman/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/Dockerfile.j2` & `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/podman/playbooks/validate-dockerfile.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/driver.py` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/modules/vagrant.py` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/modules/vagrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     c.vm.network "{{ n.name }}", {{ dict2args(n.options) }}
     {% endfor %}
 
     ##
     # instance_raw_config_args
     ##
     {% if instance.instance_raw_config_args is not none %}{% for arg in instance.instance_raw_config_args -%}
-    c.{{ arg }}
+    c.{{ arg | safe }}
     {% endfor %}{% endif %}
 
     ##
     # Provider
     ##
     c.vm.provider "{{ instance.provider }}" do |{{ instance.provider | lower }}, override|
       {% if instance.provider == "vsphere" %}
@@ -269,21 +269,21 @@
 
       {% for option, value in instance.provider_options.items() %}
       {{ instance.provider | lower }}.{{ option }} = {{ ruby_format(value) }}
       {% endfor %}
 
       {% if instance.provider_raw_config_args is not none %}
         {% for arg in instance.provider_raw_config_args %}
-      {{ instance.provider | lower }}.{{ arg }}
+      {{ instance.provider | lower }}.{{ arg | safe }}
         {% endfor %}
       {% endif %}
 
       {% if instance.provider_override_args is not none %}
         {% for arg in instance.provider_override_args -%}
-      override.{{ arg }}
+      override.{{ arg | safe }}
         {% endfor %}
       {% endif %}
 
       {% if instance.provider == 'virtualbox' %}
       {% if 'linked_clone' not in instance.provider_options %}
       virtualbox.linked_clone = true
       {% endif %}
```

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/create.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/destroy.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins/vagrant/playbooks/prepare.yml` & `molecule-plugins-23.4.1/src/molecule_plugins/vagrant/playbooks/prepare.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins.egg-info/PKG-INFO` & `molecule-plugins-23.4.1/src/molecule_plugins.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-plugins
-Version: 23.4.0
+Version: 23.4.1
 Summary: Molecule Plugins
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 Maintainer-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule-plugins
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule-plugins
@@ -33,14 +33,15 @@
 Provides-Extra: test
 Provides-Extra: azure
 Provides-Extra: docker
 Provides-Extra: ec2
 Provides-Extra: gce
 Provides-Extra: podman
 Provides-Extra: selinux
+Provides-Extra: vagrant
 License-File: LICENSE
 
 # molecule-plugins
 
 This repository contains the following molecule plugins:
 
 - azure
```

### Comparing `molecule-plugins-23.4.0/src/molecule_plugins.egg-info/SOURCES.txt` & `molecule-plugins-23.4.1/src/molecule_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/azure/functional/conftest.py` & `molecule-plugins-23.4.1/test/azure/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/azure/functional/test_azure.py` & `molecule-plugins-23.4.1/test/azure/functional/test_azure.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py` & `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.4.1/test/azure/scenarios/driver/azure/molecule/multi-node/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/containers/functional/conftest.py` & `molecule-plugins-23.4.1/test/containers/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/containers/functional/test_containers.py` & `molecule-plugins-23.4.1/test/containers/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/docker/test_func.py` & `molecule-plugins-23.4.1/test/docker/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/ec2/functional/conftest.py` & `molecule-plugins-23.4.1/test/ec2/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/ec2/functional/test_ec2.py` & `molecule-plugins-23.4.1/test/ec2/functional/test_ec2.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py` & `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py` & `molecule-plugins-23.4.1/test/ec2/scenarios/driver/ec2/molecule/multi-node/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/functional/conftest.py` & `molecule-plugins-23.4.1/test/gce/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/functional/test_func.py` & `molecule-plugins-23.4.1/test/gce/functional/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/INSTALL.md` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/create.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/destroy.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/files/windows_auth.py` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/handlers/main.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/molecule.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_linux_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/linux/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/linux/tasks/create_windows_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/INSTALL.md` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/INSTALL.md`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/create.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/destroy.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/files/windows_auth.py` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/files/windows_auth.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/handlers/main.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/molecule.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_linux_instance.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_linux_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/gce/scenarios/windows/tasks/create_windows_instance.yml` & `molecule-plugins-23.4.1/test/gce/scenarios/windows/tasks/create_windows_instance.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/podman/test_func.py` & `molecule-plugins-23.4.1/test/podman/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/functional/conftest.py` & `molecule-plugins-23.4.1/test/vagrant/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/functional/test_func.py` & `molecule-plugins-23.4.1/test/vagrant/functional/test_func.py`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/create.yml` & `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/default-compat/destroy.yml` & `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/default-compat/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/hostname/verify.yml` & `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/hostname/verify.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/multi-node/molecule.yml` & `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/multi-node/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/test/vagrant/scenarios/molecule/vagrant_root/verify.yml` & `molecule-plugins-23.4.1/test/vagrant/scenarios/molecule/vagrant_root/verify.yml`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/tools/create_testbox.sh` & `molecule-plugins-23.4.1/tools/create_testbox.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/tools/test-setup.sh` & `molecule-plugins-23.4.1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-plugins-23.4.0/tox.ini` & `molecule-plugins-23.4.1/tox.ini`

 * *Files identical despite different names*

