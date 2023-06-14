# Comparing `tmp/caikit-0.7.1.tar.gz` & `tmp/caikit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.7.1.tar` & `caikit-0.8.0.tar`

### file list

```diff
@@ -1,303 +1,304 @@
--rw-r--r--   0        0        0       60 2023-06-09 23:28:18.429314 caikit-0.7.1/.coveragerc
--rw-r--r--   0        0        0      676 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1559 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1117 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      260 2023-06-09 23:28:18.429314 caikit-0.7.1/.gitignore
--rw-r--r--   0        0        0      324 2023-06-09 23:28:18.429314 caikit-0.7.1/.isort.cfg
--rw-r--r--   0        0        0      370 2023-06-09 23:28:18.429314 caikit-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-06-09 23:28:18.429314 caikit-0.7.1/.prettierignore
--rw-r--r--   0        0        0       12 2023-06-09 23:28:18.429314 caikit-0.7.1/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-06-09 23:28:18.433315 caikit-0.7.1/.pylintrc
--rw-r--r--   0        0        0      530 2023-06-09 23:28:18.433315 caikit-0.7.1/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2023-06-09 23:28:18.433315 caikit-0.7.1/.whitesource
--rw-r--r--   0        0        0      368 2023-06-09 23:28:18.433315 caikit-0.7.1/CODEOWNERS
--rw-r--r--   0        0        0     7164 2023-06-09 23:28:18.433315 caikit-0.7.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-06-09 23:28:18.433315 caikit-0.7.1/LICENSE
--rw-r--r--   0        0        0     4448 2023-06-09 23:28:18.433315 caikit-0.7.1/README.md
--rw-r--r--   0        0        0      152 2023-06-09 23:28:18.433315 caikit-0.7.1/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/config.py
--rw-r--r--   0        0        0     6388 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    37893 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2446 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4997 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    14620 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     5127 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/json_dict.py
--rw-r--r--   0        0        0     1564 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40244 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30320 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6247 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11042 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10721 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8221 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0     7590 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1662 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14335 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    15675 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0     9607 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     4229 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13127 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5613 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/protoable.py
--rw-r--r--   0        0        0    11999 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2216 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    10766 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    12451 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5440 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    11842 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0    11924 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/train_executors.py
--rw-r--r--   0        0        0      169 2023-06-09 23:28:18.437315 caikit-0.7.1/code-of-conduct.md
--rw-r--r--   0        0        0       90 2023-06-09 23:28:18.437315 caikit-0.7.1/docs-requirements.txt
--rw-r--r--   0        0        0      639 2023-06-09 23:28:18.437315 caikit-0.7.1/docs/Makefile
--rw-r--r--   0        0        0     6860 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/001-module.md
--rw-r--r--   0        0        0     1610 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/architecture_club/README.md
--rw-r--r--   0        0        0      805 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/make.bat
--rw-r--r--   0        0        0     3053 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/source/conf.py
--rw-r--r--   0        0        0      225 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/source/index.rst
--rw-r--r--   0        0        0      837 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1422 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      615 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3283 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1234 2023-06-09 23:28:21.565361 caikit-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-06-09 23:28:18.441315 caikit-0.7.1/releases.md
--rwxr-xr-x   0        0        0      639 2023-06-09 23:28:18.441315 caikit-0.7.1/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-06-09 23:28:18.441315 caikit-0.7.1/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-06-09 23:28:18.441315 caikit-0.7.1/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     5240 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/base.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/config/test_configs.py
--rw-r--r--   0        0        0    10361 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26951 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    25446 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     2358 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_json_dict.py
--rw-r--r--   0        0        0     1104 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4378 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    12551 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_imports.py
--rw-r--r--   0        0        0    21849 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     6133 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_task.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/__init__.py
--rw-r--r--   0        0        0     7967 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1017 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      508 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_no_id/config.yml
--rw-r--r--   0        0        0      508 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     3034 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      349 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      396 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0       24 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      296 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1946 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      250 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      902 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1410 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      364 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     4035 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    17954 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     3105 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_protoable.py
--rw-r--r--   0        0        0     2345 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     8381 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    16256 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     4088 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7776 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    35791 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5072 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    17336 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3819 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2617 2023-06-09 23:28:18.445315 caikit-0.7.1/tox.ini
--rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 caikit-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-06-14 15:11:43.801701 caikit-0.8.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1559 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1117 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      260 2023-06-14 15:11:43.801701 caikit-0.8.0/.gitignore
+-rw-r--r--   0        0        0      324 2023-06-14 15:11:43.801701 caikit-0.8.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-06-14 15:11:43.801701 caikit-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-06-14 15:11:43.801701 caikit-0.8.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-06-14 15:11:43.801701 caikit-0.8.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-06-14 15:11:43.801701 caikit-0.8.0/.pylintrc
+-rw-r--r--   0        0        0      530 2023-06-14 15:11:43.801701 caikit-0.8.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-06-14 15:11:43.801701 caikit-0.8.0/.whitesource
+-rw-r--r--   0        0        0      368 2023-06-14 15:11:43.801701 caikit-0.8.0/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-06-14 15:11:43.801701 caikit-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-06-14 15:11:43.801701 caikit-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4448 2023-06-14 15:11:43.801701 caikit-0.8.0/README.md
+-rw-r--r--   0        0        0      152 2023-06-14 15:11:43.801701 caikit-0.8.0/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    37893 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4997 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    15192 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4996 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40244 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30320 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6157 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11042 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10721 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0    10558 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/task.py
+-rw-r--r--   0        0        0      982 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     1648 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14335 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15629 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2606 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12089 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0     9572 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13127 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5613 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    12397 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    11024 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12451 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    12934 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    11924 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-06-14 15:11:43.809701 caikit-0.8.0/code-of-conduct.md
+-rw-r--r--   0        0        0       90 2023-06-14 15:11:43.809701 caikit-0.8.0/docs-requirements.txt
+-rw-r--r--   0        0        0      639 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0     6860 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/001-module.md
+-rw-r--r--   0        0        0     1610 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1422 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3283 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1234 2023-06-14 15:11:47.085731 caikit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2952 2023-06-14 15:11:43.809701 caikit-0.8.0/releases.md
+-rwxr-xr-x   0        0        0      639 2023-06-14 15:11:43.809701 caikit-0.8.0/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-06-14 15:11:43.809701 caikit-0.8.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-06-14 15:11:43.809701 caikit-0.8.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0    10738 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5034 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26951 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16237 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    25955 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    13033 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21743 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7497 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_task.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     7967 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0      326 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_streaming_module/config.yml
+-rw-r--r--   0        0        0     3034 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0       24 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      176 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1474 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1946 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      296 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      902 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1410 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0     1514 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
+-rw-r--r--   0        0        0      364 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    17954 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3105 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8381 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16259 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    36461 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    17337 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2617 2023-06-14 15:11:43.817701 caikit-0.8.0/tox.ini
+-rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 caikit-0.8.0/PKG-INFO
```

### Comparing `caikit-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.8.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.github/workflows/build-library.yml` & `caikit-0.8.0/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.github/workflows/lint-code.yml` & `caikit-0.8.0/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.github/workflows/publish-library.yml` & `caikit-0.8.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.pylintrc` & `caikit-0.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/.readthedocs.yaml` & `caikit-0.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/CONTRIBUTING.md` & `caikit-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/LICENSE` & `caikit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/README.md` & `caikit-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 
 ## Contributing
 
 Check out our [contributing](CONTRIBUTING.md) guide to learn how to contribute to Caikit.
 
 ## Code of conduct
 
-Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
+Participation in the Caikit community is governed by the [Code of Conduct](code-of-conduct.md).
```

### Comparing `caikit-0.7.1/caikit-overview.png` & `caikit-0.8.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/config/__init__.py` & `caikit-0.8.0/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/config/config.py` & `caikit-0.8.0/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/config/config.yml` & `caikit-0.8.0/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/__init__.py` & `caikit-0.8.0/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/__init__.py` & `caikit-0.8.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/base.py` & `caikit-0.8.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.8.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.8.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/schemes/base.py` & `caikit-0.8.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.8.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.8.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/__init__.py` & `caikit-0.8.0/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/base.py` & `caikit-0.8.0/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.8.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/data_backends/base.py` & `caikit-0.8.0/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.8.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/dataobject.py` & `caikit-0.8.0/caikit/core/data_model/dataobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,33 @@
         yet have been generated, but the set of fields will be known since the
         class will be the raw input representation of a @dataclass
         """
 
         # Get the annotations that will go into the dataclass
         if name != "DataObjectBase":
             field_names = attrs.get("__annotations__")
-            if field_names is None:
+            parent_dataobjects = [
+                base for base in bases if isinstance(base, _DataBaseMetaClass)
+            ]
+            field_name_sets = [base.fields for base in parent_dataobjects]
+            if field_names is not None:
+                field_name_sets = [field_names] + field_name_sets
+
+            # We need at least one field name set!
+            if not field_name_sets:
                 raise TypeError(
                     "All DataObjectBase classes must follow dataclass syntax"
                 )
+
+            # Flatten the field names
+            field_names = {
+                field_name
+                for field_name_set in field_name_sets
+                for field_name in field_name_set
+            }
             attrs[_DataBaseMetaClass._FWD_DECL_FIELDS] = field_names
 
         # Delegate to the base metaclass
         return super().__new__(mcs, name, bases, attrs)
 
 
 class DataObjectBase(DataBase, metaclass=_DataObjectBaseMetaClass):
```

### Comparing `caikit-0.7.1/caikit/core/data_model/enums.py` & `caikit-0.8.0/caikit/core/data_model/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 # Standard
 from enum import Enum
 from typing import Dict, Optional, Tuple, Type
 
 # Third Party
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
+import google
 import munch
 
 # First Party
 import alog
 
 # Local
 from ..toolkit.errors import error_handler
-from ..toolkit.isa import isprotobufenum
 
 log = alog.use_channel("DATAM")
 error = error_handler.get(log)
 
 
 @classmethod
 def to_dict(cls) -> Dict[str, int]:
@@ -135,7 +135,12 @@
     protobufs = current_globals.get("protobufs")
     all_enum_names = getattr(protobufs, "all_enum_names", [])
     for name in all_enum_names:
         proto_enum = getattr(protobufs, name)
         name, rev_name = import_enum(proto_enum)
         current_globals[name] = globals()[name]
         current_globals[rev_name] = globals()[rev_name]
+
+
+def isprotobufenum(obj):
+    """Returns True if obj is a protobufs enum."""
+    return isinstance(obj, google.protobuf.internal.enum_type_wrapper.EnumTypeWrapper)
```

### Comparing `caikit-0.7.1/caikit/core/data_model/json_dict.py` & `caikit-0.8.0/caikit/core/data_model/json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/producer.py` & `caikit-0.8.0/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.8.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/__init__.py` & `caikit-0.8.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/converter.py` & `caikit-0.8.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.8.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/data_stream.py` & `caikit-0.8.0/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/resolver.py` & `caikit-0.8.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/data_model/streams/validator.py` & `caikit-0.8.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/model_manager.py` & `caikit-0.8.0/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/module_backends/__init__.py` & `caikit-0.8.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/module_backends/backend_types.py` & `caikit-0.8.0/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/module_backends/base.py` & `caikit-0.8.0/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/module_backends/local_backend.py` & `caikit-0.8.0/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/module_backends/module_backend_config.py` & `caikit-0.8.0/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/__init__.py` & `caikit-0.8.0/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/base.py` & `caikit-0.8.0/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/config.py` & `caikit-0.8.0/caikit/core/modules/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import os
-import warnings
 
 # First Party
 import aconfig
 import alog
 
 # Local
 from .. import toolkit
@@ -59,24 +58,23 @@
                         "Do not add `{}` as top-level key in `config.yml`. "
                         "This is for internal use only.".format(reserved_key)
                     ),
                 )
 
         # 🌶️🌶️🌶️: Backwards compatibility for old-style `blocks`, `workflows`, and `resources`
         if not self.module_id:  # pylint: disable=access-member-before-definition
-            warnings.warn(
-                "No module_id found in config. Re-save the block to use module_id",
-                DeprecationWarning,
-            )  # actual warning or just log.warning?
+            log.warning(
+                "No module_id found in config. Re-save the model to use module_id."
+            )
             if self.block_id:
                 log.debug("Detected legacy block_id in config")
                 self.module_id = self.block_id
             elif self.workflow_id:
                 log.debug("Detected legacy workflow_id in config")
-                self.module_id = self.block_id
+                self.module_id = self.workflow_id
             elif self.resource_id:
                 log.debug("Detected legacy resource_id in config")
                 self.module_id = self.resource_id
 
         error.value_check(
             "<COR80418932E>",
             hasattr(self, "module_id"),
```

### Comparing `caikit-0.7.1/caikit/core/modules/decorator.py` & `caikit-0.8.0/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/loader.py` & `caikit-0.8.0/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/meta.py` & `caikit-0.8.0/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/modules/saver.py` & `caikit-0.8.0/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/registries.py` & `caikit-0.8.0/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/signature_parsing/__init__.py` & `caikit-0.8.0/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/signature_parsing/docstrings.py` & `caikit-0.8.0/caikit/core/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/signature_parsing/module_signature.py` & `caikit-0.8.0/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/signature_parsing/parsers.py` & `caikit-0.8.0/caikit/core/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/__init__.py` & `caikit-0.8.0/caikit/core/toolkit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 """Contains many helpers, utilities, and commonly re-used code in the `caikit.core` library. Users
 may find helpful methods in here for more advanced use of this library.
 """
 # Local
 from . import compatibility, logging
 from .errors import *
 from .fileio import *
-from .isa import *
 from .quality_evaluation import (
     EvalTypes,
     F1Metrics,
     F1MetricsContainer,
     QualityEvaluator,
 )
 from .serializers import *
```

### Comparing `caikit-0.7.1/caikit/core/toolkit/compatibility.py` & `caikit-0.8.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/errors/__init__.py` & `caikit-0.8.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.8.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.8.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/fileio.py` & `caikit-0.8.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/logging.py` & `caikit-0.8.0/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.8.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/serializers.py` & `caikit-0.8.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/core/toolkit/wip_decorator.py` & `caikit-0.8.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/__init__.py` & `caikit-0.8.0/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/common/__init__.py` & `caikit-0.8.0/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.8.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/common/data_model/producer.py` & `caikit-0.8.0/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/runtime/__init__.py` & `caikit-0.8.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.8.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.8.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/__init__.py` & `caikit-0.8.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/dump_services.py` & `caikit-0.8.0/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/grpc_server.py` & `caikit-0.8.0/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/interceptors/__init__.py` & `caikit-0.8.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.8.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
+from typing import Callable
 import traceback
 
 # Third Party
 from grpc._utilities import RpcMethodHandler
 from prometheus_client import Gauge
 import grpc
 
@@ -187,29 +188,34 @@
                 # caikit_runtime_pb2_grpc.add_CaikitRuntimeServicer_to_server
                 # for a dict of the rpc_method_handlers we wish to re-route)
                 rerouted_rpc_method_handlers = {}
                 for method, fqm in self.intercepted_methods():
                     # Get the original grpc.RpcMethodHandler for this RPC method
                     original_rpc_handler = handler.service(DummyHandlerCallDetails(fqm))
 
-                    # Make sure this is a unary-unary RPC
-                    if not original_rpc_handler.unary_unary:
-                        raise NotImplementedError("Unary-unary RPCs only!")
+                    # Make sure this is a supported RPC flavor
+                    if (
+                        not original_rpc_handler.unary_unary
+                        and not original_rpc_handler.unary_stream
+                    ):
+                        raise NotImplementedError(
+                            "Unary-unary and unary-stream RPCs only!"
+                        )
 
                     # Now, swap out the original unary-unary callable with our
                     # generic predict method, and add this newly re-routed RPC
                     # method handler to the dict of (method, handler) pairs
                     safe_rpc_handler = self._make_new_handler(original_rpc_handler)
                     rerouted_rpc_method_handlers[method] = safe_rpc_handler
                     log.info(
                         "<RUN30032825I>",
                         "Re-routing RPC %s from %s to %s",
                         fqm,
-                        original_rpc_handler.unary_unary,
-                        rerouted_rpc_method_handlers[method].unary_unary,
+                        self._get_handler_fn(original_rpc_handler),
+                        self._get_handler_fn(rerouted_rpc_method_handlers[method]),
                     )
 
                 # Now that we have re-rerouted all the original RPC method
                 # handlers to the global predict RPC method handler, it is time
                 # to bind them to the underlying server that we are wrapping
                 generic_handler = grpc.method_handlers_generic_handler(
                     self.intercepted_service(), rerouted_rpc_method_handlers
@@ -238,39 +244,30 @@
                 self._server.add_generic_rpc_handlers(generic_rpc_handlers)
 
     def _make_new_handler(
         self,
         original_rpc_handler: RpcMethodHandler,
         replace_with_global_predict: bool = True,
     ):
+        if replace_with_global_predict:
+            behavior = self.safe_rpc_wrapper(self._global_predict)
+        else:
+            behavior = self.safe_rpc_wrapper(self._get_handler_fn(original_rpc_handler))
+
         if original_rpc_handler.unary_unary:
-            return grpc.unary_unary_rpc_method_handler(
-                self.safe_rpc_wrapper(
-                    self._global_predict
-                    if replace_with_global_predict
-                    else original_rpc_handler.unary_unary
-                ),
-                request_deserializer=original_rpc_handler.request_deserializer,
-                response_serializer=original_rpc_handler.response_serializer,
-            )
-        if original_rpc_handler.unary_stream:
-            return grpc.unary_stream_rpc_method_handler(
-                self.safe_rpc_wrapper(original_rpc_handler.unary_stream),
-                request_deserializer=original_rpc_handler.request_deserializer,
-                response_serializer=original_rpc_handler.response_serializer,
-            )
-        if original_rpc_handler.stream_unary:
-            return grpc.stream_unary_rpc_method_handler(
-                self.safe_rpc_wrapper(original_rpc_handler.stream_unary),
-                request_deserializer=original_rpc_handler.request_deserializer,
-                response_serializer=original_rpc_handler.response_serializer,
-            )
-        # Else, it's stream-stream
-        return grpc.stream_stream_rpc_method_handler(
-            self.safe_rpc_wrapper(original_rpc_handler.stream_stream),
+            handler_constructor = grpc.unary_unary_rpc_method_handler
+        elif original_rpc_handler.unary_stream:
+            handler_constructor = grpc.unary_stream_rpc_method_handler
+        elif original_rpc_handler.stream_unary:
+            handler_constructor = grpc.stream_unary_rpc_method_handler
+        else:
+            handler_constructor = grpc.stream_stream_rpc_method_handler
+
+        return handler_constructor(
+            behavior=behavior,
             request_deserializer=original_rpc_handler.request_deserializer,
             response_serializer=original_rpc_handler.response_serializer,
         )
 
     # **************************************************************************
     # Pass-through (i.e., unchanged) grpc.Server methods
     # **************************************************************************
@@ -354,7 +351,17 @@
         The timeout argument works in the same way as threading.Event.wait().
         Args:
             timeout: A floating point number specifying a timeout for the operation in seconds.
         Returns:
             A bool indicates if the operation times out.
         """
         return self._server.wait_for_termination(timeout)
+
+    @staticmethod
+    def _get_handler_fn(handler: RpcMethodHandler) -> Callable:
+        if handler.unary_unary:
+            return handler.unary_unary
+        if handler.unary_stream:
+            return handler.unary_stream
+        if handler.stream_unary:
+            return handler.stream_unary
+        return handler.stream_stream
```

### Comparing `caikit-0.7.1/caikit/runtime/metrics/__init__.py` & `caikit-0.8.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.8.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/model_management/__init__.py` & `caikit-0.8.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/model_management/batcher.py` & `caikit-0.8.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/model_management/loaded_model.py` & `caikit-0.8.0/caikit/runtime/model_management/loaded_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Standard
-from typing import Type
-
 # First Party
 import alog
 
 # Local
 from caikit.core import ModuleBase
 
 log = alog.use_channel("LOADED-MODEL")
@@ -55,15 +52,15 @@
         self._model_path = ""
         self._model_type = ""
         self._size = None
 
     def id(self) -> str:
         return self._model_id
 
-    def module(self) -> Type[ModuleBase]:
+    def module(self) -> ModuleBase:
         return self._caikit_module
 
     def type(self) -> str:
         return self._model_type
 
     def path(self) -> str:
         return self._model_path
```

### Comparing `caikit-0.7.1/caikit/runtime/model_management/model_loader.py` & `caikit-0.8.0/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/model_management/model_manager.py` & `caikit-0.8.0/caikit/runtime/model_management/model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from collections import Counter as DictCounter
-from typing import Dict, Type
+from typing import Dict
 import gc
 import os
 import threading
 
 # Third Party
 from grpc import StatusCode
 from prometheus_client import Counter, Gauge, Summary
@@ -248,15 +248,15 @@
             local_model_path (string): Local path to the model.
             model_type (string): Type of the model
         Returns:
             Model_size (int) : Estimated size of the model in bytes.
         """
         return self.model_sizer.get_model_size(model_id, local_model_path, model_type)
 
-    def retrieve_model(self, model_id) -> Type[ModuleBase]:
+    def retrieve_model(self, model_id) -> ModuleBase:
         """Retrieve a model from the loaded model map by model ID.
 
         Args:
             model_id(string): Model ID of the model to retrieve
         Returns:
             response (caikit.core.module.ModuleBase):
                 A loaded Caikit model
```

### Comparing `caikit-0.7.1/caikit/runtime/model_management/model_sizer.py` & `caikit-0.8.0/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/model_management/training_manager.py` & `caikit-0.8.0/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/__init__.py` & `caikit-0.8.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.8.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.8.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.8.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.8.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.8.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/service_factory.py` & `caikit-0.8.0/caikit/runtime/service_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,48 +125,48 @@
 
         # Then do API introspection to come up with all the API definitions to support
         clean_modules = ServicePackageFactory._get_and_filter_modules(
             caikit_config, lib
         )
 
         if service_type == cls.ServiceType.INFERENCE:
-            task_rpc_list = service_generation.create_inference_rpcs(clean_modules)
+            rpc_list = service_generation.create_inference_rpcs(clean_modules)
             service_name = f"{ai_domain_name}Service"
         else:  # service_type == cls.ServiceType.TRAINING
-            task_rpc_list = service_generation.create_training_rpcs(clean_modules)
+            rpc_list = service_generation.create_training_rpcs(clean_modules)
             service_name = f"{ai_domain_name}TrainingService"
 
-        task_rpc_list = [rpc for rpc in task_rpc_list if rpc.return_type is not None]
+        rpc_list = [rpc for rpc in rpc_list if rpc.return_type is not None]
 
         request_data_models = [
-            rpc.create_request_data_model(package_name) for rpc in task_rpc_list
+            rpc.create_request_data_model(package_name) for rpc in rpc_list
         ]
 
         client_module = ModuleType(
             "ClientMessages",
             "Package with service message class implementations",
         )
 
         for dm_class in request_data_models:
             # We need the message class that data model serializes to
             setattr(client_module, dm_class.__name__, type(dm_class().to_proto()))
 
-        rpc_jsons = [rpc.create_rpc_json(package_name) for rpc in task_rpc_list]
+        rpc_jsons = [rpc.create_rpc_json(package_name) for rpc in rpc_list]
         service_json = {"service": {"rpcs": rpc_jsons}}
         grpc_service = json_to_service(
             name=service_name, package=package_name, json_service_def=service_json
         )
 
         return ServicePackage(
             service=grpc_service.service_class,
             descriptor=grpc_service.descriptor,
             registration_function=grpc_service.registration_function,
             stub_class=grpc_service.client_stub_class,
             messages=client_module,
-            caikit_rpcs=set(task_rpc_list),
+            caikit_rpcs=set(rpc_list),
         )
 
     # Implementation details for pure python service packages #
     @staticmethod
     def _get_and_filter_modules(
         caikit_config: aconfig.Config, lib: str
     ) -> Set[Type[ModuleBase]]:
```

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.8.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/create_service.py` & `caikit-0.8.0/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.8.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/protoable.py` & `caikit-0.8.0/caikit/runtime/service_generation/protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/rpcs.py` & `caikit-0.8.0/caikit/runtime/service_generation/rpcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 Typically used for `caikit.core.module`s that expose .train and .run functions.
 """
 # Standard
 from typing import Any, Dict, List, Optional, Type, Union, get_args, get_origin
 import abc
 import copy
+import typing
 
 # First Party
 from py_to_proto.dataclass_to_proto import (  # NOTE: Imported from here for compatibility
     Annotated,
     FieldNumber,
 )
 import alog
@@ -91,20 +92,30 @@
         )
         decorated_cls = decorator(cls_)
 
         return decorated_cls
 
     def create_rpc_json(self, package_name: str) -> Dict:
         """Return json snippet for the service definition of this RPC"""
-        output_type_name = self.return_type.get_proto_class().DESCRIPTOR.full_name
+        if self.module_list[0].TASK_CLASS.is_output_streaming_task():
+            output_type_name = (
+                typing.get_args(self.return_type)[0]
+                .get_proto_class()
+                .DESCRIPTOR.full_name
+            )
+            server_streaming = True
+        else:
+            output_type_name = self.return_type.get_proto_class().DESCRIPTOR.full_name
+            server_streaming = False
 
         rpc_json = {
             "name": f"{self.name}",
             "input_type": f"{package_name}.{self.request.name}",
             "output_type": output_type_name,
+            "server_streaming": server_streaming,
         }
         return rpc_json
 
 
 class ModuleClassTrainRPC(CaikitRPCBase):
     """Helper class to create a unique RPC corresponding with the train function
     for a given module class
```

### Comparing `caikit-0.7.1/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.8.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/servicers/__init__.py` & `caikit-0.8.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.8.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.service_generation.rpcs import TaskPredictRPC
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     build_proto_response,
+    build_proto_stream,
     get_metadata,
     validate_data_model,
 )
 from caikit.runtime.work_management.abortable_action import AbortableAction
 from caikit.runtime.work_management.call_aborter import CallAborter
 
 PREDICT_RPC_COUNTER = Counter(
@@ -133,95 +134,98 @@
                 A deserialized RPC request message
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
 
         Returns:
             response (object):
                 A Caikit Library data model response object
         """
-        desc_name = request.DESCRIPTOR.name
-        outer_scope_name = "GlobalPredictServicer.Predict:%s" % desc_name
+        request_name = request.DESCRIPTOR.name
+        outer_scope_name = "GlobalPredictServicer.Predict:%s" % request_name
         inner_scope_name = (
-            "GlobalPredictServicer.Predict.caikit_library_run:%s" % desc_name
+            "GlobalPredictServicer.Predict.caikit_library_run:%s" % request_name
         )
 
         try:
             with alog.ContextLog(log.debug, outer_scope_name):
                 # Make sure the request has a model before doing anything
                 model_id = get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY)
                 # Retrieve the model from the model manager
                 log.debug("<RUN52259029D>", "Retrieving model '%s'", model_id)
                 model = self._model_manager.retrieve_model(model_id)
 
-                self._verify_model_task(model, desc_name)
+                self._verify_model_task(model, request_name)
 
                 model_class = type(model)
                 # Unmarshall the request object into the required module run argument(s)
                 with PREDICT_FROM_PROTO_SUMMARY.labels(
-                    grpc_request=desc_name, model_id=model_id
+                    grpc_request=request_name, model_id=model_id
                 ).time():
                     caikit_library_request = build_caikit_library_request_dict(
                         request,
                         model_class.RUN_SIGNATURE,
                     )
 
                 # NB: we previously recorded the size of the request, and timed this module to
                 # provide a rudimentary throughput metric of size / time
                 with alog.ContextLog(log.debug, inner_scope_name):
                     with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
-                        grpc_request=desc_name, model_id=model_id
+                        grpc_request=request_name, model_id=model_id
                     ).time():
                         if self.use_abortable_threads:
                             work = AbortableAction(
                                 CallAborter(context),
                                 model.run,
                                 **caikit_library_request,
                             )
                             response = work.do()
                         else:
                             response = model.run(**caikit_library_request)
 
                 # Marshall the response to the necessary return type
                 with PREDICT_TO_PROTO_SUMMARY.labels(
-                    grpc_request=desc_name, model_id=model_id
+                    grpc_request=request_name, model_id=model_id
                 ).time():
-                    response_proto = build_proto_response(response)
+                    if model.TASK_CLASS.is_output_streaming_task():
+                        response_proto = build_proto_stream(response)
+                    else:
+                        response_proto = build_proto_response(response)
 
             # Update Prometheus metrics
             PREDICT_RPC_COUNTER.labels(
-                grpc_request=desc_name, code=StatusCode.OK.name, model_id=model_id
+                grpc_request=request_name, code=StatusCode.OK.name, model_id=model_id
             ).inc()
             if get_config().runtime.metering.enabled:
                 self.rpc_meter.update_metrics(str(type(model)))
             return response_proto
 
         except CaikitRuntimeException as e:
             log_dict = {
                 "log_code": "<RUN50530380W>",
                 "message": e.message,
                 "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
                 "error_id": e.id,
             }
             log.warning({**log_dict, **e.metadata})
             PREDICT_RPC_COUNTER.labels(
-                grpc_request=desc_name, code=e.status_code.name, model_id=model_id
+                grpc_request=request_name, code=e.status_code.name, model_id=model_id
             ).inc()
             raise e
 
         # Duplicate code in global_train_servicer
         # pylint: disable=duplicate-code
         except (TypeError, ValueError) as e:
             log_dict = {
                 "log_code": "<RUN490439039W>",
                 "message": repr(e),
                 "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
                 "stack_trace": traceback.format_exc(),
             }
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
-                grpc_request=desc_name,
+                grpc_request=request_name,
                 code=StatusCode.INVALID_ARGUMENT.name,
                 model_id=model_id,
             ).inc()
             raise CaikitRuntimeException(
                 StatusCode.INVALID_ARGUMENT,
                 f"Exception raised during inference. This may be a problem with your input: {e}",
             ) from e
@@ -231,15 +235,17 @@
                 "log_code": "<RUN49049070W>",
                 "message": repr(e),
                 "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
                 "stack_trace": traceback.format_exc(),
             }
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
-                grpc_request=desc_name, code=StatusCode.INTERNAL.name, model_id=model_id
+                grpc_request=request_name,
+                code=StatusCode.INTERNAL.name,
+                model_id=model_id,
             ).inc()
             raise CaikitRuntimeException(
                 StatusCode.INTERNAL, "Unhandled exception during prediction"
             ) from e
 
     def _verify_model_task(self, model: ModuleBase, request_name: str):
         """Raise if the model is not supported for the task"""
```

### Comparing `caikit-0.7.1/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.8.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.8.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.8.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.8.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/types/__init__.py` & `caikit-0.8.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/types/aborted_exception.py` & `caikit-0.8.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.8.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.8.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/utils/__init__.py` & `caikit-0.8.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/utils/import_util.py` & `caikit-0.8.0/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/utils/servicer_util.py` & `caikit-0.8.0/caikit/runtime/utils/servicer_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A generic module to help Predict and Train servicers
 """
 # Standard
-from typing import Any, Dict, Iterable, Union
+from typing import Any, Dict, Iterable, Iterator, Union
 import traceback
 
 # Third Party
 from google.protobuf.descriptor import Descriptor, FieldDescriptor, ServiceDescriptor
 from google.protobuf.message import Message as ProtoMessageType
 import grpc
 
 # First Party
 import alog
 
 # Local
+from caikit.core.data_model import DataStream
 from caikit.core.data_model.base import DataBase
 from caikit.core.signature_parsing import CaikitMethodSignature
 from caikit.interfaces.runtime.data_model.training_management import ModelPointer
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import get_data_model
 
@@ -61,15 +62,42 @@
             "No `%s` method for Caikit Library CDM class %s",
             method_name,
             caikit_library_class,
         )
         raise e
 
 
-def build_proto_response(caikit_library_response):
+def build_proto_stream(
+    caikit_library_response: Iterable[DataBase],
+) -> Iterator[ProtoMessageType]:
+    """Returns an iterator that serializes each item in the model's response to protobuf"""
+
+    def _proto_generator():
+        for item in caikit_library_response:
+            try:
+                yield item.to_proto()
+            except Exception as e:
+                log.warning(
+                    {
+                        "log_code": "<RUN11567943W>",
+                        "message": "Exception while serializing response from stream: "
+                        "{}".format(e),
+                        "stack_trace": traceback.format_exc(),
+                    }
+                )
+                raise CaikitRuntimeException(
+                    grpc.StatusCode.INTERNAL,
+                    "Could not serialize output in model response stream",
+                ) from e
+
+    return iter(DataStream(_proto_generator))
+
+
+def build_proto_response(caikit_library_response: DataBase) -> ProtoMessageType:
+    """Serializes a data model instance into a protobuf message"""
     try:
         return caikit_library_response.to_proto()
     except Exception as e:
         log.warning(
             {
                 "log_code": "<RUN11230943W>",
                 "message": "Exception while serializing response: {}".format(e),
```

### Comparing `caikit-0.7.1/caikit/runtime/work_management/__init__.py` & `caikit-0.8.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/work_management/abortable_action.py` & `caikit-0.8.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/work_management/call_aborter.py` & `caikit-0.8.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.8.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/caikit/runtime/work_management/train_executors.py` & `caikit-0.8.0/caikit/runtime/work_management/train_executors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/Makefile` & `caikit-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/adrs/001-module.md` & `caikit-0.8.0/docs/adrs/001-module.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/adrs/010-data-model-definition.md` & `caikit-0.8.0/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/adrs/015-runtime-service-generation.md` & `caikit-0.8.0/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/adrs/018-shared-backends.md` & `caikit-0.8.0/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/adrs/019-loader-stack.md` & `caikit-0.8.0/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/architecture_club/04-25-23.md` & `caikit-0.8.0/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/make.bat` & `caikit-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/docs/source/conf.py` & `caikit-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/start_runtime_with_sample_lib.py` & `caikit-0.8.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/README.md` & `caikit-0.8.0/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/client.py` & `caikit-0.8.0/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.8.0/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/start_runtime.py` & `caikit-0.8.0/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/pyproject.toml` & `caikit-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.7.1"
+version = "0.8.0"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -24,15 +24,15 @@
     "ijson>=3.1.4,<3.3.0",
     "import-tracker>=3.1.5,<4",
     "munch>=2.5.0,<4.0",
     "numpy>=1.20,<2",
     "prometheus_client>=0.12.0,<1.0",
     "protobuf>=3.19.0,<5",
     "py-grpc-prometheus>=0.7.0,<0.8",
-    "py-to-proto>=0.2.0,<0.3.0,!=0.2.1",
+    "py-to-proto>=0.3.0,<0.4.0,!=0.2.1",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
 ]
```

### Comparing `caikit-0.7.1/releases.md` & `caikit-0.8.0/releases.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Release Process
 
 This process is a work-in-progress until the first major release of the project.
 
-The process will utimately aim to have:
+The process will ultimately aim to have:
 
 - A published release date for the first caikit major release, upon the availability of the first beta release
 - A well-known cycle of release dates for caikit minor and patch releases, upon the availability of the first caikit major release
 - Minor releases backwards compatible with respect to the API, upon the availability of the first caikit major release
 
 ## Semantic versioning
 
 caikit versions are expressed as x.y.z, where x is the major version, y is the minor version, and z is the patch version, following [Semantic Versioning](https://semver.org/spec/v2.0.0.html) terminology.
 
-**Note:** One key principle of semantic versioning is that breaking API changes will only be deliverd in a major release. While all care will be taken to respect this, there may be a scenario (for example, a security fix or a bug fix) where we would have to break the AI for a non major release. This would only be considered if no other alternative is available.
+**Note:** One key principle of semantic versioning is that breaking API changes will only be delivered in a major release. While all care will be taken to respect this, there may be a scenario (for example, a security fix or a bug fix) where we would have to break the AI for a non major release. This would only be considered if no other alternative is available.
 
 ## Patch releases
 
 Patch releases provide users with bug fixes and security fixes. They do not contain new features.
 
 Patch releases should be done every second week on a Wednesday (assuming there are changes since the last release). A patch release to fix a high priority regression or security issue does not have to follow this schedule, but it is highly desirable that it is released on a Wednesday if possible.
```

### Comparing `caikit-0.7.1/scripts/check_deps.sh` & `caikit-0.8.0/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/scripts/fmt.sh` & `caikit-0.8.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/__init__.py` & `caikit-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/base.py` & `caikit-0.8.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/config/test_configs.py` & `caikit-0.8.0/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/conftest.py` & `caikit-0.8.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,27 +133,17 @@
 def runtime_grpc_server(
     sample_inference_service, sample_train_service
 ) -> RuntimeGRPCServer:
     with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=sample_train_service,
     ) as server:
-
-        grpc_thread = threading.Thread(
-            target=server.start,
-        )
-        grpc_thread.daemon = False
-        grpc_thread.start()
         _check_server_readiness(server)
         yield server
 
-        # teardown
-        server.stop(0)
-        grpc_thread.join()
-
 
 @pytest.fixture(scope="session")
 def inference_stub(sample_inference_service, runtime_grpc_server) -> Type:
     inference_stub = sample_inference_service.stub_class(
         runtime_grpc_server.make_local_channel()
     )
     return inference_stub
@@ -183,14 +173,19 @@
 
 @pytest.fixture
 def good_model_path() -> str:
     return Fixtures.get_good_model_path()
 
 
 @pytest.fixture
+def streaming_model_path() -> str:
+    return os.path.join(os.path.dirname(__file__), "fixtures", "dummy_streaming_module")
+
+
+@pytest.fixture
 def other_good_model_path() -> str:
     return Fixtures.get_other_good_model_path()
 
 
 @pytest.fixture
 def sample_task_model_id(good_model_path) -> str:
     """Loaded model ID using model manager load model implementation"""
@@ -204,14 +199,30 @@
     )
     yield model_id
 
     # teardown
     model_manager.unload_model(model_id)
 
 
+@pytest.fixture
+def streaming_task_model_id(streaming_model_path) -> str:
+    """Loaded model ID using model manager load model implementation"""
+    model_id = _random_id()
+    model_manager = ModelManager.get_instance()
+    model_manager.load_model(
+        model_id,
+        local_model_path=streaming_model_path,
+        model_type=Fixtures.get_good_model_type(),
+    )
+    yield model_id
+
+    # teardown
+    model_manager.unload_model(model_id)
+
+
 @pytest.fixture
 def other_task_model_id(other_good_model_path) -> str:
     """Loaded model ID using model manager load model implementation"""
     model_id = _random_id()
     model_manager = ModelManager.get_instance()
     # model load test already tests with archive - just using a model path here
     model_manager.load_model(
```

### Comparing `caikit-0.7.1/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.8.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.8.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.8.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         assert hasattr(dm, "Foo")
         assert issubclass(dm.Foo, DataBase)
 
         data_dict = {"foo": "asdf"}
         backend = DictBackend(data_dict)
         msg = dm.Foo.from_backend(backend)
         assert msg.foo == "asdf"
-        assert msg.which_oneof("foo") == "foostr"
+        assert msg.which_oneof("foo") == "foo_str"
 
 
 def test_dict_backend_invalid_field_error():
     """Make sure that an AttributeError is raised if an invalid field is
     requested
     """
     with temp_data_model(
```

### Comparing `caikit-0.7.1/tests/core/data_model/streams/test_converter.py` & `caikit-0.8.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.8.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.8.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/streams/test_resolver.py` & `caikit-0.8.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/streams/test_validator.py` & `caikit-0.8.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/test_base.py` & `caikit-0.8.0/tests/core/data_model/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,25 +223,25 @@
             },
             mock_compiled=True,
         )
     ) as dm:
         assert isinstance(dm.ThingOne, type)
         assert issubclass(dm.ThingOne, DataBase)
         assert not issubclass(dm.ThingOne, DataObjectBase)
-        assert set(dm.ThingOne.fields) == {"foostr", "fooint"}
+        assert set(dm.ThingOne.fields) == {"foo_str", "foo_int"}
 
         # Construct with the oneof name
         inst = dm.ThingOne(foo=1)
         assert inst.foo == 1
-        assert inst.which_oneof("foo") == "fooint"
+        assert inst.which_oneof("foo") == "foo_int"
 
         # Construct with field name
-        inst = dm.ThingOne(foostr="asdf")
+        inst = dm.ThingOne(foo_str="asdf")
         assert inst.foo == "asdf"
-        assert inst.which_oneof("foo") == "foostr"
+        assert inst.which_oneof("foo") == "foo_str"
 
         # Conflicting args
         with pytest.raises(TypeError):
             dm.ThingOne(foo=1, fooster="asdf")
 
 
 ##################
```

### Comparing `caikit-0.7.1/tests/core/data_model/test_dataobject.py` & `caikit-0.8.0/tests/core/data_model/test_dataobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 from caikit.core.data_model import enums
 from caikit.core.data_model.base import DataBase, _DataBaseMetaClass
 from caikit.core.data_model.data_backends.dict_backend import DictBackend
 from caikit.core.data_model.dataobject import (
     _AUTO_GEN_PROTO_CLASSES,
     render_dataobject_protos,
 )
+from caikit.core.data_model.enums import isprotobufenum
 from caikit.core.data_model.json_dict import JsonDict
-from caikit.core.toolkit.isa import isprotobufenum
 
 ## Helpers #####################################################################
 
 
 @pytest.fixture(autouse=True)
 def temp_dpool():
     """Fixture to isolate the descriptor pool used in each test"""
@@ -526,27 +526,27 @@
 def test_dataobject_oneof_from_backend():
     """Make sure that a oneof can be correctly accessed from a backend"""
 
     @dataobject
     class Foo(DataObjectBase):
         foo: Union[int, str]
 
-    data_dict1 = {"fooint": 1234}
+    data_dict1 = {"foo_int": 1234}
     backend1 = DictBackend(data_dict1)
     msg1 = Foo.from_backend(backend1)
     assert msg1.foo == 1234
-    assert msg1.fooint == 1234
-    assert msg1.which_oneof("foo") == "fooint"
+    assert msg1.foo_int == 1234
+    assert msg1.which_oneof("foo") == "foo_int"
 
     data_dict2 = {"foo": 1234}
     backend2 = DictBackend(data_dict2)
     msg2 = Foo.from_backend(backend2)
     assert msg2.foo == 1234
-    assert msg2.fooint == 1234
-    assert msg2.which_oneof("foo") == "fooint"
+    assert msg2.foo_int == 1234
+    assert msg2.which_oneof("foo") == "foo_int"
 
 
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
@@ -872,7 +872,31 @@
     assert desc.fields_by_name["foo"].type == fld.TYPE_INT64
     assert desc.fields_by_name["bar"].type == fld.TYPE_STRING
     assert desc.fields_by_name["baz"].type == fld.TYPE_STRING
     inst = Derived(1, "asdf", "qwer")
     assert inst.foo == 1
     assert inst.bar == "asdf"
     assert inst.baz == "qwer"
+
+
+def test_dataobject_function_inheritance(temp_dpool):
+    """Make sure inheritance works to override functionality without changing
+    the schema of the parent
+    """
+
+    @dataobject
+    class Base(DataObjectBase):
+        foo: int
+
+        def doit(self):
+            return self.foo * 2
+
+    @dataobject
+    class Derived(Base):
+        def doit(self):
+            return self.foo * 3
+
+    b_inst = Base(1)
+    assert b_inst.doit() == 2
+
+    d_inst = Derived(1)
+    assert d_inst.doit() == 3
```

### Comparing `caikit-0.7.1/tests/core/data_model/test_enums.py` & `caikit-0.8.0/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/test_json_dict.py` & `caikit-0.8.0/tests/core/data_model/test_json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/data_model/test_producer.py` & `caikit-0.8.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/helpers.py` & `caikit-0.8.0/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/module_backends/test_backend_types.py` & `caikit-0.8.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.8.0/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/modules/test_module.py` & `caikit-0.8.0/tests/core/modules/test_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,37 @@
     assert config.float == 0.5
     assert isinstance(config.nested, dict)
     assert config.nested.string == "world"
     assert config.nested.integer == 2
     assert config.nested.float == -0.123
 
 
+def test_backwards_compatibility_for_block():
+    config = ModuleConfig({"block_id": "123"})
+    assert config.module_id == "123"
+
+
+def test_backwards_compatibility_for_workflow():
+    config = ModuleConfig(
+        {
+            "workflow_id": "456",
+        }
+    )
+    assert config.module_id == "456"
+
+
+def test_backwards_compatibility_for_resource():
+    config = ModuleConfig(
+        {
+            "resource_id": "789",
+        }
+    )
+    assert config.module_id == "789"
+
+
 def test_reserved_keys():
     for reserved_key in ("model_path",):
         with pytest.raises(KeyError):
             ModuleConfig(
                 {
                     reserved_key: "x",
                     "module_class": "caikit.core.modules.dummy.Dummy",
```

### Comparing `caikit-0.7.1/tests/core/modules/test_module_metadata.py` & `caikit-0.8.0/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/signature_parsing/__init__.py` & `caikit-0.8.0/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.8.0/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/signature_parsing/test_parsers.py` & `caikit-0.8.0/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/test_imports.py` & `caikit-0.8.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/test_model_manager.py` & `caikit-0.8.0/tests/core/test_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,21 +172,18 @@
 
     def test_import_module_registry(self):
         """Make sure that the module registry can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
         from caikit.core.model_manager import module_registry  # isort: skip
 
     def test_load_model_with_no_module_id(self):
-        """Test that we can load a module with the legacy block_id instead of module_id, and that
-        a DeprecationWarning is raised.
-        """
+        """Test that we can load a module with the legacy block_id instead of module_id"""
         model_path = os.path.join(self.fixtures_dir, DUMMY_NO_ID_MODEL_NAME)
-        with pytest.deprecated_call():
-            model = caikit.core.load(model_path)
-            self.assertIsInstance(model, caikit.core.ModuleBase)
+        model = caikit.core.load(model_path)
+        self.assertIsInstance(model, caikit.core.ModuleBase)
 
 
 # Pytest tests #########################################################
 
 # Setup #########################################################################
 
 DUMMY_MODULE_ID = "foo"
```

### Comparing `caikit-0.7.1/tests/core/test_no_write_permissions.py` & `caikit-0.8.0/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/test_task.py` & `caikit-0.8.0/tests/core/test_task.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Tests #######################################################################
 # Standard
-from typing import Union
+from typing import Iterable, Union
 import uuid
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core import TaskBase, task
@@ -47,14 +47,60 @@
             required_parameters={"sample_input": SampleInputType},
             output_type=str,
         )
         class SampleTask(TaskBase):
             pass
 
 
+def test_task_decorator_can_have_iterable_output():
+    """This test covers tasks + modules with streaming output"""
+
+    @task(
+        required_parameters={"sample_input": SampleInputType},
+        output_type=Iterable[SampleOutputType],
+    )
+    class StreamingTask(TaskBase):
+        pass
+
+    @caikit.core.module(
+        id=str(uuid.uuid4()),
+        name="StreamingModule",
+        version="0.0.1",
+        task=StreamingTask,
+    )
+    class StreamingModule(caikit.core.ModuleBase):
+        def run(
+            self, sample_input: SampleInputType
+        ) -> caikit.core.data_model.DataStream[SampleOutputType]:
+            pass
+
+
+def test_task_iterator_raises_on_wrong_streaming_type():
+    @task(
+        required_parameters={"sample_input": SampleInputType},
+        output_type=Iterable[SampleOutputType],
+    )
+    class StreamingTask(TaskBase):
+        pass
+
+    with pytest.raises(TypeError, match="Wrong output type for module"):
+
+        @caikit.core.module(
+            id=str(uuid.uuid4()),
+            name="InvalidStreamingModule",
+            version="0.0.1",
+            task=StreamingTask,
+        )
+        class InvalidStreamingModule(caikit.core.ModuleBase):
+            def run(
+                self, sample_input: SampleInputType
+            ) -> caikit.core.data_model.DataStream[SampleInputType]:
+                pass
+
+
 def test_task_is_set_on_module_classes():
     assert hasattr(SampleModule, "TASK_CLASS")
     assert SampleModule.TASK_CLASS == SampleTask
 
 
 def test_task_can_be_inferred_from_parent_module():
     @caikit.core.modules.module(id="foobar", name="Stuff", version="0.0.1")
```

### Comparing `caikit-0.7.1/tests/core/toolkit/test_compatibility.py` & `caikit-0.8.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/toolkit/test_error_handler.py` & `caikit-0.8.0/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/toolkit/test_fileio.py` & `caikit-0.8.0/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.8.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/toolkit/test_serializers.py` & `caikit-0.8.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.8.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/data_model_helpers.py` & `caikit-0.8.0/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/config/config.yml` & `caikit-0.8.0/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/dummy_module.zip` & `caikit-0.8.0/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/dummy_module/config.yml` & `caikit-0.8.0/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.8.0/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/fixtures.py` & `caikit-0.8.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/invalid.zip` & `caikit-0.8.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/linux.txt` & `caikit-0.8.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.8.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Dummy data model object for testing
 """
+# Standard
+import typing
 
 # Local
 from caikit.core import DataObjectBase, TaskBase, dataobject, task
 
 
 @dataobject(package="caikit_data_model.sample_lib")
 class SampleInputType(DataObjectBase):
@@ -41,11 +43,19 @@
 )
 class SampleTask(TaskBase):
     """A sample `task` for our test models"""
 
 
 @task(
     required_parameters={"sample_input": SampleInputType},
+    output_type=typing.Iterable[SampleOutputType],
+)
+class StreamingTask(TaskBase):
+    """A streaming version of a task"""
+
+
+@task(
+    required_parameters={"sample_input": SampleInputType},
     output_type=OtherOutputType,
 )
 class OtherTask(TaskBase):
     """Another sample `task` for our test models"""
```

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/generated/__init__.py` & `caikit-0.8.0/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/metrics/__init__.py` & `caikit-0.8.0/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.8.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/__init__.py` & `caikit-0.8.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/test_batcher.py` & `caikit-0.8.0/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/test_model_loader.py` & `caikit-0.8.0/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/test_model_manager.py` & `caikit-0.8.0/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.8.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/model_management/test_training_manager.py` & `caikit-0.8.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/service_generation/test_create_service.py` & `caikit-0.8.0/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.8.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/service_generation/test_protoable.py` & `caikit-0.8.0/tests/runtime/service_generation/test_protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.8.0/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.8.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/servicers/__init__.py` & `caikit-0.8.0/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.8.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.8.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,16 @@
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(jsondata=stream_type.JsonData(data=[1])).to_proto()
     train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
         model_name="Other module Training",
         training_data=training_data,
         # either of the below lines work since it's a Union now
         # TODO create a separate test, lazy
-        # sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
-        sample_inputstr="sample",
+        # sample_input_sampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        sample_input_str="sample",
         batch_size=batch_size,
     )
 
     training_response = sample_train_servicer.Train(
         train_request, Fixtures.build_context("foo")
     )
     assert training_response.model_name == "Other module Training"
@@ -144,15 +144,15 @@
     assert (
         result.MODULE_CLASS
         == "sample_lib.modules.other_task.other_implementation.OtherModule"
     )
 
     inference_response = sample_predict_servicer.Predict(
         sample_inference_service.messages.OtherTaskRequest(
-            sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto()
+            sample_input_sampleinputtype=SampleInputType(name="Gabe").to_proto()
         ),
         Fixtures.build_context(training_response.model_name),
     )
     assert (
         inference_response
         == OtherOutputType(
             farewell=f"goodbye: Gabe {batch_size} times",
```

### Comparing `caikit-0.7.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.8.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.8.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.8.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/test_grpc_server.py` & `caikit-0.8.0/tests/runtime/test_grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,32 +178,51 @@
         == "sample_lib.modules.sample_task.sample_implementation.SampleModule"
     )
     # Fields with defaults have expected values
     assert result.batch_size == 64
     assert result.learning_rate == 0.0015
 
 
-def test_predict_fake_module_ok_response(
+def test_predict_sample_module_ok_response(
     sample_task_model_id, runtime_grpc_server, sample_inference_service
 ):
-    """Test RPC CaikitRuntime.WidgetPredict successful response"""
+    """Test RPC CaikitRuntime.SampleTaskPredict successful response"""
     stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     actual_response = stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", sample_task_model_id)]
     )
     assert actual_response == HAPPY_PATH_RESPONSE
 
 
-def test_predict_fake_module_error_response(
+def test_predict_streaming_module(
+    streaming_task_model_id, runtime_grpc_server, sample_inference_service
+):
+    """Test RPC CaikitRuntime.StreamingTaskPredict successful response"""
+    stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
+    predict_request = sample_inference_service.messages.StreamingTaskRequest(
+        sample_input=HAPPY_PATH_INPUT
+    )
+    stream = stub.StreamingTaskPredict(
+        predict_request, metadata=[("mm-model-id", streaming_task_model_id)]
+    )
+
+    count = 0
+    for response in stream:
+        assert response == HAPPY_PATH_RESPONSE
+        count += 1
+    assert count == 10
+
+
+def test_predict_sample_module_error_response(
     runtime_grpc_server, sample_inference_service
 ):
-    """Test RPC CaikitRuntime.WidgetPredict error response"""
+    """Test RPC CaikitRuntime.SampleTaskPredict error response"""
     with pytest.raises(grpc.RpcError) as context:
         stub = sample_inference_service.stub_class(
             runtime_grpc_server.make_local_channel()
         )
         predict_request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         )
@@ -215,15 +234,15 @@
 
 def test_rpc_validation_on_predict(
     sample_task_model_id, runtime_grpc_server, sample_inference_service
 ):
     """Check that the server catches models sent to the wrong task RPCs"""
     stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
     predict_request = sample_inference_service.messages.OtherTaskRequest(
-        sample_inputsampleinputtype=HAPPY_PATH_INPUT
+        sample_input_sampleinputtype=HAPPY_PATH_INPUT
     )
     with pytest.raises(grpc.RpcError) as context:
         stub.OtherTaskPredict(
             predict_request, metadata=[("mm-model-id", sample_task_model_id)]
         )
     assert context.value.code() == grpc.StatusCode.INVALID_ARGUMENT
     assert "Wrong inference RPC invoked for model class" in str(context.value)
@@ -348,29 +367,29 @@
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         file=stream_type.File(filename=sample_int_file)
     ).to_proto()
 
     train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
         model_name="Bar Training",
-        sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        sample_input_sampleinputtype=SampleInputType(name="Gabe").to_proto(),
         batch_size=100,
         training_data=training_data,
     )
     actual_response = train_stub.OtherTaskOtherModuleTrain(train_request)
     is_good_train_response(
         actual_response,
         HAPPY_PATH_TRAIN_RESPONSE,
         "Bar Training",
         training_management_stub,
     )
 
     # make sure the trained model can run inference, and the batch size 100 was used
     predict_request = sample_inference_service.messages.OtherTaskRequest(
-        sample_inputsampleinputtype=HAPPY_PATH_INPUT
+        sample_input_sampleinputtype=HAPPY_PATH_INPUT
     )
     trained_inference_response = inference_stub.OtherTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     expected_trained_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 100 times"
     ).to_proto()
```

### Comparing `caikit-0.7.1/tests/runtime/test_service_factory.py` & `caikit-0.8.0/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/utils/__init__.py` & `caikit-0.8.0/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/utils/test_import_util.py` & `caikit-0.8.0/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/utils/test_servicer_util.py` & `caikit-0.8.0/tests/runtime/utils/test_servicer_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[100, 120])
     ).to_proto()
 
     train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
         model_name="Bar Training",
-        sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        sample_input_sampleinputtype=SampleInputType(name="Gabe").to_proto(),
         batch_size=100,
         training_data=training_data,
     )
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.other_task.OtherModule.TRAIN_SIGNATURE,
     )
```

### Comparing `caikit-0.7.1/tests/runtime/work_management/__init__.py` & `caikit-0.8.0/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.8.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.8.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.8.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/tox.ini` & `caikit-0.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.7.1/PKG-INFO` & `caikit-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.7.1
+Version: 0.8.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
@@ -15,15 +15,15 @@
 Requires-Dist: ijson>=3.1.4,<3.3.0
 Requires-Dist: import-tracker>=3.1.5,<4
 Requires-Dist: munch>=2.5.0,<4.0
 Requires-Dist: numpy>=1.20,<2
 Requires-Dist: prometheus_client>=0.12.0,<1.0
 Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
-Requires-Dist: py-to-proto>=0.2.0,<0.3.0,!=0.2.1
+Requires-Dist: py-to-proto>=0.3.0,<0.4.0,!=0.2.1
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
 Project-URL: Source, https://github.com/caikit/caikit
 
@@ -76,9 +76,9 @@
 
 ## Contributing
 
 Check out our [contributing](CONTRIBUTING.md) guide to learn how to contribute to Caikit.
 
 ## Code of conduct
 
-Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
+Participation in the Caikit community is governed by the [Code of Conduct](code-of-conduct.md).
```

