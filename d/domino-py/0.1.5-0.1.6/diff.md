# Comparing `tmp/domino-py-0.1.5.tar.gz` & `tmp/domino-py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.5.tar", last modified: Mon Apr 24 17:48:19 2023, max compression
+gzip compressed data, was "domino-py-0.1.6.tar", last modified: Thu Apr 27 21:17:47 2023, max compression
```

## Comparing `domino-py-0.1.5.tar` & `domino-py-0.1.6.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.850681 domino-py-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:48:08.000000 domino-py-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-24 17:48:08.000000 domino-py-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:48:19.850681 domino-py-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 17:48:08.000000 domino-py-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/create_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.850681 domino-py-0.1.5/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 17:48:08.000000 domino-py-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:48:19.850681 domino-py-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 17:48:08.000000 domino-py-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 21:17:28.000000 domino-py-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 21:17:28.000000 domino-py-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-27 21:17:47.716592 domino-py-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-27 21:17:28.000000 domino-py-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.700592 domino-py-0.1.6/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/create_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.704592 domino-py-0.1.6/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-airflow/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-airflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/Chart.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-backend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-frontend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/domino-postgres-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/ingress-api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/ingress-frontend.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.708592 domino-py-0.1.6/domino/helm/domino-base/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/jobs/domino-migrations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/helm/domino-base/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/piece_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.712592 domino-py-0.1.6/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/generate_infrasctructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/enum_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/types_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 21:17:28.000000 domino-py-0.1.6/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:17:47.716592 domino-py-0.1.6/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-27 21:17:47.000000 domino-py-0.1.6/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 21:17:46.000000 domino-py-0.1.6/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-27 21:17:28.000000 domino-py-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:17:47.716592 domino-py-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-27 21:17:28.000000 domino-py-0.1.6/setup.py
```

### Comparing `domino-py-0.1.5/LICENSE.md` & `domino-py-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/MANIFEST.in` & `domino-py-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/README.md` & `domino-py-0.1.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-[<img src="https://img.shields.io/pypi/v/flowui-project?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">](https://pypi.org/project/flowui-project/)
-[<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=Backend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-backend)
-[<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-frontend?label=Frontend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-frontend)
-[<img src="https://img.shields.io/readthedocs/flowui?color=%23799194&label=Docs&logo=Read%20the%20Docs&logoColor=white">](link)
 
 
+<p align="center">
+  <img src="./media/logo.png" width="450" title="Domino">
+</p>
+<p align="center">
+  <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
+  <img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=REST&logo=docker&style=flat">
+  <img src="https://img.shields.io/docker/v/taufferconsulting/flowui-frontend?label=Frontend&logo=docker&style=flat">
+  <img src="https://img.shields.io/readthedocs/flowui?color=%23799194&label=Docs&logo=Read%20the%20Docs&logoColor=white" >
+</p>
 
 
-# Domino Project
-Domino is an open source workflow management platform, containing:
+# Domino
+Domino is an open source workflow management platform, with:
 
-- an intuitive Graphical User Interface that facilitates creating, editing and supervising any type of Workflows (e.g. data processing, machine learning, etc...)
+- an intuitive Graphical User Interface that facilitates authoring, editing and monitoring any type of Workflows, from data processing to machine learning
 - a REST API that controls a running Apache Airflow instance
-- a standard way of writing Operators which follows good practices for data typing, documentation and distribution
+- a standard way of writing and publishing functional Pieces, which follows good practices for data modeling, documentation and distribution
 
 <br>
 
-# Domino Infrastructure
+# Domino structure
 
-Per Platform:
+A Domino platform contains the following components:
 - Frontend service
-- Backend service
+- REST api service
 - Database
 - Airflow services
 - Github repository for GitSync of Workflows
 
 <br>
 
 
@@ -44,29 +49,28 @@
 ..................../xcom_out.json
 
 
 ```
 
 <br>
 
-## Operators
-Each Operator will have:
-- A `operator.py` file with the source code to be executed, as the `piece_function()`
-- A `models.py` file containing the Pydantic models that define the input, output and secrets for the Operator
-- A `metadata.json` file containing the Operators metadata, including frontend node style
+# Pieces
+Each Domino Piece will have:
+- A `piece.py` file with the source code to be executed, as the `piece_function()`
+- A `models.py` file containing the Pydantic models that define the input, output and secrets for the Piece
+- A `metadata.json` file containing the Piece's metadata, including frontend node style
 
-Each dependency group from an Operators repository will build an independent Docker image. This dependency group image has the following basic file struture within `/home`:
+Each dependency group from a Pieces repository will build an independent Docker image. This dependency group image has the following basic file struture within `/home/domino`:
 ```
-# This path holds the source code from the Operators repository, it comes built in the Image
-/operators_repository
+/pieces_repository
 ..../config.toml
-..../operators
-......../{OPERATOR-NAME}
-............/metadata.json    # OPTIONAL
-............/model.py         # REQUIRED
-............/operator.py      # REQUIRED
-..../.flowui
+..../pieces
+......../{PIECE-NAME}
+............/metadata.json    
+............/model.py         
+............/piece.py         
+..../.domino
 ......../dependencies_map.json
 ......../compiled_metadata.json
 ..../dependencies
 ......../requirements.txt     # If dependency group was defined with a requirements.txt file
 ```
```

### Comparing `domino-py-0.1.5/domino/base_piece.py` & `domino-py-0.1.6/domino/base_piece.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,40 +19,40 @@
     def set_metadata(cls, metadata):
         """
         _summary_
 
         Args:
             metadata (_type_): _description_
         """
-        # Operator name as used by Airflow
+        # Piece name as used by Airflow
         cls.__name__ = metadata.get("name", "BasePiece")
 
         # Full metadata
         cls._metadata_ = metadata
 
 
     def __init__(
         self,
         deploy_mode: DeployModeType,
         task_id: str,
         dag_id: str,
     ) -> None:
         """
-        The base class from which every Domino custom Operator should inherit from.
-        BasePiece methods and variables that can be used by inheriting Operators classes:
+        The base class from which every Domino custom Piece should inherit from.
+        BasePiece methods and variables that can be used by inheriting Pieces classes:
         self.results_path - Path to store results data
         self.logger - Logger functionality
 
         Args:
             deploy_mode (DeployModeType): _description_
             task_id (str): _description_
             dag_id (str): _description_
         """
 
-        # Operator task attributes
+        # Piece task attributes
         self.task_id = task_id
         self.dag_id = dag_id
         self.deploy_mode = deploy_mode
 
         # Logger
         self.logger = get_configured_logger(f"{self.__class__.__name__ }-{self.task_id}")
 
@@ -115,16 +115,16 @@
                     self.upstream_tasks_data[tid]["xcom"] = json.load(f)
         else:
             raise NotImplementedError(f"Get upstream XCOM not implemented for deploy_mode=={self.deploy_mode}")
 
     
     def validate_and_get_env_secrets(self, piece_secrets_model: pydantic.BaseModel = None):
         """
-        Get secret variables for this Operator from ENV. The necessary secret variables to run the Operator should be defined in the Operator's SecretsModel.
-        The secrets can then be retrieved and used in the Operator's `piece_function` method as such:
+        Get secret variables for this Piece from ENV. The necessary secret variables to run the Piece should be defined in the Piece's SecretsModel.
+        The secrets can then be retrieved and used in the Piece's `piece_function` method as such:
         ```
         my_secret = self.secrets.my_secret
         ```
 
         Args:
             piece_secrets_model (pydantic.BaseModel): _description_
         """
@@ -149,16 +149,16 @@
 
         Returns:
             dict: XCOM dictionary
         """
         # xcom_obj = output_obj.dict()
         xcom_obj = json.loads(output_obj.json())
         if not isinstance(xcom_obj, dict):
-            print(f"Operator {self.__class__.__name__} is not returning a valid XCOM object. Auto-generating a base XCOM for it...")
-            self.logger.info(f"Operator {self.__class__.__name__} is not returning a valid XCOM object. Auto-generating a base XCOM for it...")
+            print(f"Piece {self.__class__.__name__} is not returning a valid XCOM object. Auto-generating a base XCOM for it...")
+            self.logger.info(f"Piece {self.__class__.__name__} is not returning a valid XCOM object. Auto-generating a base XCOM for it...")
             xcom_obj = dict()
 
         # Add arguments types to XCOM 
         # TODO - this is a temporary solution. We should find a better way to do this
         output_schema = output_obj.schema()
         for k, v in output_schema["properties"].items():
             if "type" in v:
@@ -224,18 +224,18 @@
         piece_secrets_model: pydantic.BaseModel = None
     ):
         """
         _summary_
 
         Args:
             airflow_context (dict): Dictionary containing Airflow context information
-            op_kwargs (dict): Dictionary containing Operator's kwargs
-            piece_input_model (pydantic.BaseModel): Operator's InputModel
-            piece_output_model (pydantic.BaseModel): Operator's OutputModel
-            piece_secrets_model (pydantic.BaseModel, optional): Operator's SecretsModel. Defaults to None.
+            op_kwargs (dict): Dictionary containing Piece's kwargs
+            piece_input_model (pydantic.BaseModel): Piece's InputModel
+            piece_output_model (pydantic.BaseModel): Piece's OutputModel
+            piece_secrets_model (pydantic.BaseModel, optional): Piece's SecretsModel. Defaults to None.
 
         Raises:
             InvalidPieceOutputError: _description_
         """
         # Start logger
         self.start_logger()
 
@@ -244,15 +244,15 @@
         self.piece_secrets_model = piece_secrets_model
 
         # Airflow context dictionary: https://composed.blog/airflow/execute-context
         # For local-bash and kubernetes deploy modes, we assemble this ourselves and the context data is more limited
         self.airflow_context = airflow_context
         self.dag_run_id = airflow_context.get("dag_run_id")
 
-        # Check if Operator's necessary secrets are present in ENV
+        # Check if Piece's necessary secrets are present in ENV
         self.validate_and_get_env_secrets(piece_secrets_model=piece_secrets_model)
 
         # Generate paths
         self.workflow_shared_storage = "/home/shared_storage"
         self.results_path = f"{self.workflow_shared_storage}/{self.task_id}/results"
         self.xcom_path = f"{self.workflow_shared_storage}/{self.task_id}/xcom"
         self.report_path = f"{self.workflow_shared_storage}/{self.task_id}/report"
@@ -348,17 +348,17 @@
             container_memory_usage = int(fp.read())
         return container_memory_usage
 
 
     @abc.abstractmethod
     def piece_function(self):
         """
-        This function carries the relevant code for the Operator run.
+        This function carries the relevant code for the Piece run.
         It should have all the necessary content for auto-generating json schemas.
         All arguments should be type annotated and docstring should carry description for each argument.
         """
         raise NotImplementedError("This method must be implemented in the child class!")        
 
     
     def generate_report(self):
-        """This function carries the relevant code for the Operator report."""
+        """This function carries the relevant code for the Piece report."""
         raise NotImplementedError("This method must be implemented in the child class!")
```

### Comparing `domino-py-0.1.5/domino/cli/cli.py` & `domino-py-0.1.6/domino/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  | |_| | (_) | | | | | | | | | | (_) |
  |____/ \___/|_| |_| |_|_|_| |_|\___/       
   
 =============================================="""
 
 
 ###############################################################################
-# FLOWUI PLATFORM
+# DOMINO PLATFORM
 ###############################################################################
 
 def validate_github_token_workflows(value):
     if value and value.startswith("ghp_"):
         return value
     return None
 
@@ -138,33 +138,33 @@
 @click.command()
 @click.option(
     "--domino-frontend-image", 
     default=None,
     help="Load a local Domino frontend image to cluster."
 )
 @click.option(
-    "--domino-backend-image", 
+    "--domino-rest-image", 
     default=None,
-    help="Load a local Domino backend image to cluster."
+    help="Load a local Domino REST image to cluster."
 )
 @click.option(
     "--run-airflow", 
     default=True,
     help="Run Domino Airflow services."
 )
 @click.option(
     "--use-gpu",
     is_flag=True,
     # Nvidia operator plugin reference: https://catalog.ngc.nvidia.com/orgs/nvidia/containers/gpu-operator
     help="Allow the platform to use GPUs. It will install NVIDIA plugins.",
     default=False
 )
-def cli_create_platform(domino_frontend_image, domino_backend_image, run_airflow, use_gpu):
+def cli_create_platform(domino_frontend_image, domino_rest_image, run_airflow, use_gpu):
     """Create cluster, install services and run Domino platform."""
-    platform.create_platform(domino_frontend_image, domino_backend_image, run_airflow, use_gpu)
+    platform.create_platform(domino_frontend_image, domino_rest_image, run_airflow, use_gpu)
 
 
 @click.group()
 @click.pass_context
 def cli_platform(ctx):
     """Domino platform actions"""
     if ctx.invoked_subcommand == "prepare":
```

### Comparing `domino-py-0.1.5/domino/cli/utils/config-domino-local.toml` & `domino-py-0.1.6/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/cli/utils/create_cluster.sh` & `domino-py-0.1.6/domino/cli/utils/create_cluster.sh`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 cluster_name=$1
 
 # Delete any existing clusters with provided name
 kind delete cluster --name cluster_name
 sleep 2
 
 # Create a kind cluster
-kind create cluster --name flowui-cluster --config kind-cluster-config.yaml
+kind create cluster --name domino-cluster --config kind-cluster-config.yaml
 
 # kind load docker-image taufferconsulting/flowui-airflow-base:0.0.1 --name flowui-cluster --nodes flowui-cluster-worker
 
 # helm dependency build dependency
 
 # helm upgrade -i -f airflow_helm_chart/values-dev.yaml airflow airflow_helm_chart/
 # helm upgrade --set github_access_token=$GITHUB_ACCESS_TOKEN -i -f flowui_helm_chart/values-dev.yaml flowui flowui_helm_chart/
```

### Comparing `domino-py-0.1.5/domino/cli/utils/pieces_repository.py` & `domino-py-0.1.6/domino/cli/utils/pieces_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,41 +105,27 @@
         while not validator.get('validator_func')(new_var):
             new_var = input(f"Wrong {var} format. Enter a new value: ")
         os.environ[var] = new_var
 
 
 def validate_config(config_dict: dict) -> None:
     """
-    Validate user config.toml file and save it to config_dict and as environment variables to be used by the docker-compose file
+    Validate config.toml file.
     """
-    # TODO check if it still being used
-    required_fields = list(CONFIG_REQUIRED_FIELDS.keys()).copy()
-    required_secrets = list()
+    required_fields = ["REGISTRY_NAME", "REPOSITORY_NAME", "VERSION"]
     sections = config_dict.keys()
     for section in sections:
         for key, value in config_dict.get(section).items():
-            # Check if PIECES_SECRETS exist in environment
-            if section == "repository" and key == "PIECES_SECRETS":
-                for v in value:
-                    if not os.getenv(v, None):
-                        required_secrets.append(v)
             # Check if required fields were defined in config file
-            elif key in CONFIG_REQUIRED_FIELDS:
-                required_fields.remove(key.upper())
-                if key in ["VOLUME_MOUNT_PATH_HOST", "FLOWUI_PATH_HOST"]:
-                    value = str(Path(value).resolve())
-                # Set config as env vars, it will be used by compose
+            if key in required_fields:
+                required_fields.remove(key)
+                # Set config vars as env vars, it will be used by docker build
                 set_config_as_env(key, value) 
-                CONFIG_REQUIRED_FIELDS[key.upper()] = value
-
     if len(required_fields) > 0:
         console.print("Missing required fields: {}".format(required_fields), style=f"bold {COLOR_PALETTE.get('error')}") 
-    if len(required_secrets) > 0:
-        missing = '\n'.join(required_secrets)
-        console.print(f"Missing required pieces secrets. These shold be defined in your ENV: \n{missing}", style=f"bold {COLOR_PALETTE.get('error')}") 
 
 
 def validate_repository_structure() -> None:
     """
     Validate the Pieces repository structure.
     The basic initial structure must contain:
     - config.toml
@@ -150,32 +136,28 @@
     organized_domino_path = Path(".") / ".domino/"
     if not organized_domino_path.is_dir():
         organized_domino_path.mkdir(parents=True, exist_ok=True)
     
     # Validating config
     config_path = Path(".") / 'config.toml'
     if not config_path.is_file():
-        console.print("Missing config file", style=f"bold {COLOR_PALETTE.get('error')}")
-        raise FileNotFoundError("Missing config file")
+        console.print("Missing config.toml file", style=f"bold {COLOR_PALETTE.get('error')}")
+        raise FileNotFoundError("Missing config.toml file")
 
     with open(config_path, "rb") as f:
         config_dict = tomli.load(f)
 
     validate_config(config_dict)
     validate_env_vars()
 
     pieces_repository = Path(".")
     if not pieces_repository.is_dir():
         console.print("Pieces repository path does not exist", style=f"bold {COLOR_PALETTE.get('error')}")
         raise Exception("Pieces repository path does not exist")
 
-    if not (pieces_repository / 'config.toml').is_file():
-        console.print("config.toml file does not exist", style=f"bold {COLOR_PALETTE.get('error')}")
-        raise Exception("config.toml file does not exist")
-
     if not (pieces_repository / 'pieces').is_dir():
         console.print("Pieces directory does not exist", style=f"bold {COLOR_PALETTE.get('error')}")
         raise Exception("Pieces directory does not exist")
     
     if not (pieces_repository / 'dependencies').is_dir():
         console.print("Dependencies directory does not exist", style=f"bold {COLOR_PALETTE.get('error')}")
         raise Exception("Dependencies directory does not exist")
@@ -192,21 +174,21 @@
     pieces_path = Path(".") / "pieces"
     dependencies_path = Path(".") / "dependencies"
     organized_domino_path = Path(".") / ".domino/"
     dependencies_files = [f.name for f in dependencies_path.glob("*")]
     name_errors = list()
     missing_file_errors = list()
     missing_dependencies_errors = list()
-    for op_dir in pieces_path.glob("*Piece"): # TODO change to *Piece
+    for op_dir in pieces_path.glob("*Piece"):
         if op_dir.is_dir():
             # Validate necessary files exist
             files_names = [f.name for f in op_dir.glob("*")]
             if 'models.py' not in files_names:
                 missing_file_errors.append(f"missing 'models.py' for {op_dir.name}")
-            if 'piece.py' not in files_names: # TODO change to piece.py
+            if 'piece.py' not in files_names: 
                 missing_file_errors.append(f"missing 'piece.py' for {op_dir.name}")
             if len(missing_file_errors) > 0:
                 raise Exception('\n'.join(missing_file_errors))
 
             # Validate metadata
             if (op_dir / "metadata.json").is_file():
                 with open(str(op_dir / "metadata.json"), "r") as f:
@@ -248,15 +230,15 @@
     shutil.rmtree(f"{repository_name}/.git")
 
     # Update config
     with open(f"{repository_name}/config.toml", "rb") as f:
         repo_config = tomli.load(f)
 
     repo_config["repository"]["REPOSITORY_NAME"] = repository_name
-    repo_config["repository"]["REGISTRY_NAME"] =  container_registry if container_registry else "ENTER-YOUR-GITHUB-REGISTRY-NAME-HERE"
+    repo_config["repository"]["REGISTRY_NAME"] =  container_registry if container_registry else "enter-your-github-registry-name-here"
 
     with open(f"{repository_name}/config.toml", "wb") as f:
         tomli_w.dump(repo_config, f)
 
     console.print(f"Pieces repository successfully create at: {repository_folder}", style=f"bold {COLOR_PALETTE.get('success')}")
     console.print("")
```

### Comparing `domino-py-0.1.5/domino/cli/utils/platform.py` & `domino-py-0.1.6/domino/cli/utils/platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     console.print("")
     console.print(f"Domino is prepared to run at: {running_path}")
     console.print(f"You can check and modify the configuration file at: {running_path}/config-domino-local.toml")
     console.print("Next, run: `domino platform create`")
     console.print("")
 
 
-def create_platform(domino_frontend_image: str = None, domino_backend_image: str = None, run_airflow: bool = True, use_gpu: bool = False) -> None:
+def create_platform(domino_frontend_image: str = None, domino_rest_image: str = None, run_airflow: bool = True, use_gpu: bool = False) -> None:
     # Load configuration values
     with open("config-domino-local.toml", "rb") as f:
         platform_config = tomli.load(f)
 
     # Create kind config file and run bash script to create Kind cluster
     kubeadm_config_patches = dict(
         kind="InitConfiguration",
@@ -130,15 +130,15 @@
                     propagation='HostToContainer'
                 )
             )
         if platform_config['local_domino_repository'].get('DOMINO_LOCAL_DOMINO_REPOSITORY'):
             extra_mounts_local_repositories.append(
                 dict(
                     hostPath=platform_config['local_domino_repository']['DOMINO_LOCAL_DOMINO_REPOSITORY'],
-                    containerPath=f"/domino_dev", # TODO change in next build
+                    containerPath=f"/domino/domino_py",
                     readOnly=True,
                     propagation='HostToContainer'
                 )
             )
 
     kubeadm_parsed = AsLiteral(yaml.dump(kubeadm_config_patches))
     use_gpu_dict = {} if not use_gpu else {"gpus": True}
@@ -202,21 +202,21 @@
     subprocess.run(["kubectl", "apply", "-f", "https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml"], stdout=subprocess.DEVNULL)
     subprocess.run(["kubectl", "wait", "--namespace", "ingress-nginx", "--for", "condition=ready", "pod", "--selector=app.kubernetes.io/component=controller", "--timeout=180s"])
 
     if domino_frontend_image:
         console.print(f"Loading local frontend image {domino_frontend_image} to Kind cluster...")
         subprocess.run(["kind", "load", "docker-image", domino_frontend_image , "--name", cluster_name, "--nodes", f"{cluster_name}-worker"])
     else:
-        domino_frontend_image = "taufferconsulting/flowui-frontend:latest" # TODO change to domino image name
+        domino_frontend_image = "ghcr.io/tauffer-consulting/domino-frontend:latest"
     
-    if domino_backend_image:
-        console.print(f"Loading local backend image {domino_backend_image} to Kind cluster...")
-        subprocess.run(["kind", "load", "docker-image", domino_backend_image , "--name", cluster_name, "--nodes", f"{cluster_name}-worker"])
+    if domino_rest_image:
+        console.print(f"Loading local REST image {domino_rest_image} to Kind cluster...")
+        subprocess.run(["kind", "load", "docker-image", domino_rest_image , "--name", cluster_name, "--nodes", f"{cluster_name}-worker"])
     else:  
-        domino_backend_image = "taufferconsulting/flowui-backend:latest" # TODO change to domino image name
+        domino_rest_image = "ghcr.io/tauffer-consulting/domino-rest:latest" 
 
     """
     In order to use nvidia gpu in our cluster we need nvidia plugins to be installed.
     We can use nvidia operator to install nvidia plugins.
 
     References: 
         https://catalog.ngc.nvidia.com/orgs/nvidia/containers/gpu-operator
@@ -241,15 +241,15 @@
     # Install Domino Services
     # TODO use remote helm chart
     subprocess.run([
         "helm", "install", 
         "--set", f"github_access_token_pieces={token_pieces}",
         "--set", f"github_access_token_workflows={token_workflows}",
         "--set", f"frontend.image={domino_frontend_image}",
-        "--set", f"backend.image={domino_backend_image}",
+        "--set", f"backend.image={domino_rest_image}",
         "--set", f"backend.workflowsRepository={platform_config['github']['DOMINO_GITHUB_WORKFLOWS_REPOSITORY']}",
         "domino",
         domino_base_helm_path
     ])
 
     if not run_airflow:
         console.print("")
@@ -280,15 +280,15 @@
                     "claimName": "domino-dev-volume-claim"
                 }
             }
         ]
         workers_extra_volumes_mounts = [
             {
                 "name": "domino-dev-extra",
-                "mountPath": "/opt/airflow/domino_dev" # TODO change to /domino_dev
+                "mountPath": "/opt/airflow/domino/domino_py"
             }
         ]
         workers = {
             "workers": {
                 "extraVolumes": workers_extra_volumes,
                 "extraVolumeMounts": workers_extra_volumes_mounts,
             }
@@ -308,15 +308,15 @@
                     "name": "DOMINO_DEV_MODE",
                     "value": platform_config['kind']["dev_mode"]
                 },
             ],
             "images": {
                 "useDefaultImageForMigration": False,
                 "airflow": {
-                    "repository": "taufferconsulting/flowui-airflow-base", # TODO change to prod # TODO change to domino image name when we have it
+                    "repository": "ghcr.io/tauffer-consulting/domino-airflow-base", # TODO change to prod # TODO change to domino image name when we have it
                     "tag": "latest",
                     "pullPolicy": "IfNotPresent"
                 }
             },
             "extraSecrets": {
                 "airflow-ssh-secret": {
                     "data": airflow_ssh_config_parsed
@@ -485,15 +485,15 @@
             k8s_client.create_namespaced_persistent_volume_claim(namespace="default", body=pvc)
             pv = client.V1PersistentVolume(
                 metadata=client.V1ObjectMeta(name="domino-dev-volume"),
                 spec=client.V1PersistentVolumeSpec(
                     storage_class_name="standard",
                     access_modes=["ReadWriteMany"],
                     capacity={"storage": "2Gi"},
-                    host_path=client.V1HostPathVolumeSource(path="/domino_dev"), # TODO - change this to domino_dev once we have a domino_dev in the docker images
+                    host_path=client.V1HostPathVolumeSource(path="/domino/domino_py"),
                     claim_ref=client.V1ObjectReference(
                         namespace="default",
                         name="domino-dev-volume-claim",
                     ),
                     node_affinity=client.V1VolumeNodeAffinity(
                         required=client.V1NodeSelector(
                             node_selector_terms=[
```

### Comparing `domino-py-0.1.5/domino/client/airflow_client.py` & `domino-py-0.1.6/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/client/domino_backend_client.py` & `domino-py-0.1.6/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/client/fs_client.py` & `domino-py-0.1.6/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/client/github_rest_client.py` & `domino-py-0.1.6/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/client/local_files_client.py` & `domino-py-0.1.6/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/client/s3_client.py` & `domino-py-0.1.6/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/custom_operators/bash_operator.py` & `domino-py-0.1.6/domino/custom_operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/custom_operators/k8s_operator.py` & `domino-py-0.1.6/domino/custom_operators/k8s_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             'AIRFLOW_UPSTREAM_TASKS_IDS_SHARED_STORAGE': str(self.shared_storage_upstream_ids_list),
         }
 
         self.shared_storage_sidecar_container_name = f"domino-shared-storage-sidecar-{self.task_id_replaced}"
         sidecar_container = k8s.V1Container(
             name=self.shared_storage_sidecar_container_name,
             command=['bash', '-c', './sidecar_lifecycle.sh'],
-            image='taufferconsulting/flowui_shared_storage_sidecar:latest',
+            image='ghcr.io/tauffer-consulting/domino_shared_storage_sidecar:latest',
             volume_mounts=volume_mounts_sidecar_container,
             security_context=k8s.V1SecurityContext(privileged=True),
             env=[k8s.V1EnvVar(name=k, value=v) for k, v in env_vars.items()],
             resources=k8s.V1ResourceRequirements(
                 requests={
                     "cpu": "1m",
                     "memory": "128Mi",
```

### Comparing `domino-py-0.1.5/domino/custom_operators/python_operator.py` & `domino-py-0.1.6/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/custom_operators/sidecar/logger.py` & `domino-py-0.1.6/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/custom_operators/sidecar/mount.py` & `domino-py-0.1.6/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/exceptions/exceptions.py` & `domino-py-0.1.6/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz` & `domino-py-0.1.6/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/helm/domino-airflow/values.yaml` & `domino-py-0.1.6/domino/helm/domino-airflow/values.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # # Airflow services override
 airflow:
   enabled: true
   images:
     useDefaultImageForMigration: false
     airflow:
-      repository: taufferconsulting/flowui-airflow-base
+      repository: ghcr.io/tauffer-consulting/domino-airflow-base
       tag: latest
       pullPolicy: IfNotPresent
 
   extraSecrets:
     airflow-ssh-secret:
       # github ssh private deploy key for workflow repository
       data: |
```

### Comparing `domino-py-0.1.5/domino/helm/domino-base/templates/domino-backend-deployment.yml` & `domino-py-0.1.6/domino/helm/domino-base/templates/domino-backend-deployment.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
           image: {{ .Values.backend.image }}
           {{- if .Values.backend.entrypointCommand }}
           command:
             {{ toYaml .Values.backend.entrypointCommand | indent 12 }}
           args:
             {{ toYaml .Values.backend.entrypointArgs | indent 12 }}
           {{- end }}
+
           ports:
             - containerPort: 8000
           imagePullPolicy: IfNotPresent
           env: 
             # TODO use load balancer instead of service ip for airflow webserver ?
             - name: AIRFLOW_WEBSERVER_HOST
               value: http://{{ .Release.Name }}-airflow-webserver:8080
```

### Comparing `domino-py-0.1.5/domino/helm/domino-base/templates/domino-frontend-deployment.yml` & `domino-py-0.1.6/domino/helm/domino-base/templates/domino-frontend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/helm/domino-base/templates/domino-postgres-deployment.yml` & `domino-py-0.1.6/domino/helm/domino-base/templates/domino-postgres-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/helm/domino-base/templates/jobs/domino-migrations.yml` & `domino-py-0.1.6/domino/helm/domino-base/templates/jobs/domino-migrations.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/logger.py` & `domino-py-0.1.6/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/schemas/piece_metadata.py` & `domino-py-0.1.6/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/schemas/shared_storage.py` & `domino-py-0.1.6/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/scripts/create_docker_compose_file.py` & `domino-py-0.1.6/domino/scripts/create_docker_compose_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import yaml
 import json
 import os
 from pathlib import Path
 
 
+# TODO - UPDATE THIS
+
+
 class MyDumper(yaml.SafeDumper):
     def write_line_break(self, data=None):
         """
         Insert blank lines between top-level objects
         From here: https://github.com/yaml/pyyaml/issues/127#issuecomment-525800484
         inspired by https://stackoverflow.com/a/44284819/3786245
         """
```

### Comparing `domino-py-0.1.5/domino/scripts/docker_compose_constants.py` & `domino-py-0.1.6/domino/scripts/docker_compose_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import copy
 import os
 from domino.scripts.docker_compose_scripts import init_script
 
 
+# TODO - UPDATE THIS
+
 # Airflow configuration variables reference:
 # https://airflow.apache.org/docs/apache-airflow/stable/configurations-ref.html
 
 
 # Variables shared by most services
 code_repository_source = os.environ.get('CODE_REPOSITORY_SOURCE', 'local')
 volume_mount_path_host = os.environ.get('VOLUME_MOUNT_PATH_HOST', './mnt/fs')
```

### Comparing `domino-py-0.1.5/domino/scripts/docker_compose_scripts.py` & `domino-py-0.1.6/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/scripts/generate_infrasctructure.py` & `domino-py-0.1.6/domino/scripts/generate_infrasctructure.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/scripts/load_piece.py` & `domino-py-0.1.6/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/scripts/run_piece_bash.py` & `domino-py-0.1.6/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/scripts/run_piece_dry.py` & `domino-py-0.1.6/domino/scripts/run_piece_dry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
     secrets_input: dict = None,
     results_path: str = None
 ):
     if not results_path:
         results_path = Path('./dry_run_results')
         results_path.mkdir(parents=True, exist_ok=True)
 
-    pieces_folder_path = str(Path(repository_folder_path).resolve() / "operators")
+    pieces_folder_path = str(Path(repository_folder_path).resolve() / "pieces")
     if pieces_folder_path not in sys.path:
         sys.path.append(pieces_folder_path)
 
     # Load Operator class
     importlib.invalidate_caches()
-    piece_module = importlib.import_module(f"{piece_name}.operator")
+    piece_module = importlib.import_module(f"{piece_name}.piece")
     piece_class = getattr(piece_module, piece_name)
 
     # Load metadata
     metadata_path = Path(pieces_folder_path) / f"{piece_name}/metadata.json"
     with open(metadata_path, "r") as f:
         metadata = json.load(f)
```

### Comparing `domino-py-0.1.5/domino/scripts/run_piece_k8s.py` & `domino-py-0.1.6/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino/task.py` & `domino-py-0.1.6/domino/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from domino.utils import dict_deep_update
 from domino.logger import get_configured_logger
 from domino.schemas.shared_storage import StorageSource
 from domino.schemas.container_resources import ContainerResourcesModel
 from kubernetes import client, config
 import os
 
+
 class Task(object):
     """
     The Task object represents a task in a workflow. 
     It is only instantiated by processes parsing dag files in Airflow.
     """
 
     def __init__(
@@ -29,15 +30,14 @@
         piece_input_kwargs: dict,
         workflow_shared_storage: dict = None,
         container_resources: dict = None,
         deploy_mode: str = 'k8s',
     ) -> None:
         # Task configuration and attributes
         self.task_id = task_id
-        # Logger
         self.logger = get_configured_logger(f"{self.__class__.__name__ }-{self.task_id}")
         self.logger.info('### Configuring task object ###')
         self.dag = dag
         self.dag_id = self.dag.dag_id
         self.repository_id = piece["repository_id"]
         self.piece = piece
         if not workflow_shared_storage:
@@ -98,20 +98,21 @@
                         "dag_id": self.dag_id,
                     }),
                     "DOMINO_BASHOPERATOR_RUN_PIECE_KWARGS": str(piece_input_kwargs),
                 },
                 append_env=True
             )
 
-        # Ref: https://airflow.apache.org/docs/apache-airflow/1.10.14/_api/airflow/contrib/operators/kubernetes_pod_operator/index.html
-        # Good example: https://github.com/apache/airflow/blob/main/tests/system/providers/cncf/kubernetes/example_kubernetes.py
-        # Commands HAVE to go in a list object, ref: https://stackoverflow.com/a/55149915/11483674
+        # References: 
+        # - https://airflow.apache.org/docs/apache-airflow/1.10.14/_api/airflow/contrib/operators/kubernetes_pod_operator/index.html
+        # - https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html
+        # - https://www.astronomer.io/guides/templating/
+        # - good example: https://github.com/apache/airflow/blob/main/tests/system/providers/cncf/kubernetes/example_kubernetes.py
+        # - commands HAVE to go in a list object: https://stackoverflow.com/a/55149915/11483674
         elif self.deploy_mode == "k8s":
-            # https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html
-            # https://www.astronomer.io/guides/templating/
             container_env_vars = {
                 "DOMINO_K8S_PIECE": self.piece["name"],
                 "DOMINO_K8S_INSTANTIATE_PIECE_KWARGS": str({
                     "deploy_mode": self.deploy_mode,
                     "task_id": self.task_id,
                     "dag_id": self.dag_id,
                 }),
@@ -139,15 +140,15 @@
             #self.container_resources = ContainerResourcesModel(**self.container_resources)
             container_resources_obj = k8s.V1ResourceRequirements(**basic_container_resources)
 
             # Volumes
             all_volumes = []
             all_volume_mounts = []
 
-            ######################## For local FLOWUI_DEV_MODEOperators dev ###########################################
+            ######################## For local DOMINO_DEV_MODE Operators dev ###########################################
             if os.environ.get('DOMINO_DEV_MODE') == 'local':
                 source_image = self.piece.get('source_image')
                 repository_raw_project_name = str(source_image).split('/')[1].split(':')[0]
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 persistent_volume_name = 'pv-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
@@ -198,15 +199,15 @@
                 if pvc_exists:
                     volume_dev = k8s.V1Volume(
                         name='jobs-persistent-storage-dev',
                         persistent_volume_claim=k8s.V1PersistentVolumeClaimVolumeSource(claim_name=domino_package_local_claim_name),
                     )
                     volume_mount_dev = k8s.V1VolumeMount(
                         name='jobs-persistent-storage-dev', 
-                        mount_path='/home/domino_dev', 
+                        mount_path='/home/domino/domino_py', 
                         sub_path=None,
                         read_only=True
                     )
                     all_volumes.append(volume_dev)
                     all_volume_mounts.append(volume_mount_dev)
             ############################################################################################
 
@@ -221,25 +222,23 @@
                 task_id=self.task_id,
                 name=f"airflow-worker-pod-{self.task_id}",
                 startup_timeout_seconds=pod_startup_timeout_in_seconds,
                 # cmds=["python"],
                 # arguments=["-c", "'import time; time.sleep(10000)'"],
                 cmds=["domino"],
                 arguments=["run-piece-k8s"],
-                # cmds=['sleep'],
-                # arguments=['65'],
                 env_vars=container_env_vars,
                 do_xcom_push=True,
                 in_cluster=True,
-                # labels={"foo": "bar"},
-                # secrets=[secret_file, secret_env, secret_all_keys],
-                # ports=[port],
                 volumes=all_volumes,
                 volume_mounts=all_volume_mounts,
                 container_resources=container_resources_obj,
+                # labels={"foo": "bar"},
+                # secrets=[secret_file, secret_env, secret_all_keys],
+                # ports=[port],
                 # env_from=configmaps,
                 # affinity=affinity,
                 # is_delete_piece_pod=True,
                 # hostnetwork=False,
                 # tolerations=tolerations,
                 # init_containers=[init_container],
                 # priority_class_name="medium",
```

### Comparing `domino-py-0.1.5/domino/utils/validators.py` & `domino-py-0.1.6/domino/utils/validators.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.5/domino_py.egg-info/SOURCES.txt` & `domino-py-0.1.6/domino_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 domino/helm/domino-base/templates/domino-backend-deployment.yml
 domino/helm/domino-base/templates/domino-frontend-deployment.yml
 domino/helm/domino-base/templates/domino-postgres-deployment.yml
 domino/helm/domino-base/templates/ingress-api.yaml
 domino/helm/domino-base/templates/ingress-frontend.yaml
 domino/helm/domino-base/templates/secrets.yaml
 domino/helm/domino-base/templates/jobs/domino-migrations.yml
-domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
-domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
+domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
+domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
 domino/schemas/__init__.py
 domino/schemas/container_resources.py
 domino/schemas/from_upstream.py
 domino/schemas/piece_metadata.py
 domino/schemas/shared_storage.py
 domino/scripts/__init__.py
 domino/scripts/build_docker_images_pieces.py
```

### Comparing `domino-py-0.1.5/setup.py` & `domino-py-0.1.6/setup.py`

 * *Files identical despite different names*

