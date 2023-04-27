# Comparing `tmp/caikit-0.1.6.tar.gz` & `tmp/caikit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.1.6.tar", last modified: Fri Apr 21 19:59:58 2023, max compression
+gzip compressed data, was "caikit-0.2.0.tar", last modified: Thu Apr 27 17:16:34 2023, max compression
```

## Comparing `caikit-0.1.6.tar` & `caikit-0.2.0.tar`

### file list

```diff
@@ -1,294 +1,293 @@
--rw-r--r--   0        0        0       60 2023-04-21 19:59:49.341120 caikit-0.1.6/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0     1272 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-21 19:59:49.341120 caikit-0.1.6/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-04-21 19:59:49.341120 caikit-0.1.6/.gitignore
--rw-r--r--   0        0        0      310 2023-04-21 19:59:49.341120 caikit-0.1.6/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-21 19:59:49.341120 caikit-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-21 19:59:49.341120 caikit-0.1.6/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-21 19:59:49.341120 caikit-0.1.6/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-21 19:59:49.341120 caikit-0.1.6/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-21 19:59:49.341120 caikit-0.1.6/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-21 19:59:49.341120 caikit-0.1.6/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     6510 2023-04-21 19:59:49.341120 caikit-0.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-21 19:59:49.341120 caikit-0.1.6/LICENSE
--rw-r--r--   0        0        0       18 2023-04-21 19:59:49.341120 caikit-0.1.6/OWNERS
--rw-r--r--   0        0        0     3757 2023-04-21 19:59:49.345121 caikit-0.1.6/README.md
--rw-r--r--   0        0        0    44878 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit-overview.png
--rw-r--r--   0        0        0      323 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/__init__.py
--rw-r--r--   0        0        0     1837 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1104 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/config/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/config/config.py
--rw-r--r--   0        0        0     1010 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/config/config.yml
--rw-r--r--   0        0        0      962 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29207 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13676 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20448 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/model_manager.py
--rw-r--r--   0        0        0    51878 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module.py
--rw-r--r--   0        0        0     7643 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5500 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1001 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0     1787 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/config_utils.py
--rw-r--r--   0        0        0      637 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18275 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1864 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-21 19:59:49.345121 caikit-0.1.6/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     5353 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/config/config.yml
--rw-r--r--   0        0        0     1716 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13853 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6068 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12138 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4194 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    20064 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5763 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12289 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    10693 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10301 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4911 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     7655 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12008 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14523 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10554 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1696 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/utils/config_parser.py
--rw-r--r--   0        0        0     6692 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0     1686 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/utils/log_config.py
--rw-r--r--   0        0        0    17900 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-21 19:59:49.349120 caikit-0.1.6/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0     3693 2023-04-21 19:59:49.353121 caikit-0.1.6/docs/adrs/README.md
--rw-r--r--   0        0        0      837 2023-04-21 19:59:49.353121 caikit-0.1.6/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1154 2023-04-21 19:59:53.021172 caikit-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-21 19:59:49.353121 caikit-0.1.6/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-21 19:59:49.353121 caikit-0.1.6/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/base.py
--rw-r--r--   0        0        0     8909 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    12691 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26013 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    13533 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     2909 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     3080 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_config.py
--rw-r--r--   0        0        0      521 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_imports.py
--rw-r--r--   0        0        0    18315 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17317 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_module.py
--rw-r--r--   0        0        0     4751 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8441 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0     1953 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_config_utils.py
--rw-r--r--   0        0        0    14999 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    15618 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/__init__.py
--rw-r--r--   0        0        0       27 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-21 19:59:49.353121 caikit-0.1.6/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      176 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1995 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2411 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1404 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2498 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      202 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/config.py
--rw-r--r--   0        0        0      141 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6439 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11774 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18079 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5053 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     7253 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3280 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18350 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1372 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7923 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    14808 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3533 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7386 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29936 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    10451 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     3785 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/utils/test_configs.py
--rw-r--r--   0        0        0     5041 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26086 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-21 19:59:49.357121 caikit-0.1.6/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1025 2023-04-21 19:59:49.357121 caikit-0.1.6/tox.ini
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-27 17:16:26.218927 caikit-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-04-27 17:16:26.218927 caikit-0.2.0/.gitignore
+-rw-r--r--   0        0        0      310 2023-04-27 17:16:26.218927 caikit-0.2.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-27 17:16:26.218927 caikit-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-27 17:16:26.218927 caikit-0.2.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-27 17:16:26.218927 caikit-0.2.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-27 17:16:26.218927 caikit-0.2.0/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-27 17:16:26.218927 caikit-0.2.0/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-27 17:16:26.218927 caikit-0.2.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      336 2023-04-27 17:16:26.218927 caikit-0.2.0/CODEOWNERS
+-rw-r--r--   0        0        0     7094 2023-04-27 17:16:26.218927 caikit-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-27 17:16:26.218927 caikit-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3757 2023-04-27 17:16:26.218927 caikit-0.2.0/README.md
+-rw-r--r--   0        0        0    44878 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     5392 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6140 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1770 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0      962 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29207 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13676 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20457 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    52621 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module.py
+-rw-r--r--   0        0        0     6735 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5500 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1001 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18059 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13923 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6047 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    20071 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5716 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12221 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10693 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10301 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4911 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     7655 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    11938 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    14711 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1579 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0     3693 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      837 2023-04-27 17:16:26.226928 caikit-0.2.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1154 2023-04-27 17:16:29.570632 caikit-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-27 17:16:26.226928 caikit-0.2.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-27 17:16:26.226928 caikit-0.2.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     4345 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8447 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11631 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    13533 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     2909 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    19262 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17485 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_module.py
+-rw-r--r--   0        0        0     5581 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8529 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    15068 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14580 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      498 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1847 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2283 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1276 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2370 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      141 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1687 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6402 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11607 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18018 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5373 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     1654 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     7253 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3280 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18336 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1372 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7923 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    14666 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    29994 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    10935 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1133 2023-04-27 17:16:26.234929 caikit-0.2.0/tox.ini
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.2.0/PKG-INFO
```

### Comparing `caikit-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.2.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.github/workflows/build-library.yml` & `caikit-0.2.0/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.github/workflows/lint-code.yml` & `caikit-0.2.0/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.github/workflows/publish-library.yml` & `caikit-0.2.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/.pylintrc` & `caikit-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/CODE-OF-CONDUCT.md` & `caikit-0.2.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/LICENSE` & `caikit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/README.md` & `caikit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit-overview.png` & `caikit-0.2.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/__init__.py` & `caikit-0.2.0/caikit/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,26 +24,16 @@
 # We're filtering (most) warnings for now
 import warnings as _warnings
 
 _warnings.filterwarnings("ignore")
 
 # Local
 # must import toolkit first since we need alog to be set up before it is used
-from . import (
-    blocks,
-    config,
-    data_model,
-    module,
-    module_config,
-    resources,
-    toolkit,
-    workflows,
-)
+from . import blocks, data_model, module, module_config, resources, toolkit, workflows
 from .blocks.base import BlockBase, block
-from .config import *
 from .data_model import dataobject
 from .model_manager import *
 from .module import *
 from .module_backend_config import configure as backend_configure
 from .module_backends import *
 from .module_config import ModuleConfig
 from .resources.base import ResourceBase, resource
```

### Comparing `caikit-0.1.6/caikit/core/augmentors/__init__.py` & `caikit-0.2.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/base.py` & `caikit-0.2.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.2.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.2.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/schemes/base.py` & `caikit-0.2.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.2.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.2.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/blocks/__init__.py` & `caikit-0.2.0/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/blocks/base.py` & `caikit-0.2.0/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/config/__init__.py` & `caikit-0.2.0/caikit/config/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Top-level configuration for the `caikit.core` library.  Mainly used for model management and
-version.
+"""Top-level configuration for the `caikit` library.
 """
 
-# Standard
-import os
-
 # Local
-from ..toolkit.errors import error_handler
-from .config import *
-
-lib_config = Config.get_config(
-    "caikit.core",
-    os.path.join(os.path.abspath(os.path.dirname(__file__)), "config.yml"),
-)
-
-# Update the global error configurations
-error_handler.ENABLE_ERROR_CHECKS = lib_config.enable_error_checks
-error_handler.MAX_EXCEPTION_LOG_MESSAGES = lib_config.max_exception_log_messages
+# Export public configuration functions
+from .config import configure, get_config
```

### Comparing `caikit-0.1.6/caikit/core/config/config.yml` & `caikit-0.2.0/caikit/core/resources/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,28 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-enable_error_checks: true
-max_exception_log_messages: 4
-load_path: null
 
-# Local is always enabled unless explicitly disabled
-disable_local_backend: False
+"""Resource Base. All implementations of resource types are imported here.
+"""
 
-backend_priority:
-    - LOCAL
-
-backends:
-    spark:
-        # These are aribtrary nested kwargs that will be passed to the
-        # backend-specific configuration file
-        foo: 1
-        bar: 2
-    ray:
-        baz: 3
-        bat:
-            buz:
-                biz: 5
+# Local
+from .base import ResourceSaver, resource
```

### Comparing `caikit-0.1.6/caikit/core/data_model/__init__.py` & `caikit-0.2.0/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/base.py` & `caikit-0.2.0/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.2.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/data_backends/base.py` & `caikit-0.2.0/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.2.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/dataobject.py` & `caikit-0.2.0/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/enums.py` & `caikit-0.2.0/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/producer.py` & `caikit-0.2.0/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.2.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/__init__.py` & `caikit-0.2.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/converter.py` & `caikit-0.2.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.2.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/data_stream.py` & `caikit-0.2.0/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/resolver.py` & `caikit-0.2.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/data_model/streams/validator.py` & `caikit-0.2.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/model_manager.py` & `caikit-0.2.0/caikit/core/model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 import zipfile
 
 # First Party
 import alog
 
 # Local
 from . import module_backend_config as backend_config
-from .config import lib_config
 from .module import (
     _MODULE_TYPES,
     MODULE_BACKEND_REGISTRY,
     MODULE_REGISTRY,
     SUPPORTED_LOAD_BACKENDS_VAR_NAME,
     ModuleBase,
     ModuleConfig,
 )
 from .module_backends import backend_types
 from .toolkit.errors import error_handler
+from caikit.config import get_config
 
 log = alog.use_channel("MDLMNG")
 error = error_handler.get(log)
 
 # restrict functions that are imported so we don't pollute the base module namespace
 __all__ = [
     "get_valid_module_ids",
@@ -91,15 +91,15 @@
         Returns:
             subclass of blocks.base.BlockBase
                 Model object that is loaded, configured, and ready for prediction.
         """
         error.type_check("<COR98255724E>", bool, load_singleton=load_singleton)
 
         # This allows a user to load their own model (e.g. model saved to disk)
-        load_path = lib_config.load_path
+        load_path = get_config().load_path
         if load_path is not None and isinstance(module_path, str):
             if not os.path.exists(module_path):
                 module_path = os.path.join(load_path, module_path)
 
         # Ensure that we have a loadable directory.
         error.type_check("<COR98255419E>", str, BytesIO, bytes, module_path=module_path)
         if isinstance(module_path, str):
@@ -255,15 +255,15 @@
                 )
                 loaded_artifact: ModuleBase = backend_impl.load(
                     module_path, *args, **kwargs
                 )
                 break
 
         # If model not able to load still, it is a model that probably
-        # does not define the "backed_type" or "supported_load_backends".
+        # does not define the "backend_type" or "supported_load_backends".
         # These would all be 'LOCAL' backend model, thus try to load with that
         if not loaded_artifact and local_enabled:
             module_class = MODULE_REGISTRY.get(module_id)
             loaded_artifact: ModuleBase = module_class.load(
                 module_path, *args, **kwargs
             )
```

### Comparing `caikit-0.1.6/caikit/core/module.py` & `caikit-0.2.0/caikit/core/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # broken out into another file (e.g. Python sub-modules)
 # pylint: disable=too-many-lines
 
 # abstract methods may define arguments but not use them
 # pylint: disable=unused-argument
 
 # Standard
+from importlib import metadata
 from io import BytesIO
 from typing import Any, Dict, List, Optional, Type, Union
 import collections
 import datetime
 import os
 import shutil
 import tempfile
@@ -46,14 +47,15 @@
 from .data_model import DataStream
 from .module_backends import backend_types
 from .module_config import ModuleConfig
 from .module_meta import _ModuleBaseMeta
 from .toolkit import ObjectSerializer, fileio
 from .toolkit.errors import DataValidationError, error_handler
 from .toolkit.wip_decorator import TempDisableWIP, WipCategory, work_in_progress
+from caikit.config import get_config
 
 log = alog.use_channel("MODULE")
 error = error_handler.get(log)
 
 # This file is `*` imported so we need to override what is exposed
 __all__ = [
     "_MODULE_TYPES",
@@ -773,31 +775,51 @@
     """
 
     SAVED_KEY_NAME = "saved"
     CREATED_KEY_NAME = "created"
     TRACKING_KEY_NAME = "tracking_id"
     MODULE_VERSION_KEY_NAME = "version"
 
-    def __init__(self, module: ModuleBase, model_path, library_name, library_version):
+    def __init__(self, module: ModuleBase, model_path):
         """Construct a new module saver.
 
         Args:
             module:  caikit.core.module.Module
                 The instance of the module to be saved.
             model_path:  str
                 The absolute path to the directory where the model will be saved.  If this directory
                 does not exist, it will be created.
-            library_name:  str
-                Name of library or extension calling the block saver.
-            library_version:  str
-                Version of library or extension calling the block saver.
         """
         self.model_path = os.path.normpath(model_path)
-        self.library_name = library_name
-        self.library_version = library_version
+
+        # Get possibly nested caikit library path
+        module_path = module.__module__
+        lib_name_generator = (
+            k
+            for k, v in get_config().libraries.items()
+            if module_path.startswith(v.module_path)
+        )
+        try:
+            self.library_name = next(lib_name_generator)
+        except StopIteration:
+            # This assumes no nested module path by default
+            self.library_name = module_path.split(".")[0]  # tests
+
+        try:
+            self.library_version = metadata.version(self.library_name)
+        except metadata.PackageNotFoundError:
+            log.debug("<COR25991305D>", "No library version found")
+            if (
+                self.library_name in get_config().libraries
+                and "version" in get_config().libraries[self.library_name]
+            ):
+                self.library_version = get_config().libraries[self.library_name].version
+            else:
+                self.library_version = "0.0.0"
+
         self.config = {
             self.library_name + "_version": self.library_version,
             self.CREATED_KEY_NAME: str(datetime.datetime.now()),
             self.SAVED_KEY_NAME: str(datetime.datetime.now()),
             "name": module.MODULE_NAME,
             self.TRACKING_KEY_NAME: str(uuid.uuid4()),
         }
```

### Comparing `caikit-0.1.6/caikit/core/module_backend_config.py` & `caikit-0.2.0/caikit/core/module_backend_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
-from typing import List, Optional
-import os
+from typing import List
 import threading
 
 # First Party
-# First party
-import aconfig
 import alog
 
 # Local
 from .module import MODULE_BACKEND_REGISTRY
 from .module_backends.backend_types import (
     MODULE_BACKEND_CONFIG_FUNCTIONS,
     MODULE_BACKEND_TYPES,
 )
 from .module_backends.base import BackendBase
-from .toolkit.config_utils import merge_configs
 from .toolkit.errors import error_handler
+from caikit.config import get_config
 
 log = alog.use_channel("CONF")
 error = error_handler.get(log)
 
 _CONFIGURED_BACKENDS = {}
 _BACKEND_START_LOCKS = {}
 
@@ -72,51 +69,36 @@
     """This function exposes the list of configured backends for downstream
     checks
     """
     # NOTE: Return a copy to avoid accidentally mutating the global
     return list(_CONFIGURED_BACKENDS.keys())
 
 
-def configure(*_, config_file: Optional[str] = None, **overrides):
-    """Configure the backend environment based on configuration available
-    in the given arguments.
+def configure():
+    """Configure the backend environment
 
     NOTE: This function is NOT thread safe!
-
-    KWargs:
-        config_file:  Optional[str]
-            Path to a configuration yaml file to use instead of the default
-        **overrides
-            overrides dict to apply on top of the loaded coniguration
     """
-    # Load the config file either from the default location or from the given
-    # path with environment overides
-    config_file = config_file or _DEFAULT_CONFIG_FILE
-    error.file_check("<COR37636675E>", config_file)
-
-    config_object = aconfig.Config.from_yaml(config_file, override_env_vars=True)
-
-    # Deep merge the given overrides on top of the the loaded config
-    config_object = merge_configs(config_object, overrides)
+    config_object = get_config().module_backends
 
     log.debug3("Full Config: %s", config_object)
 
     # Determine the priority list of enabled backends
     #
     # NOTE: All backends are held in UPPERCASE, but this is not canonical for
     #   yaml or function arguments, so we allow lowercase names in the config
     #   and coerce them to upper here
-    backend_priority = config_object.backend_priority or []
+    backend_priority = config_object.priority or []
     error.type_check("<COR46006487E>", list, backend_priority=backend_priority)
 
-    # Check if disable_local_backend is set
-    disable_local_backend = config_object.disable_local_backend or False
+    # Check if disable_local is set
+    disable_local_backend = config_object.disable_local or False
 
     # Add local at the end of priority by default
-    # TODO: Should we remove LOCAL if from priority it is disabled?
+    # TODO: Should we remove LOCAL from priority if it is disabled?
     if not disable_local_backend and (
         MODULE_BACKEND_TYPES.LOCAL not in backend_priority
     ):
         log.debug3("Adding fallback priority to [%s]", MODULE_BACKEND_TYPES.LOCAL)
         backend_priority.append(MODULE_BACKEND_TYPES.LOCAL)
     backend_priority = [backend.upper() for backend in backend_priority]
 
@@ -129,15 +111,15 @@
             i,
         )
     log.debug2("Backend Priority: %s", backend_priority)
 
     # Iterate through the config objects for each enabled backend in order and
     # do the actual config
     backend_configs = {
-        key.lower(): val for key, val in config_object.get("backends", {}).items()
+        key.lower(): val for key, val in config_object.get("configs", {}).items()
     }
     for backend in backend_priority:
         log.debug("Configuring backend [%s]", backend)
         backend_config = backend_configs.get(backend.lower(), {})
         log.debug3("Backend [%s] config: %s", backend, backend_config)
 
         if backend in configured_backends() and backend != MODULE_BACKEND_TYPES.LOCAL:
@@ -161,18 +143,14 @@
         _BACKEND_START_LOCKS[backend] = threading.Lock()
 
     log.debug2("All configured backends: %s", _CONFIGURED_BACKENDS)
 
 
 ## Implementation Details ######################################################
 
-_DEFAULT_CONFIG_FILE = os.path.realpath(
-    os.path.join(os.path.dirname(__file__), "config", "config.yml")
-)
-
 # The global map of configured backends
 _CONFIGURED_BACKENDS = {}
 
 
 # Thread-safe lock for each backend to ensure that starting is not performed
 # multiple times on any given backend
 _BACKEND_START_LOCKS = {}
```

### Comparing `caikit-0.1.6/caikit/core/module_backends/__init__.py` & `caikit-0.2.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/module_backends/backend_types.py` & `caikit-0.2.0/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/module_backends/base.py` & `caikit-0.2.0/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/module_backends/local_backend.py` & `caikit-0.2.0/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/module_config.py` & `caikit-0.2.0/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/module_meta.py` & `caikit-0.2.0/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/resources/__init__.py` & `caikit-0.2.0/tests/runtime/generated/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# Standard
+import os
+import sys
 
-
-"""Resource Base. All implementations of resource types are imported here.
-"""
-
-# Local
-from .base import ResourceSaver, resource
+# Allow generated _pb2 files in here to import each other
+script_loc = os.path.dirname(os.path.realpath(__file__))
+sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.1.6/caikit/core/resources/base.py` & `caikit-0.2.0/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/__init__.py` & `caikit-0.2.0/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/compatibility.py` & `caikit-0.2.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/errors/__init__.py` & `caikit-0.2.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.2.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,16 @@
 """
 
 # Standard
 from collections.abc import Iterable
 from types import GeneratorType
 import os
 
-# Global enablement switch for *_check functions. This will be set once the
-# library config has been fully parsed and can be overridden by the
-# `ENABLE_ERROR_CHECKS` environment variable
-ENABLE_ERROR_CHECKS = True
-
-# Maximum number of times that a single exception is logged. This will be set
-# once the library config has been fully parsed and can be overriden by the
-# `MAX_EXCEPTION_LOG_MESSAGES` environment variable
-MAX_EXCEPTION_LOG_MESSAGES = 4
+# Local
+from caikit.config import get_config
 
 # dictionary mapping string log channel name to error handler instances
 # there is only one error handler instance for each log channel name
 _error_handlers = {}
 
 
 def get(log_chan):
@@ -72,28 +65,34 @@
         """Handle number of exception log messages to avoid overflows"""
         # increment the log message counter attribute or add it if not present
         if hasattr(exception, "_caikit_core_nexception_log_messages"):
             exception._caikit_core_nexception_log_messages += 1
         else:
             exception._caikit_core_nexception_log_messages = 0
 
+        caikit_config = get_config()
+
         # if less than max log messages, then omit a log message
-        if exception._caikit_core_nexception_log_messages < MAX_EXCEPTION_LOG_MESSAGES:
+        if (
+            exception._caikit_core_nexception_log_messages
+            < caikit_config.max_exception_log_messages
+        ):
             self.log_chan.error(
                 log_code, "exception raised: {}".format(repr(exception))
             )
 
         # if at the limit omit one message stating that we will no longer log
         elif (
-            exception._caikit_core_nexception_log_messages == MAX_EXCEPTION_LOG_MESSAGES
+            exception._caikit_core_nexception_log_messages
+            == caikit_config.max_exception_log_messages
         ):
             self.log_chan.error(
                 log_code,
                 "reached MAX_EXCEPTION_LOG_MESSAGES of `{}`, will no log exception `{}`".format(
-                    MAX_EXCEPTION_LOG_MESSAGES, repr(exception)
+                    caikit_config.max_exception_log_messages, repr(exception)
                 ),
             )
 
     def log_raise(self, log_code, exception, root_exception=None):
         """Log an exception with a log code and then re-raise it.  Using this instead of simply
         using the `raise` keyword with your exceptions will ensure that log message is omitted on
         the `error` level for the log channel associated with this handler.  This is invaluable for
@@ -164,15 +163,15 @@
         Examples:
             # this will raise a `TypeError` because `foo` is not `None` or a `list` or `tuple`
             > error.type_check('<COR99962332E>', None, list, tuple, foo='hello world')
 
             # this type check verifies that `foo` and `bar` are both strings
             > error.type_check('<COR03761101E>', str, foo=foo, bar=bar)
         """
-        if not ENABLE_ERROR_CHECKS:
+        if not get_config().enable_error_checks:
             return
 
         if not types:
             self(log_code, RuntimeError("invalid type check: no types specified"))
 
         if not variables:
             self(log_code, RuntimeError("invalid type check: no variables specified"))
@@ -218,15 +217,15 @@
             # this type check fails because `bar` contains a `str`
             # but not for any other reason
             > foo = [1, 2, 3]
             > bar = [4, 5, 'x']
             > baz = None
             > error.type_check('<COR40818868E>', None, int, foo=foo, bar=bar, baz=None)
         """
-        if not ENABLE_ERROR_CHECKS:
+        if not get_config().enable_error_checks:
             return
 
         if not types:
             self(log_code, RuntimeError("invalid type check: no types specified"))
 
         if not variables:
             self(log_code, RuntimeError("invalid type check: no variables specified"))
@@ -298,15 +297,15 @@
                 string interpolation can be lazily performed on `msg` using `{}` format syntax by
                 passing additional arguments.  This is the preferred method for performing string
                 interpolation on `msg` so that it is only done if an error condition is encountered.
             *args:
                 Additional `{}`-style string formatting arguments to be lazily interpolated into
                 the `msg` argument.
         """
-        if not ENABLE_ERROR_CHECKS:
+        if not get_config().enable_error_checks:
             return
 
         if not condition:
             interpolated_msg = msg.format(*args)
             self(
                 log_code, ValueError("value check failed: {}".format(interpolated_msg))
             )
@@ -324,15 +323,15 @@
                 level short-code, one of `{'fatal': 'F', 'error': 'E', 'warning': 'W', 'info': 'I',
                 'trace': 'T', 'debug': 'D'}`.
             *file_paths:  str
                 Variadic argument containing strings specifying the file paths to check.  If any
                 of these file paths does not exist or is not a regular file, then a
                 log message will be omitted and a `FileNotFoundError` will be raised.
         """
-        if not ENABLE_ERROR_CHECKS:
+        if not get_config().enable_error_checks:
             return
 
         for file_path in file_paths:
             if not os.path.exists(file_path):
                 self(
                     log_code,
                     FileNotFoundError(
@@ -360,15 +359,15 @@
                 level short-code, one of `{'fatal': 'F', 'error': 'E', 'warning': 'W', 'info': 'I',
                 'trace': 'T', 'debug': 'D'}`.
             *dir_paths:  str
                 Variadic argument containing strings specifying the directory paths to check.  If
                 any of these file paths does not exist or is not a regular file, then a log message
                 will be omitted and a `FileNotFoundError` or `NotADirectoryError` will raised.
         """
-        if not ENABLE_ERROR_CHECKS:
+        if not get_config().enable_error_checks:
             return
 
         for dir_path in dir_paths:
             if not os.path.exists(dir_path):
                 self(
                     log_code,
                     FileNotFoundError(
```

### Comparing `caikit-0.1.6/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.2.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/fileio.py` & `caikit-0.2.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/isa.py` & `caikit-0.2.0/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.2.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/serializers.py` & `caikit-0.2.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/toolkit/wip_decorator.py` & `caikit-0.2.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/workflows/__init__.py` & `caikit-0.2.0/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/core/workflows/base.py` & `caikit-0.2.0/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/__init__.py` & `caikit-0.2.0/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/common/__init__.py` & `caikit-0.2.0/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.2.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/common/data_model/producer.py` & `caikit-0.2.0/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/runtime/__init__.py` & `caikit-0.2.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.2.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.2.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/__init__.py` & `caikit-0.2.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/config/config.yml` & `caikit-0.2.0/caikit/config/config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,170 @@
+# Copyright The Caikit Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 # User can set comma-separated string of config file locations to read
 config_files: ""
 
-# Configuration items for service generation:
-service_generation:
-    enabled: true
-    client_package_name: ""
-    module_types:
-        included: ["blocks", "workflows"]
-    module_guids:
-        included: []
-        excluded: []
-    primitive_data_model_types: []
-    task_types:
-        included: []
-        excluded: []
-
-use_abortable_threads: true
-
-metering:
-    # Switch off metering by default
-    enabled: false
-    # Directory to save metrics files
-    log_dir: "metering_logs"
-    # Write to log file every N seconds
-    log_interval: 3600
-
-local_models_dir: models
-
-# Model Mesh capacity in bytes for holding models (1024 ^ 3)
-capacity: 10737418240
-max_loading_concurrency: 2
-# Should be big enough to load any really chonky models
-model_loading_timeout_ms: 121000
-
-# Model Mesh's Default model size in bytes. This needs to be a
-# certain size, or else Model Mesh won't come up correctly (18 * 1024 ^ 2)
-default_model_size: 18874368
-default_model_size_multiplier: 10
-model_size_multipliers:
-    categories_esa: 2.95
-    concepts_alchemy: 13
-    entities_alchemy-disambig: 13.76
-    entity-mentions_bilstm: 1.44
-    entity-mentions_rbr: 1.8
-    sentiment_cnn: 2.73
-    syntax_izumo: 43000
-    fake_block: 2
-
-# Configuration for batch inference. This dict contains entries for individual
-# model types and can be extended using additional overlay config files to add
-# sections for model types beyond those listed here. Each section should contain
-# the `size` value where a 0 indicates no batching and may optionally contain a
-# `collect_delay_s` value as a float number of seconds >= 0. This will indicate
-# the amount of time the batch should wait for more requests before running a
-# partial batch.
-batching:
-    default:
-        size: 0
-        collect_delay_s: 0.0
-    fake_batch_block:
-        size: 10
+# Global config switch for runtime check functions (type_check, value_check, file_check...)
+enable_error_checks: true
+# Maximum number of times that a single exception is logged
+max_exception_log_messages: 4
+load_path: null
 
 # Configuration for loading alternate module implementations via
 # distributed backends
-distributed:
+module_backends:
     # Toggle distributed loading globally
     enabled: false
+    # Local is always enabled unless explicitly disabled
+    disable_local: false
     # Configuration overrides for distributed backends configuration.
     # Specific fields that may be of interest:
     #
-    # backend_priority: List of ordered string names for the order that backend
-    #   implementations should be used
-    # backends.<backend name>: Per-backend configuration blobs
-    config: {}
-
-numeric_runtime_version: 0
-# Whether or not model-mesh should respect MAX_MODEL_CONCURRENCY and scale out model loads appropriately
-latency_based_autoscaling_enabled: true
-# If latency based autoscaling is enabled, the default max in-flight requests per copy of each model
-max_model_concurrency: 2
-# ...which can also be set per-model-type
-max_model_concurrency_per_type:
-    keywords_text-rank: 8
-
-# Service exposure options
-service_port: 8085
-metrics_port: 8086
-find_available_port: false
-unix_socket_path: /tmp/mmesh/grpc.sock
-
-# Default level for all python loggers
-log_level: info
-# Alog filter customization [comma separated list of channels and the level to set them to]
-alog_filters: botocore:off,urllib3:off,matplotlib:off,boto3:off,jnius.reflect:off
-# Width of channels in ALOG when using the pretty formatter
-alog_channel_width: 12
-# if bool(int(ALOG_THREAD_ID)), then ALOG will also log information about thread IDs
-alog_thread_id: true
-# Which formatter to use. options are 'json' or 'pretty'
-alog_formatter: json
-
-# Number of workers with which we will run the gRPC server
-server_thread_pool_size: 5
-# The caikit* library (or libraries) whose models we want to serve using Caikit Runtime. This should
-# be a snake case string, e.g., caikit_nlp or caikit_cv.
-caikit_library: sample_lib
-service_proto_gen_module_dir: unused
+    # priority: List for the order that backend implementations should be used
+    priority:
+        - LOCAL
+    configs: {}
+
+log:
+    # Default level for all python loggers
+    level: info
+    # Alog filter customization [comma separated list of channels and the level to set them to]
+    filters: botocore:off,urllib3:off,matplotlib:off,boto3:off,jnius.reflect:off
+    # Width of channels in ALOG when using the pretty formatter
+    channel_width: 12
+    # if bool(int(ALOG_THREAD_ID)), then ALOG will also log information about thread IDs
+    thread_id: true
+    # Which formatter to use. options are 'json' or 'pretty'
+    formatter: json
 
 # Configuration for data streams and how they're handled in the server
 data_streams:
     # Base directory where stream source relative paths should be found
     file_source_base: null
 
-# Configuration for training
-training:
-    # The directory to save trained models in
-    output_dir: training_output
-    # Whether to automatically load the trained model
-    auto_load_trained_model: false
-    # Run training jobs in isolated processes
-    use_subprocess: false
-
-# gRPC Server shutdown grace period
-server_shutdown_grace_period_seconds: 45
-
-# Per-environment configurations
-environment: prod
-test:
-    find_available_port: true
-    runtime_version: mock
-    caikit_library: sample_lib
-    service_proto_gen_module_dir: tests.fixtures.protobufs
-    metering:
-        # Switch on metering by default
-        enabled: true
-        # Directory to save metrics files
-        log_dir: "test/metering_logs"
-        # Write to log file every N seconds
-        log_interval: 5
+### Runtime configurations
+runtime:
+    # The runtime library (or libraries) whose models we want to serve using Caikit Runtime. This should
+    # be a snake case string, e.g., caikit_nlp or caikit_cv.
+    library: sample_lib # TODO: replace with libraries below when runtime can support multiple libraries
+    local_models_dir: models
+
+    # TLS configs
+    tls:
+        server:
+            key: ""
+            cert: ""
+        client:
+            cert: ""
+
+    # Service exposure options
+    port: 8085
+    metrics:
+        port: 8086
+    find_available_port: false
+    unix_socket_path: /tmp/mmesh/grpc.sock
+
+    # Number of workers with which we will run the gRPC server
+    server_thread_pool_size: 5
+    use_abortable_threads: true
+    # gRPC Server shutdown grace period
+    server_shutdown_grace_period_seconds: 45
+
+    compiled_proto_module_dir: unused
+
+    # Configuration items for service generation
     service_generation:
-        client_package_name: ""
+        enabled: true
         module_types:
             included: ["blocks", "workflows"]
         module_guids:
             included: []
             excluded: []
-        primitive_data_model_types:
-            - "sample_lib.data_model.SampleInputType"
+        primitive_data_model_types: []
         task_types:
             included: []
             excluded: []
-    # training configs for tests
+
+    # Configuration for batch inference. This dict contains entries for individual
+    # model types and can be extended using additional overlay config files to add
+    # sections for model types beyond those listed here. Each section should contain
+    # the `size` value where a 0 indicates no batching and may optionally contain a
+    # `collect_delay_s` value as a float number of seconds >= 0. This will indicate
+    # the amount of time the batch should wait for more requests before running a
+    # partial batch.
+    batching:
+        default:
+            size: 0
+            collect_delay_s: 0.0
+        fake_batch_block:
+            size: 10
+
+    metering:
+        # Switch off metering by default
+        enabled: false
+        # Directory to save metrics files
+        log_dir: "metering_logs"
+        # Write to log file every N seconds
+        log_interval: 3600
+
+    # Training configuration for server
     training:
-        auto_load_trained_model: true
-        output_dir: test/training_output
-dev:
-    runtime_version: real_implementation
-prod:
-    runtime_version: real
-
-# TLS configs
-tls:
-    server:
-        key: ""
-        cert: ""
-    client:
-        cert: ""
+        # The directory to save trained models in
+        output_dir: training_output
+        # Whether to automatically load the trained model
+        auto_load_trained_model: false
+        # Run training jobs in isolated processes
+        use_subprocess: false
+
+inference_plugin:
+    model_mesh:
+        # Model Mesh specific versions
+        runtime_version: real
+        numeric_runtime_version: 0
+
+        # Model Mesh capacity in bytes for holding models (1024 ^ 3)
+        capacity: 10737418240
+        max_loading_concurrency: 2
+        # Should be big enough to load any really chonky models
+        model_loading_timeout_ms: 121000
+        # Whether or not model-mesh should respect MAX_MODEL_CONCURRENCY and scale out model loads appropriately
+        latency_based_autoscaling_enabled: true
+        # If latency based autoscaling is enabled, the default max in-flight requests per copy of each model
+        max_model_concurrency: 2
+        # ...which can also be set per-model-type
+        max_model_concurrency_per_type:
+            keywords_text-rank: 8
+
+        # Model Mesh's Default model size in bytes. This needs to be a
+        # certain size, or else Model Mesh won't come up correctly (18 * 1024 ^ 2)
+        default_model_size: 18874368
+        default_model_size_multiplier: 10
+        model_size_multipliers:
+            # NOTE: This won't work until https://github.com/caikit/caikit/issues/37 is addressed
+            categories_esa: 2.95
+            concepts_alchemy: 13
+            entities_alchemy-disambig: 13.76
+            entity-mentions_bilstm: 1.44
+            entity-mentions_rbr: 1.8
+            sentiment_cnn: 2.73
+            syntax_izumo: 43000
+            fake_block: 2
+
+### Libraries configuration
+libraries:
+    sample_lib:
+        # Version override for dev running
+        version: 1.2.3
+        # Module path override if nested
+        module_path: sample_lib
```

### Comparing `caikit-0.1.6/caikit/runtime/dump_services.py` & `caikit-0.2.0/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/grpc_server.py` & `caikit-0.2.0/caikit/runtime/grpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,28 @@
 
 # First Party
 import aconfig
 import alog
 
 # Local
 # Get the injectable servicer class definitions
+from caikit import get_config
 from caikit.runtime.interceptors.caikit_runtime_server_wrapper import (
     CaikitRuntimeServerWrapper,
 )
 from caikit.runtime.protobufs import model_runtime_pb2_grpc, process_pb2_grpc
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.servicers.model_runtime_servicer import ModelRuntimeServicerImpl
 from caikit.runtime.servicers.model_train_servicer import ModelTrainServicerImpl
 from caikit.runtime.servicers.training_management_servicer import (
     TrainingManagementServicerImpl,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
-from caikit.runtime.utils.log_config import initialize_logging
 
 # Have pylint ignore broad exception catching in this file so that we can log all
 # unexpected errors using alog.
 # pylint: disable=W0703
 import caikit.core.data_model
 
 log = alog.use_channel("GRPC-SERVR")
@@ -62,32 +61,34 @@
     def __init__(
         self,
         infer_srv: ServicePackage,
         train_srv: Optional[ServicePackage],
         tls_config_override: aconfig.Config = None,
         hndle_terms: bool = False,
     ):
-        self.config = ConfigParser.get_instance()
+        self.config = get_config()
         self.inference_service = infer_srv
         self.training_service = train_srv
 
         self.port = (
-            self._find_port(self.config.service_port)
-            if self.config.find_available_port
-            else self.config.service_port
+            self._find_port(self.config.runtime.port)
+            if self.config.runtime.find_available_port
+            else self.config.runtime.port
         )
-        if self.port != self.config.service_port:
+        if self.port != self.config.runtime.port:
             log.warning(
-                "Port %s was in use, had to find another!", self.config.service_port
+                "Port %s was in use, had to find another!", self.config.runtime.port
             )
 
         # Initialize basic server
         # py_grpc_prometheus.server_metrics.
         self.server = grpc.server(
-            futures.ThreadPoolExecutor(max_workers=self.config.server_thread_pool_size),
+            futures.ThreadPoolExecutor(
+                max_workers=self.config.runtime.server_thread_pool_size
+            ),
             interceptors=(PROMETHEUS_METRICS_INTERCEPTOR,),
         )
 
         # Intercept an Inference Service
         self._global_predict_servicer = GlobalPredictServicer(self.inference_service)
         self.server = CaikitRuntimeServerWrapper(
             server=self.server,
@@ -144,30 +145,32 @@
             experimental_non_blocking=True,
             experimental_thread_pool=futures.ThreadPoolExecutor(max_workers=1),
         )
         health_pb2_grpc.add_HealthServicer_to_server(health_srvcer, self.server)
 
         # Listen on a unix socket as well for model mesh.
         try:
-            self.server.add_insecure_port(f"unix://{self.config.unix_socket_path}")
+            self.server.add_insecure_port(
+                f"unix://{self.config.runtime.unix_socket_path}"
+            )
             log.info(
                 "<RUN10001011I>",
                 "Caikit Runtime is communicating through address: unix://%s",
-                self.config.unix_socket_path,
+                self.config.runtime.unix_socket_path,
             )
         except RuntimeError:
             log.info(
                 "<RUN10001100I>",
                 "Binding failed for: unix://%s",
-                self.config.unix_socket_path,
+                self.config.runtime.unix_socket_path,
             )
 
         # Pull TLS config from app config, unless an explicit override was passed
         self.tls_config = (
-            tls_config_override if tls_config_override else self.config.tls
+            tls_config_override if tls_config_override else self.config.runtime.tls
         )
 
         if (
             self.tls_config
             and self.tls_config.server.key
             and self.tls_config.server.cert
         ):
@@ -211,15 +214,15 @@
         # Start the server. This is non-blocking, so we need to wait after
         self.server.start()
 
         log.info(
             "<RUN10001001I>",
             "Caikit Runtime is serving on port: %s with thread pool size: %s",
             self.port,
-            self.config.server_thread_pool_size,
+            self.config.runtime.server_thread_pool_size,
         )
 
         if blocking:
             self.server.wait_for_termination(None)
 
     def interrupt(self, signal_):
         """Interrupt the server. Implements the interface for Python signal.signal
@@ -237,18 +240,20 @@
         """Stop the server, with an optional grace period.
 
         Args:
             grace_period_seconds (Union[float, int]): Grace period for service shutdown.
                 Defaults to application config
         """
         if not grace_period_seconds:
-            grace_period_seconds = self.config.server_shutdown_grace_period_seconds
+            grace_period_seconds = (
+                self.config.runtime.server_shutdown_grace_period_seconds
+            )
         self.server.stop(grace_period_seconds)
         # Ensure we flush out any remaining billing metrics and stop metering
-        if self.config.metering.enabled:
+        if self.config.runtime.metering.enabled:
             self._global_predict_servicer.rpc_meter.flush_metrics()
             self._global_predict_servicer.rpc_meter.end_writer_thread()
 
     def render_protos(self, proto_out_dir: str) -> None:
         """Renders all the necessary protos for this service into a directory
         Args:
             proto_out_dir (str): Path to the directory to write proto files to
@@ -313,28 +318,28 @@
     if os.path.exists(secret):
         with open(secret, "r", encoding="utf-8") as secret_file:
             return secret_file.read()
     return secret
 
 
 def main():
-    # Configure using the log level and formatter type specified in configparser.
-    config_parser = ConfigParser.get_instance()
-    initialize_logging()
+    # Configure using the log level and formatter type specified in config.
+    caikit.core.toolkit.logging.configure()
 
     # Start serving Prometheus metrics
-    start_http_server(config_parser.metrics_port)
+    caikit_config = get_config()
+    start_http_server(caikit_config.runtime.metrics.port)
 
     # Enable signal handling
     handle_terminations = True
 
     # Assume we want compiled services for now
     service_source = (
         ServicePackageFactory.ServiceSource.GENERATED
-        if config_parser.service_generation.enabled
+        if caikit_config.runtime.service_generation.enabled
         else ServicePackageFactory.ServiceSource.COMPILED
     )
     log.debug("Running with service source: %s", service_source)
 
     # We should always be able to stand up an inference service
     inference_service: ServicePackage = ServicePackageFactory.get_service_package(
         ServicePackageFactory.ServiceType.INFERENCE,
```

### Comparing `caikit-0.1.6/caikit/runtime/interceptors/__init__.py` & `caikit-0.2.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.2.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/metrics/__init__.py` & `caikit-0.2.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.2.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import uuid
 
 # First Party
 import alog
 
 # Local
-from caikit.runtime.utils.config_parser import ConfigParser
+from caikit import get_config
 
 log = alog.use_channel("RPC_METER")
 
 
 # pylint: disable=too-many-instance-attributes
 class RPCMeter:
     """This class contains metering logic for RPC calls affiliated with the Caikit Runtime that are
@@ -25,15 +25,15 @@
         """Initialize a RPCMeter instance and start the log writer thread."""
 
         self.predict_rpc_counter = []
         self.logs_writer_thread = threading.Thread(target=self.write_metrics)
         self.metering_event = threading.Event()
         self.rpc_counter_lock = threading.Lock()
         self.write_file_lock = threading.Lock()
-        self.metrics_dir = ConfigParser.get_instance().metering.log_dir
+        self.metrics_dir = get_config().runtime.metering.log_dir
         self.unique_id = str(uuid.uuid4()).replace("-", "_")
         self.file_path = os.path.join(
             self.metrics_dir,
             "predict_rpc_metrics_{}.json".format(self.unique_id),
         )
         if not os.path.exists(self.metrics_dir):
             os.makedirs(self.metrics_dir)
@@ -77,15 +77,15 @@
             log.debug(
                 "<RUN76774002I>",
                 "Metering log file writing to %s",
                 self.file_path,
             )
             self._write_metrics()
             notified = self.metering_event.wait(
-                ConfigParser.get_instance().metering.log_interval
+                get_config().runtime.metering.log_interval
             )
             if notified:
                 log.debug("<RUN76774003I>", "Shutting down metering writer log thread")
                 break
 
     def _write_metrics(self):
         """Writes all metrics to directory specified in config and resets counters"""
```

### Comparing `caikit-0.1.6/caikit/runtime/metrics/throughput.py` & `caikit-0.2.0/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/model_management/__init__.py` & `caikit-0.2.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/model_management/batcher.py` & `caikit-0.2.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/model_management/loaded_model.py` & `caikit-0.2.0/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/model_management/model_loader.py` & `caikit-0.2.0/caikit/runtime/model_management/model_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 from grpc import StatusCode
 from prometheus_client import Summary
 
 # First Party
 import alog
 
 # Local
+from caikit.config import get_config
 from caikit.core import MODEL_MANAGER
 from caikit.core.module_backend_config import configure
 from caikit.runtime.model_management.batcher import Batcher
 from caikit.runtime.model_management.loaded_model import LoadedModel
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 import caikit.core
 
 log = alog.use_channel("MODEL-LOADER")
 
 CAIKIT_CORE_LOAD_DURATION_SUMMARY = Summary(
     "caikit_core_load_model_duration_seconds",
     "Summary of the duration (in seconds) of caikit.core.load(model)",
@@ -45,21 +45,22 @@
 
     __instance = None
 
     def __init__(self):
         # Re-instantiating this is a programming error
         assert self.__class__.__instance is None, "This class is a singleton!"
         ModelLoader.__instance = self
-        self.config_parser = ConfigParser.get_instance()
+        # We will call get_config() each time in case there are updates since this
+        # class is a singleton
 
-        # If distributed loading is enabled, set up the loader
-        if self.config_parser.distributed.enabled:
-            log.info("<RUN89711118I>", "Configuring for distributed loading")
-            log.debug("Distributed config: %s", self.config_parser.distributed.config)
-            configure(**self.config_parser.distributed.config)
+        # If backends loading is enabled, set up the loader
+        if get_config().module_backends.enabled:
+            log.info("<RUN89711118I>", "Configuring for backends loading")
+            log.debug("Backends config: %s", get_config().module_backends)
+            configure()
 
     def load_model(self, model_id, local_model_path, model_type) -> LoadedModel:
         """Load a model using model_path (in Cloud Object Storage) & give it a model ID.
         This always cleans up files on disk, no matter if the load succeeds or fails
 
         Args:
             model_id (string):  Model ID string for the model to load.
@@ -139,17 +140,17 @@
         caikit_core_model: caikit.core.ModuleBase,
         model_type: str,
         model_id: str,
     ) -> Union[Batcher, caikit.core.ModuleBase]:
         """Perform Batcher wrapping on the given module if configured, otherwise
         return the model as is
         """
-        batch_config = self.config_parser.batching.get(
+        batch_config = get_config().runtime.batching.get(
             model_type,
-            self.config_parser.batching.get("default", {}),
+            get_config().runtime.batching.get("default", {}),
         )
         log.debug2("Batch config for model type [%s]: %s", model_type, batch_config)
         batch_size = batch_config.get("size", 0)
         if batch_size > 0:
             log.info(
                 "<RUN89713768I>",
                 "Enabling batch size [%s] for [%s] of type [%s]",
```

### Comparing `caikit-0.1.6/caikit/runtime/model_management/model_manager.py` & `caikit-0.2.0/caikit/runtime/model_management/model_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 from grpc import StatusCode
 from prometheus_client import Counter, Gauge, Summary
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.core import ModuleBase
 from caikit.runtime.model_management.loaded_model import LoadedModel
 from caikit.runtime.model_management.model_loader import ModelLoader
 from caikit.runtime.model_management.model_sizer import ModelSizer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 
 log = alog.use_channel("MODEL-MANAGR")
 
 MODEL_SIZE_GAUGE = Gauge(
     "total_loaded_models_size",
     "Total size of loaded models reported to model-mesh",
     ["model_type"],
@@ -76,15 +76,15 @@
         # And a ModelSizer
         self.model_sizer = ModelSizer.get_instance()
 
         # set up the local map for model ID to loaded model
         self.loaded_models: Dict[str, LoadedModel] = {}
 
         # Optionally load models mounted into a local directory
-        local_models_path = ConfigParser.get_instance().local_models_dir
+        local_models_path = get_config().runtime.local_models_dir
         if os.path.exists(local_models_path) and len(os.listdir(local_models_path)) > 0:
             log.info("<RUN44739400I>", "Loading local models into Caikit Runtime...")
             self.load_local_models(local_models_path)
 
     def load_model(self, model_id, local_model_path, model_type) -> int:
         """Load a model using model_path (in Cloud Object Storage) & give it a model ID
         Args:
```

### Comparing `caikit-0.1.6/caikit/runtime/model_management/model_sizer.py` & `caikit-0.2.0/caikit/runtime/model_management/model_sizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,31 +20,30 @@
 # Third Party
 import grpc
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 
 log = alog.use_channel("MODEL-SIZER")
 
 
 class ModelSizer:
     """Model Loader class. The singleton class contains the core implementation details
     for loading models in from S3."""
 
     __instance = None
 
     def __init__(self):
         # Re-instantiating this is a programming error
         assert self.__class__.__instance is None, "This class is a singleton!"
         ModelSizer.__instance = self
-        self.config_parser = ConfigParser.get_instance()
 
         # Cache of archive sizes: cos model path -> archive size in bytes
         self._model_archive_sizes: Dict[str, int] = {}
 
     def get_model_size(self, model_id, local_model_path, model_type) -> int:
         """
         Returns the estimated memory footprint of a model
@@ -63,23 +62,32 @@
             )
 
         return self.__estimate_with_multiplier(
             model_id, model_type, self._model_archive_sizes[local_model_path]
         )
 
     def __estimate_with_multiplier(self, model_id, model_type, archive_size) -> int:
-        if model_type in self.config_parser.model_size_multipliers:
-            multiplier = self.config_parser.model_size_multipliers[model_type]
+        if (
+            model_type
+            in get_config().inference_plugin.model_mesh.model_size_multipliers
+        ):
+            multiplier = (
+                get_config().inference_plugin.model_mesh.model_size_multipliers[
+                    model_type
+                ]
+            )
             log.debug(
                 "Using size multiplier '%f' for model '%s' to estimate model size",
                 multiplier,
                 model_id,
             )
         else:
-            multiplier = self.config_parser.default_model_size_multiplier
+            multiplier = (
+                get_config().inference_plugin.model_mesh.default_model_size_multiplier
+            )
             log.info(
                 "<RUN62161564I>",
                 "No configured model size multiplier found for model type '%s' for model '%s'. "
                 "Using default multiplier '%f'",
                 model_type,
                 model_id,
                 multiplier,
```

### Comparing `caikit-0.1.6/caikit/runtime/model_management/training_manager.py` & `caikit-0.2.0/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/__init__.py` & `caikit-0.2.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.2.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.2.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.2.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.2.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.2.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_factory.py` & `caikit-0.2.0/caikit/runtime/service_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 # First Party
 from jtd_to_proto.json_to_service import (
     json_to_service,
     service_descriptor_to_client_stub,
     service_descriptor_to_server_registration_function,
     service_descriptor_to_service,
 )
+import aconfig
 import alog
 
 # Local
+from caikit import get_config
 from caikit.core import dataobject
 from caikit.core.data_model.base import DataBase
 from caikit.core.module import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
@@ -45,15 +47,14 @@
 from caikit.runtime.service_generation.core_module_helpers import get_module_info
 from caikit.runtime.service_generation.serializers import (
     RPCSerializerBase,
     snake_to_upper_camel,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils import import_util
-from caikit.runtime.utils.config_parser import ConfigParser
 import caikit.core
 
 log = alog.use_channel("SVC-FACTORY")
 
 TRAINING_MANAGEMENT_SERVICE_NAME = "TrainingManagement"
 TRAINING_MANAGEMENT_SERVICE_SPEC = {
     "service": {
@@ -122,32 +123,32 @@
         if source == cls.ServiceSource.COMPILED:
             # Use our import_utils to extract the correct bits out of a set of compiled pb2
             # packages
             lib_name = cls._get_lib_name_for_servicer()
 
             if service_type == cls.ServiceType.INFERENCE:
                 # 🌶️🌶️🌶️! hardcoded service names
-                compiled_pb2_package = cls._get_service_proto_module(
+                compiled_pb2_package = cls._get_compiled_proto_module(
                     "caikit_runtime_pb2"
                 )
-                compiled_pb2_grpc_package = cls._get_service_proto_module(
+                compiled_pb2_grpc_package = cls._get_compiled_proto_module(
                     "caikit_runtime_pb2_grpc"
                 )
             elif service_type == cls.ServiceType.TRAINING_MANAGEMENT:
                 raise CaikitRuntimeException(
                     grpc.StatusCode.INTERNAL,
                     "Not allowed to get Training Management services from compiled packages",
                 )
             else:  # elif  service_type == cls.ServiceType.TRAINING:
                 # (using final _else_ for static analysis happiness)
                 # 🌶️🌶️🌶️! hardcoded service names
-                compiled_pb2_package = cls._get_service_proto_module(
+                compiled_pb2_package = cls._get_compiled_proto_module(
                     "caikit_runtime_train_pb2"
                 )
-                compiled_pb2_grpc_package = cls._get_service_proto_module(
+                compiled_pb2_grpc_package = cls._get_compiled_proto_module(
                     "caikit_runtime_train_pb2_grpc"
                 )
 
             # Dynamically create a new module to hold all the service's messages
             client_module = ModuleType(
                 "ClientMessages", "Package with service message class implementations"
             )
@@ -185,22 +186,22 @@
             )
 
         if source == cls.ServiceSource.GENERATED:
             # First make sure we import the data model for the correct library
             # !!!! This will use the `caikit_library` config
             _ = import_util.get_data_model()
 
-            config_parser = ConfigParser.get_instance()
-            lib = config_parser.caikit_library
+            caikit_config = get_config()
+            lib = caikit_config.runtime.library
             ai_domain_name = snake_to_upper_camel(lib.replace("caikit_", ""))
             package_name = f"caikit.runtime.{ai_domain_name}"
 
             # Then do API introspection to come up with all the API definitions to support
             clean_modules = ServicePackageFactory._get_and_filter_modules(
-                config_parser, lib
+                caikit_config, lib
             )
 
             if service_type == cls.ServiceType.INFERENCE:
                 task_rpc_list = service_generation.create_inference_rpcs(clean_modules)
                 service_name = f"{ai_domain_name}Service"
             else:  # service_type == cls.ServiceType.TRAINING
                 task_rpc_list = service_generation.create_training_rpcs(clean_modules)
@@ -242,46 +243,46 @@
                 stub_class=service_descriptor_to_client_stub(service_descriptor),
                 messages=client_module,
             )
 
     # Implementation details for pure python service packages #
     @staticmethod
     def _get_and_filter_modules(
-        config_parser: ConfigParser, lib: str
+        caikit_config: aconfig.Config, lib: str
     ) -> Set[Type[ModuleBase]]:
         clean_modules = set()
         modules = [
             module_class
             for module_class in caikit.core.MODULE_REGISTRY.values()
             if module_class.__module__.partition(".")[0] == lib
         ]
         log.debug("Found all modules %s for library %s.", modules, lib)
 
         # Check config for any explicit inclusions
         included_task_types = (
-            config_parser.service_generation
-            and config_parser.service_generation.task_types
-            and config_parser.service_generation.task_types.included
+            caikit_config.runtime.service_generation
+            and caikit_config.runtime.service_generation.task_types
+            and caikit_config.runtime.service_generation.task_types.included
         )
         included_modules = (
-            config_parser.service_generation
-            and config_parser.service_generation.module_guids
-            and config_parser.service_generation.module_guids.included
+            caikit_config.runtime.service_generation
+            and caikit_config.runtime.service_generation.module_guids
+            and caikit_config.runtime.service_generation.module_guids.included
         )
 
         # Check config for any exclusions
         excluded_task_types = (
-            config_parser.service_generation
-            and config_parser.service_generation.task_types
-            and config_parser.service_generation.task_types.excluded
+            caikit_config.runtime.service_generation
+            and caikit_config.runtime.service_generation.task_types
+            and caikit_config.runtime.service_generation.task_types.excluded
         )
         excluded_modules = (
-            config_parser.service_generation
-            and config_parser.service_generation.module_guids
-            and config_parser.service_generation.module_guids.excluded
+            caikit_config.runtime.service_generation
+            and caikit_config.runtime.service_generation.module_guids
+            and caikit_config.runtime.service_generation.module_guids.excluded
         )
 
         for ck_module in modules:
             # Only create for modules from defined included and exclusion list
             module_info = get_module_info(ck_module)
             if excluded_task_types and module_info.type in excluded_task_types:
                 log.debug("Skipping module %s of type %s", ck_module, module_info.type)
@@ -453,43 +454,42 @@
             grpc.StatusCode.INTERNAL,
             "Could not find servicer stub in caikit_runtime_pb2_grpc",
         )
 
     @staticmethod
     def _get_lib_name_for_servicer() -> str:
         """Get caikit library name from Config, make upper case and not include caikit_"""
-        config_parser = ConfigParser.get_instance()
-        lib_names = import_util.clean_lib_names(config_parser.caikit_library)
+        lib_names = import_util.clean_lib_names(get_config().runtime.library)
         assert len(lib_names) == 1, "Only 1 caikit library supported for now"
         return ServicePackageFactory._snake_to_upper_camel(
             lib_names[0].replace("caikit_", "")
         )
 
     @staticmethod
-    def _get_service_proto_module(
+    def _get_compiled_proto_module(
         module: str,
-        config: ConfigParser = None,
+        config=None,
     ) -> ModuleType:
         """
-        Dynamically import the service module. This is accomplished via dynamic
-        import on the SERVICE_PROTO_GEN_MODULE_DIR's environment variable.
+        Dynamically import the compiled service module. This is accomplished via dynamic
+        import on the RUNTIME_COMPILED_PROTO_MODULE_DIR's environment variable.
 
         Args:
-            config(ConfigParser): Config parser instance
+            config(aconfig.Config): caikit configuration
 
         Returns:
             (module): Handle to the module after dynamic import
         """
         if not config:
-            config = ConfigParser.get_instance()
-        module_dir = config.service_proto_gen_module_dir
+            config = get_config()
+        module_dir = config.runtime.compiled_proto_module_dir
         service_proto_gen_module = import_util.get_dynamic_module(module, module_dir)
         if service_proto_gen_module is None:
             message = (
-                "Unable to load service proto gen module: %s within dir %s"
+                "Unable to load compiled proto module: %s within dir %s"
                 % (module)
                 % (module_dir)
             )
             log.error("<RUN22291313E>", message)
             raise CaikitRuntimeException(grpc.StatusCode.INTERNAL, message)
         return service_proto_gen_module
```

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.2.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.2.0/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/create_service.py` & `caikit-0.2.0/caikit/runtime/service_generation/create_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 from enum import Enum
 from typing import List, Type
 
 # First Party
 import alog
 
 # Local
+from ... import get_config
 from .core_module_helpers import get_module_info
 from .primitives import is_primitive_method
 from .serializers import ModuleClassTrainRPC, RPCSerializerBase, TaskPredictRPC
 from .signature_parsing.module_signature import CaikitCoreModuleMethodSignature
 from caikit.core.module import ModuleBase
-from caikit.runtime.utils.config_parser import ConfigParser
 
 log = alog.use_channel("CREATE-RPCS")
 
 ## Globals #####################################################################
 
 INFERENCE_FUNCTION_NAME = "run"
 TRAIN_FUNCTION_NAME = "train"
@@ -46,15 +46,15 @@
     TRAINING = 2
 
 
 def create_inference_rpcs(modules: List[Type[ModuleBase]]) -> List[RPCSerializerBase]:
     """Handles the logic to create all the RPCs for inference"""
 
     primitive_data_model_types = (
-        ConfigParser.get_instance().service_generation.primitive_data_model_types
+        get_config().runtime.service_generation.primitive_data_model_types
     )
 
     rpcs = []
     # Inference specific logic:
     primitive_modules = _remove_non_primitive_modules(
         modules, primitive_data_model_types
     )
@@ -71,15 +71,15 @@
 
 def create_training_rpcs(modules: List[Type[ModuleBase]]) -> List[RPCSerializerBase]:
     """Handles the logic to create all the RPCs for training"""
 
     rpcs = []
 
     primitive_data_model_types = (
-        ConfigParser.get_instance().service_generation.primitive_data_model_types
+        get_config().runtime.service_generation.primitive_data_model_types
     )
 
     for ck_module in modules:
         # If this train function has not been changed from the base, skip it as
         # a module that can't be trained
         #
         # HACK alert! I'm struggling to find the right way to identify this
```

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.2.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 # Local
 from caikit.core.data_model import dataobject
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.dataobject import _NATIVE_TYPE_TO_JTD
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 import caikit
 
 # This global holds the mapping of element types to their respective
 # DataStreamSource wrappers so that the same message is not recreated
 # unnecessarily
 _DATA_STREAM_SOURCE_TYPES = {}
 
@@ -185,15 +184,15 @@
             return cls.ELEMENT_TYPE.from_json(raw_element)
         return raw_element
 
     @staticmethod
     def _get_resolved_source_path(input_path: str) -> str:
         """Get a fully resolved path, including any shared prefix"""
         # Get any configured prefix
-        source_pfx = ConfigParser.get_instance().data_streams.file_source_base
+        source_pfx = caikit.get_config().data_streams.file_source_base
         # If a prefix is configured, use it, otherwise return the path as is
         # NOTE: os.path.join will ignore the prefix if input_path is absolute
         return os.path.join(source_pfx, input_path) if source_pfx else input_path
 
 
 def make_data_stream_source(data_element_type: Type) -> Type[DataBase]:
     """Dynamically create a data stream source message type that supports
```

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/primitives.py` & `caikit-0.2.0/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/serializers.py` & `caikit-0.2.0/caikit/runtime/service_generation/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.2.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/servicers/__init__.py` & `caikit-0.2.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.2.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 from prometheus_client import Counter, Summary
 import grpc
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.core import ModuleBase
 from caikit.runtime.metrics.rpc_meter import RPCMeter
 from caikit.runtime.metrics.throughput import Throughput
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 from caikit.runtime.utils.import_util import clean_lib_names
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     build_proto_response,
     get_metadata,
     validate_data_model,
 )
@@ -94,18 +94,18 @@
 
     # Input size in code points, provided by orchestrator
     INPUT_SIZE_KEY = "input-length"
 
     def __init__(
         self,
         inference_service: ServicePackage,
-        use_abortable_threads: bool = ConfigParser.get_instance().use_abortable_threads,
+        use_abortable_threads: bool = get_config().runtime.use_abortable_threads,
     ):
         self._model_manager = ModelManager.get_instance()
-        if ConfigParser.get_instance().metering.enabled:
+        if get_config().runtime.metering.enabled:
             self.rpc_meter = RPCMeter()
             log.info(
                 "<RUN76773775I>",
                 "Metering is enabled, to disable set `metering.enabled` in config to false",
             )
         else:
             log.info(
@@ -117,17 +117,17 @@
         self._inference_service = inference_service
         # Validate that the Caikit Library CDM is compatible with our service descriptor
         validate_data_model(self._inference_service.descriptor)
         log.info("<RUN76773778I>", "Validated Caikit Library CDM successfully")
 
         # Duplicate code in global_train_servicer
         # pylint: disable=duplicate-code
-        library = clean_lib_names(ConfigParser.get_instance().caikit_library)[0]
+        library = clean_lib_names(get_config().runtime.library)[0]
         try:
-            lib_version = version(self.library)
+            lib_version = version(library)
         except Exception:  # pylint: disable=broad-exception-caught
             lib_version = "unknown"
 
         log.info(
             "<RUN76884779I>",
             "Constructed inference service for library: %s, version: %s",
             library,
@@ -198,15 +198,15 @@
                 ).time():
                     response_proto = build_proto_response(response)
 
             # Update Prometheus metrics
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=desc_name, code=StatusCode.OK.name, model_id=model_id
             ).inc()
-            if ConfigParser.get_instance().metering.enabled:
+            if get_config().runtime.metering.enabled:
                 self.rpc_meter.update_metrics(str(type(model)))
             return response_proto
 
         except CaikitRuntimeException as e:
             log_dict = {
                 "log_code": "<RUN50530380W>",
                 "message": e.message,
```

### Comparing `caikit-0.1.6/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.2.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 from grpc import StatusCode
 import grpc
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.core.module import ModuleBase
 from caikit.interfaces.runtime.data_model import TrainingJob
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.model_management.training_manager import TrainingManager
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 from caikit.runtime.utils.import_util import clean_lib_names, get_data_model
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     snake_to_upper_camel,
     validate_data_model,
 )
 import caikit.core
@@ -61,29 +61,33 @@
     def __init__(self, training_service: ServicePackage):
         self._training_service = training_service
         self._model_manager = ModelManager.get_instance()
         self.training_manager = TrainingManager.get_instance()
         self.executor = concurrent.futures.ThreadPoolExecutor()
         # store the map of model ids to job ids
         self.training_map = self.training_manager.training_futures
-        cfg = ConfigParser.get_instance()
-        self.training_output_dir = cfg.training.output_dir
-        self.auto_load_trained_model = cfg.training.auto_load_trained_model
-        self.use_subprocess = cfg.training.use_subprocess
+        caikit_config = get_config()
+        self.training_output_dir = caikit_config.runtime.training.output_dir
+        self.auto_load_trained_model = (
+            caikit_config.runtime.training.auto_load_trained_model
+        )
+        self.use_subprocess = caikit_config.runtime.training.use_subprocess
 
         # TODO: think about if we really want to do this here:
         self.cdm = get_data_model()
 
         # Validate that the Caikit Library CDM is compatible with our service descriptor
         validate_data_model(self._training_service.descriptor)
         log.info("<RUN76773777I>", "Validated Caikit Library CDM successfully")
 
+        # TODO: support multiple libs? `caikit_config.libraries` dict
+        # Or grab the `libraries` off of the `training_service` instead of config here?
         # Duplicate code in global_train_servicer
         # pylint: disable=duplicate-code
-        self.library = clean_lib_names(ConfigParser.get_instance().caikit_library)[0]
+        self.library = clean_lib_names(caikit_config.runtime.library)[0]
         try:
             lib_version = version(self.library)
         except Exception:  # pylint: disable=broad-exception-caught
             lib_version = "unknown"
 
         log.info(
             "<RUN76884779I>",
```

### Comparing `caikit-0.1.6/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.2.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,31 +15,30 @@
 # Have pylint ignore Class XXXX has no YYYY member so that we can use gRPC enums.
 # pylint: disable=E1101
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.protobufs import model_runtime_pb2, model_runtime_pb2_grpc
 from caikit.runtime.types.aborted_exception import AbortedException
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 from caikit.runtime.work_management.abortable_action import AbortableAction
 from caikit.runtime.work_management.call_aborter import CallAborter
 
 log = alog.use_channel("MR-SERVICR-I")
 
 
 class ModelRuntimeServicerImpl(model_runtime_pb2_grpc.ModelRuntimeServicer):
     """This class contains the implementation of all of the RPCs that are required to run a
     service in Model Mesh as a Model-Runtime."""
 
     def __init__(self):
-        self.config_parser = ConfigParser.get_instance()
         self.model_manager = ModelManager.get_instance()
 
     def loadModel(self, request, context):
         """Model loading .
         Args:
             request(model_runtime_pb2.LoadModelRequest):
                 gRPC request, gen from model-runtime.proto
@@ -52,16 +51,16 @@
             log.info(
                 {
                     "log_code": "<RUN10000106I>",
                     "message": "Loading model '%s'" % request.modelId,
                     "model_id": request.modelId,
                 }
             )
-
-            if self.config_parser.use_abortable_threads:
+            caikit_config = get_config()
+            if caikit_config.runtime.use_abortable_threads:
                 work = AbortableAction(
                     CallAborter(context),
                     self.model_manager.load_model,
                     request.modelId,
                     request.modelPath,
                     request.modelType,
                 )
@@ -105,20 +104,21 @@
                     "model_id": request.modelId,
                     "error_id": e.id,
                 }
             )
             raise e
 
         # get concurrency
-        if request.modelType in self.config_parser.max_model_concurrency_per_type:
-            max_concurrency = self.config_parser.max_model_concurrency_per_type[
+        model_mesh_config = get_config().inference_plugin.model_mesh
+        if request.modelType in model_mesh_config.max_model_concurrency_per_type:
+            max_concurrency = model_mesh_config.max_model_concurrency_per_type[
                 request.modelType
             ]
         else:
-            max_concurrency = self.config_parser.max_model_concurrency
+            max_concurrency = model_mesh_config.max_model_concurrency
 
         return model_runtime_pb2.LoadModelResponse(
             sizeInBytes=model_size, maxConcurrency=max_concurrency
         )
 
     def unloadModel(self, request, context):
         """Model unloading.
@@ -254,22 +254,23 @@
                 GRPC request, gen from model-runtime.proto
             context(grpc.ServicerContext):
                 Context object (contains request metadata, etc)
         Returns:
             model_runtime_pb2.RuntimeStatusResponse:
                 Gen from model-runtime.proto
         """
+        model_mesh_config = get_config().inference_plugin.model_mesh
         log.info(
             "<RUN25209721I>",
             "Starting Model Runtime version: %s",
-            self.config_parser.runtime_version,
+            model_mesh_config.runtime_version,
         )
         return model_runtime_pb2.RuntimeStatusResponse(
             status=model_runtime_pb2.RuntimeStatusResponse.READY,
-            capacityInBytes=self.config_parser.capacity,
-            maxLoadingConcurrency=self.config_parser.max_loading_concurrency,
-            modelLoadingTimeoutMs=self.config_parser.model_loading_timeout_ms,
-            defaultModelSizeInBytes=self.config_parser.default_model_size,
-            runtimeVersion=self.config_parser.runtime_version,
-            numericRuntimeVersion=self.config_parser.numeric_runtime_version,
-            limitModelConcurrency=self.config_parser.latency_based_autoscaling_enabled,
+            capacityInBytes=model_mesh_config.capacity,
+            maxLoadingConcurrency=model_mesh_config.max_loading_concurrency,
+            modelLoadingTimeoutMs=model_mesh_config.model_loading_timeout_ms,
+            defaultModelSizeInBytes=model_mesh_config.default_model_size,
+            runtimeVersion=model_mesh_config.runtime_version,
+            numericRuntimeVersion=model_mesh_config.numeric_runtime_version,
+            limitModelConcurrency=model_mesh_config.latency_based_autoscaling_enabled,
         )
```

### Comparing `caikit-0.1.6/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.2.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.2.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 
 # Local
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime.model_management.training_manager import TrainingManager
-from caikit.runtime.utils.config_parser import ConfigParser
 
 log = alog.use_channel("MR-SERVICR-I")
 
 
 class TrainingManagementServicerImpl:
     """This class contains the implementation of all of the RPCs that are required to run a
     service in Model Mesh as a Model-Runtime."""
 
     def __init__(self):
-        self.config_parser = ConfigParser.get_instance()
         self.training_manager = TrainingManager.get_instance()
 
     def GetTrainingStatus(self, request, context):  # pylint: disable=unused-argument
         """Missing associated documentation comment in .proto file."""
         training_info = TrainingInfoRequest.from_proto(request)
 
         return TrainingInfoResponse(
```

### Comparing `caikit-0.1.6/caikit/runtime/types/__init__.py` & `caikit-0.2.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/types/aborted_exception.py` & `caikit-0.2.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.2.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.2.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/utils/__init__.py` & `caikit-0.2.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/utils/import_util.py` & `caikit-0.2.0/caikit/runtime/utils/import_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 import re
 import sys
 
 # Third Party
 from grpc import StatusCode
 
 # First Party
+import aconfig
 import alog
 
 # Local
+from caikit import get_config
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 import caikit.core
 
 log = alog.use_channel("COM-LIB-INIT")
 
 
 class UnifiedDataModel:
     """This class acts as an aggregator between the data models of multiple
@@ -64,34 +65,34 @@
         if len(candidates) > 1:
             raise AttributeError(
                 f"Multiple library implementations of {name} found: {list(candidates.keys())}"
             )
         return super().__getattr__(name)
 
 
-def get_data_model(config: ConfigParser = None) -> UnifiedDataModel:
+def get_data_model(config: aconfig.Config = None) -> UnifiedDataModel:
     """
     Get the data model from the Caikit library of interest. This is accomplished
     via dynamic import on the caikit_library's environment variable.
 
     NOTE: This function also has the side-effect of importing each of the
         caikit_library libraries for the first time, causing their modules to
         be registered with the caikit.core MODULE_REGISTRY. It is a critical
         step in initializing the set of modules that can be loaded by this
         running server instance.
 
     Args:
-        config(ConfigParser): Config parser instance
+        config(aconfig.Config): caikit configuration
 
     Returns:
         (module): Handle to the module after dynamic wild import
     """
     if not config:
-        config = ConfigParser.get_instance()
-    lib_names = clean_lib_names(config.caikit_library)
+        config = get_config()
+    lib_names = clean_lib_names(config.runtime.library)
 
     # Add all caikit.interfaces.X modules
     lib_names.extend(
         [
             lib_name
             for lib_name in sys.modules
             if lib_name.startswith("caikit.interfaces.") and lib_name.count(".") == 2
```

### Comparing `caikit-0.1.6/caikit/runtime/utils/servicer_util.py` & `caikit-0.2.0/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/work_management/__init__.py` & `caikit-0.2.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/work_management/abortable_action.py` & `caikit-0.2.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/work_management/call_aborter.py` & `caikit-0.2.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.2.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/docs/adrs/README.md` & `caikit-0.2.0/docs/adrs/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/examples/start_runtime_with_sample_lib.py` & `caikit-0.2.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/pyproject.toml` & `caikit-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.1.6"
+version = "0.2.0"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "alchemy-config>=1.0.0",
+    "alchemy-config>=1.1.1",
     "alchemy-logging>=1.0.4",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
-    "ijson>=3.1.4,<3.2.0",
+    "ijson>=3.1.4,<3.3.0",
     "munch>=2.5.0,<3.0",
     "protobuf>=3.19.0,<5",
     "prometheus_client==0.12.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
-    "semver>=2.13.0,<3.0",
+    "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
     "wheel>=0.37.0",
     "jtd-to-proto>=0.12.1,<0.13.0",
     "import-tracker>=3.1.5,<4",
 ]
```

### Comparing `caikit-0.1.6/scripts/fmt.sh` & `caikit-0.2.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/__init__.py` & `caikit-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/base.py` & `caikit-0.2.0/tests/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,14 @@
     # Other things that we use often
     block_fixtures_dir = os.path.join(fixtures_dir, "blocks")
     resource_fixtures_dir = os.path.join(fixtures_dir, "resources")
     workflow_fixtures_dir = os.path.join(fixtures_dir, "workflows")
     toolkit_fixtures_dir = os.path.join(fixtures_dir, "toolkit")
 
     def __init__(self, *args, **kwargs):
-        # configure logging from env
-        default_level = os.environ.get("ALOG_DEFAULT_LEVEL", "error")
-        filters = os.environ.get("ALOG_FILTERS", "")
-        logging.configure(default_level, filters)
-
         # initialize parent class
         super().__init__(*args, **kwargs)
 
     def _compare_seqs(self, obj_seq1, obj_seq2, properties):
         """Given two sequences, ensure that they are the same length, and that each specified
         property is equal per object. This method explodes if the sequences are not the same
         as defined by assertEqual on the properties of interest.
```

### Comparing `caikit-0.1.6/tests/conftest.py` & `caikit-0.2.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,67 @@
 """
 This sets up global test configs when pytest starts
 """
 
 # Standard
 from contextlib import contextmanager
 from typing import Type
+from unittest.mock import patch
+import copy
 import json
 import os
 import sys
 import tempfile
 import threading
 import time
 import uuid
 
 # Third Party
 from grpc_health.v1 import health_pb2, health_pb2_grpc
 import grpc
 import pytest
-import yaml
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.core.data_model.dataobject import render_dataobject_protos
 from caikit.core.toolkit import logging
 from caikit.runtime.grpc_server import RuntimeGRPCServer
-from caikit.runtime.model_management.model_loader import ModelLoader
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
-from caikit.runtime.utils.config_parser import ConfigParser
 from tests.fixtures import Fixtures
+import caikit
 
 log = alog.use_channel("TEST-CONFTEST")
 
-# Make sample_lib available for import
-sys.path.append(
-    os.path.join(
-        os.path.dirname(__file__),
-        "fixtures",
-    ),
+FIXTURES_DIR = os.path.join(
+    os.path.dirname(__file__),
+    "fixtures",
 )
 
+# Make sample_lib available for import
+sys.path.append(FIXTURES_DIR)
+# Local
+import sample_lib
+
 # Configure logging from the environment
-logging.configure(
-    default_level=os.environ.get("LOG_LEVEL", "off"),
-    filters=os.environ.get("LOG_FILTERS", "urllib3:off"),
-    thread_id=os.environ.get("LOG_THREAD_ID", "") == "true",
-)
+logging.configure()
 
 
 @pytest.fixture(autouse=True, scope="session")
 def test_environment():
-    """The most important fixture: This sets `ENVIRONMENT=test` for all tests.
-    This is required to pick up the `test` section of config so that our unit
-    tests pick up the correct settings.
-    """
-    old_env = os.environ.get("ENVIRONMENT")
-    os.environ["ENVIRONMENT"] = "test"
-    # hack: delete any config that exists
-    ConfigParser._ConfigParser__instance = None
-    cfg = ConfigParser.get_instance()
-    # Make sure we picked up teh test configs
-    assert cfg.environment == "test"
-    # Test away!
+    """The most important fixture: This runs caikit configuration with the base test config overrides"""
+    test_config_path = os.path.join(FIXTURES_DIR, "config", "config.yml")
+    caikit.configure(test_config_path)
     yield
-    # Reset environment back to previous state
-    if old_env is None:
-        os.unsetenv("ENVIRONMENT")
-    else:
-        os.environ["ENVIRONMENT"] = old_env
+    # No cleanup required...?
 
 
 @pytest.fixture(scope="session")
 def sample_inference_service(render_protos) -> ServicePackage:
     """Service package pointing to `sample_lib` for testing"""
     inference_service = ServicePackageFactory().get_service_package(
         ServicePackageFactory.ServiceType.INFERENCE,
@@ -192,32 +178,30 @@
     yield model_id
 
     # teardown
     model_manager.unload_model(model_id)
 
 
 @contextmanager
-def temp_config_parser(config_overrides):
-    """Temporarily overwrite the ConfigParser singleton"""
-    real_singleton = ConfigParser.get_instance()
-    prev_config_path = os.environ.get("CONFIG_FILES")
-    ConfigParser._ConfigParser__instance = None
-    with tempfile.NamedTemporaryFile(suffix=".yaml", mode="w") as temp_cfg:
-        yaml.safe_dump(config_overrides, temp_cfg)
-        temp_cfg.flush()
-        os.environ["CONFIG_FILES"] = temp_cfg.name
-        temp_inst = ConfigParser.get_instance()
-        ModelLoader.get_instance().config_parser = temp_inst
-        yield temp_inst
-    ConfigParser._ConfigParser__instance = real_singleton
-    ModelLoader.get_instance().config_parser = ConfigParser.get_instance()
-    if prev_config_path is None:
-        del os.environ["CONFIG_FILES"]
-    else:
-        os.environ["CONFIG_FILES"] = prev_config_path
+def temp_config(config_overrides: dict):
+    """Temporarily edit the caikit config in a mock context"""
+    existing_config = copy.deepcopy(getattr(caikit.config.config, "_CONFIG"))
+    # Patch out the internal config, starting with a fresh copy of the current config
+    with patch.object(caikit.config.config, "_CONFIG", existing_config):
+        # Patch the immutable view of the config as well
+        # This is required otherwise the updated immutable view will persist after the test
+        with patch.object(caikit.config.config, "_IMMUTABLE_CONFIG", None):
+            # Run our config overrides inside the patch
+            if config_overrides:
+                caikit.configure(config_dict=config_overrides)
+            else:
+                # or just slap some random uuids in there. Barf, but we need to call `.configure()`
+                caikit.configure(config_dict={str(uuid.uuid4()): str(uuid.uuid4())})
+            # Yield to the test with the new overriden config
+            yield get_config()
 
 
 # fixtures to optionally generate the protos for easier debugging
 def pytest_addoption(parser):
     parser.addoption(
         "--render-protos",
         action="store_true",
```

### Comparing `caikit-0.1.6/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.2.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.2.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/blocks/__init__.py` & `caikit-0.2.0/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/blocks/test_base.py` & `caikit-0.2.0/tests/core/blocks/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 # Standard
 import os
 import shutil
 import tempfile
 
 # Local
+from caikit.config import get_config
 from caikit.core.blocks import block
 from caikit.core.blocks.base import BlockSaver
-from caikit.core.config import lib_config
 from caikit.core.toolkit.serializers import JSONSerializer
 
 # pylint: disable=import-error
 from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model.sample import SampleInputType
 
 # Unit Test Infrastructure
@@ -151,30 +151,22 @@
         with self.assertRaises(RuntimeError):
             declare_block()  # Should fail (block was already registered)
 
 
 class TestBlockSaver(TestCaseBase):
     @classmethod
     def setUpClass(cls):
-        @caikit.core.block(
-            "2D391918-13FE-45D8-B6C5-549BCD5EAA1B", "SampleBlock", "0.0.1"
-        )
-        class TestSampleBlock(caikit.core.BlockBase):
-            pass
-
-        cls.dummy_block = TestSampleBlock()
+        cls.dummy_block = SampleBlock()
 
     def test_block_saver_attribs(self):
         # make sure the saver has the desired config attrs
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 # name
                 self.assertIsInstance(block_saver.config.get("name"), str)
                 self.assertEqual(
                     block_saver.config.get("name"), self.dummy_block.BLOCK_NAME
                 )
 
@@ -192,36 +184,32 @@
 
                 # block id
                 self.assertIsInstance(block_saver.config.get("block_id"), str)
                 self.assertEqual(
                     block_saver.config.get("block_id"), self.dummy_block.BLOCK_ID
                 )
 
-                # caikit.core version
-                self.assertIsInstance(
-                    block_saver.config.get("caikit.core_version"), str
-                )
+                # sample_lib_version
+                self.assertIsInstance(block_saver.config.get("sample_lib_version"), str)
                 self.assertEqual(
-                    block_saver.config.get("caikit.core_version"),
-                    lib_config.library_version,
+                    block_saver.config.get("sample_lib_version"),
+                    "1.2.3",
                 )
 
                 # creation date
                 self.assertIsInstance(block_saver.config.get("created"), str)
 
             # and that the config gets written
             self.assertTrue(os.path.isfile(os.path.join(tempdir, "config.yml")))
 
     def test_add_dir(self):
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 # add a directory called `a`
                 a_rel, a_abs = block_saver.add_dir("a")
                 self.assertEqual(os.path.normpath(a_rel), os.path.basename(a_abs))
                 self.assertTrue(os.path.isdir(a_abs))
 
                 # add `b/c` inside `a`
@@ -234,16 +222,14 @@
 
     def test_update_config(self):
         # verify that we can add some config options with `saver.update_config`
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 block_saver.update_config(
                     {
                         "training_mode": "stochastic",
                         "training_epochs": 1000,
                     }
                 )
@@ -253,16 +239,14 @@
 
     def test_copy_file(self):
         # verify that we can copy a file into the model with `saver.copy_file`
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 block_saver.copy_file(
                     os.path.join(self.fixtures_dir, "linux.txt"), "artifacts"
                 )
             self.assertTrue(
                 os.path.isfile(os.path.join(tempdir, "artifacts/linux.txt"))
             )
@@ -274,16 +258,14 @@
 
         try:
             # verify that exceptions are re-raised from the context manager
             with self.assertRaises(RuntimeError):
                 with BlockSaver(
                     self.dummy_block,
                     model_path=tempdir,
-                    library_name=lib_config.library_name,
-                    library_version=lib_config.library_version,
                 ) as block_saver:
                     block_saver.add_dir("artifacts")
                     raise RuntimeError("test")
 
             # verify that our error caused the model tree to be removed
             self.assertFalse(os.path.exists(os.path.join(tempdir, "config.yml")))
             self.assertFalse(os.path.exists(os.path.join(tempdir, "artifacts")))
@@ -292,30 +274,26 @@
             shutil.rmtree(tempdir, ignore_errors=True)
 
     def test_save_object_saves_a_json_object_to_model_root_dir(self):
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 serializer = JSONSerializer()
 
                 block_saver.save_object({"foo": "bar"}, "test.json", serializer)
 
                 self.assertTrue(os.path.exists(os.path.join(tempdir, "test.json")))
 
     def test_save_object_saves_a_json_object_to_model_sub_dir(self):
         with tempfile.TemporaryDirectory() as tempdir:
             with BlockSaver(
                 self.dummy_block,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as block_saver:
                 serializer = JSONSerializer()
 
                 block_saver.save_object(
                     {"foo": "bar"}, "test.json", serializer, "artifacts"
                 )
```

### Comparing `caikit-0.1.6/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.2.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/streams/test_converter.py` & `caikit-0.2.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.2.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.2.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/streams/test_resolver.py` & `caikit-0.2.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/streams/test_validator.py` & `caikit-0.2.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/test_base.py` & `caikit-0.2.0/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/test_dataobject.py` & `caikit-0.2.0/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/data_model/test_producer.py` & `caikit-0.2.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/helpers.py` & `caikit-0.2.0/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/module_backends/test_backend_types.py` & `caikit-0.2.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/test_imports.py` & `caikit-0.2.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/test_model_manager.py` & `caikit-0.2.0/tests/core/test_model_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 """
 
 # Standard
 from contextlib import contextmanager
 import os
 import tempfile
 
-# Third Party
-import pytest
-
 # Local
-from caikit.core.config import lib_config
-from caikit.core.module_backend_config import configure, configured_backends
-from caikit.core.module_backends import LocalBackend, backend_types
+from caikit.config import get_config
+from caikit.core.module_backend_config import configure
+from caikit.core.module_backends import LocalBackend
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
+from tests.conftest import temp_config
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
 from tests.core.helpers import *
 import caikit.core
 
 
 class TestModelManager(TestCaseBase):
@@ -68,25 +66,16 @@
 
     @pytest.fixture
     def global_load_path(self):
         """Set load_path prior to importing caikit.core."""
         # Set test load path
         test_load_path = os.path.join(self.fixtures_dir, "models")
 
-        # Save the original load path so that it can be undone
-        std_load_path = lib_config.load_path
-
-        # Overwrite the load path with the test fixtures path
-        lib_config.load_path = test_load_path
-
-        # Yield execution to the test itself
-        yield
-
-        # Undo the load path patching
-        lib_config.load_path = std_load_path
+        with temp_config({"load_path": test_load_path}):
+            yield
 
     def test_load_can_return_a_block(self):
         model = caikit.core.load(self.model_path)
         self.assertIsInstance(model, caikit.core.BlockBase)
 
     def test_load_can_load_a_block_as_a_singleton(self):
         # load a model with no hash config
@@ -201,28 +190,25 @@
         """Test that loading a model from a path defined in the load_path config variable works."""
         model = caikit.core.load("foo")
         self.assertIsInstance(model, caikit.core.BlockBase)
 
     def test_import_block_registry(self):
         """Make sure that the BLOCK_REGISTRY can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        # Local
-        from caikit.core.model_manager import BLOCK_REGISTRY
+        from caikit.core.model_manager import BLOCK_REGISTRY  # isort: skip
 
     def test_import_workflow_registry(self):
         """Make sure that the WORKFLOW_REGISTRY can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        # Local
-        from caikit.core.model_manager import WORKFLOW_REGISTRY
+        from caikit.core.model_manager import WORKFLOW_REGISTRY  # isort: skip
 
     def test_import_resource_registry(self):
         """Make sure that the RESOURCE_REGISTRY can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
-        # Local
-        from caikit.core.model_manager import RESOURCE_REGISTRY
+        from caikit.core.model_manager import RESOURCE_REGISTRY  # isort: skip
 
 
 # Pytest tests #########################################################
 
 # Setup #########################################################################
 
 DUMMY_MODULE_ID = "foo"
@@ -266,16 +252,14 @@
     def load(cls, *args, **kwargs):
         return cls()
 
     def save(self, model_path):
         block_saver = caikit.core.blocks.BlockSaver(
             self,
             model_path=model_path,
-            library_name="foo",
-            library_version="0.42.0",
         )
         with block_saver:
             pass
 
 
 @contextmanager
 def temp_saved_model(model):
@@ -289,92 +273,132 @@
 
 
 def test_backend_supported_model_load_successfully(reset_globals):
     """Test backend supported model can load successfully"""
 
     _, DummyBar = setup_saved_model(MockBackend)
     # Configure backend
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": {}})
-
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
-    assert isinstance(model, DummyBar)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
+
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
+        assert isinstance(model, DummyBar)
 
 
 def test_local_model_load_successfully(reset_globals):
     """Test regular / local model can load successfully"""
     DummyFoo, DummyBar = setup_saved_model(MockBackend)
 
     # Configure backend
-    configure(backend_priority=[backend_types.LOCAL], backends={"mock": {}})
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.LOCAL],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
 
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
 
-    assert isinstance(model, DummyFoo)
-    assert not isinstance(model, DummyBar)
+        assert isinstance(model, DummyFoo)
+        assert not isinstance(model, DummyBar)
 
 
 def test_local_model_loaded_backend_successfully(reset_globals):
     """Test if local models can be loaded in specified backend
     if available in SUPPORTED_LOAD_BACKENDS
     """
     _, DummyBar = setup_saved_model(MockBackend)
     # Configure backend
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": {}})
-
-    DummyBar.SUPPORTED_LOAD_BACKENDS.append("LOCAL")
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
-    assert isinstance(model, DummyBar)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
+
+        DummyBar.SUPPORTED_LOAD_BACKENDS.append("LOCAL")
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
+        assert isinstance(model, DummyBar)
 
 
 def test_backend_model_loaded_as_singleton(reset_globals):
     """Test that backend specific model can be loaded as a singleton"""
 
     _, DummyBar = setup_saved_model(MockBackend)
     # Configure backend
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": {}})
-
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
-    model1 = caikit.core.load(dummy_model_path, load_singleton=True)
-    model2 = caikit.core.load(dummy_model_path, load_singleton=True)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
+
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
+        model1 = caikit.core.load(dummy_model_path, load_singleton=True)
+        model2 = caikit.core.load(dummy_model_path, load_singleton=True)
 
-    # Pointers should be same
-    assert id(model1) == id(model2)
+        # Pointers should be same
+        assert id(model1) == id(model2)
 
 
 def test_singleton_cache_can_be_cleared(reset_globals):
     """Test that a singleton cache can be cleared"""
     dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
     # Setup the mock backend
     _, _ = setup_saved_model(MockBackend)
-    model = caikit.core.load(dummy_model_path, load_singleton=True)
+    _ = caikit.core.load(dummy_model_path, load_singleton=True)
 
     assert len(caikit.core.MODEL_MANAGER.get_singleton_model_cache_info()) > 0
 
     # Clear cache
     caikit.core.MODEL_MANAGER.clear_singleton_cache()
     assert len(caikit.core.MODEL_MANAGER.get_singleton_model_cache_info()) == 0
 
 
 def test_singleton_cache_with_different_backend(reset_globals):
     """Test singleton cache doesn't stop different backend models"""
 
-    DummyFoo, DummyBar = setup_saved_model(MockBackend)
+    _, _ = setup_saved_model(MockBackend)
     # Configure backend
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": {}})
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
 
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
-    model1 = caikit.core.load(dummy_model_path, load_singleton=True)
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
+        _ = caikit.core.load(dummy_model_path, load_singleton=True)
 
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
-    model2 = caikit.core.load(dummy_model_path, load_singleton=True)
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+        _ = caikit.core.load(dummy_model_path, load_singleton=True)
 
-    assert len(caikit.core.MODEL_MANAGER.get_singleton_model_cache_info()) == 2
+        assert len(caikit.core.MODEL_MANAGER.get_singleton_model_cache_info()) == 2
 
 
 def test_get_module_class():
     """Test to verify get_module_class function can return appropriate module class"""
     # Block
     config = {"block_id": "foo", "block_class": "Foo"}
     module_config = caikit.core.module.ModuleConfig(config)
@@ -391,58 +415,84 @@
     assert caikit.core.ModelManager.get_module_class_from_config(module_config) == "Foo"
 
 
 def test_fall_back_to_local(reset_globals):
     """Make sure that if LOCAL is enabled and a given module doesn't have any
     registered backends, the default caikit.core.load is used.
     """
-    configure(backend_priority=[])
-    with temp_saved_model(NonDistributedBlock()) as model_path:
-        model = caikit.core.load(model_path)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [],
+            }
+        }
+    ):
+        configure()
+        with temp_saved_model(NonDistributedBlock()) as model_path:
+            model = caikit.core.load(model_path)
 
-    assert isinstance(model, NonDistributedBlock)
+        assert isinstance(model, NonDistributedBlock)
 
 
 def test_no_local_if_disabled(reset_globals):
     """Make sure that if LOCAL is disabled and a given module doesn't have any
     registered backends, loading fails.
     """
     _ = setup_saved_model(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], disable_local_backend=True)
-    with temp_saved_model(NonDistributedBlock()) as model_path:
-        with pytest.raises(ValueError):
-            caikit.core.load(model_path)
+    with temp_config(
+        {"module_backends": {"priority": [backend_types.MOCK], "disable_local": True}}
+    ):
+        configure()
+        with temp_saved_model(NonDistributedBlock()) as model_path:
+            with pytest.raises(ValueError):
+                caikit.core.load(model_path)
 
 
 def test_preferred_backend_enabled(reset_globals):
     """Make sure that for a model artifact saved with a local backend can be
     loaded with an enabled non-local backend if given as a preferred_backend.
     """
     _, DummyBar = setup_saved_model(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": {}})
-
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
-    assert isinstance(model, DummyBar)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": {}},
+            }
+        }
+    ):
+        configure()
+
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
+        assert isinstance(model, DummyBar)
 
 
 def test_preferred_backend_disabled(reset_globals):
     """Make sure that for a model artifact saved with a local backend loads as
     local even with a preferred_backend when the preferred backend is disabled.
     """
     DummyFoo, DummyBar = setup_saved_model(MockBackend)
-    configure(backend_priority=[backend_types.LOCAL], backends={})
-
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
-    assert isinstance(model, DummyFoo)
-    assert not isinstance(model, DummyBar)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.LOCAL],
+                "configs": {},
+            }
+        }
+    ):
+        configure()
+
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_LOCAL_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
+        assert isinstance(model, DummyFoo)
+        assert not isinstance(model, DummyBar)
 
 
-def test_non_local_supported_backed(reset_globals):
+def test_non_local_supported_backend(reset_globals):
     """Make sure model artifact saved with as non-local backend loads as
     non-local backend if supported by SUPPORTED_LOAD_BACKENDS
     """
     DummyFoo, _ = setup_saved_model(MockBackend)
 
     class MockBackend2(BackendBase):
         backend_type = "MOCK2"
@@ -462,12 +512,20 @@
     class DummyBaz:
         SUPPORTED_LOAD_BACKENDS = [backend_types.MOCK, backend_types.MOCK2]
 
         @classmethod
         def load(self, *args, **kwargs):
             return DummyBaz()
 
-    configure(backend_priority=[backend_types.MOCK2], backends={})
-
-    dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
-    model = caikit.core.load(dummy_model_path)
-    assert isinstance(model, DummyBaz)
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK2],
+                "configs": {},
+            }
+        }
+    ):
+        configure()
+
+        dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
+        model = caikit.core.load(dummy_model_path)
+        assert isinstance(model, DummyBaz)
```

### Comparing `caikit-0.1.6/tests/core/test_module.py` & `caikit-0.2.0/tests/core/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model.sample import SampleInputType
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
+from tests.conftest import temp_config
 from tests.core.helpers import *
 import caikit.core
 
 
 class TestModuleBase(TestCaseBase):
     def setUp(self):
         self.base_module_instance = caikit.core.ModuleBase()
@@ -401,20 +402,27 @@
     assert DummyBar.PRODUCER_ID
 
     # Fetch without config raises
     with pytest.raises(ValueError):
         assert get_backend(DummyBar.BACKEND_TYPE)
 
     # Configure and make sure it can be fetched by the class
-    caikit.core.module_backend_config.configure(backend_priority=[backend_types.MOCK])
-    assert DummyBar.BACKEND_TYPE == backend_types.MOCK
-
-    # Make sure an instance can fetch via get_backend()
-    inst = DummyBar()
-    assert inst.test_fetching_backend().backend_type == backend_types.MOCK
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+            }
+        }
+    ):
+        caikit.core.module_backend_config.configure()
+        assert DummyBar.BACKEND_TYPE == backend_types.MOCK
+
+        # Make sure an instance can fetch via get_backend()
+        inst = DummyBar()
+        assert inst.test_fetching_backend().backend_type == backend_types.MOCK
 
 
 def test_default_load_supported_backend(reset_globals):
     """Test the defined backend gets added as the supported backend by default"""
     _, DummyBar = configure_alternate_backend_impl()
     assert hasattr(DummyBar, module.SUPPORTED_LOAD_BACKENDS_VAR_NAME)
     assert len(DummyBar.SUPPORTED_LOAD_BACKENDS) == 1
```

### Comparing `caikit-0.1.6/tests/core/test_module_backend_config.py` & `caikit-0.2.0/tests/core/test_module_backend_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,77 +12,112 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Tests for the backend configuration framework
 """
 
-# Standard
-from unittest.mock import Mock
-
 # Local
 from caikit.core.blocks import base, block
 from caikit.core.module_backend_config import (
     _CONFIGURED_BACKENDS,
     configure,
     configured_backends,
     get_backend,
     start_backends,
 )
 from caikit.core.module_backends import backend_types
+from tests.conftest import temp_config
 from tests.core.helpers import *
 
 # Setup #########################################################################
 
 foo_cfg = {"mock": 1}
 
 ## Tests #######################################################################
 
 
 def test_configure_with_module(reset_globals):
-    """Test that configuring with a configured bakend type that has a
+    """Test that configuring with a configured backend type that has a
     configuration module obj works
     """
     backend_types.register_backend_type(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": foo_cfg})
-    assert "MOCK" in configured_backends()
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
-    assert foo_cfg == _CONFIGURED_BACKENDS[backend_types.MOCK].config
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": foo_cfg},
+            }
+        }
+    ):
+        configure()
+        assert "MOCK" in configured_backends()
+        assert (
+            _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
+        )
+        assert foo_cfg == _CONFIGURED_BACKENDS[backend_types.MOCK].config
 
 
 def test_non_supported_backend_raises():
     """Test that backend provided as priority to configure raises
     if not registered"""
-    with pytest.raises(ValueError):
-        configure(backend_priority=[Mock()])
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": ["unsupported"],
+            }
+        }
+    ):
+        with pytest.raises(ValueError):
+            configure()
 
 
 def test_disabling_local_backend(reset_globals):
     """Test that disabling local backend does not add it to priority automatically"""
     backend_types.register_backend_type(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], disable_local_backend=True)
-    assert "LOCAL" not in configured_backends()
+    with temp_config(
+        {"module_backends": {"priority": [backend_types.MOCK], "disable_local": True}}
+    ):
+        configure()
+        assert "LOCAL" not in configured_backends()
 
 
 def test_duplicate_config_raises(reset_globals):
     """Test that duplicate configuration of a backend raises"""
     backend_types.register_backend_type(MockBackend)
-    configure(backend_priority=[backend_types.MOCK])
-    with pytest.raises(AssertionError):
-        configure(backend_priority=[backend_types.MOCK])
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+            }
+        }
+    ):
+        configure()
+        with pytest.raises(AssertionError):
+            configure()
 
 
 def test_one_configured_backend_can_start(reset_globals):
     """Test that the configured backend can be started"""
     backend_types.register_backend_type(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], backends={"mock": foo_cfg})
-    start_backends()
-    # This is configured to be True in helpers
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+                "configs": {"mock": foo_cfg},
+            }
+        }
+    ):
+        configure()
+        start_backends()
+        # This is configured to be True in helpers
+        assert (
+            _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
+        )
+        assert _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
 
 
 def test_multiple_module_same_backend_configures(reset_globals):
     """Test to check if multiple modules for same backend
     can override backend configurations"""
     # Register backend type
     backend_types.register_backend_type(MockBackend)
@@ -111,25 +146,37 @@
         backend_config_override={"bar2": 2},
     )
     class DummyBar:
         pass
 
     # Initiate configuration
 
-    configure(backend_priority=[backend_types.MOCK])
-    assert "MOCK" in configured_backends()
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
-    assert "bar1" in _CONFIGURED_BACKENDS[backend_types.MOCK].config
-    assert "bar2" in _CONFIGURED_BACKENDS[backend_types.MOCK].config
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].config["bar1"] == 1
+    with temp_config(
+        {
+            "module_backends": {
+                "priority": [backend_types.MOCK],
+            }
+        }
+    ):
+        configure()
+        assert "MOCK" in configured_backends()
+        assert (
+            _CONFIGURED_BACKENDS[backend_types.MOCK].backend_type == backend_types.MOCK
+        )
+        assert "bar1" in _CONFIGURED_BACKENDS[backend_types.MOCK].config
+        assert "bar2" in _CONFIGURED_BACKENDS[backend_types.MOCK].config
+        assert _CONFIGURED_BACKENDS[backend_types.MOCK].config["bar1"] == 1
 
 
 def test_get_backend_starts_backend(reset_globals):
     """Test that fetching a handle to a backend with get_backend ensures that it
     is started
     """
     backend_types.register_backend_type(MockBackend)
-    configure(backend_priority=[backend_types.MOCK], disable_local_backend=True)
-    assert not _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
-    backend = get_backend(backend_types.MOCK)
-    assert backend.is_started
-    assert _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
+    with temp_config(
+        {"module_backends": {"priority": [backend_types.MOCK], "disable_local": True}}
+    ):
+        configure()
+        assert not _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
+        backend = get_backend(backend_types.MOCK)
+        assert backend.is_started
+        assert _CONFIGURED_BACKENDS[backend_types.MOCK].is_started
```

### Comparing `caikit-0.1.6/tests/core/test_module_metadata.py` & `caikit-0.2.0/tests/core/test_module_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     class _FunkyModel(SampleBlock):
         @classmethod
         def load(cls, model_path):
             return (super().load(model_path), "something else")
 
     model = _FunkyModel()
     with tempfile.TemporaryDirectory() as tempdir:
+        # NOTE: the module will get detected as tests since _FunkyModel is defined here
         model.save(tempdir)
         caikit.core.load(tempdir)
 
 
 # pylint: disable=redefined-outer-name
 def test_load_can_be_called_directly_with_non_standard_kwargs(sample_model_path):
     initial_metadata = _load_model_metadata(sample_model_path)
```

### Comparing `caikit-0.1.6/tests/core/test_no_write_permissions.py` & `caikit-0.2.0/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/toolkit/test_compatibility.py` & `caikit-0.2.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/toolkit/test_error_handler.py` & `caikit-0.2.0/tests/core/toolkit/test_error_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import alog
 
 # Local
 from caikit.core.toolkit.errors import error_handler
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
+import caikit
 
 
 class TestErrorHandler(TestCaseBase):
     def setUp(self):
         """Construct a new log channel and error handler."""
         self.log = alog.use_channel("TEST_ERR_HAN")
         self.error = error_handler.get(self.log)
@@ -80,62 +81,63 @@
         # verify that one log line was omitted
         self.assertEqual(len(self.caplog.records), 1)
 
     def test_log_raises_max(self):
         """Verify that `log_raises` will not keep logging after max log lines written."""
         # raise the same exception over and over, max + 10 times
         exception = AttributeError("this is a test")
-        for i in range(error_handler.MAX_EXCEPTION_LOG_MESSAGES + 10):
+        for i in range(caikit.get_config().max_exception_log_messages + 10):
             try:
                 self.error("<BBB>", exception)
             except:
                 pass
 
         # verify that tracking attribute was set
         self.assertTrue(hasattr(exception, "_caikit_core_nexception_log_messages"))
         # verify that it was incremented for every raise
         self.assertEqual(
             exception._caikit_core_nexception_log_messages,
-            error_handler.MAX_EXCEPTION_LOG_MESSAGES + 10 - 1,
+            caikit.get_config().max_exception_log_messages + 10 - 1,
         )
         # verify that it only wrote the max log lines
         # one for extra for message that logging will stop
         self.assertEqual(
-            len(self.caplog.records), error_handler.MAX_EXCEPTION_LOG_MESSAGES + 1
+            len(self.caplog.records), caikit.get_config().max_exception_log_messages + 1
         )
 
     def test_log_raises_max_with_root(self):
         """Verify that `log_raises` will not keep logging after max log lines written."""
         # raise the same exception over and over, max + 10 times
         exception = AttributeError("this is a test")
         root_exception = ValueError("this is the root ex")
-        for i in range(error_handler.MAX_EXCEPTION_LOG_MESSAGES + 10):
+        for i in range(caikit.get_config().max_exception_log_messages + 10):
             try:
                 self.error("<BBB>", exception, root_exception)
             except:
                 pass
 
         # verify that tracking attribute was set
         self.assertTrue(hasattr(exception, "_caikit_core_nexception_log_messages"))
         self.assertTrue(hasattr(root_exception, "_caikit_core_nexception_log_messages"))
         # verify that it was incremented for every raise
         self.assertEqual(
             exception._caikit_core_nexception_log_messages,
-            error_handler.MAX_EXCEPTION_LOG_MESSAGES + 10 - 1,
+            caikit.get_config().max_exception_log_messages + 10 - 1,
         )
         self.assertEqual(
             root_exception._caikit_core_nexception_log_messages,
-            error_handler.MAX_EXCEPTION_LOG_MESSAGES + 10 - 1,
+            caikit.get_config().max_exception_log_messages + 10 - 1,
         )
 
         # verify that it only wrote the max log lines
         # one for extra for message that logging will stop
         # Length of all records == 2 * MAX (one for each: exception and root exception)
         self.assertEqual(
-            len(self.caplog.records), 2 * (error_handler.MAX_EXCEPTION_LOG_MESSAGES + 1)
+            len(self.caplog.records),
+            2 * (caikit.get_config().max_exception_log_messages + 1),
         )
 
     def test_type_check_raises(self):
         """Verify that `type_check` raises a `TypeError`."""
         with self.assertRaises(TypeError):
             self.error.type_check("<HHH>", int, float, bad_type="hello world")
```

### Comparing `caikit-0.1.6/tests/core/toolkit/test_fileio.py` & `caikit-0.2.0/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.2.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/toolkit/test_serializers.py` & `caikit-0.2.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.2.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/workflows/__init__.py` & `caikit-0.2.0/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/core/workflows/test_base.py` & `caikit-0.2.0/tests/core/workflows/test_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 # Standard
 import os
 import tempfile
 
 # Local
-from caikit.core.config import lib_config
+from caikit.config import get_config
 from caikit.core.workflows import workflow
 from caikit.core.workflows.base import WorkflowLoader, WorkflowSaver
 
 # pylint: disable=import-error
 from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model.sample import SampleInputType
 from sample_lib.workflows.sample_task import SampleWorkflow
@@ -199,30 +199,22 @@
         for module in loaded_modules:
             self.assertIsInstance(module, SampleBlock)
 
 
 class TestWorkflowSaver(TestCaseBase):
     @classmethod
     def setUpClass(cls):
-        @caikit.core.workflow(
-            "A32D68FA-E5E6-41BD-BAAE-77A880EB6877", "SampleWorkflow", "0.0.1"
-        )
-        class TestSampleWorkflow(caikit.core.WorkflowBase):
-            pass
-
-        cls.dummy_workflow = TestSampleWorkflow()
+        cls.dummy_workflow = SampleWorkflow()
 
     def test_workflow_saver_attribs(self):
         # make sure the saver has the desired config attrs
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 # name
                 self.assertIsInstance(workflow_saver.config.get("name"), str)
                 self.assertEqual(
                     workflow_saver.config.get("name"), self.dummy_workflow.WORKFLOW_NAME
                 )
 
@@ -243,21 +235,21 @@
                 # workflow id
                 self.assertIsInstance(workflow_saver.config.get("workflow_id"), str)
                 self.assertEqual(
                     workflow_saver.config.get("workflow_id"),
                     self.dummy_workflow.WORKFLOW_ID,
                 )
 
-                # caikit.core version
+                # sample_lib_version
                 self.assertIsInstance(
-                    workflow_saver.config.get("caikit.core_version"), str
+                    workflow_saver.config.get("sample_lib_version"), str
                 )
                 self.assertEqual(
-                    workflow_saver.config.get("caikit.core_version"),
-                    caikit.core.lib_config.library_version,
+                    workflow_saver.config.get("sample_lib_version"),
+                    "1.2.3",
                 )
 
                 # creation date
                 self.assertIsInstance(workflow_saver.config.get("created"), str)
 
             # and that the config gets written
             self.assertTrue(os.path.isfile(os.path.join(tempdir, "config.yml")))
@@ -266,16 +258,14 @@
         dummy_path = os.path.join(self.fixtures_dir, "dummy_workflow", "dummy_block")
         dummy_block = caikit.core.load(dummy_path)
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 workflow_saver.save_module(dummy_block, "dummy")
 
                 self.assertTrue(os.path.exists(os.path.join(tempdir, "dummy")))
                 self.assertIsNotNone(workflow_saver.config.get("module_paths"))
                 self.assertEqual(
                     workflow_saver.config.get("module_paths"), {"dummy": "./dummy"}
@@ -285,16 +275,14 @@
         dummy_path = os.path.join(self.fixtures_dir, "dummy_workflow", "dummy_block")
         dummy_block = caikit.core.load(dummy_path)
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 workflow_saver.save_module(dummy_block, "dummy")
                 workflow_saver.save_module(dummy_block, "dummy2")
                 workflow_saver.save_params(test2="val2", test3="val3")
                 self.assertTrue(os.path.exists(os.path.join(tempdir, "dummy")))
                 self.assertTrue(os.path.exists(os.path.join(tempdir, "dummy2")))
                 self.assertIsNotNone(workflow_saver.config.get("module_paths"))
@@ -309,64 +297,56 @@
         """Test when the input module for the save is invalid."""
         dummy_models_with_rel_path = {"dummy": "invalid"}
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 with self.assertRaises(TypeError):
                     workflow_saver.save_module_list(
                         dummy_models_with_rel_path, "dummy_model"
                     )
 
     def test_save_module_list_invalid_dict(self):
         """Test when the input dict for the save is invalid."""
         dummy_models_with_rel_path = "invalid"
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 with self.assertRaises(TypeError):
                     workflow_saver.save_module_list(dummy_models_with_rel_path, "dummy")
 
     def test_save_module_list_invalid_config_key(self):
         """Test when the config key is invalid."""
         dummy_path = os.path.join(self.fixtures_dir, "dummy_workflow", "dummy_block")
         dummy_block = caikit.core.load(dummy_path)
         dummy_models_with_rel_path = {"dummy_sad": dummy_block}
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 with self.assertRaises(TypeError):
                     workflow_saver.save_module_list(dummy_models_with_rel_path, {})
 
     def test_save_module_list(self):
         """Test valid module list save with a list of syntax blocks."""
         dummy_path = os.path.join(self.fixtures_dir, "dummy_workflow", "dummy_block")
         dummy_block = caikit.core.load(dummy_path)
         dummy_models_with_rel_path = {"dummy_path": dummy_block}
 
         with tempfile.TemporaryDirectory() as tempdir:
             with WorkflowSaver(
                 self.dummy_workflow,
                 model_path=tempdir,
-                library_name=lib_config.library_name,
-                library_version=lib_config.library_version,
             ) as workflow_saver:
                 list_of_rel_path, _ = workflow_saver.save_module_list(
                     dummy_models_with_rel_path, "dummy"
                 )
                 # Ensure that we only get one relative path back
                 self.assertEqual(len(list_of_rel_path), 1)
                 # And that if we split our path components up, get 2 parts...
```

### Comparing `caikit-0.1.6/tests/data_model_helpers.py` & `caikit-0.2.0/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_block.zip` & `caikit-0.2.0/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_block/config.yml` & `caikit-0.2.0/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.2.0/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_resource.zip` & `caikit-0.2.0/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_workflow.zip` & `caikit-0.2.0/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/fixtures.py` & `caikit-0.2.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/invalid.zip` & `caikit-0.2.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/linux.txt` & `caikit-0.2.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/primitive_party.proto` & `caikit-0.2.0/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.2.0/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 A sample block for sample things!
 """
 # Standard
 from typing import Union
 
 # Local
-from ...config import lib_config
-from ...data_model.sample import OtherOutputType, SampleInputType, SampleTrainingType
+from ...data_model.sample import OtherOutputType, SampleInputType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
 
 @caikit.core.block("33221100-0405-0607-0809-0a0b02dd0e0f", "OtherBlock", "0.0.1")
 class OtherBlock(caikit.core.BlockBase):
@@ -30,16 +29,14 @@
         config = loader.config
         return cls(config["train"]["batch_size"], config["train"]["learning_rate"])
 
     def save(self, model_path):
         module_saver = ModuleSaver(
             self,
             model_path=model_path,
-            library_name="sample_lib",
-            library_version=lib_config.library_version,
         )
         with module_saver:
             config_options = {
                 "train": {
                     "batch_size": self.batch_size,
                     "learning_rate": self.learning_rate,
                 },
```

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 A sample block for sample things!
 """
 # Standard
 from typing import List
 
 # Local
-from ...config import lib_config
 from ...data_model.sample import SampleInputType, SampleOutputType, SampleTrainingType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
 
 @caikit.core.block("00af2203-0405-0607-0263-0a0b02dd0c2f", "ListBlock", "0.0.1")
@@ -43,16 +42,14 @@
             raise ValueError(f"{self.POISON_PILL_NAME} is not allowed!")
         return SampleOutputType(f"Hello {sample_input.name}")
 
     def save(self, model_path):
         module_saver = ModuleSaver(
             self,
             model_path=model_path,
-            library_name="sample_lib",
-            library_version=lib_config.library_version,
         )
         with module_saver:
             config_options = {
                 "train": {
                     "batch_size": self.batch_size,
                     "learning_rate": self.learning_rate,
                 },
```

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 A block meant to flex a bit of the protobufs primitive support
 """
 # Standard
 from typing import List
 
 # Local
-from ...config import lib_config
 from ...data_model.sample import SampleOutputType
 from caikit.core.module import ModuleSaver
 import caikit.core
 
 
 @caikit.core.block("00112233-0405-0607-0809-0a0b02dd0e0f", "SampleBlock", "0.0.1")
 class SamplePrimitiveBlock(caikit.core.BlockBase):
@@ -37,12 +36,10 @@
         assert isinstance(bytes_type, bytes)
         return SampleOutputType(f"hello: primitives!")
 
     def save(self, model_path):
         module_saver = ModuleSaver(
             self,
             model_path=model_path,
-            library_name="sample_lib",
-            library_version=lib_config.library_version,
         )
         with module_saver:
             pass
```

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 A sample block for sample things!
 """
 # Local
-from ...config import lib_config
 from ...data_model.sample import SampleInputType, SampleOutputType, SampleTrainingType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
 
 @caikit.core.block("00110203-0405-0607-0809-0a0b02dd0e0f", "SampleBlock", "0.0.1")
@@ -41,16 +40,14 @@
             raise ValueError(f"{self.POISON_PILL_NAME} is not allowed!")
         return SampleOutputType(f"Hello {sample_input.name}")
 
     def save(self, model_path):
         module_saver = ModuleSaver(
             self,
             model_path=model_path,
-            library_name="sample_lib",
-            library_version=lib_config.library_version,
         )
         with module_saver:
             config_options = {
                 "train": {
                     "batch_size": self.batch_size,
                     "learning_rate": self.learning_rate,
                 },
```

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.2.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     def _load(cls, workflow_loader: WorkflowLoader):
         return SampleWorkflow(workflow_loader.load_module("dummy_model"))
 
     def save(self, model_path):
         saver = WorkflowSaver(
             module=self,
             model_path=model_path,
-            library_name="sample_lib",
-            library_version="0.0.1",
         )
         with saver:
             saver.save_module(self.block, "dummy_model")
 
     @classmethod
     def train(cls, sample_block: SampleBlock) -> "SampleWorkflow":
         return cls(sample_block)
```

### Comparing `caikit-0.1.6/tests/runtime/generated/__init__.py` & `caikit-0.2.0/tests/runtime/metrics/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# Standard
-import os
-import sys
-
-# Allow generated _pb2 files in here to import each other
-script_loc = os.path.dirname(os.path.realpath(__file__))
-sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.1.6/tests/runtime/metrics/__init__.py` & `caikit-0.2.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.2.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/metrics/test_throughput.py` & `caikit-0.2.0/tests/runtime/metrics/test_throughput.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 from prometheus_client import core, parser, start_http_server
 import requests
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.runtime.metrics.throughput import Throughput
-from caikit.runtime.utils.config_parser import ConfigParser
 
 log = alog.use_channel("TEST-THROUGHPT")
 # add 1 to get a new unused metrics port for this test. (Can't seem to shutdown the prometheus server)
-METRICS_PORT = int(ConfigParser.get_instance().metrics_port) + 1
+METRICS_PORT = int(get_config().runtime.metrics.port) + 1
 
 
 def scrape_metrics() -> Dict[str, core.Metric]:
     r = requests.get("http://localhost:{}".format(METRICS_PORT))
     metrics = {}
     for metric in parser.text_string_to_metric_families(r.text):
         metrics[metric.name] = metric
```

### Comparing `caikit-0.1.6/tests/runtime/model_management/__init__.py` & `caikit-0.2.0/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/model_management/test_batcher.py` & `caikit-0.2.0/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/model_management/test_model_loader.py` & `caikit-0.2.0/tests/runtime/model_management/test_model_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 import uuid
 
 # Third Party
 import grpc
 import pytest
 
 # Local
+from caikit.config import get_config
 from caikit.core import ModuleConfig
 from caikit.core.blocks import base, block
 from caikit.core.module_backend_config import _CONFIGURED_BACKENDS, configure
 from caikit.core.module_backends import BackendBase, backend_types
 from caikit.core.module_backends.backend_types import register_backend_type
+from caikit.runtime.model_management import model_loader
 from caikit.runtime.model_management.batcher import Batcher
 from caikit.runtime.model_management.model_loader import ModelLoader
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
 from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model import SampleInputType, SampleOutputType
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 from tests.fixtures import Fixtures
 
 ## Helpers #####################################################################
 
 
 def _random_test_id():
     return "test-any-model-" + str(uuid.uuid4())
@@ -224,88 +225,82 @@
         """
         model = self.model_loader.load_model(
             "load_with_batch",
             Fixtures.get_good_model_path(),
             model_type="fake_batch_block",
         ).module()
         assert isinstance(model, Batcher)
-        assert (
-            model._batch_size
-            == ConfigParser.get_instance().batching.fake_batch_block.size
-        )
+        assert model._batch_size == get_config().runtime.batching.fake_batch_block.size
 
         # Make sure another model loads without batching
         model = self.model_loader.load_model(
             "load_without_batch",
             Fixtures.get_good_model_path(),
             model_type=Fixtures.get_good_model_type(),
         ).module()
         assert not isinstance(model, Batcher)
 
     def test_with_batching_by_default(self):
         """Make sure that a model type without specific batching enabled will
         load with a batcher if default is enabled
         """
-        with temp_config_parser({"batching": {"default": {"size": 10}}}) as cfg:
+        with temp_config({"runtime": {"batching": {"default": {"size": 10}}}}) as cfg:
             model = self.model_loader.load_model(
                 "load_with_batch_default",
                 Fixtures.get_good_model_path(),
                 model_type=Fixtures.get_good_model_type(),
             ).module()
             assert isinstance(model, Batcher)
-            assert model._batch_size == cfg.batching.default.size
+            assert model._batch_size == cfg.runtime.batching.default.size
 
     def test_with_batching_collect_delay(self):
         """Make sure that a non-zero collect_delay_s is read correctly"""
         model_type = Fixtures.get_good_model_type()
-        with temp_config_parser(
+        with temp_config(
             {
-                "batching": {
-                    model_type: {
-                        "size": 10,
-                        "collect_delay_s": 0.01,
-                    },
+                "runtime": {
+                    "batching": {
+                        model_type: {
+                            "size": 10,
+                            "collect_delay_s": 0.01,
+                        },
+                    }
                 }
             }
         ) as cfg:
             model = self.model_loader.load_model(
                 "load_with_batch_default",
                 Fixtures.get_good_model_path(),
                 model_type=model_type,
             ).module()
             assert isinstance(model, Batcher)
-            assert model._batch_size == getattr(cfg.batching, model_type).size
+            assert model._batch_size == getattr(cfg.runtime.batching, model_type).size
             assert (
                 model._batch_collect_delay_s
-                == getattr(cfg.batching, model_type).collect_delay_s
+                == getattr(cfg.runtime.batching, model_type).collect_delay_s
             )
 
     def test_load_distributed_impl(self):
         """Make sure that when configured, an alternate distributed
         implementation of a block can be loaded
         """
         with tempfile.TemporaryDirectory() as model_path:
             # Create and save the model directly with the local impl
             SampleBlock().save(model_path)
 
             model_type = "gadget"
             with reset_distributed_config():
-                with temp_config_parser(
+                with temp_config(
                     {
-                        "distributed": {
+                        "module_backends": {
                             "enabled": True,
-                            "config": {
-                                "backend_priority": [
-                                    backend_types.TEST,
-                                    backend_types.LOCAL,
-                                ],
-                            },
-                            "preferred_backends": {
-                                model_type: backend_types.TEST,
-                            },
+                            "priority": [
+                                backend_types.TEST,
+                                backend_types.LOCAL,
+                            ],
                         },
                     }
                 ):
                     with temp_model_loader() as model_loader:
                         # Load the distributed version
                         model = model_loader.load_model(
                             "remote_gadget",
```

### Comparing `caikit-0.1.6/tests/runtime/model_management/test_model_manager.py` & `caikit-0.2.0/tests/runtime/model_management/test_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 import unittest
 import uuid
 
 # Third Party
 import grpc
 
 # Local
+from caikit import get_config
 from caikit.core.blocks.base import BlockBase
 from caikit.core.module_backend_config import _CONFIGURED_BACKENDS, configure
 from caikit.runtime.model_management.loaded_model import LoadedModel
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils import config_parser
-from caikit.runtime.utils.config_parser import ConfigParser
 from caikit.runtime.utils.import_util import get_dynamic_module
+from tests.conftest import temp_config
 from tests.fixtures import Fixtures
 
 
 def _random_test_id():
     return "test-any-model-" + str(uuid.uuid4())
 
 
@@ -90,23 +90,23 @@
                 Fixtures.get_good_model_path(), os.path.join(tempdir, "model1")
             )
             shutil.copy(
                 Fixtures.get_good_model_archive_path(),
                 os.path.join(tempdir, "model2.zip"),
             )
             ModelManager._ModelManager__instance = None
-            ConfigParser.get_instance().local_models_dir = tempdir
-            self.model_manager = ModelManager()
+            with temp_config({"runtime": {"local_models_dir": tempdir}}):
+                self.model_manager = ModelManager()
 
-            self.assertEqual(len(self.model_manager.loaded_models), 2)
-            self.assertIn("model1", self.model_manager.loaded_models.keys())
-            self.assertIn("model2.zip", self.model_manager.loaded_models.keys())
-            self.assertNotIn(
-                "model-does-not-exist.zip", self.model_manager.loaded_models.keys()
-            )
+                self.assertEqual(len(self.model_manager.loaded_models), 2)
+                self.assertIn("model1", self.model_manager.loaded_models.keys())
+                self.assertIn("model2.zip", self.model_manager.loaded_models.keys())
+                self.assertNotIn(
+                    "model-does-not-exist.zip", self.model_manager.loaded_models.keys()
+                )
 
     def test_model_manager_raises_if_all_local_models_fail_to_load(self):
         with TemporaryDirectory() as tempdir:
             shutil.copy(
                 Fixtures.get_bad_model_archive_path(), os.path.join(tempdir, "model1")
             )
             shutil.copy(
@@ -248,15 +248,14 @@
         """Test model size's model is None error response"""
         with self.assertRaises(CaikitRuntimeException) as context:
             self.model_manager.get_model_size(None)
         self.assertEqual(context.exception.status_code, grpc.StatusCode.NOT_FOUND)
 
     def test_estimate_model_size_ok_response_on_loaded_model(self):
         """Test if loaded model correctly returns model size"""
-        print("CONFIGUREREREDDDD", _CONFIGURED_BACKENDS)
         self.model_manager.load_model(
             model_id=_random_test_id(),
             local_model_path=Fixtures.get_good_model_path(),
             model_type=Fixtures.get_good_model_type(),
         )
         self.assertTrue(
             self.model_manager.estimate_model_size(
@@ -272,15 +271,15 @@
                 "test", Fixtures.get_good_model_path(), Fixtures.get_good_model_type()
             )
             > 0
         )
 
     def test_estimate_model_size_by_type(self):
         """Test that a model's size is estimated differently based on its type"""
-        config = config_parser.ConfigParser.get_instance()
+        config = get_config().inference_plugin.model_mesh
         self.assertTrue(Fixtures.get_good_model_type() in config.model_size_multipliers)
 
         typed_model_size = self.model_manager.estimate_model_size(
             "test", Fixtures.get_good_model_path(), Fixtures.get_good_model_type()
         )
         untyped_model_size = self.model_manager.estimate_model_size(
             "test", Fixtures.get_good_model_path(), "test-not-a-model-type"
```

### Comparing `caikit-0.1.6/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.2.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from tempfile import TemporaryDirectory
-from unittest.mock import MagicMock, patch
 import os
-import pathlib
 import unittest
 import uuid
 
 # Third Party
 import grpc
 
 # Local
+from caikit import get_config
 from caikit.runtime.model_management.model_sizer import ModelSizer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.config_parser import ConfigParser
+from tests.conftest import temp_config
 from tests.fixtures import Fixtures
 
 
 def _random_test_id() -> str:
     return "test-any-model-" + str(uuid.uuid4())
 
 
@@ -38,15 +37,14 @@
 
 
 class TestModelSizer(unittest.TestCase):
     """This test suite tests the model sizer class"""
 
     def setUp(self):
         """This method runs before each test begins to run"""
-        self.config = ConfigParser.get_instance()
         self.model_sizer = ModelSizer.get_instance()
 
     @staticmethod
     def _add_file(path, charsize) -> int:
         with open(path, "w") as f:
             content = ""
             for i in range(charsize):
@@ -61,46 +59,58 @@
 
             # add a nested file as well
             subdir = os.path.join(d, "some_dir")
             os.makedirs(subdir)
             total_size += TestModelSizer._add_file(
                 os.path.join(subdir, "some_file"), 512
             )
-
             model_type = _random_test_model_type()
             mult = 7
-            self.config.model_size_multipliers[model_type] = mult
-            expected_size = total_size * mult
-
-            size = self.model_sizer.get_model_size(
-                model_id=_random_test_id(),
-                local_model_path=d,
-                model_type=model_type,
-            )
-            self.assertEqual(size, expected_size)
+            with temp_config(
+                {
+                    "inference_plugin": {
+                        "model_mesh": {"model_size_multipliers": {model_type: mult}}
+                    }
+                }
+            ):
+                expected_size = total_size * mult
+                size = self.model_sizer.get_model_size(
+                    model_id=_random_test_id(),
+                    local_model_path=d,
+                    model_type=model_type,
+                )
+                self.assertEqual(size, expected_size)
 
     def test_it_can_size_a_model_archive(self):
         """Get local model archive file size"""
         model_type = _random_test_model_type()
         mult = 42
-        self.config.model_size_multipliers[model_type] = mult
-        expected_size = os.path.getsize(Fixtures.get_good_model_archive_path()) * mult
+        with temp_config(
+            {
+                "inference_plugin": {
+                    "model_mesh": {"model_size_multipliers": {model_type: mult}}
+                }
+            }
+        ):
+            expected_size = (
+                os.path.getsize(Fixtures.get_good_model_archive_path()) * mult
+            )
 
-        size = self.model_sizer.get_model_size(
-            model_id=_random_test_id(),
-            local_model_path=Fixtures.get_good_model_archive_path(),
-            model_type=model_type,
-        )
-        self.assertEqual(size, expected_size)
+            size = self.model_sizer.get_model_size(
+                model_id=_random_test_id(),
+                local_model_path=Fixtures.get_good_model_archive_path(),
+                model_type=model_type,
+            )
+            self.assertEqual(size, expected_size)
 
     def test_it_uses_the_default_multiplier_for_unknown_model_types(self):
         model_type = "definitely not a real type"
         expected_size = (
             os.path.getsize(Fixtures.get_good_model_archive_path())
-            * self.config.default_model_size_multiplier
+            * get_config().inference_plugin.model_mesh.default_model_size_multiplier
         )
 
         size = self.model_sizer.get_model_size(
             model_id=_random_test_id(),
             local_model_path=Fixtures.get_good_model_archive_path(),
             model_type=model_type,
         )
```

### Comparing `caikit-0.1.6/tests/runtime/model_management/test_training_manager.py` & `caikit-0.2.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.2.0/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/test_create_service.py` & `caikit-0.2.0/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.2.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DataStreamSourceBase,
     _make_data_stream_source_type_name,
     get_data_stream_source,
     make_data_stream_source,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.data_model.sample import SampleTrainingType
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 import caikit
 
 ################################################
 # Fixtures
 
 
 @pytest.fixture
@@ -214,15 +214,15 @@
 
 
 def test_data_stream_source_base_path():
     """Make sure that a globally configured base path is used"""
     stream_source = make_data_stream_source(int)
     source_data = [1, 2, 3, 4]
     with tempfile.TemporaryDirectory() as workdir:
-        with temp_config_parser({"data_streams": {"file_source_base": workdir}}):
+        with temp_config({"data_streams": {"file_source_base": workdir}}):
             nested_dir = os.path.join("foo", "bar")
             full_nested_dir = os.path.join(workdir, nested_dir)
             os.makedirs(full_nested_dir)
             fname = os.path.join(nested_dir, "data.json")
             full_fname = os.path.join(workdir, fname)
             with open(full_fname, "w") as handle:
                 handle.write(json.dumps(source_data))
```

### Comparing `caikit-0.1.6/tests/runtime/service_generation/test_primitives.py` & `caikit-0.2.0/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.2.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/servicers/__init__.py` & `caikit-0.2.0/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.2.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.2.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 import time
 import uuid
 
 # Third Party
 import pytest
 
 # Local
-from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
 from sample_lib.data_model.sample import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 from tests.fixtures import Fixtures
-from tests.fixtures.protobufs import primitive_party_pb2
 import caikit.core
 
 ## Helpers #####################################################################
 
 
 def _random_test_id():
     return "test-any-model-" + str(uuid.uuid4())
@@ -74,15 +72,15 @@
 
 
 @pytest.fixture(autouse=True, params=[True, False])
 def set_train_location(request):
     """This fixture ensures that all tests in this file will be run with both
     subprocess and local training styles
     """
-    with temp_config_parser({"training": {"use_subprocess": request.param}}):
+    with temp_config({"training": {"use_subprocess": request.param}}):
         yield
 
 
 # Train tests for the GlobalTrainServicer class ############################################################
 ##############
 # Normal cases
 ##############
```

### Comparing `caikit-0.1.6/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.2.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,38 +14,43 @@
 # Standard
 from threading import Event, Thread
 from unittest.mock import MagicMock, patch
 import time
 import unittest
 
 # Local
+from caikit import get_config
 from caikit.runtime.protobufs import model_runtime_pb2
 from caikit.runtime.servicers.model_runtime_servicer import ModelRuntimeServicerImpl
-from caikit.runtime.utils.config_parser import ConfigParser
 from tests.fixtures import Fixtures
 
 
 class TestModelRuntimeServicerImpl(unittest.TestCase):
     """This test suite tests the ModelRuntimeServicerImpl class"""
 
     def setUp(self):
         """This method runs before each test begins to run"""
         self.servicer = ModelRuntimeServicerImpl()
-        self.config = ConfigParser.get_instance()
 
     def test_model_load_sets_per_model_concurrency(self):
         model = "test-any-model-id"
         # Grab a model type that has some max concurrency set
-        model_type = list(self.config.max_model_concurrency_per_type.keys())[0]
+        model_type = list(
+            get_config().inference_plugin.model_mesh.max_model_concurrency_per_type.keys()
+        )[0]
         request = model_runtime_pb2.LoadModelRequest(
             modelId=model, modelType=model_type
         )
         context = Fixtures.build_context(model)
 
-        expected_concurrency = self.config.max_model_concurrency_per_type[model_type]
+        expected_concurrency = (
+            get_config().inference_plugin.model_mesh.max_model_concurrency_per_type[
+                model_type
+            ]
+        )
         mock_manager = MagicMock()
         mock_manager.load_model.return_value = 1
 
         with patch.object(self.servicer, "model_manager", mock_manager):
             response = self.servicer.loadModel(request, context)
         self.assertEqual(expected_concurrency, response.maxConcurrency)
 
@@ -53,15 +58,17 @@
         model = "test-any-model-id"
         model_type = "some-fake-model-type"
         request = model_runtime_pb2.LoadModelRequest(
             modelId=model, modelType=model_type
         )
         context = Fixtures.build_context(model)
 
-        expected_concurrency = self.config.max_model_concurrency
+        expected_concurrency = (
+            get_config().inference_plugin.model_mesh.max_model_concurrency
+        )
         mock_manager = MagicMock()
         mock_manager.load_model.return_value = 1
 
         with patch.object(self.servicer, "model_manager", mock_manager):
             response = self.servicer.loadModel(request, context)
         self.assertEqual(expected_concurrency, response.maxConcurrency)
```

### Comparing `caikit-0.1.6/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.2.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pytest
 
 # Local
 from caikit.interfaces.runtime.data_model import TrainingStatus
 from caikit.runtime.protobufs import process_pb2
 from caikit.runtime.servicers.model_train_servicer import ModelTrainServicerImpl
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 import sample_lib
 
 
 @pytest.fixture
 def sample_model_train_servicer(sample_train_service) -> ModelTrainServicerImpl:
     servicer = ModelTrainServicerImpl(training_service=sample_train_service)
     yield servicer
@@ -55,15 +55,15 @@
 
 
 @pytest.fixture(autouse=True, params=[True, False])
 def set_train_location(request):
     """This fixture ensures that all tests in this file will be run with both
     subprocess and local training styles
     """
-    with temp_config_parser({"training": {"use_subprocess": request.param}}):
+    with temp_config({"training": {"use_subprocess": request.param}}):
         yield
 
 
 #####################################################################
 # Error tests
```

### Comparing `caikit-0.1.6/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.2.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/test_grpc_server.py` & `caikit-0.2.0/tests/runtime/test_grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import pytest
 import tls_test_tools
 
 # First Party
 import alog
 
 # Local
+from caikit import get_config
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
     TrainingJob,
     TrainingStatus,
 )
 from caikit.runtime.grpc_server import RuntimeGRPCServer
@@ -44,22 +45,21 @@
 from caikit.runtime.protobufs import (
     model_runtime_pb2,
     model_runtime_pb2_grpc,
     process_pb2,
     process_pb2_grpc,
 )
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
-from caikit.runtime.utils.config_parser import ConfigParser
 from sample_lib.data_model import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 from tests.fixtures import Fixtures
 import caikit
 import sample_lib
 
 log = alog.use_channel("TEST-SERVE-I")
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
@@ -508,15 +508,15 @@
 
     model_size_request = model_runtime_pb2.ModelSizeRequest(modelId=loaded_model_id)
     actual_response = stub.modelSize(model_size_request)
     # Mar. 14, 23
     # The size of the directory pointed to by Fixtures.get_good_model_path() is 355 now.
     expected_size = (
         355
-        * ConfigParser.get_instance().model_size_multipliers[
+        * get_config().inference_plugin.model_mesh.model_size_multipliers[
             Fixtures.get_good_model_type()
         ]
     )
     assert abs(actual_response.sizeInBytes - expected_size) < 100
 
 
 def test_model_size_model_notfound_error_response(runtime_grpc_server):
@@ -536,19 +536,22 @@
     """Test run-time status successful response."""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
         runtime_grpc_server.make_local_channel()
     )
     runtime_status_request = model_runtime_pb2.RuntimeStatusRequest()
     actual_response = stub.runtimeStatus(runtime_status_request)
     assert actual_response.status == model_runtime_pb2.RuntimeStatusResponse.READY
-    assert actual_response.capacityInBytes == ConfigParser.get_instance().capacity
+    assert (
+        actual_response.capacityInBytes
+        == get_config().inference_plugin.model_mesh.capacity
+    )
     assert actual_response.maxLoadingConcurrency == 2
     assert (
         actual_response.modelLoadingTimeoutMs
-        == ConfigParser.get_instance().model_loading_timeout_ms
+        == get_config().inference_plugin.model_mesh.model_loading_timeout_ms
     )
     assert actual_response.defaultModelSizeInBytes == 18874368
     assert actual_response.numericRuntimeVersion == 0
 
 
 #### Health Probe tests ####
 def test_grpc_health_probe_ok_response(runtime_grpc_server):
@@ -730,18 +733,20 @@
 
 
 def test_out_of_range_port(sample_inference_service):
     """Test that the server can use a port outside of the default 8888-9000
     range
     """
     free_high_port = RuntimeGRPCServer._find_port(50000, 60000)
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_port": free_high_port,
-            "find_available_port": False,
+            "runtime": {
+                "port": free_high_port,
+                "find_available_port": False,
+            }
         }
     ):
         with RuntimeGRPCServer(
             infer_srv=sample_inference_service,
             train_srv=None,
         ) as server:
             _assert_connection(grpc.insecure_channel(f"localhost:{free_high_port}"))
```

### Comparing `caikit-0.1.6/tests/runtime/test_service_factory.py` & `caikit-0.2.0/tests/runtime/test_service_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for the service factory"""
 # Standard
-from types import ModuleType, SimpleNamespace
+from types import ModuleType
 
 # Third Party
 import pytest
 
 # Local
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from tests.conftest import temp_config_parser
+from tests.conftest import temp_config
 import caikit
 
 
 # 🌶️🌶️🌶️🌶️🌶️
 # Fixtures related to the protoc-compiled service interfaces created by `test/__init__.py`
 # These compiled fixtures should be deleted with a move to `json-to-service`d service interfaces
 @pytest.fixture
 def compiled_caikit_runtime_inference_pb2() -> ModuleType:
-    return ServicePackageFactory._get_service_proto_module("caikit_runtime_pb2")
+    return ServicePackageFactory._get_compiled_proto_module("caikit_runtime_pb2")
 
 
 @pytest.fixture
 def compiled_caikit_runtime_inference_pb2_grpc() -> ModuleType:
-    return ServicePackageFactory._get_service_proto_module("caikit_runtime_pb2_grpc")
+    return ServicePackageFactory._get_compiled_proto_module("caikit_runtime_pb2_grpc")
 
 
 @pytest.fixture
 def compiled_caikit_runtime_train_pb2() -> ModuleType:
-    return ServicePackageFactory._get_service_proto_module("caikit_runtime_train_pb2")
+    return ServicePackageFactory._get_compiled_proto_module("caikit_runtime_train_pb2")
 
 
 # /🌶️🌶️🌶️🌶️🌶️
 
 
 @pytest.fixture
 def compiled_inference_service() -> ServicePackage:
@@ -129,167 +129,189 @@
 #         get_servicer_stub(None)
 
 
 ### _get_service_proto_module #############################################################
 # Tests already existed - thus testing private method
 
 
-def test_invalid_get_service_proto_module_dir():
+def test_invalid_get_compiled_proto_module_dir():
     """If an invalid directory is provided, should throw module not found"""
 
-    mock_config = SimpleNamespace(
-        **{"service_proto_gen_module_dir": "invalid_proto_module_dir"}
-    )
-    with pytest.raises(ModuleNotFoundError):
-        ServicePackageFactory._get_service_proto_module(
-            "caikit_runtime_pb2", mock_config
-        )
+    with temp_config(
+        {"runtime": {"compiled_proto_module_dir": "invalid_proto_module_dir"}}
+    ):
+        with pytest.raises(ModuleNotFoundError):
+            ServicePackageFactory._get_compiled_proto_module("caikit_runtime_pb2")
 
 
-def test_invalid_get_service_proto_module():
-    """If an invalid module is provided to _get_service_proto_module, it throws a ValueError"""
+def test_invalid_get_compiled_proto_module():
+    """If an invalid module is provided to _get_compiled_proto_module, it throws a ValueError"""
 
-    mock_config = SimpleNamespace(
-        **{"service_proto_gen_module_dir": "tests.fixtures.protobufs"}
-    )
-    with pytest.raises(CaikitRuntimeException):
-        ServicePackageFactory._get_service_proto_module("invalid_module", mock_config)
+    with temp_config(
+        {"runtime": {"compiled_proto_module_dir": "tests.fixtures.protobufs"}}
+    ):
+        with pytest.raises(CaikitRuntimeException):
+            ServicePackageFactory._get_compiled_proto_module("invalid_module")
 
 
-def test_get_service_proto_module():
-    """If caikit_runtime_pb2 is provided to _get_service_proto_module, the module is returned"""
+def test_get_compiled_proto_module():
+    """If caikit_runtime_pb2 is provided to _get_compiled_proto_module, the module is returned"""
     # Local
     from tests.fixtures.protobufs import caikit_runtime_pb2
 
-    mock_config = SimpleNamespace(
-        **{"service_proto_gen_module_dir": "tests.fixtures.protobufs"}
-    )
-    service_proto_module = ServicePackageFactory._get_service_proto_module(
-        "caikit_runtime_pb2", mock_config
-    )
-    assert service_proto_module == caikit_runtime_pb2
+    with temp_config(
+        {"runtime": {"compiled_proto_module_dir": "tests.fixtures.protobufs"}}
+    ):
+        service_proto_module = ServicePackageFactory._get_compiled_proto_module(
+            "caikit_runtime_pb2"
+        )
+        assert service_proto_module == caikit_runtime_pb2
 
 
 # Local
 import sample_lib
 
 MODULE_LIST = [
     module_class
     for module_class in caikit.core.MODULE_REGISTRY.values()
     if module_class.__module__.partition(".")[0] == "sample_lib"
 ]
 
 ### Test ServicePackageFactory._get_and_filter_modules function
 def test_get_and_filter_modules_respects_excluded_task_type():
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
-        {"service_generation": {"task_types": {"excluded": ["sample_task"]}}}
+    with temp_config(
+        {
+            "runtime": {
+                "service_generation": {"task_types": {"excluded": ["sample_task"]}}
+            }
+        }
     ) as cfg:
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 1
         assert "sample_task" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_excluded_modules():
     assert "InnerBlock" in str(MODULE_LIST)
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "module_guids": {"excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]}
+            "runtime": {
+                "service_generation": {
+                    "module_guids": {
+                        "excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
+                    }
+                }
             }
         }  # excluding InnerBlock
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 5
         assert "InnerBlock" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_excluded_modules_and_excluded_task_type():
     assert "InnerBlock" in str(MODULE_LIST)
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "module_guids": {"excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]},
-                "task_types": {"excluded": ["other_task"]},
+            "runtime": {
+                "service_generation": {
+                    "module_guids": {
+                        "excluded": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
+                    },
+                    "task_types": {"excluded": ["other_task"]},
+                }
             }
         }  # excluding InnerBlock and OtherBlock
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 4
         assert "InnerBlock" not in str(clean_modules)
         assert "OtherBlock" not in str(clean_modules)
         assert "other_task" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_modules_and_included_task_types():
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "module_guids": {"included": ["00110203-baad-beef-0809-0a0b02dd0e0f"]},
-                "task_types": {"included": ["other_task"]},
+            "runtime": {
+                "service_generation": {
+                    "module_guids": {
+                        "included": ["00110203-baad-beef-0809-0a0b02dd0e0f"]
+                    },
+                    "task_types": {"included": ["other_task"]},
+                }
             }
         }  # only want InnerBlock and OtherBlock
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 2
         assert "InnerBlock" in str(clean_modules)
         assert "OtherBlock" in str(clean_modules)
         assert "ListBlock" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_modules():
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "module_guids": {
-                    "included": [
-                        "00110203-baad-beef-0809-0a0b02dd0e0f",
-                        "00af2203-0405-0607-0263-0a0b02dd0c2f",
-                    ]
-                },
+            "runtime": {
+                "service_generation": {
+                    "module_guids": {
+                        "included": [
+                            "00110203-baad-beef-0809-0a0b02dd0e0f",
+                            "00af2203-0405-0607-0263-0a0b02dd0c2f",
+                        ]
+                    },
+                }
             }
         }  # only want InnerBlock and ListBlock
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 2
         assert "InnerBlock" in str(clean_modules)
         assert "ListBlock" in str(clean_modules)
         assert "OtherBlock" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_task_types():
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "task_types": {"included": ["sample_task"]},
+            "runtime": {
+                "service_generation": {
+                    "task_types": {"included": ["sample_task"]},
+                }
             }
         }  # only want sample_task which has 5 modules
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 5
         assert "InnerBlock" in str(clean_modules)
         assert "OtherBlock" not in str(clean_modules)
 
 
 def test_get_and_filter_modules_respects_included_task_types_and_excluded_modules():
     assert len(MODULE_LIST) == 6  # there are 6 modules in sample_lib
-    with temp_config_parser(
+    with temp_config(
         {
-            "service_generation": {
-                "task_types": {"included": ["sample_task"]},
-                "module_guids": {"excluded": ["00af2203-0405-0607-0263-0a0b02dd0c2f"]},
+            "runtime": {
+                "service_generation": {
+                    "task_types": {"included": ["sample_task"]},
+                    "module_guids": {
+                        "excluded": ["00af2203-0405-0607-0263-0a0b02dd0c2f"]
+                    },
+                }
             }
         }  # only want sample_task but not ListBlock
     ) as cfg:
 
         clean_modules = ServicePackageFactory._get_and_filter_modules(cfg, "sample_lib")
         assert len(clean_modules) == 4
         assert "InnerBlock" in str(clean_modules)
```

### Comparing `caikit-0.1.6/tests/runtime/utils/__init__.py` & `caikit-0.2.0/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/utils/test_import_util.py` & `caikit-0.2.0/tests/runtime/utils/test_import_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
-from types import SimpleNamespace
 import inspect
 import sys
 
 # Third Party
 import pytest
 
 # Local
@@ -25,14 +24,15 @@
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import (
     UnifiedDataModel,
     clean_lib_names,
     get_data_model,
     get_dynamic_module,
 )
+from tests.conftest import temp_config
 
 ## Setup #########################################################################
 
 multi_lib_names = "caikit_libraryfoo[foo.bar]>=1.0.0-rc15 caikit_librarybar foo-bar==1"
 multi_lib_cleaned_list = ["caikit_libraryfoo", "caikit_librarybar", "foo_bar"]
 
 ## Tests ########################################################################
@@ -88,26 +88,26 @@
 
 
 ### get_data_model #############################################################
 
 
 def test_get_data_model_throws_on_nonimportable_lib():
     """If an invalid module is provided to get_data_model, it throws a ValueError"""
-    mock_config = SimpleNamespace(**{"caikit_library": "caikit_bad_lib"})
-    with pytest.raises(CaikitRuntimeException):
-        get_data_model(mock_config)
+    with temp_config({"runtime": {"library": "caikit_bad_lib"}}):
+        with pytest.raises(CaikitRuntimeException):
+            get_data_model()
 
 
 def test_get_data_model_ok_on_lib_with_no_data_model():
     """If a valid module with no data model is provided to get_data_model it
     returns an empty module object
     """
-    mock_config = SimpleNamespace(**{"caikit_library": "sys"})
-    data_model = get_data_model(mock_config)
-    assert isinstance(data_model, UnifiedDataModel)
+    with temp_config({"runtime": {"library": "sys"}}):
+        data_model = get_data_model()
+        assert isinstance(data_model, UnifiedDataModel)
 
 
 def test_get_data_model_is_accessible():
     """get_data_model should return the stuff in the `sample_lib.data_model` package"""
     # Local
     import sample_lib
 
@@ -123,25 +123,20 @@
 
 
 def test_multiple_caikit_libraries():
     """Make sure that multiple libraries can be imported and merged into a
     unified data model
     """
     lib_names = ["caikit.interfaces.runtime", "sample_lib"]
-    # sys.path.append(
-    #     os.path.realpath(
-    #         os.path.join(os.path.dirname(os.path.dirname(__file__)), "fixtures")
-    #     )
-    # )
-    mock_config = SimpleNamespace(**{"caikit_library": " ".join(lib_names)})
-    cdm = get_data_model(mock_config)
-    for lib_name in lib_names:
-        assert lib_name in sys.modules
-        lib_mod = sys.modules[lib_name]
-        attrs_match = [
-            (hasattr(cdm, attr_name) and getattr(cdm, attr_name) == attr_val)
-            for attr_name, attr_val in vars(lib_mod.data_model).items()
-            if not attr_name.startswith("_")
-            and inspect.isclass(attr_val)
-            and issubclass(attr_val, DataBase)
-        ]
-        assert all(attrs_match)
+    with temp_config({"runtime": {"library": " ".join(lib_names)}}):
+        cdm = get_data_model()
+        for lib_name in lib_names:
+            assert lib_name in sys.modules
+            lib_mod = sys.modules[lib_name]
+            attrs_match = [
+                (hasattr(cdm, attr_name) and getattr(cdm, attr_name) == attr_val)
+                for attr_name, attr_val in vars(lib_mod.data_model).items()
+                if not attr_name.startswith("_")
+                and inspect.isclass(attr_val)
+                and issubclass(attr_val, DataBase)
+            ]
+            assert all(attrs_match)
```

### Comparing `caikit-0.1.6/tests/runtime/utils/test_servicer_util.py` & `caikit-0.2.0/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.2.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.2.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.2.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.6/tox.ini` & `caikit-0.2.0/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 description = run tests with pytest with coverage
 deps =
     pytest>=6.2.5,<7.0
     pytest-cov>=2.10.1,<3.0
     pytest-html>=3.1.1,<4.0
     tls_test_tools>=0.1.1
     wheel>=0.38.4
-commands = pytest --cov=caikit --cov-report=term --cov-report=html tests
+passenv =
+    LOG_LEVEL
+    LOG_FILTERS
+    LOG_FORMATTER
+    LOG_THREAD_ID
+    LOG_CHANNEL_WIDTH
+commands = pytest --cov=caikit --cov-report=term --cov-report=html {posargs:tests}
 
 ; Unclear: We probably want to test wheel packaging
 ; But! tox will fail when this is set and _any_ interpreter is missing
 ; Without this, sdist packaging is tested so that's a start.
 package=wheel
 
 [testenv:fmt]
```

### Comparing `caikit-0.1.6/PKG-INFO` & `caikit-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.1.6
+Version: 0.2.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: alchemy-config>=1.0.0
+Requires-Dist: alchemy-config>=1.1.1
 Requires-Dist: alchemy-logging>=1.0.4
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
-Requires-Dist: ijson>=3.1.4,<3.2.0
+Requires-Dist: ijson>=3.1.4,<3.3.0
 Requires-Dist: munch>=2.5.0,<3.0
 Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: prometheus_client==0.12.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
-Requires-Dist: semver>=2.13.0,<3.0
+Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
 Requires-Dist: wheel>=0.37.0
 Requires-Dist: jtd-to-proto>=0.12.1,<0.13.0
 Requires-Dist: import-tracker>=3.1.5,<4
 Project-URL: Source, https://github.com/caikit/caikit
```

