# Comparing `tmp/pureml-0.3.5.tar.gz` & `tmp/pureml-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.5.tar", max compression
+gzip compressed data, was "pureml-0.3.6.tar", max compression
```

## Comparing `pureml-0.3.5.tar` & `pureml-0.3.6.tar`

### file list

```diff
@@ -1,105 +1,108 @@
--rw-r--r--   0        0        0    11370 2023-04-05 12:44:15.330474 pureml-0.3.5/README.md
--rw-r--r--   0        0        0      734 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/__init__.py
--rw-r--r--   0        0        0     2534 2023-02-10 14:59:50.822240 pureml-0.3.5/pureml/cli/__init__.py
--rw-r--r--   0        0        0     9059 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/cli/auth.py
--rw-r--r--   0        0        0     1046 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3198 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/main.py
--rw-r--r--   0        0        0     3236 2023-04-18 20:20:22.611483 pureml-0.3.5/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.5/pureml/cli/public.pem
--rw-r--r--   0        0        0     1696 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7290 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2116 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/components/__init__.py
--rw-r--r--   0        0        0     1748 2023-03-15 11:32:06.993246 pureml-0.3.5/pureml/components/auth.py
--rw-r--r--   0        0        0    15690 2023-04-08 14:57:03.440354 pureml-0.3.5/pureml/components/dataset.py
--rw-r--r--   0        0        0       99 2023-04-05 12:44:15.342474 pureml-0.3.5/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     7073 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6852 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6830 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9667 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6801 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/image.py
--rw-r--r--   0        0        0     2052 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/components/log/log.py
--rw-r--r--   0        0        0     6045 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     6016 2023-04-05 12:44:15.702483 pureml-0.3.5/pureml/components/log/params.py
--rw-r--r--   0        0        0     6198 2023-04-10 21:10:47.279602 pureml-0.3.5/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6214 2023-04-10 21:10:47.311604 pureml-0.3.5/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6084 2023-04-10 21:10:47.323604 pureml-0.3.5/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6909 2023-04-05 12:44:15.698483 pureml-0.3.5/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6308 2023-04-05 12:44:15.698483 pureml-0.3.5/pureml/components/log/video.py
--rw-r--r--   0        0        0    13620 2023-04-08 23:11:11.562439 pureml-0.3.5/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.5/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.5/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.5/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.5/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.5/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.5/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.5/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.5/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.5/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.5/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.5/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.5/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.5/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.5/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.5/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.5/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.5/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.5/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.5/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.5/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.5/pureml/package/__init__.py
--rw-r--r--   0        0        0     6324 2023-04-15 12:47:43.506059 pureml-0.3.5/pureml/package/docker.py
--rw-r--r--   0        0        0     5913 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.5/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.5/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.5/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.5/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      365 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2578 2023-04-18 20:24:19.682573 pureml-0.3.5/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.5/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.5/pureml/schema/dataset.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.5/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.5/pureml/schema/paths.py
--rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/schema/predict.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.5/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.5/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.5/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.5/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.5/pureml/utils/constants.py
--rw-r--r--   0        0        0     2998 2023-03-15 11:32:07.825248 pureml-0.3.5/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.5/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.5/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.5/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.5/pureml/utils/predict.py
--rw-r--r--   0        0        0      815 2023-02-10 14:59:51.066213 pureml-0.3.5/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.5/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.5/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.5/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.5/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1927 2023-04-18 20:24:19.682573 pureml-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    13291 1970-01-01 00:00:00.000000 pureml-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-04-27 08:41:10.100182 pureml-0.3.6/README.md
+-rw-r--r--   0        0        0      735 2023-04-27 08:41:10.100182 pureml-0.3.6/pureml/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 08:41:10.100182 pureml-0.3.6/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9746 2023-04-27 08:41:10.116182 pureml-0.3.6/pureml/cli/auth.py
+-rw-r--r--   0        0        0     2447 2023-04-27 08:41:10.128183 pureml-0.3.6/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3201 2023-04-27 08:41:10.128183 pureml-0.3.6/pureml/cli/main.py
+-rw-r--r--   0        0        0     3365 2023-04-27 08:41:10.140183 pureml-0.3.6/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.6/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1697 2023-04-27 08:41:10.140183 pureml-0.3.6/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7182 2023-04-27 08:41:10.148183 pureml-0.3.6/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2861 2023-04-27 08:41:10.148183 pureml-0.3.6/pureml/components/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/auth.py
+-rw-r--r--   0        0        0    15075 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/dataset.py
+-rw-r--r--   0        0        0       88 2023-04-27 08:41:10.156183 pureml-0.3.6/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-27 08:41:10.168184 pureml-0.3.6/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6634 2023-04-27 08:41:10.180184 pureml-0.3.6/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6708 2023-04-27 08:41:10.188184 pureml-0.3.6/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9603 2023-04-27 08:41:10.196184 pureml-0.3.6/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6679 2023-04-27 08:41:10.200184 pureml-0.3.6/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2041 2023-04-27 08:41:10.200184 pureml-0.3.6/pureml/components/log/log.py
+-rw-r--r--   0        0        0     5929 2023-04-27 08:41:10.212185 pureml-0.3.6/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     5925 2023-04-27 08:41:10.224185 pureml-0.3.6/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6166 2023-04-27 08:41:10.228185 pureml-0.3.6/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6181 2023-04-27 08:41:10.240185 pureml-0.3.6/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6049 2023-04-27 08:41:10.248185 pureml-0.3.6/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6776 2023-04-27 08:41:10.264186 pureml-0.3.6/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6168 2023-04-27 08:41:10.268186 pureml-0.3.6/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13206 2023-04-27 08:41:10.276186 pureml-0.3.6/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.6/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.6/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.6/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.6/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.6/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.6/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.6/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.6/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.6/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.6/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.6/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.6/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.6/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.6/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.6/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.6/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.6/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.6/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.6/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.6/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.6/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.6/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6446 2023-04-27 08:41:10.288186 pureml-0.3.6/pureml/package/docker.py
+-rw-r--r--   0        0        0     6014 2023-04-27 08:41:10.300186 pureml-0.3.6/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.6/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.6/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.6/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.6/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      439 2023-04-27 08:41:10.308187 pureml-0.3.6/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2580 2023-04-27 08:41:10.308187 pureml-0.3.6/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.6/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.6/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      163 2023-04-27 08:41:10.312187 pureml-0.3.6/pureml/schema/env.py
+-rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.6/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.6/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1095 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/schema/predict.py
+-rw-r--r--   0        0        0      308 2023-04-27 08:41:10.316187 pureml-0.3.6/pureml/schema/request.py
+-rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.6/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.6/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.6/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.6/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.6/pureml/utils/constants.py
+-rw-r--r--   0        0        0     1230 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/env.py
+-rw-r--r--   0        0        0     2942 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.6/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.6/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.6/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.6/pureml/utils/predict.py
+-rw-r--r--   0        0        0      816 2023-04-27 08:41:10.324187 pureml-0.3.6/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-04-11 17:20:43.542513 pureml-0.3.6/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.6/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.6/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.6/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1927 2023-04-27 08:41:10.324187 pureml-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 pureml-0.3.6/PKG-INFO
```

### Comparing `pureml-0.3.5/README.md` & `pureml-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 <br />
 
 # 🔮 Core design principles
 
 |                                     |                                                                                                                 |
 | ----------------------------------- | --------------------------------------------------------------------------------------------------------------- |
 | Easy developer experience           | An intuitive open source package aimed to bridge the gaps in data science teams                                 |
-| Engineering best practices built-in | Integrating PureML functionalities in your code doesnot disrupt your workflow                                   |
+| Engineering best practices built-in | Integrating PureML functionalities in your code does not disrupt your workflow                                  |
 | Object Versioning                   | A reliable object versioning mechanism to track changes to your datasets, and models                            |
 | Data is a first-class citizen       | Your data is secure. It will never leave your system.                                                           |
 | Reduce Friction                     | Have access to operations performed on data using data lineage without having to spend time on lengthy meetings |
 
 <br />
 
 # ⚙ Core abstractions
@@ -286,19 +286,19 @@
 Work with mutual respect.
 
 <br />
 
 # 👨‍👩‍👧‍👦 Community
 
 To get quick updates, feature release for PureML follow us on
-| |
-| --- |
-| [<img alt="Twitter" height="20" src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />](https://twitter.com/getPureML) |
-[<img alt="LinkedIn" height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/company/pureml-inc/) |
-| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />](https://github.com/PureML-Inc/PureML) |
-| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />](https://discord.gg/DBvedzGu) |
+|                                                                                                                                                                                         |
+| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [<img alt="Twitter" height="20" src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />](https://twitter.com/getPureML)                   |
+| [<img alt="LinkedIn" height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/company/pureml-inc/) |
+| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />](https://github.com/PureML-Inc/PureML)               |
+| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />](https://discord.gg/DBvedzGu)                      |
 
 # 📄 License
 
 See the [Apache-2.0](./License) file for licensing information.
 
 <br />
```

### Comparing `pureml-0.3.5/pureml/__init__.py` & `pureml-0.3.6/pureml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 from .evaluate import grader, eval
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
-__version__ = "0.3.5"
+
+__version__ = "0.3.6"
```

### Comparing `pureml-0.3.5/pureml/cli/auth.py` & `pureml-0.3.6/pureml/cli/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import socket
 from time import sleep, time
 import requests
 import typer
 from rich import print
-from pureml.cli.helpers import save_auth
-
+from pureml.cli.helpers import get_auth_headers, save_auth
+from pureml.schema import ContentTypeHeader, AcceptHeader
 from pureml.schema.backend import get_backend_base_url, get_frontend_base_url
 from .orgs import select
 from rich.progress import Progress, SpinnerColumn, TextColumn
-from pureml.components import delete_token, get_org_id, get_token
+from pureml.components import delete_token, get_api_token, get_org_id, get_token
 from urllib.parse import urljoin
 import json
 import platform
 import ipapi
 
 app = typer.Typer()
 
+
 def get_location():
     try:
         response = ipapi.location(output="json")
     except:
         try:
             # print("Getting device details...")
-            response = requests.get(f'https://api64.ipify.org?format=json').json()
-            response = requests.get(f"https://ipapi.co/{response['ip']}/json/", headers={
-                    "User-Agent": "pureml-cli"
-                }).json()
+            response = requests.get(f"https://api64.ipify.org?format=json").json()
+            response = requests.get(
+                f"https://ipapi.co/{response['ip']}/json/",
+                headers={"User-Agent": "pureml-cli"},
+            ).json()
         except:
             response = {
                 "ip": socket.gethostbyname(socket.gethostname()),
                 "city": "Unknown",
                 "region": "Unknown",
                 "country": "Unknown",
             }
@@ -37,21 +39,27 @@
         "ip": response["ip"] or socket.gethostbyname(socket.gethostname()),
         "city": response["city"] or "Unknown",
         "region": response["region"] or "Unknown",
         "country": response["country_name"] or "Unknown",
     }
     return location_data
 
+
 @app.command()
 def details():
     token = get_token()
+    api_token = get_api_token()
     org_id = get_org_id()
 
     print("Org Id: ", org_id)
-    print("Access Token: ", token)
+    if token is not None:
+        print("Access Token: ", token)
+    if api_token is not None:
+        print("API Id: ", api_token["api_id"])
+        print("API Key: ", api_token["api_key"])
 
 
 @app.callback()
 def callback():
     """
     Authentication user command
 
@@ -61,15 +69,22 @@
     signup - Creates new user
     login - Logs in user
     logout - Logs out user
     """
 
 
 @app.command()
-def signup(backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def signup(
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    )
+):
     try:
         print("\nCreate a new account/\n")
         email: str = typer.prompt("Enter new email")
         handle: str = typer.prompt("Enter new user handle")
         name: str = typer.prompt("Enter new user name")
         password: str = typer.prompt(
             "Enter new password", confirmation_prompt=True, hide_input=True
@@ -84,34 +99,48 @@
 
         response = requests.post(url, json=data)
 
         if not response.ok:
             print(f"[red]Could not create account! Please try again later")
             return
         elif response.status_code == 202:
-            print(f"[green]Successfully created your account! You need to verify your email to login!")
             print(
-                f"[green]You can then login using `pureml auth login`"
+                f"[green]Successfully created your account! You need to verify your email to login!"
             )
+            print(f"[green]You can then login using `pureml auth login`")
         else:
             print(f"[green]Successfully created your account!")
-            print(
-                f"[green]You can now login using `pureml auth login`"
-            )
+            print(f"[green]You can now login using `pureml auth login`")
     except Exception as e:
         print(f"[red]Could not create account! Please try again later")
         print(e)
 
+
 @app.command()
 def login(
-    backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance"),
-    frontend_url: str = typer.Option("", "--frontend-url", "-f", help="Frontend URL for self-hosted or custom pureml frontend instance"),
-    browserless: bool = typer.Option(False, "--browserless", "-s", help="Browserless login for ssh or pipelines"),
-    interactive: bool = typer.Option(False, "--interactive", "-i", help="Login with email and password interactively"),
-    ):
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    ),
+    frontend_url: str = typer.Option(
+        "",
+        "--frontend-url",
+        "-f",
+        help="Frontend URL for self-hosted or custom pureml frontend instance",
+    ),
+    browserless: bool = typer.Option(
+        False, "--browserless", "-s", help="Browserless login for ssh or pipelines"
+    ),
+    interactive: bool = typer.Option(
+        False, "--interactive", "-i", help="Login with email and password interactively"
+    ),
+    api_key: bool = typer.Option(False, "--api-key", "-k", help="Login with api key"),
+):
     try:
         backend_base_url = get_backend_base_url(backend_url)
         frontend_base_url = get_frontend_base_url(frontend_url)
         # Interactive login with email and password
         if interactive:
             print(f"\n[Enter your credentials to login[/\n")
             email: str = typer.prompt("Enter your email")
@@ -131,60 +160,71 @@
                 email = token["email"]
 
                 save_auth(access_token=access_token, email=email)
 
                 print(f"[green]Successfully logged in as {email}!")
 
                 # Select organization
-                org_id = select()
-                if org_id is not None:
-                    save_auth(org_id=org_id, access_token=access_token, email=email)
-                    print(f"[green]Successfully linked to organization {org_id}!")
-                else:
-                    print(f"[red]Organization details not found! Please contact your admin to add you to an organization!")
+                select()
 
             else:
                 print(f"[red]Unable to login to your account!")
-        
+
+        # API key login
+        elif api_key:
+            print(f"\n[Enter your credentials to login[/\n")
+            api_id: str = typer.prompt("Enter your api id")
+            api_key: str = typer.prompt("Enter your api key")
+            save_auth(api_id=api_id, api_key=api_key)
+            select()
+
         # Browser based login
         else:
             # Get device details
             device = platform.platform()
             device_data = get_location()
             device_id = device_data["ip"]
-            device_location = device_data["city"] + ", " + device_data["region"] + ", " + device_data["country"]
+            device_location = (
+                device_data["city"]
+                + ", "
+                + device_data["region"]
+                + ", "
+                + device_data["country"]
+            )
 
             # Create session
             device_data = {
                 "device": device,
                 "device_id": device_id,
-                "device_location": device_location
+                "device_location": device_location,
             }
             url_path = "user/create-session"
             url = urljoin(backend_base_url, url_path)
 
             # print(device_data)
             response = requests.post(url, json=device_data)
 
             if not response.ok:
                 print(f"[red]Unable to create session! Please try again later")
                 return
-            
+
             session_id = response.json()["data"][0]["session_id"]
 
             # Generater link & Open browser
             link = urljoin(frontend_base_url, f"verify-session/{session_id}")
 
             if browserless:
-                print(f"Please open the following link in your browser to login: [underline]{link}[/underline]")
+                print(
+                    f"Please open the following link in your browser to login: [underline]{link}[/underline]"
+                )
             else:
                 # Open browser
                 print(f"Opening the browser : [underline]{link}[/underline]")
                 typer.launch(link)
-            
+
             with Progress(
                 SpinnerColumn(),
                 TextColumn("[progress.description]{task.description}"),
                 transient=True,
             ) as progress:
                 progress.add_task(description="Waiting for response...", total=None)
                 # Hit the endpoint to check if the session is verified
@@ -210,39 +250,42 @@
 
                         break
                     else:
                         if response.status_code == 404:
                             print(f"[red]Session not found! Please try again later")
                             return
                         elif response.status_code == 403:
-                            print(f"[red]Session expired or invalid device! Please try again later")
+                            print(
+                                f"[red]Session expired or invalid device! Please try again later"
+                            )
                             return
 
                     if time() - start_time > 60 * 10:
                         print(f"[red]Session timed out!")
                         return
-                    
+
                     sleep(1)
             print(f"[green]Successfully logged in as {email}!")
-            
+
             # Select organization
             select()
     except Exception as e:
         print(f"[red]Unable to contact the server! Please try again later")
         print(e)
 
 
 @app.command()
 def status():
-    exists = get_token()
+    exists = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
     if exists:
         print(f"[green]You are logged in!")
 
 
 @app.command()
 def logout():
-    exists = get_token()
+    exists = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
     if exists:
         delete_token()
 
+
 if __name__ == "__main__":
     app()
```

### Comparing `pureml-0.3.5/pureml/cli/main.py` & `pureml-0.3.6/pureml/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,25 @@
         None, "--backend-url", "-b", help="The backend url to use"
     ),
     frontend_url: str = typer.Option(
         None, "--frontend-url", "-f", help="The frontend url to use"
     ),
 ):
     """
-    This command will initialize the puremlconfig.yml file for your project
+    This command will initialize the puremlconfig.yaml file for your project
     """
     from pathlib import Path
 
     project_path = Path.cwd()
 
-    puremlconfig = PureMLConfigYML(project_path / "puremlconfig.yml")
+    puremlconfig = PureMLConfigYML(project_path / "puremlconfig.yaml")
     
     # check if the config file exists
     if puremlconfig.file.exists():
-        print("A puremlconfig.yml file already exists in this directory - aborting")
+        print("A puremlconfig.yaml file already exists in this directory - aborting")
         return
     
     # if not silent, ask for the config values
     if not silent:
         print("Let's get started with the configuration of your project")
 
         # if not repository:
```

### Comparing `pureml-0.3.5/pureml/cli/orgs.py` & `pureml-0.3.6/pureml/cli/orgs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Dict, List
 import requests
 import typer
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from urllib.parse import urljoin
-from pureml.cli.helpers import save_auth
-from pureml.schema import BackendSchema, PathSchema
-from pureml.components import get_token
+from pureml.cli.helpers import get_auth_headers, save_auth
+from pureml.schema import BackendSchema, PathSchema, ContentTypeHeader, AcceptHeader
 from pureml.schema.backend import get_backend_base_url
 
-
-
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 app = typer.Typer()
 
 
 @app.callback()
 def callback():
@@ -24,24 +21,28 @@
 
     Use with show or select option
 
     show - lists all the organizations\n
     select - select an organization
     """
 
+
 @app.command()
-def show(backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
-    access_token = get_token()
+def show(
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    )
+):
     url_path = "org"
     url = urljoin(get_backend_base_url(backend_url), url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
     response = requests.get(url, headers=headers)
     if response.ok:
         print()
         print("[bold green] You are part of following Organizations!")
         org_all = response.json()["data"]
         console = Console()
         count = 0
@@ -55,46 +56,59 @@
         console.print(table)
         print()
         return count, org_data
     else:
         print("[bold red]Unable to get the list of organizations!")
         return None, None
 
+
 @app.command()
-def select(backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def select(
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    )
+):
     print("[bold green] Select the Sr.No. of Organization")
     count, org_data = show(backend_url=backend_url)
     if count:
         sr_no = -1
         while int(sr_no) not in range(1, count + 1):
-            sr_no: str = typer.prompt("Enter your Sr.No. of Organization (1 .... " + str(count) + ")")
+            sr_no: str = typer.prompt(
+                "Enter your Sr.No. of Organization (1 .... " + str(count) + ")"
+            )
             if int(sr_no) not in range(1, count + 1):
                 print("[bold red]Invalid Sr.No. of Organization!")
         save_auth(org_id=org_data[int(sr_no)]["id"])
         selected_org_name = org_data[int(sr_no)]["name"]
         print(f"[green]Successfully linked to organization {selected_org_name}!")
     else:
         print("[bold red]Did not Select any organization!")
         return None
 
+
 # Possibly useful for future commands
 # Moved from auth.py
-def check_org_status(access_token: str, base_url: str):
+def check_org_status(headers: dict, base_url: str):
+    """
+    Headers: dict
+        headers from get_auth_headers() invocation of parent function
+
+    base_url: str
+        base_url from get_backend_base_url() invocation of parent function
+    """
 
     org_id: str = typer.prompt("Enter your Org Id")
 
     url_path = "org/id/{}".format(org_id)
     url = urljoin(base_url, url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
-
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # print("[green]Organization Exists!")
         return org_id
     else:
         print("[red]Organization does not Exists!")
-        return None
+        return None
```

### Comparing `pureml-0.3.5/pureml/cli/puremlconfig.py` & `pureml-0.3.6/pureml/cli/puremlconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         
     def __str__(self) -> str:
         return self._path.as_posix()
     
 
 class PureMLConfigYML():
     """
-    PureMLConfigYML is a class that is used to generate the configuration file `puremlconfig.yml`
+    PureMLConfigYML is a class that is used to generate the configuration file `puremlconfig.yaml`
     It is capable of reading and writing the configuration file
     """
     def __init__(self, path: Path):
         self._yaml_file = YAMLFile(path)
         self._yaml_document = None 
 
     @property
```

### Comparing `pureml-0.3.5/pureml/cli/secrets.py` & `pureml-0.3.6/pureml/cli/secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from urllib.parse import urljoin
 import jwt
 import requests
 import typer
 from rich import print
 from rich.console import Console
 from rich.table import Table
+from pureml.cli.helpers import get_auth_headers
 from pureml.schema.backend import get_backend_base_url
 from pureml.cli.puremlconfig import PureMLConfigYML
-from pureml.components import get_org_id, get_token
-from pureml.schema.backend import BackendSchema
-from pureml.schema.paths import PathSchema
+from pureml.components import get_org_id
+from pureml.schema import BackendSchema, PathSchema, ContentTypeHeader
+
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 app = typer.Typer()
 
 
 @app.callback()
@@ -30,15 +31,22 @@
     all - Gets all secret names for the organization
     show - Show all secrets of secret name
     delete - Delete secrets under secret name
     """
 
 
 @app.command()
-def add(backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def add(
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    )
+):
     """
     Add a new integration and it's secrets
 
     Usage:
     pureml secrets add
     """
     backend_base_url = get_backend_base_url(backend_url)
@@ -71,15 +79,14 @@
         secret_value = typer.prompt(f"Enter the value for {secret_key}")
         if not secret_value:
             print(f"[bold red]Invalid value for {secret_key}[/bold red]")
             return
         user_secrets[secret_key] = secret_value
 
     # Add secret
-    access_token = get_token()
     org_id = get_org_id()
 
     data = {}
     url_path = ""
 
     # match integration_id:
     if integration_id == "s3":
@@ -102,48 +109,48 @@
             "public_url": user_secrets["public_url"],
             "secret_name": secret_name,
         }
         url_path = f"org/{org_id}/secret/r2/connect"
 
     url = urljoin(backend_base_url, url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
 
     response = requests.post(url, json=data, headers=headers)
 
     if response.ok:
         print(f"[bold green]Successfully added secrets for {secret_name}[/bold green]")
 
     else:
         print("[bold red]Unable to fetch secrets!")
 
 
 @app.command()
-def all(backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def all(
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    )
+):
     """
     Get all secret names for the organization
 
     Usage:
     pureml secrets all
     """
     backend_base_url = get_backend_base_url(backend_url)
 
     print()
-    access_token = get_token()
     org_id = get_org_id()
     url_path = f"org/{org_id}/secret"
     url = urljoin(backend_base_url, url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         secrets_all = response.json()["data"]
         if not secrets_all or len(secrets_all) == 0:
             print("[bold red]No secrets found[/bold red]")
@@ -157,33 +164,37 @@
         console.print(table)
         print()
     else:
         print("[bold red]Unable to fetch secrets!")
 
 
 @app.command()
-def show(secret_name: str = typer.Argument(..., case_sensitive=True), backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def show(
+    secret_name: str = typer.Argument(..., case_sensitive=True),
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    ),
+):
     """
     Shows the secrets under given secret name
 
     Usage:
     pureml secrets show "secret_name"
     """
     backend_base_url = get_backend_base_url(backend_url)
-    
+
     print()
-    access_token = get_token()
     org_id = get_org_id()
     url_path = f"org/{org_id}/secret/{secret_name}"
     url = urljoin(backend_base_url, url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         secrets_all = response.json()["data"]
         if not secrets_all or len(secrets_all) == 0:
             print(f"[bold red]No secrets found for {secret_name}[/bold red]")
@@ -202,15 +213,23 @@
         print()
 
     else:
         print("[bold red]Unable to fetch secrets!")
 
 
 @app.command()
-def delete(secret_name: str = typer.Argument(..., case_sensitive=True), backend_url: str = typer.Option("", "--backend-url", "-b", help="Backend URL for self-hosted or custom pureml backend instance")):
+def delete(
+    secret_name: str = typer.Argument(..., case_sensitive=True),
+    backend_url: str = typer.Option(
+        "",
+        "--backend-url",
+        "-b",
+        help="Backend URL for self-hosted or custom pureml backend instance",
+    ),
+):
     """
     Delete secrets using key
 
     Usage:
     purecli secrets delete "secret_name"
     """
     backend_base_url = get_backend_base_url(backend_url)
@@ -220,23 +239,19 @@
     confirm = typer.confirm(
         f"Are you sure you want to delete the {secret_name} secrets?"
     )
     if not confirm:
         return
 
     # Delete secret
-    access_token = get_token()
     org_id = get_org_id()
     url_path = f"org/{org_id}/secret/{secret_name}"
     url = urljoin(backend_base_url, url_path)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(access_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
 
     response = requests.delete(url, headers=headers)
 
     if response.ok:
         print(f"[bold green]Successfully deleted {secret_name} secrets[/bold green]")
     else:
         print("[bold red]Unable to delete secrets!")
```

### Comparing `pureml-0.3.5/pureml/components/dataset.py` & `pureml-0.3.6/pureml/components/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import json
 import os
 from urllib.parse import urljoin
 import time
 import joblib
 import pandas as pd
 import requests
+from pureml.cli.helpers import get_auth_headers
 
-from pureml.schema import DatasetSchema, StorageSchema, ConfigKeys
+from pureml.schema import (
+    DatasetSchema,
+    StorageSchema,
+    ConfigKeys,
+    ContentTypeHeader,
+    AcceptHeader,
+)
 from pureml.utils.hash import generate_hash_for_file
 from pureml.utils.readme import load_readme
 from rich import print
 
-from . import get_org_id, get_token
+from . import get_org_id
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 config_keys = ConfigKeys
 storage = StorageSchema().get_instance()
 
 
 def init_branch(label: str):
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch/create".format(org_id, name)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_JSON)
 
     data = {"dataset_name": name, "branch_name": branch}
 
     data = json.dumps(data)
 
     response = requests.post(url, data=data, headers=headers)
 
@@ -51,22 +54,21 @@
         return False
 
 
 def check_dataset_hash(hash: str, label: str):
 
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch/{}/hash-status".format(org_id, name, branch)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     data = {"hash": hash, "branch": branch}
 
     data = json.dumps(data)
 
     response = requests.post(url, data=data, headers=headers)
 
@@ -77,25 +79,21 @@
 
     return hash_exists
 
 
 def branch_details(label: str):
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch/{}".format(org_id, name, branch)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         response_text = response.json()
         # T-1161 standardize api response to contains Data as a list
         details = response_text["data"]
@@ -119,25 +117,21 @@
     else:
         return False
 
 
 def branch_delete(label: str) -> str:
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch/{}/delete".format(org_id, name, branch)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.delete(url, headers=headers)
 
     if response.ok:
         print(f"[bold green]Dataset branch has been deleted")
 
     else:
@@ -146,25 +140,21 @@
     return response.text
 
 
 def branch_list(label: str) -> str:
 
     name, _, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch".format(org_id, name)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         response_text = response.json()
         branch_list = response_text["data"]
 
@@ -181,25 +171,21 @@
 
     Returns
     -------
         A list of all the datasets
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/all".format(org_id)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # print(f"[bold green]Obtained list of models")
 
         response_text = response.json()
@@ -213,36 +199,29 @@
     return
 
 
 def init(label: str, readme: str = None):
 
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
+    headers = get_auth_headers(content_type=ContentTypeHeader.ALL)
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     if readme is None:
         readme = dataset_schema.PATH_DATASET_README
 
     file_content, file_type = load_readme(path=readme)
 
     branch_user = "dev" if branch is None else branch
     branch_main = "main"
 
     url = "org/{}/dataset/{}/create".format(org_id, name)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        # "Content-Type": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-        # 'accept': 'application/json',
-        "Content-Type": "*/*",
-    }
-
     data = {
         "name": name,
         "branch_names": [branch_main, branch_user],
         "readme": {"file_type": file_type, "content": file_content},
     }
 
     data = json.dumps(data)
@@ -288,15 +267,14 @@
         The name of the dataset.
     version: str, optional
         The version of the dataset.
 
     """
     name, branch, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     dataset_path = save_dataset(dataset, name)
     name_with_ext = dataset_path.split("/")[-1]
 
     dataset_hash = generate_hash_for_file(
@@ -339,18 +317,15 @@
         print(f"[bold red]Dataset already exists. Not registering a new version!")
         return True, dataset_hash, "latest"
     else:
 
         url = "org/{}/dataset/{}/branch/{}/register".format(org_id, name, branch)
         url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-        headers = {
-            "Authorization": "Bearer {}".format(user_token),
-            "accept": "application/json",
-        }
+        headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
         files = {"file": (name_with_ext, open(dataset_path, "rb"))}
 
         lineage = json.dumps(lineage)
 
         data = {
             "name": name,
@@ -360,21 +335,25 @@
             "is_empty": is_empty,
             "storage": storage.STORAGE,
         }
 
         # data = json.dumps(data)
 
         response = requests.post(url, files=files, data=data, headers=headers)
+        # print(response.request.headers)
+        # print(response.request.body)
 
         if response.ok:
 
             # print(response.json())
             try:
                 dataset_version = response.json()["data"][0]["version"]
                 print("Version: ", dataset_version)
+                dataset_label = ":".join([label, dataset_label])
+                print("Dataset label: ", dataset_label)
 
                 if is_empty:
                     print(f"[bold green]Lineage has been registered!")
                 else:
                     print(f"[bold green]Dataset and lineage have been registered!")
 
                 # reset_config(key=config_keys.dataset.value)
@@ -421,25 +400,21 @@
     -------
         The details of the dataset.
 
     """
 
     name, _, _ = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}".format(org_id, name)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # print(f"[bold green]Dataset details have been fetched")
         response_text = response.json()
         dataset_details = response_text["data"][0]
@@ -464,25 +439,21 @@
     -------
         The details of the dataset.
 
     """
 
     name, branch, version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     url = "org/{}/dataset/{}/branch/{}/version/{}".format(org_id, name, branch, version)
     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # print(f"[bold green]Dataset Version details have been fetched")
         response_text = response.json()
         dataset_details = response_text["data"][0]
@@ -509,15 +480,14 @@
     -------
         The dataset dataframe is being returned.
 
     """
 
     name, branch, version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
     dataset_schema = DatasetSchema()
 
     dataset_details = version_details(label=label)
 
     if dataset_details is None:
         print(f"[bold red]Unable to fetch Dataset version")
@@ -532,18 +502,15 @@
     # storage_path = dataset_details["path"]["source_path"]
     # storage_source_type = dataset_details["path"]["source_type"]["public_url"]
 
     # dataset_url = urljoin(storage_source_type, storage_path)
 
     dataset_url = dataset_details["path"]
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     # print('url', dataset_url)
 
     response = requests.get(dataset_url)
 
     if response.ok:
         dataset_bytes = response.content
@@ -581,15 +548,15 @@
 #     org_id = get_org_id()
 #     dataset_schema = DatasetSchema()
 
 #     url = "org/{}/dataset/{}/delete".format(org_id, name)
 #     url = urljoin(dataset_schema.backend.BASE_URL, url)
 
 #     headers = {
-#         "Content-Type": "application/x-www-form-urlencoded",
+#         "Content-Type": ContentTypeHeader.APP_FORM_URL_ENCODED.value,
 #         "Authorization": "Bearer {}".format(user_token),
 #     }
 
 #     data = {"version": version}
 
 #     data = json.dumps(data)
```

### Comparing `pureml-0.3.5/pureml/components/log/arrays.py` & `pureml-0.3.6/pureml/components/log/arrays.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 import os
 import json
 
 
 from urllib.parse import urljoin
 
+from pureml.cli.helpers import get_auth_headers
+
 from . import get_token, get_org_id
 
-from pureml.schema import PathSchema, BackendSchema
+from pureml.schema import PathSchema, BackendSchema, ContentTypeHeader
 from joblib import Parallel, delayed
 from PIL import Image
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 
@@ -46,26 +48,22 @@
     model_version: str
         The version of the model
     name : str
         The name of the array.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         res_text = json.loads(response.text)
 
         if len(res_text) == 0:
@@ -102,33 +100,32 @@
 
     Returns
     -------
         The response is a JSON object
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
     array_paths = save_images(arrays=array)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     files = {}
     for file_name, file_path in array_paths.items():
 
         if os.path.isfile(file_path):
             files[file_name] = open(file_path, "rb")
         else:
-            print("[bold red] array", file_name, "doesnot exist at the given path")
+            print("[bold red] array", file_name, "does not exist at the given path")
 
     data = {"name_path_mapping": array_paths}
 
     response = requests.post(url, data=data, files=files, headers=headers)
 
     if response.status_code == 200:
         print(f"[bold green]arrays have been registered!")
@@ -156,31 +153,27 @@
 
     Returns
     -------
         The response text is being returned.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_array(array_details: dict):
 
         url = array_details["location"]
         file_path_temp = array_details["path"]
         file_name = file_path_temp.split(os.path.sep)[-1]
         save_path = os.path.join(path_schema.PATH_ARRAY_DIR, file_name)
         print("save path", save_path)
 
         name_fetched = array_details["array"]
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
         print("array url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         print(response.status_code)
@@ -242,26 +235,22 @@
     model_name : str
         The name of the model you want to delete the array from
     model_version: str
         The version of the model
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     # array_details = details(model_name=model_name, array=array)
 
     # if array_details is None:
     #     print('[bold red] Unable to find array details')
     #     return
```

### Comparing `pureml-0.3.5/pureml/components/log/artifacts.py` & `pureml-0.3.6/pureml/components/log/video.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,257 +9,230 @@
 
 import os
 import json
 import typing
 
 from urllib.parse import urljoin
 
-from . import get_token, get_org_id
+from pureml.cli.helpers import get_auth_headers
 
-from pureml.schema import PathSchema, BackendSchema
+from . import get_org_id
+
+from pureml.schema import PathSchema, BackendSchema, ContentTypeHeader
 from joblib import Parallel, delayed
 
+
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 
-def details(
-    model_name: str, model_branch: str, model_version: str = "latest", name: str = ""
-):
-    """This function returns the details of the artifact for a given model
+def add(
+    video: str, model_name: str, model_branch: str, model_version: str = "latest"
+) -> str:
+    """`add` function takes in the path of the video, name of the video and the model name and
+    registers the video
 
     Parameters
     ----------
+    video : str
+        The path to the video file.
+    name : str
+        The name of the video.
     model_name : str
-        The name of the model you want to get the artifact details for
+        The name of the model you want to add video to.
     model_version: str
         The version of the model
-    name : str
-        The name of the artifact.
+
+    Returns
+    -------
+        The response is a JSON object
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
-    response = requests.get(url, headers=headers)
-
-    if response.status_code == 200:
-        res_text = json.loads(response.text)
+    files = {}
+    for file_name, file_path in video.items():
 
-        if len(res_text) == 0:
-            print("[bold yellow] No Artifacts have been found for the model")
-            print(res_text)
-            return
+        if os.path.isfile(file_path):
+            files[file_name] = open(file_path, "rb")
         else:
-            print("[bold green]Artifacts have been found for the model")
-            print(res_text)
-            return res_text
+            print("[bold red] video", file_name, "does not exist at the given path")
 
-    else:
-        print("[bold red]Unable to obtain the artifact details")
-        print(response.text)
-        return
+    data = {"name_path_mapping": video}
 
+    response = requests.post(url, data=data, files=files, headers=headers)
 
-# @app.command()
-def add(
-    artifact: str,
-    name: str,
-    model_name: str,
-    model_branch: str,
-    model_version: str = "latest",
-) -> str:
-    """`add` function takes in the path of the artifact, name of the artifact and the model name and
-    registers the artifact
+    if response.status_code == 200:
+        print(f"[bold green]videos have been registered!")
 
-    Parameters
-    ----------
-    artifact : str
-        The path to the artifact file.
-    name : str
-        The name of the artifact.
-    model_name : str
-        The name of the model you want to add artifacts to.
-    model_version: str
-        The version of the model
+    else:
+        print(f"[bold red]videos have not been registered!")
+        print(response.text)
 
-    Returns
-    -------
-        The response is a JSON object
+    return response.text
 
-    """
 
-    user_token = get_token()
+def details(model_name: str, model_branch: str, model_version: str = "latest"):
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
-    if os.path.isfile(artifact):
-        file = {"file": (name, open(artifact, "rb"))}
-    else:
-        print("[bold red] Artifact doesnot exist at the given path")
+    response = requests.get(url, headers=headers)
 
-    data = {"name": name, "path": artifact}
+    if response.ok:
+        # T-1161 standardize api response to contains Models as a list
+        response_text = response.json()
+        details = response_text["data"]
 
-    response = requests.post(url, data=data, files=file, headers=headers)
+        # print(model_details)
 
-    if response.status_code == 200:
-        print(f"[bold green]Artifacts have been registered!")
+        return details
 
     else:
-        print(f"[bold red]Artifacts have not been registered!")
-        print(response.text)
-
-    return response.text
+        print(f"[bold red]Branch details details have not been found")
+        return
 
 
-# @app.command()
-def fetch(model_name: str, model_version: str = "latest", name: str = ""):
-    """It fetches the artifact from the server and stores it in the local directory
+def fetch(
+    model_name: str, model_branch: str, model_version: str = "latest", name: str = ""
+):
+    """It fetches the video from the server and stores it in the local directory
 
     Parameters
     ----------
     model_name : str
-        The name of the model you want to fetch the artifact from.
+        The name of the model you want to fetch the video from.
     model_version: str
         The version of the model
     name : str
-        The name of the artifact to be fetched. If not specified, all artifacts will be fetched.
+        The name of the video to be fetched. If not specified, all videos will be fetched.
 
     Returns
     -------
         The response text is being returned.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
-    def fetch_artifact(artifact_details: dict):
+    def fetch_video(video_details: dict):
 
-        url = artifact_details["location"]
-        file_path_temp = artifact_details["path"]
+        url = video_details["location"]
+        file_path_temp = video_details["path"]
         file_name = file_path_temp.split(os.path.sep)[-1]
-        save_path = os.path.join(path_schema.PATH_ARTIFACT_DIR, file_name)
+        save_path = os.path.join(path_schema.PATH_VIDEO_DIR, file_name)
         print("save path", save_path)
 
-        name_fetched = artifact_details["artifact"]
+        name_fetched = video_details["video"]
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
-        print("Artifact url", url)
+        print("video url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         print(response.status_code)
 
         if response.status_code == 200:
-            print("[bold green] Artifact {} has been fetched".format(name_fetched))
+            print("[bold green] video {} has been fetched".format(name_fetched))
 
             save_dir = os.path.dirname(save_path)
 
             os.makedirs(save_dir, exist_ok=True)
 
-            artifact_bytes = response.content
+            video_bytes = response.content
 
-            open(save_path, "wb").write(artifact_bytes)
+            open(save_path, "wb").write(video_bytes)
 
             print(
-                "[bold green] Artifact {} has been stored at {}".format(
+                "[bold green] video {} has been stored at {}".format(
                     name_fetched, save_path
                 )
             )
 
             return response.text
         else:
-            print("[bold red] Unable to fetch the artifact")
+            print("[bold red] Unable to fetch the video")
 
             return response.text
 
-    artifact_details = details(
-        model_name=model_name, name=name, model_version=model_version
+    video_details = details(
+        model_name=model_name,
+        model_branch=model_branch,
+        name=name,
+        model_version=model_version,
     )
 
-    if artifact_details is None:
+    if video_details is None:
         return
 
-    if type(artifact_details) is dict:
+    if type(video_details) is dict:
 
-        res_text = fetch_artifact(artifact_details)
+        res_text = fetch_video(video_details)
 
-    elif type(artifact_details) is list:
+    elif type(video_details) is list:
         res_text = Parallel(n_jobs=-1)(
-            delayed(fetch_artifact)(art_det) for art_det in artifact_details
+            delayed(fetch_video)(art_det) for art_det in video_details
         )
 
     return res_text
 
 
-# @app.command()
-def delete(
-    name: str, model_name: str, model_branch: str, model_version: str = "latest"
-) -> str:
-    """`delete()` deletes an artifact from a model
+# def delete(name:str, model_name:str,  model_version:str='latest') -> str:
+#     '''`delete()` deletes an video from a model
 
-    Parameters
-    ----------
-    name : str
-        The name of the artifact you want to delete.
-    model_name : str
-        The name of the model you want to delete the artifact from
-    model_version: str
-        The version of the model
+#     Parameters
+#     ----------
+#     name : str
+#         The name of the video you want to delete.
+#     model_name : str
+#         The name of the model you want to delete the video from
+#     model_version: str
+#         The version of the model
 
-    """
+#     '''
 
-    user_token = get_token()
-    org_id = get_org_id()
+#     user_token = get_token()
+#     org_id = get_org_id()
+#     project_id = get_project_id()
 
-    url = "org/{}/model/{}/branch/{}/version/{}/log".format(
-        org_id, model_name, model_branch, model_version
-    )
-    url = urljoin(backend_schema.BASE_URL, url)
+#     url_path_1 = '{}/project/{}/model/{}/{}/video/{}/delete'.format(org_id, project_id, model_name, model_version, name)
+#     url = urljoin(BASE_URL, url_path_1)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
-
-    # artifact_details = details(model_name=model_name, artifact=artifact)
-
-    # if artifact_details is None:
-    #     print('[bold red] Unable to find artifact details')
-    #     return
 
-    response = requests.delete(url, headers=headers)
+#     headers = {
+#         'Content-Type': 'application/x-www-form-urlencoded',
+#         'Authorization': 'Bearer {}'.format(user_token)
+#     }
 
-    if response.status_code == 200:
-        print(f"[bold green]Artifact has been deleted")
 
-    else:
-        print(f"[bold red]Unable to delete artifact")
+#     # video_details = details(model_name=model_name, video=video)
 
-    return response.text
+#     # if video_details is None:
+#     #     print('[bold red] Unable to find video details')
+#     #     return
+
+
+#     response = requests.delete(url, headers=headers)
+
+
+#     if response.status_code == 200:
+#         print(f"[bold green]video has been deleted")
 
+#     else:
+#         print(f"[bold red]Unable to delete video")
 
-# if __name__ == "__main__":
-#     app()
+#     return response.text
```

### Comparing `pureml-0.3.5/pureml/components/log/audio.py` & `pureml-0.3.6/pureml/components/log/audio.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 import os
 import json
 import typing
 
 from urllib.parse import urljoin
 
+from pureml.cli.helpers import get_auth_headers
+
 from . import get_token, get_org_id
 
-from pureml.schema import PathSchema, BackendSchema
+from pureml.schema import PathSchema, BackendSchema, ContentTypeHeader
 from joblib import Parallel, delayed
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 
 def details(
@@ -34,26 +36,22 @@
     model_version: str
         The version of the model
     name : str
         The name of the audio.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         res_text = json.loads(response.text)
 
         if len(res_text) == 0:
@@ -90,33 +88,32 @@
 
     Returns
     -------
         The response is a JSON object
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
     user_token = get_token()
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     files = {}
     for file_name, file_path in audio.items():
 
         if os.path.isfile(file_path):
             files[file_name] = open(file_path, "rb")
         else:
-            print("[bold red] audio", file_name, "doesnot exist at the given path")
+            print("[bold red] audio", file_name, "does not exist at the given path")
 
     data = {"name_path_mapping": audio}
 
     response = requests.post(url, data=data, files=files, headers=headers)
 
     if response.status_code == 200:
         print(f"[bold green]audios have been registered!")
@@ -144,31 +141,27 @@
 
     Returns
     -------
         The response text is being returned.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_audio(audio_details: dict):
 
         url = audio_details["location"]
         file_path_temp = audio_details["path"]
         file_name = file_path_temp.split(os.path.sep)[-1]
         save_path = os.path.join(path_schema.PATH_AUDIO_DIR, file_name)
         print("save path", save_path)
 
         name_fetched = audio_details["audio"]
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
         print("audio url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/components/log/figure.py` & `pureml-0.3.6/pureml/components/log/figure.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 import os
 from urllib.parse import urljoin
 
 import numpy as np
 import requests
 from joblib import Parallel, delayed
 from PIL import Image
+from pureml.cli.helpers import get_auth_headers
 
 from pureml.utils.pipeline import add_figures_to_config
 from pureml.schema import (
     PathSchema,
     BackendSchema,
     StorageSchema,
     LogSchema,
     ConfigKeys,
+    AcceptHeader,
+    ContentTypeHeader,
 )
 from rich import print
-from . import get_org_id, get_token
+from . import get_org_id
 
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
@@ -51,35 +54,34 @@
 
         figure_paths[figure_key] = save_name
 
     return figure_paths
 
 
 def post_figures(figure_paths, model_name: str, model_branch: str, model_version: str):
-    user_token = get_token()
     org_id = get_org_id()
 
     # print('figure_paths', figure_paths)
 
     url = "org/{}/model/{}/branch/{}/version/{}/logfile".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     files = []
     for file_name, file_path in figure_paths.items():
         # print("filename", file_name)
 
         if os.path.isfile(file_path):
             files.append(("file", (file_name, open(file_path, "rb"))))
 
         else:
-            print("[bold red] figure", file_name, "doesnot exist at the given path")
+            print("[bold red] figure", file_name, "does not exist at the given path")
 
     data = {
         "data": figure_paths,
         "key": "figure",
         "storage": storage.STORAGE,
     }
 
@@ -91,14 +93,15 @@
 
     if response.ok:
         print(f"[bold green]Figures have been registered!")
         reset_config(key=config_keys.figure.value)
 
     else:
         print(f"[bold red]Figures have not been registered!")
+        print(response.text)
 
     return response
     # except Exception as e:
     #     return
 
 
 def add(label: str = None, figure: dict = None, file_paths: dict = None) -> str:
@@ -152,26 +155,22 @@
         # print(response.text)
 
     # return response.text
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
@@ -200,28 +199,24 @@
     Returns
     -------
         The response text is being returned.
 
     """
     model_name, model_branch, model_version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_figure(file_details):
 
         file_name, url = file_details
 
         save_path = os.path.join(path_schema.PATH_FIGURE_DIR, file_name)
         # print("save path in fetching", save_path)
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
         # print("figure url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         # print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/components/log/image.py` & `pureml-0.3.6/pureml/components/log/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 import os
 import json
 import typing
 
 from urllib.parse import urljoin
 
+from pureml.cli.helpers import get_auth_headers
+
 from . import get_token, get_org_id
 
-from pureml.schema import PathSchema, BackendSchema
+from pureml.schema import PathSchema, BackendSchema, ContentTypeHeader
 from joblib import Parallel, delayed
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 
 def details(
@@ -34,26 +36,22 @@
     model_version: str
         The version of the model
     name : str
         The name of the image.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         res_text = json.loads(response.text)
 
         if len(res_text) == 0:
@@ -90,32 +88,31 @@
 
     Returns
     -------
         The response is a JSON object
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
 
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     files = {}
     for file_name, file_path in image.items():
 
         if os.path.isfile(file_path):
             files[file_name] = open(file_path, "rb")
         else:
-            print("[bold red] image", file_name, "doesnot exist at the given path")
+            print("[bold red] image", file_name, "does not exist at the given path")
 
     data = {"name_path_mapping": image}
 
     response = requests.post(url, data=data, files=files, headers=headers)
 
     if response.status_code == 200:
         print(f"[bold green]images have been registered!")
@@ -143,31 +140,27 @@
 
     Returns
     -------
         The response text is being returned.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_image(image_details: dict):
 
         url = image_details["location"]
         file_path_temp = image_details["path"]
         file_name = file_path_temp.split(os.path.sep)[-1]
         save_path = os.path.join(path_schema.PATH_IMAGE_DIR, file_name)
         print("save path", save_path)
 
         name_fetched = image_details["image"]
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
         print("image url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/components/log/log.py` & `pureml-0.3.6/pureml/components/log/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import figure as pure_figure
 from . import predict as pure_predict
 from . import pip_requirement as pure_pip_req
 from pureml.utils.version_utils import parse_version_label
 from pureml.schema import PathSchema, BackendSchema, LogSchema
 import requests
 from urllib.parse import urljoin
-from . import get_org_id, get_token
+from . import get_org_id
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 post_keys = LogSchema().key
```

### Comparing `pureml-0.3.5/pureml/components/log/metrics.py` & `pureml-0.3.6/pureml/components/log/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import json
 from urllib.parse import urljoin
 
 import requests
-from pureml.schema import BackendSchema, LogSchema, ConfigKeys
+from pureml.cli.helpers import get_auth_headers
+from pureml.schema import BackendSchema, LogSchema, ConfigKeys, ContentTypeHeader
 from pureml.utils.log_utils import merge_step_with_value
 from pureml.utils.pipeline import add_metrics_to_config
 from rich import print
 
-from . import convert_values_to_string, get_org_id, get_token
+from . import convert_values_to_string, get_org_id
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 
 backend_schema = BackendSchema().get_instance()
 post_key_predict = LogSchema().key.metrics.value
 config_keys = ConfigKeys
 
 
 def post_metrics(metrics, model_name: str, model_branch: str, model_version: str):
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Content-Type": "*/*",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.ALL)
 
     metrics = json.dumps(metrics)
     data = {"data": metrics, "key": post_key_predict}
 
     data = json.dumps(data)
 
     response = requests.post(url, data=data, headers=headers)
@@ -98,26 +94,22 @@
         # return response.text
 
     # return
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
```

### Comparing `pureml-0.3.5/pureml/components/log/params.py` & `pureml-0.3.6/pureml/components/log/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import json
 from urllib.parse import urljoin
 
 import requests
-from pureml.schema import BackendSchema, LogSchema, ConfigKeys
+from pureml.cli.helpers import get_auth_headers
+from pureml.schema import BackendSchema, LogSchema, ConfigKeys, ContentTypeHeader
 from pureml.utils.log_utils import merge_step_with_value
 from pureml.utils.pipeline import add_params_to_config
 from rich import print
 
-from . import convert_values_to_string, get_org_id, get_token
+from . import convert_values_to_string, get_org_id
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 backend_schema = BackendSchema().get_instance()
 post_key_params = LogSchema().key.params.value
 config_keys = ConfigKeys
 
 
 def post_params(params, model_name: str, model_branch: str, model_version: str):
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     params = json.dumps(params)
 
     data = {"data": params, "key": post_key_params}
 
     data = json.dumps(data)
 
@@ -97,26 +94,22 @@
     #     return response.text
 
     # return
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
```

### Comparing `pureml-0.3.5/pureml/components/log/pip_requirement.py` & `pureml-0.3.6/pureml/components/log/pip_requirement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
 import os
 from urllib.parse import urljoin
 
 import numpy as np
 import requests
 from joblib import Parallel, delayed
+from pureml.cli.helpers import get_auth_headers
 
 from pureml.utils.pipeline import add_pip_req_to_config
 from pureml.schema import (
     PathSchema,
     BackendSchema,
     StorageSchema,
     LogSchema,
     ConfigKeys,
+    AcceptHeader,
+    ContentTypeHeader,
 )
 from rich import print
-from . import get_org_id, get_token
+from . import get_org_id
 
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
@@ -27,36 +30,35 @@
 config_keys = ConfigKeys
 storage = StorageSchema().get_instance()
 
 
 def post_pip_requirement(
     file_paths, model_name: str, model_branch: str, model_version: str
 ):
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/logfile".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     files = []
     for file_name, file_path in file_paths.items():
         # print("filename", file_name)
 
         if os.path.isfile(file_path):
             files.append(("file", (file_name, open(file_path, "rb"))))
 
         else:
             print(
                 "[bold red] pip_requirement",
                 file_name,
-                "doesnot exist at the given path",
+                "does not exist at the given path",
             )
 
     data = {
         "data": file_paths,
         "key": post_key_pip_req,
         "storage": storage.STORAGE,
     }
@@ -103,26 +105,22 @@
         print(response.text)
 
     # return response.text
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
@@ -135,28 +133,27 @@
         print(f"[bold red]Unable to fetch pip_requirement file!")
         return
 
 
 def fetch(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_pip_requirement(file_details):
 
         file_name, url = file_details
 
         save_path = os.path.join(path_schema.PATH_PREDICT_DIR, file_name)
         print("save path", save_path)
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(
+            content_type=ContentTypeHeader.APP_FORM_URL_ENCODED,
+            accept=AcceptHeader.APP_JSON,
+        )
 
         # print("figure url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         # print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/components/log/predict.py` & `pureml-0.3.6/pureml/components/log/predict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
 import os
 from urllib.parse import urljoin
 
 import numpy as np
 import requests
 from joblib import Parallel, delayed
+from pureml.cli.helpers import get_auth_headers
 
 from pureml.utils.pipeline import add_pred_to_config
 from pureml.schema import (
     PathSchema,
     BackendSchema,
     StorageSchema,
     LogSchema,
     ConfigKeys,
+    AcceptHeader,
+    ContentTypeHeader,
 )
 from rich import print
-from . import get_org_id, get_token, pip_requirement, resources
+from . import get_org_id, pip_requirement, resources
 import shutil
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
@@ -27,33 +30,32 @@
 post_key_requirements = LogSchema().key.requirements.value
 post_key_resources = LogSchema().key.resources.value
 config_keys = ConfigKeys
 storage = StorageSchema().get_instance()
 
 
 def post_predict(file_paths, model_name: str, model_branch: str, model_version: str):
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/logfile".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     files = []
     for file_name, file_path in file_paths.items():
         # print("filename", file_name)
 
         if os.path.isfile(file_path):
             files.append(("file", (file_name, open(file_path, "rb"))))
 
         else:
-            print("[bold red] Predict", file_name, "doesnot exist at the given path")
+            print("[bold red] Predict", file_name, "does not exist at the given path")
 
     data = {
         "data": file_paths,
         "key": post_key_predict,
         "storage": storage.STORAGE,
     }
 
@@ -107,26 +109,22 @@
         print(response.text)
 
     # return response.text
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
@@ -139,29 +137,27 @@
         print(f"[bold red]Unable to fetch Predict!")
         return
 
 
 def fetch(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_predict(file_details):
 
         file_name, url = file_details
 
         save_path = os.path.join(path_schema.PATH_PREDICT_DIR, file_name)
         # print("save path", save_path)
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
-
+        headers = get_auth_headers(
+            content_type=ContentTypeHeader.APP_FORM_URL_ENCODED,
+            accept=AcceptHeader.APP_JSON,
+        )
         # print("predict url", url)
 
         response = requests.get(url)
 
         # print(response.status_code)
 
         if response.ok:
```

### Comparing `pureml-0.3.5/pureml/components/log/resources.py` & `pureml-0.3.6/pureml/components/log/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import json
 import os
 from urllib.parse import urljoin
 
 import numpy as np
 import requests
 from joblib import Parallel, delayed
+from pureml.cli.helpers import get_auth_headers
 
 from pureml.utils.pipeline import add_resource_to_config
 from pureml.utils.resources import zip_content, unzip_content
 from pureml.schema import (
     PathSchema,
     BackendSchema,
     StorageSchema,
     LogSchema,
     PredictSchema,
     ConfigKeys,
+    AcceptHeader,
+    ContentTypeHeader,
 )
 from rich import print
-from . import get_org_id, get_token
+from . import get_org_id
 
 from pureml.utils.version_utils import parse_version_label
 from pureml.utils.config import reset_config
 
 
 path_schema = PathSchema().get_instance()
 predict_schema = PredictSchema()
 backend_schema = BackendSchema().get_instance()
 post_key_resources = LogSchema().key.resources.value
 config_keys = ConfigKeys
 storage = StorageSchema().get_instance()
 
 
 def post_resource(path, model_name: str, model_branch: str, model_version: str):
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/logfile".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     try:
         zip_content(src_path=path, dst_path=predict_schema.PATH_RESOURCES)
     except Exception as e:
         print(e)
 
     if not os.path.exists(predict_schema.PATH_RESOURCES):
@@ -96,33 +98,29 @@
         response = post_resource(
             path=path,
             model_name=model_name,
             model_branch=model_branch,
             model_version=model_version,
         )
 
-        # print(response.text)
+        print(response.text)
 
     # return response.text
 
 
 def details(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "accept": "application/json",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=None, accept=AcceptHeader.APP_JSON)
 
     response = requests.get(url, headers=headers)
 
     if response.ok:
         # T-1161 standardize api response to contains Models as a list
         response_text = response.json()
         details = response_text["data"]
@@ -135,28 +133,27 @@
         print(f"[bold red]Unable to fetch resource!")
         return
 
 
 def fetch(label: str):
     model_name, model_branch, model_version = parse_version_label(label)
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_resource(file_details):
 
         file_name, url = file_details
 
         save_path = os.path.join(path_schema.PATH_PREDICT_DIR, file_name)
         # print("save path", save_path)
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(
+            content_type=ContentTypeHeader.APP_FORM_URL_ENCODED,
+            accept=AcceptHeader.APP_JSON,
+        )
 
         # print("resorce url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         # print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/components/log/tabular.py` & `pureml-0.3.6/pureml/components/log/tabular.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 import os
 import json
 import typing
 
 from urllib.parse import urljoin
 
-from . import get_token, get_org_id
+from pureml.cli.helpers import get_auth_headers
 
-from pureml.schema import PathSchema, BackendSchema
+from . import get_org_id
+
+from pureml.schema import PathSchema, BackendSchema, ContentTypeHeader
 from joblib import Parallel, delayed
 
 
 path_schema = PathSchema().get_instance()
 backend_schema = BackendSchema().get_instance()
 
 
@@ -35,26 +37,22 @@
     model_version: str
         The version of the model
     name : str
         The name of the tabular.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-        "Authorization": "Bearer {}".format(user_token),
-    }
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     response = requests.get(url, headers=headers)
 
     if response.status_code == 200:
         res_text = json.loads(response.text)
 
         if len(res_text) == 0:
@@ -91,31 +89,30 @@
 
     Returns
     -------
         The response is a JSON object
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     url = "org/{}/model/{}/branch/{}/version/{}/log".format(
         org_id, model_name, model_branch, model_version
     )
     url = urljoin(backend_schema.BASE_URL, url)
 
-    headers = {"Authorization": "Bearer {}".format(user_token)}
+    headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
     files = {}
     for file_name, file_path in tabular.items():
 
         if os.path.isfile(file_path):
             files[file_name] = open(file_path, "rb")
         else:
-            print("[bold red] Tabular", file_name, "doesnot exist at the given path")
+            print("[bold red] Tabular", file_name, "does not exist at the given path")
 
     data = {"name_path_mapping": tabular}
 
     response = requests.post(url, data=data, files=files, headers=headers)
 
     if response.status_code == 200:
         print(f"[bold green]tabulars have been registered!")
@@ -143,31 +140,27 @@
 
     Returns
     -------
         The response text is being returned.
 
     """
 
-    user_token = get_token()
     org_id = get_org_id()
 
     def fetch_tabular(tabular_details: dict):
 
         url = tabular_details["location"]
         file_path_temp = tabular_details["path"]
         file_name = file_path_temp.split(os.path.sep)[-1]
         save_path = os.path.join(path_schema.PATH_TABULAR_DIR, file_name)
         print("save path", save_path)
 
         name_fetched = tabular_details["tabular"]
 
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "Bearer {}".format(user_token),
-        }
+        headers = get_auth_headers(content_type=ContentTypeHeader.APP_FORM_URL_ENCODED)
 
         print("tabular url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
         print(response.status_code)
```

### Comparing `pureml-0.3.5/pureml/config/parser.py` & `pureml-0.3.6/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/dataset.py` & `pureml-0.3.6/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/load_data.py` & `pureml-0.3.6/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/model.py` & `pureml-0.3.6/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/pip_requirements.py` & `pureml-0.3.6/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/predict.py` & `pureml-0.3.6/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/decorators/transformer.py` & `pureml-0.3.6/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/classification.py` & `pureml-0.3.6/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/eval.py` & `pureml-0.3.6/pureml/evaluate/eval.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/grade.py` & `pureml-0.3.6/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.6/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.6/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/f1.py` & `pureml-0.3.6/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/mae.py` & `pureml-0.3.6/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/mse.py` & `pureml-0.3.6/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/precision.py` & `pureml-0.3.6/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/recall.py` & `pureml-0.3.6/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.6/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/evaluate/regression.py` & `pureml-0.3.6/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/lineage/data/create_lineage.py` & `pureml-0.3.6/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/package/docker.py` & `pureml-0.3.6/pureml/package/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import docker
 from .fastapi import create_fastapi_file
 from pureml.schema import FastAPISchema, PredictSchema, DockerSchema
 import string, random
+from pureml.utils.env import generate_env_dict, validate_env_docker
 
 prediction_schema = PredictSchema()
 fastapi_schema = FastAPISchema()
 docker_schema = DockerSchema()
 
 
 def generate_sys_commands(sys_commands):
@@ -14,15 +15,15 @@
     if len(sys_commands) > 0:
         sys_commands = ["RUN " + i for i in sys_commands]
         commands += "\n".join(sys_commands)
 
     return commands
 
 
-def create_docker_file(org_id, access_token, sys_commands):
+def create_docker_file(sys_commands):
     # os.makedirs(PATH_DOCKER_DIR, exist_ok=True)
     os.makedirs(prediction_schema.paths.PATH_PREDICT_DIR, exist_ok=True)
 
     req_pos = prediction_schema.PATH_PREDICT_REQUIREMENTS.rfind(
         prediction_schema.REQUIREMENTS_NAME
     )
     req_path = prediction_schema.PATH_PREDICT_REQUIREMENTS[req_pos:]
@@ -36,17 +37,14 @@
 
     docker = """
     
 FROM {BASE_IMAGE}
 
 {commands}
 
-ENV ORG_ID={ORG_ID}
-ENV ACCESS_TOKEN={ACCESS_TOKEN}
-
 RUN mkdir -p {PREDICT_DIR}
 
 WORKDIR {PREDICT_DIR}
 
 ADD . {PREDICT_DIR}
 
 COPY . .
@@ -62,16 +60,14 @@
 CMD ["python", "{API_PATH}"]    
 """.format(
         BASE_IMAGE=docker_schema.BASE_IMAGE_DOCKER,
         PORT=docker_schema.PORT_DOCKER,
         PREDICT_DIR=prediction_schema.paths.PATH_PREDICT_DIR_RELATIVE,
         API_PATH=api_path,
         REQUIREMENTS_PATH=req_path,
-        ORG_ID=org_id,
-        ACCESS_TOKEN=access_token,
         commands=commands,
     )
 
     with open(docker_schema.PATH_DOCKER_IMAGE, "w") as docker_file:
         docker_file.write(docker)
 
     docker_yaml = """version: '3'
@@ -133,15 +129,15 @@
         print(e)
         image = None
         build_log = None
 
     return image, build_log, image_tag
 
 
-def run_docker_container(image, runtime, gpu_ids, host_port, docker_port):
+def run_docker_container(image, runtime, gpu_ids, host_port, docker_port, env_dict):
     client = docker.from_env()
     name = image.tags[0].replace(":", "-")
 
     random_value = "".join(random.choices(string.ascii_lowercase + string.digits, k=8))
     name = "-".join([name, random_value])
 
     docker_port = "{p}/tcp".format(p=docker_port)
@@ -150,14 +146,15 @@
     container_args = {
         "image": image,
         "ports": {docker_port: host_port},
         "detach": True,
         "auto_remove": True,
         "name": name,
         "runtime": runtime,
+        "environment": env_dict,
     }
 
     if len(gpu_ids) != 0:
         gpu_ids = [str(id) for id in gpu_ids]
         container_args["device_requests"] = [
             docker.types.DeviceRequest(device_ids=gpu_ids, capabilities=[["gpu"]])
         ]
@@ -173,31 +170,36 @@
     # )
 
     return container
 
 
 def create(
     label,
-    org_id,
-    access_token,
+    # org_id,
+    # access_token,
+    env_path,
     runtime=None,
     gpu_ids=[],
     port=None,
     predict_path=None,
     requirements_path=None,
     sys_commands=[],
 ):
 
+    env_dict = generate_env_dict(env_path=env_path)
+    env_valid = validate_env_docker(env_dict=env_dict)
+
+    if not env_valid:
+        return None
+
     create_fastapi_file(
         label=label, predict_path=predict_path, requirements_path=requirements_path
     )
 
-    create_docker_file(
-        org_id=org_id, access_token=access_token, sys_commands=sys_commands
-    )
+    create_docker_file(sys_commands=sys_commands)
 
     image, build_log, image_tag = create_docker_image(label=label)
 
     if image is not None:
 
         if port is None:
             host_port = docker_schema.PORT_HOST
@@ -208,14 +210,15 @@
 
         container = run_docker_container(
             image=image,
             runtime=runtime,
             gpu_ids=gpu_ids,
             host_port=host_port,
             docker_port=docker_port,
+            env_dict=env_dict,
         )
 
         print("Created Docker container")
         print("Container Name: ", container.name)
         print("Container Long Id: ", container.id)
         print("Container id: ", container.short_id)
```

### Comparing `pureml-0.3.5/pureml/package/fastapi.py` & `pureml-0.3.6/pureml/package/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         zip_content(resources_path, prediction_schema.PATH_RESOURCES)
 
         if os.path.exists(prediction_schema.PATH_RESOURCES):
             unzip_content(
                 prediction_schema.PATH_RESOURCES, path_schema.PATH_PREDICT_DIR
             )
         else:
-            raise Exception(resources_path, "doesnot exists!!!")
+            raise Exception(resources_path, "does not exists!!!")
     else:
         print("Taking the fetched resources file path")
 
 
 def get_predict_file(label, predict_path):
 
     predict.fetch(label)
@@ -52,15 +52,15 @@
             print("Taking the default predict.py file path: ", predict_path)
         else:
             print("Taking the predict.py file path: ", predict_path)
 
         if os.path.exists(predict_path):
             shutil.copy(predict_path, prediction_schema.PATH_PREDICT)
         else:
-            raise Exception(predict_path, "doesnot exists!!!")
+            raise Exception(predict_path, "does not exists!!!")
     else:
         print("Taking the fetched predict.py file path")
 
 
 def get_requirements_file(label, requirements_path):
     pip_requirement.fetch(label=label)
 
@@ -71,15 +71,15 @@
             print("Taking the default requirements.txt file path: ", requirements_path)
         else:
             print("Taking the requirements.txt file path: ", requirements_path)
 
         if os.path.exists(requirements_path):
             shutil.copy(requirements_path, prediction_schema.PATH_PREDICT_REQUIREMENTS)
         else:
-            raise Exception(requirements_path, "doesnot exists!!!")
+            raise Exception(requirements_path, "does not exists!!!")
     else:
         print("Taking the fetched requirements.txt file path")
 
 
 def generate_api(label: str):
     name, branch, version = parse_version_label(label=label)
 
@@ -99,17 +99,19 @@
 
 import nest_asyncio
 from pyngrok import ngrok
 
 load_dotenv()
 
 org_id = os.getenv('ORG_ID')
-access_token = os.getenv('ACCESS_TOKEN')
+api_id = os.getenv('API_ID')
+api_key = os.getenv('API_KEY')
 
-pureml.login(org_id=org_id, access_token=access_token)
+if api_id is not None and api_key is not None and org_id is not None:
+    pureml.login(org_id=org_id, api_id=api_id, api_key=api_key)
 
 predictor = Predictor()
 predictor.load_models()
 
 # input_type, input_shape = process_input(input=predictor.input)
 # output_type, output_shape = process_output(output=predictor.output)
```

### Comparing `pureml-0.3.5/pureml/packaging/__init__.py` & `pureml-0.3.6/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_framework.py` & `pureml-0.3.6/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.6/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.6/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.6/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.6/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.6/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.6/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.6/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.6/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.6/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/packaging.py` & `pureml-0.3.6/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/packaging/packaging_utils.py` & `pureml-0.3.6/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/predictor/predictor.py` & `pureml-0.3.6/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/schema/backend.py` & `pureml-0.3.6/pureml/schema/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import typer
 
 from pathlib import Path
 from pureml.cli.puremlconfig import PureMLConfigYML
 
 
 project_path = Path.cwd()
-if Path.exists(project_path / "puremlconfig.yml"):
-    puremlconfig = PureMLConfigYML(project_path / "puremlconfig.yml")
+if Path.exists(project_path / "puremlconfig.yaml"):
+    puremlconfig = PureMLConfigYML(project_path / "puremlconfig.yaml")
 else:
     puremlconfig = None
 
 
 def get_backend_base_url(backend_url: str = None):
     if (
         backend_url is not None
```

### Comparing `pureml-0.3.5/pureml/schema/packaging.py` & `pureml-0.3.6/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/schema/paths.py` & `pureml-0.3.6/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/schema/predict.py` & `pureml-0.3.6/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/config.py` & `pureml-0.3.6/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/constants.py` & `pureml-0.3.6/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/hash.py` & `pureml-0.3.6/pureml/utils/hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 import string
 import random
 from .config import load_config, save_config
 import json
 import inspect
 import re
 from datetime import datetime
-from pureml.components import get_org_id, get_token
+from pureml.components import get_org_id
 
 
 def file_reader_chunk(file_obj, chunk_size=1024):
     """Generator that reads a file in chunks of bytes"""
     while True:
         chunk = file_obj.read(chunk_size)
         if not chunk:
             return
         yield chunk
 
 
 def generate_hash_unique(name, branch, hash=hashlib.md5):
 
     org_id = get_org_id()
-    access_token = get_token()
 
     time_current = str(datetime.now())
 
     string_random = "".join(
         random.choices(string.ascii_lowercase + string.digits, k=16)
     )
 
     hash_content = "puremlHash".join(
-        [org_id, access_token, name, branch, time_current, string_random]
+        [org_id, name, branch, time_current, string_random]
     )
 
     # print('hash content', hash_content)
 
     value_str = hash_content.encode()
     # print('value_str', value_str)
```

### Comparing `pureml-0.3.5/pureml/utils/log_utils.py` & `pureml-0.3.6/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/package.py` & `pureml-0.3.6/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/pipeline.py` & `pureml-0.3.6/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/predict.py` & `pureml-0.3.6/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/readme.py` & `pureml-0.3.6/pureml/utils/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
                 file_type = path.rsplit('.',1)[-1]
             except Exception as e:
                 print('Unable to read the ReadME file.')
                 print('Creating an Empty ReadME file')
     else:
         with open(path, 'w') as f:
             f.write(file_content)
-        print('ReadME file doesnot exist.')
+        print('ReadME file does not exist.')
         print('Creating an Empty ReadME file')
         
 
         
     return file_content, file_type
```

### Comparing `pureml-0.3.5/pureml/utils/resources.py` & `pureml-0.3.6/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pureml/utils/version_utils.py` & `pureml-0.3.6/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.5/pyproject.toml` & `pureml-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
```

### Comparing `pureml-0.3.5/PKG-INFO` & `pureml-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -266,15 +266,15 @@
 <br />
 
 # 🔮 Core design principles
 
 |                                     |                                                                                                                 |
 | ----------------------------------- | --------------------------------------------------------------------------------------------------------------- |
 | Easy developer experience           | An intuitive open source package aimed to bridge the gaps in data science teams                                 |
-| Engineering best practices built-in | Integrating PureML functionalities in your code doesnot disrupt your workflow                                   |
+| Engineering best practices built-in | Integrating PureML functionalities in your code does not disrupt your workflow                                  |
 | Object Versioning                   | A reliable object versioning mechanism to track changes to your datasets, and models                            |
 | Data is a first-class citizen       | Your data is secure. It will never leave your system.                                                           |
 | Reduce Friction                     | Have access to operations performed on data using data lineage without having to spend time on lengthy meetings |
 
 <br />
 
 # ⚙ Core abstractions
@@ -332,20 +332,20 @@
 Work with mutual respect.
 
 <br />
 
 # 👨‍👩‍👧‍👦 Community
 
 To get quick updates, feature release for PureML follow us on
-| |
-| --- |
-| [<img alt="Twitter" height="20" src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />](https://twitter.com/getPureML) |
-[<img alt="LinkedIn" height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/company/pureml-inc/) |
-| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />](https://github.com/PureML-Inc/PureML) |
-| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />](https://discord.gg/DBvedzGu) |
+|                                                                                                                                                                                         |
+| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| [<img alt="Twitter" height="20" src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />](https://twitter.com/getPureML)                   |
+| [<img alt="LinkedIn" height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/company/pureml-inc/) |
+| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />](https://github.com/PureML-Inc/PureML)               |
+| [<img alt="GitHub" height="20" src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" />](https://discord.gg/DBvedzGu)                      |
 
 # 📄 License
 
 See the [Apache-2.0](./License) file for licensing information.
 
 <br />
```

