# Comparing `tmp/corvic_engine-0.1.8.tar.gz` & `tmp/corvic_engine-0.1.9.tar.gz`

## Comparing `corvic_engine-0.1.8.tar` & `corvic_engine-0.1.9.tar`

### file list

```diff
@@ -1,157 +1,159 @@
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 corvic_engine-0.1.8/python/Cargo.toml
--rw-r--r--   0     1001      127     2076 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/expression_pb2.py
--rw-r--r--   0     1001      127     1690 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/expression_pb2.pyi
--rw-r--r--   0     1001      127      159 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0     1001      127      976 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/expression_pb2_grpc.pyi
--rw-r--r--   0     1001      127     2057 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/priv/private_pb2.py
--rw-r--r--   0     1001      127     1239 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/priv/private_pb2.pyi
--rw-r--r--   0     1001      127      159 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0     1001      127      976 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/priv/private_pb2_grpc.pyi
--rw-r--r--   0     1001      127   143172 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/validate_pb2.py
--rw-r--r--   0     1001      127    25824 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/validate_pb2.pyi
--rw-r--r--   0     1001      127      159 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0     1001      127      976 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/buf/validate/validate_pb2_grpc.pyi
--rw-r--r--   0     1001      127     1041 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/context/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/context/py.typed
--rw-r--r--   0     1001      127      139 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/embed/__init__.py
--rw-r--r--   0     1001      127     7171 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/embed/node2vec.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/embed/py.typed
--rw-r--r--   0     1001      127      946 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/engine/__init__.py
--rw-r--r--   0     1001      127     1335 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/engine/_native.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/engine/py.typed
--rw-r--r--   0     1001      127      388 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/__init__.py
--rw-r--r--   0     1001      127     1301 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/defaults.py
--rw-r--r--   0     1001      127      251 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/errors.py
--rw-r--r--   0     1001      127     4255 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/experiments.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/py.typed
--rw-r--r--   0     1001      127     2534 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/resources.py
--rw-r--r--   0     1001      127     6476 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/sources.py
--rw-r--r--   0     1001      127    20060 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/spaces.py
--rw-r--r--   0     1001      127     3371 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/model/wrapped_orm.py
--rw-r--r--   0     1001      127      528 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/__init__.py
--rw-r--r--   0     1001      127      156 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/errors.py
--rw-r--r--   0     1001      127     8870 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/feature_types.py
--rw-r--r--   0     1001      127    20852 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/ops.py
--rw-r--r--   0     1001      127     2043 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/proto_wrapper.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/py.typed
--rw-r--r--   0     1001      127     7232 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/op_graph/row_filters.py
--rw-r--r--   0     1001      127    11580 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/__init__.py
--rw-r--r--   0     1001      127     1091 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/base.py
--rw-r--r--   0     1001      127      512 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/errors.py
--rw-r--r--   0     1001      127     3115 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/ids.py
--rw-r--r--   0     1001      127     1747 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/keys.py
--rw-r--r--   0     1001      127    11453 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/mixins.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/py.typed
--rw-r--r--   0     1001      127     1486 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/orm/utc.py
--rw-r--r--   0     1001      127    14953 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/result/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/result/py.typed
--rw-r--r--   0     1001      127      822 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/sql/__init__.py
--rw-r--r--   0     1001      127    13633 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/sql/parse_ops.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/sql/py.typed
--rw-r--r--   0     1001      127     2876 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/sql/rockset.py
--rw-r--r--   0     1001      127      625 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/__init__.py
--rw-r--r--   0     1001      127      596 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/client.py
--rw-r--r--   0     1001      127      716 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/in_memory_executor.py
--rw-r--r--   0     1001      127      402 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/op_graph_executor.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/py.typed
--rw-r--r--   0     1001      127      727 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/staging.py
--rw-r--r--   0     1001      127     4446 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system/storage.py
--rw-r--r--   0     1001      127      176 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system_sqlite/__init__.py
--rw-r--r--   0     1001      127    10401 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system_sqlite/blob_store.py
--rw-r--r--   0     1001      127     4927 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system_sqlite/client.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system_sqlite/py.typed
--rw-r--r--   0     1001      127     5781 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/system_sqlite/staging.py
--rw-r--r--   0     1001      127      599 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/table/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/table/py.typed
--rw-r--r--   0     1001      127    11851 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/table/schema.py
--rw-r--r--   0     1001      127    17347 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/table/table.py
--rw-r--r--   0     1001      127     1080 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/version/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/version/py.typed
--rw-r--r--   0     1001      127      385 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/well_known_types/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/python/corvic/well_known_types/py.typed
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/__init__.py
--rw-------   0     1001      127     1392 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2.py
--rw-------   0     1001      127      872 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2.pyi
--rw-------   0     1001      127      159 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2_grpc.py
--rw-------   0     1001      127      400 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/v1/__init__.py
--rw-------   0     1001      127     5837 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2.py
--rw-------   0     1001      127     5360 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2.pyi
--rw-------   0     1001      127     9619 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2_grpc.py
--rw-------   0     1001      127     4438 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/v1/__init__.py
--rw-------   0     1001      127     7906 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2.py
--rw-------   0     1001      127     9638 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2.pyi
--rw-------   0     1001      127     9736 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2_grpc.py
--rw-------   0     1001      127     4460 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/v1/__init__.py
--rw-------   0     1001      127    18496 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2.py
--rw-------   0     1001      127    21631 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2.pyi
--rw-------   0     1001      127      159 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2_grpc.py
--rw-------   0     1001      127      400 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/v1/__init__.py
--rw-------   0     1001      127     2207 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2.py
--rw-------   0     1001      127     1543 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2.pyi
--rw-------   0     1001      127      159 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2_grpc.py
--rw-------   0     1001      127      400 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/__init__.py
--rw-------   0     1001      127     6556 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2.py
--rw-------   0     1001      127     5101 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2.pyi
--rw-------   0     1001      127    10158 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2_grpc.py
--rw-------   0     1001      127     4810 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2_grpc.pyi
--rw-------   0     1001      127     5412 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2.py
--rw-------   0     1001      127     4968 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2.pyi
--rw-------   0     1001      127     8150 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2_grpc.py
--rw-------   0     1001      127     5285 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v1/__init__.py
--rw-------   0     1001      127    10320 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2.py
--rw-------   0     1001      127     8246 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2.pyi
--rw-------   0     1001      127    23354 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2_grpc.py
--rw-------   0     1001      127    13658 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/__init__.py
--rw-------   0     1001      127     8663 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2.py
--rw-------   0     1001      127     6450 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2.pyi
--rw-------   0     1001      127    12855 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2_grpc.py
--rw-------   0     1001      127     9374 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2_grpc.pyi
--rw-------   0     1001      127     5337 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2.py
--rw-------   0     1001      127     2625 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2.pyi
--rw-------   0     1001      127     7714 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2_grpc.py
--rw-------   0     1001      127     3537 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2_grpc.pyi
--rw-------   0     1001      127     8207 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2.py
--rw-------   0     1001      127     5432 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2.pyi
--rw-------   0     1001      127     9791 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2_grpc.py
--rw-------   0     1001      127     5243 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2_grpc.pyi
--rw-------   0     1001      127     6167 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2.py
--rw-------   0     1001      127     4220 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2.pyi
--rw-------   0     1001      127     7973 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2_grpc.py
--rw-------   0     1001      127     4437 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/v1/__init__.py
--rw-------   0     1001      127    13234 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2.py
--rw-------   0     1001      127    16165 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2.pyi
--rw-------   0     1001      127      159 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2_grpc.py
--rw-------   0     1001      127      400 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/__init__.py
--rw-------   0     1001      127     2174 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2.py
--rw-------   0     1001      127     1985 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2.pyi
--rw-------   0     1001      127      159 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2_grpc.py
--rw-------   0     1001      127      400 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2_grpc.pyi
--rw-------   0     1001      127     1453 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2.py
--rw-------   0     1001      127      480 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2.pyi
--rw-------   0     1001      127     2670 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2_grpc.py
--rw-------   0     1001      127     1460 2024-03-20 23:33:18.000000 corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2_grpc.pyi
--rw-r--r--   0     1001      127    11713 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 corvic_engine-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127     9032 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/pyproject.toml
--rw-r--r--   0     1001      127     1015 2024-03-20 23:33:02.000000 corvic_engine-0.1.8/LICENSE
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 corvic_engine-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 corvic_engine-0.1.9/python/Cargo.toml
+-rw-r--r--   0     1001      127     2076 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/expression_pb2.py
+-rw-r--r--   0     1001      127     1690 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/expression_pb2.pyi
+-rw-r--r--   0     1001      127      159 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0     1001      127      976 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/expression_pb2_grpc.pyi
+-rw-r--r--   0     1001      127     2057 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/priv/private_pb2.py
+-rw-r--r--   0     1001      127     1239 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/priv/private_pb2.pyi
+-rw-r--r--   0     1001      127      159 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0     1001      127      976 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/priv/private_pb2_grpc.pyi
+-rw-r--r--   0     1001      127   143172 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/validate_pb2.py
+-rw-r--r--   0     1001      127    25824 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/validate_pb2.pyi
+-rw-r--r--   0     1001      127      159 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0     1001      127      976 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/buf/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0     1001      127     1041 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/context/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/context/py.typed
+-rw-r--r--   0     1001      127      139 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/embed/__init__.py
+-rw-r--r--   0     1001      127     7798 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/embed/node2vec.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/embed/py.typed
+-rw-r--r--   0     1001      127      946 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/engine/__init__.py
+-rw-r--r--   0     1001      127     1335 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/engine/_native.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/engine/py.typed
+-rw-r--r--   0     1001      127      388 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/__init__.py
+-rw-r--r--   0     1001      127     1301 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/defaults.py
+-rw-r--r--   0     1001      127      251 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/errors.py
+-rw-r--r--   0     1001      127     4308 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/experiments.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/py.typed
+-rw-r--r--   0     1001      127     2534 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/resources.py
+-rw-r--r--   0     1001      127     6476 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/sources.py
+-rw-r--r--   0     1001      127    22200 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/spaces.py
+-rw-r--r--   0     1001      127     3371 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/model/wrapped_orm.py
+-rw-r--r--   0     1001      127      528 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/__init__.py
+-rw-r--r--   0     1001      127      156 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/errors.py
+-rw-r--r--   0     1001      127     8870 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/feature_types.py
+-rw-r--r--   0     1001      127    20852 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/ops.py
+-rw-r--r--   0     1001      127     2043 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/proto_wrapper.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/py.typed
+-rw-r--r--   0     1001      127     7232 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/op_graph/row_filters.py
+-rw-r--r--   0     1001      127    11668 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/__init__.py
+-rw-r--r--   0     1001      127     1275 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/base.py
+-rw-r--r--   0     1001      127      512 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/errors.py
+-rw-r--r--   0     1001      127      382 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/func/__init__.py
+-rw-r--r--   0     1001      127     1486 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/func/utc_func.py
+-rw-r--r--   0     1001      127     1161 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/func/uuid_func.py
+-rw-r--r--   0     1001      127     3115 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/ids.py
+-rw-r--r--   0     1001      127     1747 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/keys.py
+-rw-r--r--   0     1001      127    11453 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/mixins.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/orm/py.typed
+-rw-r--r--   0     1001      127    14953 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/result/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/result/py.typed
+-rw-r--r--   0     1001      127      822 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/sql/__init__.py
+-rw-r--r--   0     1001      127    13633 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/sql/parse_ops.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/sql/py.typed
+-rw-r--r--   0     1001      127     2876 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/sql/rockset.py
+-rw-r--r--   0     1001      127      625 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/__init__.py
+-rw-r--r--   0     1001      127      596 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/client.py
+-rw-r--r--   0     1001      127      673 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/in_memory_executor.py
+-rw-r--r--   0     1001      127      378 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/op_graph_executor.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/py.typed
+-rw-r--r--   0     1001      127      659 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/staging.py
+-rw-r--r--   0     1001      127     4446 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system/storage.py
+-rw-r--r--   0     1001      127      176 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system_sqlite/__init__.py
+-rw-r--r--   0     1001      127    10401 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system_sqlite/blob_store.py
+-rw-r--r--   0     1001      127     4927 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system_sqlite/client.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system_sqlite/py.typed
+-rw-r--r--   0     1001      127     5775 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/system_sqlite/staging.py
+-rw-r--r--   0     1001      127      599 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/table/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/table/py.typed
+-rw-r--r--   0     1001      127    11851 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/table/schema.py
+-rw-r--r--   0     1001      127    17620 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/table/table.py
+-rw-r--r--   0     1001      127     1080 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/version/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/version/py.typed
+-rw-r--r--   0     1001      127      385 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/well_known_types/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/python/corvic/well_known_types/py.typed
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/__init__.py
+-rw-------   0     1001      127     1392 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2.py
+-rw-------   0     1001      127      872 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2.pyi
+-rw-------   0     1001      127      159 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2_grpc.py
+-rw-------   0     1001      127      400 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/v1/__init__.py
+-rw-------   0     1001      127     5837 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2.py
+-rw-------   0     1001      127     5360 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2.pyi
+-rw-------   0     1001      127     9619 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2_grpc.py
+-rw-------   0     1001      127     4438 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/v1/__init__.py
+-rw-------   0     1001      127     7906 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2.py
+-rw-------   0     1001      127     9638 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2.pyi
+-rw-------   0     1001      127     9736 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2_grpc.py
+-rw-------   0     1001      127     4460 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/v1/__init__.py
+-rw-------   0     1001      127    18496 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2.py
+-rw-------   0     1001      127    21631 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2.pyi
+-rw-------   0     1001      127      159 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2_grpc.py
+-rw-------   0     1001      127      400 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/v1/__init__.py
+-rw-------   0     1001      127     2207 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2.py
+-rw-------   0     1001      127     1543 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2.pyi
+-rw-------   0     1001      127      159 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2_grpc.py
+-rw-------   0     1001      127      400 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/__init__.py
+-rw-------   0     1001      127     6777 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2.py
+-rw-------   0     1001      127     5388 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2.pyi
+-rw-------   0     1001      127    10158 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2_grpc.py
+-rw-------   0     1001      127     4810 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2_grpc.pyi
+-rw-------   0     1001      127     5412 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2.py
+-rw-------   0     1001      127     4968 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2.pyi
+-rw-------   0     1001      127     8150 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2_grpc.py
+-rw-------   0     1001      127     5285 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v1/__init__.py
+-rw-------   0     1001      127    10320 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2.py
+-rw-------   0     1001      127     8246 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2.pyi
+-rw-------   0     1001      127    23354 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2_grpc.py
+-rw-------   0     1001      127    13658 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/__init__.py
+-rw-------   0     1001      127     8663 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2.py
+-rw-------   0     1001      127     6450 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2.pyi
+-rw-------   0     1001      127    12855 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2_grpc.py
+-rw-------   0     1001      127     9374 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2_grpc.pyi
+-rw-------   0     1001      127     5337 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2.py
+-rw-------   0     1001      127     2625 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2.pyi
+-rw-------   0     1001      127     7714 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2_grpc.py
+-rw-------   0     1001      127     3537 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2_grpc.pyi
+-rw-------   0     1001      127     8207 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2.py
+-rw-------   0     1001      127     5432 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2.pyi
+-rw-------   0     1001      127     9791 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2_grpc.py
+-rw-------   0     1001      127     5243 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2_grpc.pyi
+-rw-------   0     1001      127     6167 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2.py
+-rw-------   0     1001      127     4220 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2.pyi
+-rw-------   0     1001      127     7973 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2_grpc.py
+-rw-------   0     1001      127     4437 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/v1/__init__.py
+-rw-------   0     1001      127    13234 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2.py
+-rw-------   0     1001      127    16165 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2.pyi
+-rw-------   0     1001      127      159 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2_grpc.py
+-rw-------   0     1001      127      400 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/__init__.py
+-rw-r--r--   0     1001      127        0 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/__init__.py
+-rw-------   0     1001      127     2174 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2.py
+-rw-------   0     1001      127     1985 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2.pyi
+-rw-------   0     1001      127      159 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2_grpc.py
+-rw-------   0     1001      127      400 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2_grpc.pyi
+-rw-------   0     1001      127     1453 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2.py
+-rw-------   0     1001      127      480 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2.pyi
+-rw-------   0     1001      127     2670 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2_grpc.py
+-rw-------   0     1001      127     1460 2024-03-21 21:47:34.000000 corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    11713 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 corvic_engine-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      127     9032 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      127     1015 2024-03-21 21:47:19.000000 corvic_engine-0.1.9/LICENSE
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 corvic_engine-0.1.9/PKG-INFO
```

### Comparing `corvic_engine-0.1.8/python/Cargo.toml` & `corvic_engine-0.1.9/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/expression_pb2.py` & `corvic_engine-0.1.9/python/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/expression_pb2.pyi` & `corvic_engine-0.1.9/python/buf/validate/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/expression_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/buf/validate/expression_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/priv/private_pb2.py` & `corvic_engine-0.1.9/python/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/priv/private_pb2.pyi` & `corvic_engine-0.1.9/python/buf/validate/priv/private_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/priv/private_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/buf/validate/priv/private_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/validate_pb2.py` & `corvic_engine-0.1.9/python/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/validate_pb2.pyi` & `corvic_engine-0.1.9/python/buf/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/buf/validate/validate_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/buf/validate/validate_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/context/__init__.py` & `corvic_engine-0.1.9/python/corvic/context/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/embed/node2vec.py` & `corvic_engine-0.1.9/python/corvic/embed/node2vec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """Node2Vec embeddings."""
 
 from __future__ import annotations
 
-from collections.abc import Mapping, Sequence
-from typing import Any, Generic, TypeVar
+import functools
+from collections.abc import Mapping
+from typing import Any, TypeVar
 
 import numpy as np
 import numpy.typing as npt
+import polars as pl
 from tqdm.auto import trange
 
 from corvic import engine
+from corvic.result import BadArgumentError
 
 _MAX_SENTENCE_LEN = 10000
 
 K = TypeVar("K")
 
 
-class KeyedVectors(Generic[K]):
+class KeyedVectors:
     """Vectors whose entries are keyed by an arbitrary value.
 
     Used to represent embeddings.
     """
 
     _vectors: npt.NDArray[np.float32]
-    _key_to_index: dict[K, int]
-    _index_to_key: list[K]
+    _index_to_key: pl.Series
 
-    def __init__(self, *, dim: int, index_to_key: list[K], key_to_index: dict[K, int]):
+    def __init__(self, *, dim: int, index_to_key: pl.Series):
         """Create keyed vectors.
 
         Args:
           dim: dimension of vectors
           key_to_index: mapping of key to index
           index_to_key: mapping of index to key
         """
         self.dim = dim
-        self._key_to_index = key_to_index
         self._index_to_key = index_to_key
         self._vectors = self._initial_vectors(len(index_to_key), dim)
 
     @classmethod
     def _initial_vectors(cls, nrows: int, dim: int):
         rng = np.random.default_rng()
         vectors = rng.random((nrows, dim), dtype=np.float32)
@@ -52,94 +53,111 @@
         """Return the number of keys."""
         return len(self.index_to_key)
 
     def __getitem__(self, key: Any) -> npt.NDArray[np.float32]:
         """Return vector for key."""
         return self.vectors[self.key_to_index[key]]
 
-    @property
-    def key_to_index(self) -> Mapping[K, int]:
+    @functools.cached_property
+    def key_to_index(self) -> Mapping[str, int]:
         """Return a mapping from keys to index."""
-        return self._key_to_index
+        return {name: i for i, name in enumerate(self._index_to_key)}
 
     @property
-    def index_to_key(self) -> Sequence[K]:
+    def index_to_key(self) -> pl.Series:
         """Return a mapping from index to key."""
         return self._index_to_key
 
     @property
     def vectors(self) -> npt.NDArray[np.float32]:
         """Return raw vectors keyed by index space.
 
         Use KeyedVectors[key] to retrieve vectors by original key.
         """
         return self._vectors
 
 
-class Space(Generic[K]):
+class Space:
     """A feature space, i.e., a graph."""
 
     graph: engine.CSRGraph
-    _index_to_key: list[K]
-    _key_to_index: dict[K, int]
+    _index_to_key: pl.Series
 
     def __init__(
         self,
-        edges: Sequence[tuple[K, K]],
+        edges: pl.DataFrame,
         *,
         directed: bool = True,
     ):
         """Create a space from a sequence of edges."""
-        index_to_key: list[K] = []
-        key_to_index: dict[K, int] = {}
+        if len(edges.columns) != 2:  # noqa: PLR2004
+            raise BadArgumentError("edges DataFrame should have exactly two columns")
 
-        num_edges = len(edges)
-        edge_array = np.empty((num_edges, 2), dtype=np.uint32)
-        for idx, edge in enumerate(edges):
-            src = self._ensure_node(edge[0], key_to_index, index_to_key)
-            dst = self._ensure_node(edge[1], key_to_index, index_to_key)
-            edge_array[idx] = (src, dst)
+        start_name, end_name = edges.columns[0], edges.columns[1]
+        nodes = (
+            pl.DataFrame(
+                {"id": pl.concat([edges[start_name], edges[end_name]]).unique()}
+            )
+            .with_row_index()
+            .with_columns(pl.col("index").cast(pl.UInt32))
+        )
+
+        if len(edges):
+            edge_starts_by_index = (
+                edges.select([start_name])
+                .join(nodes, left_on=start_name, right_on="id", how="left")
+                .select(["index"])
+                .rename({"index": "start"})
+            )
+            edge_ends_by_index = (
+                edges.select([end_name])
+                .join(nodes, left_on=end_name, right_on="id", how="left")
+                .select(["index"])
+                .rename({"index": "end"})
+            )
+            edge_array = pl.concat(
+                [edge_starts_by_index, edge_ends_by_index], how="horizontal"
+            ).to_numpy()
+        else:
+            edge_array = np.empty((0, 2), dtype=np.uint32)
 
         self.directed = directed
         self.graph = engine.csr_from_edges(edges=edge_array, directed=directed)
-        self._index_to_key = index_to_key
-        self._key_to_index = key_to_index
+        self._index_to_key = nodes["id"]
 
     @classmethod
     def _ensure_node(
         cls, key: K, key_to_index: dict[K, int], index_to_key: list[K]
     ) -> int:
         if key not in key_to_index:
             idx = len(index_to_key)
             key_to_index[key] = idx
             index_to_key.append(key)
             return idx
         return key_to_index[key]
 
-    def make_keyed_vectors(self, dim: int) -> KeyedVectors[K]:
+    def make_keyed_vectors(self, dim: int) -> KeyedVectors:
         """Make keyed vectors appropriate to the space."""
-        return KeyedVectors(
-            dim=dim, index_to_key=self._index_to_key, key_to_index=self._key_to_index
-        )
+        return KeyedVectors(dim=dim, index_to_key=self._index_to_key)
 
 
-class Node2Vec(Generic[K]):
+class Node2Vec:
     """Node to vector algorithm."""
 
     _params: engine.Node2VecParams
-    _keyed_vectors: KeyedVectors[K]
-    _space: Space[K]
+    _keyed_vectors: KeyedVectors
+    _space: Space
     # TODO(ddn): Use seed
     _seed: int | None
 
     _syn1neg: npt.NDArray[np.float32] | None
 
     def __init__(  # noqa: PLR0913
         self,
-        space: Space[K],
+        space: Space,
         dim: int,
         walk_length: int,
         window: int,
         p: float = 1.0,
         q: float = 1.0,
         batch_words: int | None = None,
         alpha: float = 0.025,
@@ -214,20 +232,22 @@
             epochs,
             dynamic_ncols=True,
             desc="Epochs",
             leave=False,
             disable=not verbose,
         ):
             gen = np.random.Generator(np.random.get_bit_generator())
-            next_random = gen.integers(np.int32(2**31 - 1), dtype=np.int32)  # pyright: ignore[reportUnknownMemberType]
+            next_random = gen.integers(  # pyright: ignore[reportUnknownMemberType]
+                np.int32(2**31 - 1), dtype=np.int32
+            )
             engine.train_node2vec_epoch(
                 graph=self._space.graph,
                 params=self._params,
                 embeddings=self._keyed_vectors.vectors,
                 hidden_layer=self._syn1neg,
                 next_random=np.uint64(next_random),
             )
 
     @property
-    def wv(self) -> KeyedVectors[K]:
+    def wv(self) -> KeyedVectors:
         """Return computed embeddings."""
         return self._keyed_vectors
```

### Comparing `corvic_engine-0.1.8/python/corvic/engine/__init__.py` & `corvic_engine-0.1.9/python/corvic/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/engine/_native.pyi` & `corvic_engine-0.1.9/python/corvic/engine/_native.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/model/defaults.py` & `corvic_engine-0.1.9/python/corvic/model/defaults.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/model/experiments.py` & `corvic_engine-0.1.9/python/corvic/model/experiments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Experiments."""
 
 from collections.abc import Iterable, Iterator
-from typing import Any, TypeAlias
+from typing import TypeAlias
 
 import polars as pl
 
 from corvic import embed, orm
 from corvic.model.spaces import Space, SpaceEdgeTableMetadata
 from corvic.model.wrapped_orm import WrappedOrmObject
 from corvic.result import BadArgumentError
@@ -35,15 +35,15 @@
         q: float = 1.0,
         batch_words: int | None = None,
         alpha: float = 0.025,
         seed: int | None = None,
         workers: int | None = None,
         min_alpha: float = 0.0001,
         negative: int = 5,
-    ) -> embed.Node2Vec[str]:
+    ) -> embed.Node2Vec:
         """Run Node2Vec on the graph described by the space.
 
         Args:
             space: The space to run Node2Vec on
             dim: The dimensionality of the embedding
             walk_length: Length of the random walk to be computed
             window: Size of the window. This is half of the context,
@@ -65,45 +65,45 @@
 
         Returns:
             An Experiment
         """
         if not space.relationships:
             raise BadArgumentError("Node2Vec requires some relationships")
 
-        directed = space.relationships[0].directional
-        if any(rel.directional != directed for rel in space.relationships):
-            raise NotImplementedError(
-                "node2vec with mixed directionality not yet implemented"
-            )
-
-        def normalize(id_val: Any, source_name: str):
-            return f"{source_name}-{id_val}"
-
         edge_tables = space.output_edge_tables()
         if not edge_tables:
             raise BadArgumentError(
                 "Node2Vec requires some with_sources to be output=True"
             )
 
         def edge_generator():
             for table in space.output_edge_tables():
                 edge_table_info = table.get_typed_metadata(SpaceEdgeTableMetadata)
-                for row in table.to_dicts().unwrap_or_raise():
-                    yield (
-                        normalize(
-                            row[edge_table_info.start_source_column_name],
-                            edge_table_info.start_source_name,
-                        ),
-                        normalize(
-                            row[edge_table_info.end_source_column_name],
-                            edge_table_info.end_source_name,
-                        ),
-                    )
-
-        n2v_space = embed.Space(list(edge_generator()), directed=directed)
+                for batch in table.to_polars().unwrap_or_raise():
+                    yield batch.with_columns(
+                        pl.concat_str(
+                            [
+                                pl.lit(edge_table_info.start_source_name),
+                                pl.lit("-"),
+                                pl.col(edge_table_info.start_source_column_name),
+                            ]
+                        ).alias("start_id"),
+                        pl.concat_str(
+                            [
+                                pl.lit(edge_table_info.end_source_name),
+                                pl.lit("-"),
+                                pl.col(edge_table_info.end_source_column_name),
+                            ]
+                        ).alias("end_id"),
+                    ).select("start_id", "end_id")
+
+        n2v_space = embed.Space(
+            pl.concat((edge_list for edge_list in edge_generator()), rechunk=False),
+            directed=True,
+        )
         return embed.Node2Vec(
             space=n2v_space,
             dim=dim,
             walk_length=walk_length,
             window=window,
             p=p,
             q=q,
```

### Comparing `corvic_engine-0.1.8/python/corvic/model/resources.py` & `corvic_engine-0.1.9/python/corvic/model/resources.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/model/sources.py` & `corvic_engine-0.1.9/python/corvic/model/sources.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/model/spaces.py` & `corvic_engine-0.1.9/python/corvic/model/spaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,24 +69,48 @@
 
     def in_(self, value: list[Any]) -> RowFilter:
         """Return rows where column matches any in a list of values."""
         return row_filter.in_(column_name=self._column_name, literals=value)
 
 
 @dataclasses.dataclass(frozen=True)
+class FkeyRelationship:
+    """A foreign key relationship between sources."""
+
+    source_with_fkey: SourceID
+    fkey_column_name: str
+    referenced_source: SourceID
+    pkey_column_name: str
+
+
+@dataclasses.dataclass(frozen=True)
 class Relationship:
     """A connection between two sources within a space."""
 
-    from_source_id: Final[SourceID]
-    to_source_id: Final[SourceID]
-    directional: Final[bool]
-    space: Final[Space]
-    from_column_name: Final[str]
-    to_column_name: Final[str]
-    new_column_name: Final[str]
+    from_source_id: SourceID
+    to_source_id: SourceID
+    space: Space
+
+    fkey_relationship: FkeyRelationship
+
+    @property
+    def from_column_name(self) -> str:
+        if self.from_source_id == self.fkey_relationship.source_with_fkey:
+            return self.fkey_relationship.fkey_column_name
+        return self.fkey_relationship.pkey_column_name
+
+    @property
+    def to_column_name(self) -> str:
+        if self.to_source_id == self.fkey_relationship.source_with_fkey:
+            return self.fkey_relationship.fkey_column_name
+        return self.fkey_relationship.pkey_column_name
+
+    @property
+    def new_column_name(self) -> str:
+        return self.fkey_relationship.fkey_column_name
 
     @property
     def from_space_source(self):
         return self.space.get_space_source(self.from_source_id)
 
     @property
     def to_space_source(self):
@@ -119,16 +143,17 @@
         if self.from_column_name == start_pk.name:
             result_columns = (self.new_column_name, end_pk.name)
         else:
             result_columns = (start_pk.name, self.new_column_name)
 
         result = self.joined_table().select(result_columns)
 
-        for row in result.to_dicts().unwrap_or_raise():
-            yield (row[result_columns[0]], row[result_columns[1]])
+        for batch in result.to_polars().unwrap_or_raise():
+            for row in batch.rows(named=True):
+                yield (row[result_columns[0]], row[result_columns[1]])
 
 
 class SpaceSource(WrappedOrmObject[SpaceSourceID, orm.SpaceSource]):
     """A table from a source with some extra operations defined by a space."""
 
     _source: Final[Source]
 
@@ -227,26 +252,30 @@
 
     def _sub_orm_objects(self, orm_object: orm.Space) -> Iterable[orm.Base]:
         _ = (orm_object,)
         return []
 
     @property
     def relationships(self) -> list[Relationship]:
-        return self._relationships
+        return list(self._relationships)
 
-    def _calculate_paths_to_outputs(self, output: SourceID, rels: set[Relationship]):
+    def _calculate_paths_to_outputs(self, output: SourceID, rels: list[Relationship]):
         paths: list[list[Relationship]] = []
-        next_layer_rels = rels
         for rel in rels:
             if rel.from_source_id == output:
                 if rel.to_source_id in self._output_sources:
                     paths.append([rel])
                 else:
                     child_paths = self._calculate_paths_to_outputs(
-                        rel.to_source_id, next_layer_rels - {rel}
+                        rel.to_source_id,
+                        [  # we only want to use a fkey relationship once per path
+                            next_rel
+                            for next_rel in rels
+                            if next_rel.fkey_relationship != rel.fkey_relationship
+                        ],
                     )
                     paths.extend([rel, *child_path] for child_path in child_paths)
         return paths
 
     @staticmethod
     def _find_source_dest_columns(rels: list[Relationship]) -> tuple[str, str]:
         # source is the new column if new_column and to_column match because it was
@@ -263,15 +292,15 @@
             dest = pk.name if pk else ""
 
         return (source, dest)
 
     def output_edge_tables(self) -> list[Table]:
         paths_between_outputs = list(
             flatten(
-                self._calculate_paths_to_outputs(output, set(self.relationships))
+                self._calculate_paths_to_outputs(output, self.relationships)
                 for output in self._output_sources
             )
         )
         edge_tables = list[Table]()
         for path in paths_between_outputs:
             path_itr = iter(path)
             rel = next(path_itr)
@@ -446,14 +475,32 @@
             if from_foreign_keys:
                 from_foreign_key = from_foreign_keys[0]
             if to_foreign_keys:
                 to_foreign_key = to_foreign_keys[0]
 
         return (from_foreign_key, to_foreign_key)
 
+    def with_all_implied_relationships(self) -> Space:
+        """Automatically define non-directional relationships based on foreign keys."""
+        new_space = self
+        for space_source in self.space_sources:
+            for field in space_source.source.table.schema:
+                match field.ftype:
+                    case feature_type.ForeignKey(referenced_source_id):
+                        # We don't know the intended direction, add both directions
+                        new_space = new_space.with_relationship(
+                            referenced_source_id,
+                            space_source.source.id,
+                            to_foreign_key=field.name,
+                            directional=False,
+                        )
+                    case _:
+                        pass
+        return new_space
+
     def with_relationship(
         self,
         from_source_id: SourceID,
         to_source_id: SourceID,
         *,
         from_foreign_key: str | None = None,
         to_foreign_key: str | None = None,
@@ -493,58 +540,66 @@
             )
 
         from_foreign_key, to_foreign_key = self._check_or_infer_foreign_keys(
             from_source_id, to_source_id, from_foreign_key, to_foreign_key
         )
 
         if from_foreign_key:
-            from_column_name = from_foreign_key
             pk = self._space_sources[from_source_id].table.schema.get_primary_key()
             if not pk:
                 raise BadArgumentError(
                     "source has no primary key, "
                     + "so it cannot be referenced by foreign key",
                     from_source_id=str(from_source_id),
                 )
 
-            to_column_name = pk.name
-            new_column_name = from_column_name
+            fkey_relationship = FkeyRelationship(
+                source_with_fkey=from_source_id,
+                fkey_column_name=from_foreign_key,
+                referenced_source=to_source_id,
+                pkey_column_name=pk.name,
+            )
         elif to_foreign_key:
-            to_column_name = to_foreign_key
             pk = self._space_sources[to_source_id].table.schema.get_primary_key()
             if not pk:
                 raise BadArgumentError(
                     "source has no primary key, "
                     + "so it cannot be referenced by foreign key",
                     to_source_id=str(to_source_id),
                 )
-            from_column_name = pk.name
-            new_column_name = to_column_name
+            fkey_relationship = FkeyRelationship(
+                source_with_fkey=to_source_id,
+                fkey_column_name=to_foreign_key,
+                referenced_source=from_source_id,
+                pkey_column_name=pk.name,
+            )
         else:
             raise BadArgumentError(
                 "foreign key relationship was not provided and could not be inferred"
             )
 
-        relationships = [
-            dataclasses.replace(val)
-            for val in self._relationships
-            if val.from_source_id != from_source_id and val.to_source_id != to_source_id
-        ]
+        relationships = [dataclasses.replace(val) for val in self._relationships]
 
         relationships.append(
             Relationship(
                 from_source_id=from_source_id,
                 to_source_id=to_source_id,
-                directional=directional,
                 space=self,
-                from_column_name=from_column_name,
-                to_column_name=to_column_name,
-                new_column_name=new_column_name,
+                fkey_relationship=fkey_relationship,
             )
         )
+        if not directional:
+            relationships.append(
+                Relationship(
+                    from_source_id=to_source_id,
+                    to_source_id=from_source_id,
+                    space=self,
+                    fkey_relationship=fkey_relationship,
+                )
+            )
 
         return Space(
             self.client,
             dataclasses.replace(self._orm_self, id=None),
             derived_from_id=self.derived_from_id,
             space_sources=self._space_sources,
             relationships=relationships,
```

### Comparing `corvic_engine-0.1.8/python/corvic/model/wrapped_orm.py` & `corvic_engine-0.1.9/python/corvic/model/wrapped_orm.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/op_graph/__init__.py` & `corvic_engine-0.1.9/python/corvic/op_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/op_graph/feature_types.py` & `corvic_engine-0.1.9/python/corvic/op_graph/feature_types.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/op_graph/ops.py` & `corvic_engine-0.1.9/python/corvic/op_graph/ops.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/op_graph/proto_wrapper.py` & `corvic_engine-0.1.9/python/corvic/op_graph/proto_wrapper.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/op_graph/row_filters.py` & `corvic_engine-0.1.9/python/corvic/op_graph/row_filters.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/orm/__init__.py` & `corvic_engine-0.1.9/python/corvic/orm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
     __tablename__ = "experiment_run"
 
     id: MappedPrimaryKey = primary_key_column()
     experiment_id: sa_orm.Mapped[int] = sa_orm.mapped_column(
         Experiment.foreign_key().make(ondelete="CASCADE"), nullable=False, default=None
     )
     experiment: sa_orm.Mapped[Experiment] = sa_orm.relationship(init=True, default=None)
+    result_url: sa_orm.Mapped[str | None] = sa_orm.mapped_column(sa.Text, default=None)
 
 
 __all__ = [
     "Base",
     "DefaultObjects",
     "DeletedObjectError",
     "Experiment",
```

### Comparing `corvic_engine-0.1.8/python/corvic/orm/base.py` & `corvic_engine-0.1.9/python/corvic/orm/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,41 @@
 
 from datetime import datetime
 from typing import Any, ClassVar
 
 import sqlalchemy as sa
 import sqlalchemy.orm as sa_orm
 
+from corvic.orm.func import gen_uuid, utc_now
 from corvic.orm.keys import ForeignKey, MappedPrimaryKey, primary_key_column
-from corvic.orm.utc import UTCNow
 
 
 class Base(sa_orm.MappedAsDataclass, sa_orm.DeclarativeBase):
     """Base class for all DB mapped classes."""
 
     created_at: sa_orm.Mapped[datetime] = sa_orm.mapped_column(
-        sa.DateTime, server_default=UTCNow(), init=False
+        sa.DateTime, server_default=utc_now(), init=False
     )
     updated_at: sa_orm.Mapped[datetime] = sa_orm.mapped_column(
-        sa.DateTime, onupdate=UTCNow(), nullable=True, init=False
+        sa.DateTime, onupdate=utc_now(), nullable=True, init=False
     )
 
     @classmethod
     def foreign_key(cls):
         return ForeignKey(cls=cls)
 
 
 class OrgBase(Base):
     """An organization it a top level grouping of resources."""
 
     __tablename__ = "org"
 
     # overriding table_args is the recommending way of defining these base model types
-    __table_args__: ClassVar[Any] = {"extend_existing": True}
+    __table_args__: ClassVar[Any] = (
+        sa.UniqueConstraint("name"),
+        {"extend_existing": True},
+    )
 
     id: MappedPrimaryKey = primary_key_column()
+    name: sa_orm.Mapped[str] = sa_orm.mapped_column(
+        sa.Text, server_default=gen_uuid(), default=None
+    )
```

### Comparing `corvic_engine-0.1.8/python/corvic/orm/errors.py` & `corvic_engine-0.1.9/python/corvic/orm/errors.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/orm/ids.py` & `corvic_engine-0.1.9/python/corvic/orm/ids.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/orm/keys.py` & `corvic_engine-0.1.9/python/corvic/orm/keys.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/orm/mixins.py` & `corvic_engine-0.1.9/python/corvic/orm/mixins.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/orm/utc.py` & `corvic_engine-0.1.9/python/corvic/orm/func/utc_func.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/result/__init__.py` & `corvic_engine-0.1.9/python/corvic/result/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/sql/__init__.py` & `corvic_engine-0.1.9/python/corvic/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/sql/parse_ops.py` & `corvic_engine-0.1.9/python/corvic/sql/parse_ops.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/sql/rockset.py` & `corvic_engine-0.1.9/python/corvic/sql/rockset.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system/__init__.py` & `corvic_engine-0.1.9/python/corvic/system/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system/client.py` & `corvic_engine-0.1.9/python/corvic/system/client.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system/in_memory_executor.py` & `corvic_engine-0.1.9/python/corvic/system/in_memory_executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Staging-agnostic in-memory executor."""
 
-from collections.abc import Iterable
-from typing import Any
+import pyarrow as pa
 
 from corvic import op_graph, sql
 from corvic.system.staging import StagingDB
 
 
 class InMemoryExecutor:
     """Executes op_graphs in memory (after staging queries)."""
 
     def __init__(self, staging_db: StagingDB):
         self._staging_db = staging_db
 
     def _staging_query_generator(self, blob_names: list[str], column_names: list[str]):
         return self._staging_db.query_for_blobs(blob_names, column_names)
 
-    def execute(self, op: op_graph.Op) -> Iterable[dict[str, Any]]:
+    def execute(self, op: op_graph.Op) -> pa.RecordBatchReader:
         query = sql.parse_op_graph(op, self._staging_query_generator)
         return self._staging_db.run_select_query(query)
```

### Comparing `corvic_engine-0.1.8/python/corvic/system/staging.py` & `corvic_engine-0.1.9/python/corvic/system/staging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Corvic system data staging protocol."""
 
-from collections.abc import Iterable
-from typing import Any
+from typing import Protocol
 
+import pyarrow as pa
 import sqlglot
-from typing_extensions import Protocol
 
 
 class StagingDB(Protocol):
     """A connection to some database where staging data can be found."""
 
     def count_ingested_rows(self, blob_name: str, *other_blob_names: str) -> int:
         """Returns the number of rows of the given blobs available for querying.
@@ -17,10 +16,8 @@
         """
         ...
 
     def query_for_blobs(
         self, blob_names: list[str], column_names: list[str]
     ) -> sqlglot.exp.Query: ...
 
-    def run_select_query(
-        self, query: sqlglot.exp.Query
-    ) -> Iterable[dict[str, Any]]: ...
+    def run_select_query(self, query: sqlglot.exp.Query) -> pa.RecordBatchReader: ...
```

### Comparing `corvic_engine-0.1.8/python/corvic/system/storage.py` & `corvic_engine-0.1.9/python/corvic/system/storage.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system_sqlite/blob_store.py` & `corvic_engine-0.1.9/python/corvic/system_sqlite/blob_store.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system_sqlite/client.py` & `corvic_engine-0.1.9/python/corvic/system_sqlite/client.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/system_sqlite/staging.py` & `corvic_engine-0.1.9/python/corvic/system_sqlite/staging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Sqlite backed staging system."""
 
 import functools
 import uuid
 from collections.abc import Iterable
-from typing import Any
 
 import duckdb
+import pyarrow as pa
 import pyarrow.parquet as pq
 import sqlglot
 
 from corvic.system import StorageManager
 
 
 class DuckDBStaging:
@@ -138,22 +138,22 @@
         )
         return (
             sqlglot.select(*column_names)
             .from_(staging_union_table)
             .with_(staging_union_table, as_=union)
         )
 
-    def run_select_query(self, query: sqlglot.exp.Query) -> Iterable[dict[str, Any]]:
+    def run_select_query(self, query: sqlglot.exp.Query) -> pa.RecordBatchReader:
         """Run a select query to extract and transform staging data.
 
         N.B. this behaves a little differently than rockset would.
         Rockset has one super-wide table, so it would silently omit data. This
         implementation will complain loudly if the query references an unstaged blob.
         That tradeoff is somewhat reasonable since if data isn't staged in this case it
         means the caller is doing something wrong (in Rockset's case there's some
         asynchrony which could lead to the data not being staged).
         """
         self._update_blobs()
         with self._db_conn.cursor() as cur:
             cur.execute(query.sql(dialect="duckdb"))
             result = cur.fetch_arrow_table()
-        return result.to_pylist()
+        return result.to_reader()
```

### Comparing `corvic_engine-0.1.8/python/corvic/table/__init__.py` & `corvic_engine-0.1.9/python/corvic/table/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/table/schema.py` & `corvic_engine-0.1.9/python/corvic/table/schema.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic/table/table.py` & `corvic_engine-0.1.9/python/corvic/table/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Table."""
 
 from __future__ import annotations
 
 import dataclasses
 import functools
-import itertools
 from collections.abc import Iterable, Mapping, Sequence
 from typing import (
     Any,
     Final,
     Literal,
     Protocol,
     TypeAlias,
     TypeVar,
     cast,
 )
 
 import more_itertools
 import polars as pl
+import pyarrow as pa
 import pyarrow.parquet as pq
 from typing_extensions import Self
 
 from corvic import op_graph
 from corvic.result import BadArgumentError, Error, NotFoundError, Ok
 from corvic.system import Client, DataMisplacedError
 from corvic.table.schema import Schema
@@ -107,14 +107,19 @@
         client: Client,
         op: op_graph.Op,
     ):
         self._client = client
         self._op = op
         self._staged = False
 
+    def __eq__(self, other: object):
+        if not isinstance(other, type(self)):
+            return False
+        return self._op == other._op
+
     @property
     def client(self):
         return self._client
 
     @property
     def op_graph(self):
         return self._op
@@ -236,32 +241,36 @@
         return Ok(cls.from_ops(client, op))
 
     def to_bytes(self):
         return self.op_graph.to_bytes()
 
     def to_polars(self) -> Ok[Iterable[pl.DataFrame]] | NotReadyError:
         """Stream over the view as a series of Polars DataFrames."""
-        match self.to_dicts():
-            case Ok(it):
+        match self.to_batches():
+            case Ok(batch_reader):
                 pass
             case NotReadyError() as error:
                 return error
-        polars_schema = cast(
+        empty_table = cast(
             pl.DataFrame, pl.from_arrow(self.schema.to_arrow().empty_table())
-        ).schema
+        )
+        polars_schema = empty_table.schema
 
         def generator():
-            while True:
-                df_slice = pl.DataFrame(
-                    list(itertools.islice(it, self.MAX_ROWS_PER_SLICE)),
-                    schema=polars_schema,
-                )
-                yield df_slice
-                if len(df_slice) < self.MAX_ROWS_PER_SLICE:
-                    break
+            some = False
+            for batch in batch_reader:
+                df_batch = cast(
+                    pl.DataFrame,
+                    pl.from_arrow(batch, rechunk=False, schema_overrides=polars_schema),
+                ).select(key for key in polars_schema)
+
+                some = True
+                yield df_batch
+            if not some:
+                yield empty_table
 
         return Ok(generator())
 
     def _staging_op_satisfied(self, staging_op: op_graph.op.SelectFromStaging) -> bool:
         result = self.client.staging_db.count_ingested_rows(*staging_op.blob_names)
         if result < staging_op.expected_rows:
             return False
@@ -320,15 +329,15 @@
         self, new_feature_types: Mapping[str, op_graph.FeatureType]
     ) -> Table:
         return Table(
             self.client,
             self.op_graph.update_feature_types(new_feature_types=new_feature_types),
         )
 
-    def to_dicts(self) -> Ok[Iterable[dict[str, Any]]] | NotReadyError:
+    def to_batches(self) -> Ok[pa.RecordBatchReader] | NotReadyError:
         """Convert every row to a dictionary of Python-native values."""
         match self._must_wait_for_staging():
             case Ok():
                 return Ok(self.client.executor.execute(self.op_graph))
             case NotReadyError() as err:
                 return err
```

### Comparing `corvic_engine-0.1.8/python/corvic/version/__init__.py` & `corvic_engine-0.1.9/python/corvic/version/__init__.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/algorithm/graph/v1/graph_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/algorithm/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/chat/v1/service_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/chat/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/completion/v1/service_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/completion/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/config/v1/settings_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/config/v1/settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/embedding/v1/models_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/embedding/v1/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,52 +11,53 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from corvic_generated.algorithm.graph.v1 import graph_pb2 as corvic_dot_algorithm_dot_graph_dot_v1_dot_graph__pb2
 from corvic_generated.embedding.v1 import models_pb2 as corvic_dot_embedding_dot_v1_dot_models__pb2
+from corvic_generated.status.v1 import event_pb2 as corvic_dot_status_dot_v1_dot_event__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"corvic/feature/v1/experiment.proto\x12\x11\x63orvic.feature.v1\x1a\x1b\x62uf/validate/validate.proto\x1a%corvic/algorithm/graph/v1/graph.proto\x1a corvic/embedding/v1/models.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x85\x02\n\nParameters\x12\x19\n\x08space_id\x18\x01 \x01(\tR\x07spaceId\x12p\n\x1b\x63olumn_embedding_parameters\x18\x02 \x01(\x0b\x32..corvic.embedding.v1.ColumnEmbeddingParametersH\x00R\x19\x63olumnEmbeddingParameters\x12`\n\x13node2vec_parameters\x18\x03 \x01(\x0b\x32-.corvic.algorithm.graph.v1.Node2VecParametersH\x00R\x12node2vecParametersB\x08\n\x06params\"\x82\x01\n\nExperiment\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xbaH\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06params\x18\x03 \x03(\x0b\x32\x1d.corvic.feature.v1.ParametersR\x06params\"\xc9\x01\n\x0f\x45xperimentEntry\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\x12#\n\rexperiment_id\x18\x02 \x01(\tR\x0c\x65xperimentId\x12\x39\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12=\n\nexperiment\x18\x04 \x01(\x0b\x32\x1d.corvic.feature.v1.ExperimentR\nexperiment\";\n\x14GetExperimentRequest\x12#\n\rexperiment_id\x18\x01 \x01(\tR\x0c\x65xperimentId\"f\n\x15GetExperimentResponse\x12M\n\x10\x65xperiment_entry\x18\x01 \x01(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x0f\x65xperimentEntry\"1\n\x16ListExperimentsRequest\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\"l\n\x17ListExperimentsResponse\x12Q\n\x12\x65xperiment_entries\x18\x01 \x03(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x11\x65xperimentEntries\"\xce\x01\n\x17\x43reateExperimentRequest\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\x12\x41\n\nexperiment\x18\x02 \x01(\x0b\x32\x1d.corvic.feature.v1.ExperimentB\x02\x18\x01R\nexperiment\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06params\x18\x04 \x03(\x0b\x32\x1d.corvic.feature.v1.ParametersR\x06params\"i\n\x18\x43reateExperimentResponse\x12M\n\x10\x65xperiment_entry\x18\x01 \x01(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x0f\x65xperimentEntry\")\n\x17\x44\x65leteExperimentRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1a\n\x18\x44\x65leteExperimentResponse\"R\n\x1aGetExperimentResultRequest\x12\x34\n\rexperiment_id\x18\x01 \x01(\tB\x0f\xbaH\x0cr\n2\x08^[0-9]+$R\x0c\x65xperimentId\"<\n\x1bGetExperimentResultResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl2\xbb\x04\n\x11\x45xperimentService\x12\x64\n\rGetExperiment\x12\'.corvic.feature.v1.GetExperimentRequest\x1a(.corvic.feature.v1.GetExperimentResponse\"\x00\x12m\n\x10\x43reateExperiment\x12*.corvic.feature.v1.CreateExperimentRequest\x1a+.corvic.feature.v1.CreateExperimentResponse\"\x00\x12m\n\x10\x44\x65leteExperiment\x12*.corvic.feature.v1.DeleteExperimentRequest\x1a+.corvic.feature.v1.DeleteExperimentResponse\"\x00\x12j\n\x0fListExperiments\x12).corvic.feature.v1.ListExperimentsRequest\x1a*.corvic.feature.v1.ListExperimentsResponse\"\x00\x12v\n\x13GetExperimentResult\x12-.corvic.feature.v1.GetExperimentResultRequest\x1a..corvic.feature.v1.GetExperimentResultResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"corvic/feature/v1/experiment.proto\x12\x11\x63orvic.feature.v1\x1a\x1b\x62uf/validate/validate.proto\x1a%corvic/algorithm/graph/v1/graph.proto\x1a corvic/embedding/v1/models.proto\x1a\x1c\x63orvic/status/v1/event.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x85\x02\n\nParameters\x12\x19\n\x08space_id\x18\x01 \x01(\tR\x07spaceId\x12p\n\x1b\x63olumn_embedding_parameters\x18\x02 \x01(\x0b\x32..corvic.embedding.v1.ColumnEmbeddingParametersH\x00R\x19\x63olumnEmbeddingParameters\x12`\n\x13node2vec_parameters\x18\x03 \x01(\x0b\x32-.corvic.algorithm.graph.v1.Node2VecParametersH\x00R\x12node2vecParametersB\x08\n\x06params\"\x82\x01\n\nExperiment\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xbaH\x04r\x02\x10\x01R\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06params\x18\x03 \x03(\x0b\x32\x1d.corvic.feature.v1.ParametersR\x06params\"\x87\x02\n\x0f\x45xperimentEntry\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\x12#\n\rexperiment_id\x18\x02 \x01(\tR\x0c\x65xperimentId\x12\x39\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12=\n\nexperiment\x18\x04 \x01(\x0b\x32\x1d.corvic.feature.v1.ExperimentR\nexperiment\x12<\n\rrecent_events\x18\x05 \x03(\x0b\x32\x17.corvic.status.v1.EventR\x0crecentEvents\";\n\x14GetExperimentRequest\x12#\n\rexperiment_id\x18\x01 \x01(\tR\x0c\x65xperimentId\"f\n\x15GetExperimentResponse\x12M\n\x10\x65xperiment_entry\x18\x01 \x01(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x0f\x65xperimentEntry\"1\n\x16ListExperimentsRequest\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\"l\n\x17ListExperimentsResponse\x12Q\n\x12\x65xperiment_entries\x18\x01 \x03(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x11\x65xperimentEntries\"\xce\x01\n\x17\x43reateExperimentRequest\x12\x17\n\x07room_id\x18\x01 \x01(\tR\x06roomId\x12\x41\n\nexperiment\x18\x02 \x01(\x0b\x32\x1d.corvic.feature.v1.ExperimentB\x02\x18\x01R\nexperiment\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06params\x18\x04 \x03(\x0b\x32\x1d.corvic.feature.v1.ParametersR\x06params\"i\n\x18\x43reateExperimentResponse\x12M\n\x10\x65xperiment_entry\x18\x01 \x01(\x0b\x32\".corvic.feature.v1.ExperimentEntryR\x0f\x65xperimentEntry\")\n\x17\x44\x65leteExperimentRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1a\n\x18\x44\x65leteExperimentResponse\"R\n\x1aGetExperimentResultRequest\x12\x34\n\rexperiment_id\x18\x01 \x01(\tB\x0f\xbaH\x0cr\n2\x08^[0-9]+$R\x0c\x65xperimentId\"<\n\x1bGetExperimentResultResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl2\xbb\x04\n\x11\x45xperimentService\x12\x64\n\rGetExperiment\x12\'.corvic.feature.v1.GetExperimentRequest\x1a(.corvic.feature.v1.GetExperimentResponse\"\x00\x12m\n\x10\x43reateExperiment\x12*.corvic.feature.v1.CreateExperimentRequest\x1a+.corvic.feature.v1.CreateExperimentResponse\"\x00\x12m\n\x10\x44\x65leteExperiment\x12*.corvic.feature.v1.DeleteExperimentRequest\x1a+.corvic.feature.v1.DeleteExperimentResponse\"\x00\x12j\n\x0fListExperiments\x12).corvic.feature.v1.ListExperimentsRequest\x1a*.corvic.feature.v1.ListExperimentsResponse\"\x00\x12v\n\x13GetExperimentResult\x12-.corvic.feature.v1.GetExperimentResultRequest\x1a..corvic.feature.v1.GetExperimentResultResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'corvic.feature.v1.experiment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_EXPERIMENT'].fields_by_name['name']._options = None
   _globals['_EXPERIMENT'].fields_by_name['name']._serialized_options = b'\272H\004r\002\020\001'
   _globals['_CREATEEXPERIMENTREQUEST'].fields_by_name['experiment']._options = None
   _globals['_CREATEEXPERIMENTREQUEST'].fields_by_name['experiment']._serialized_options = b'\030\001'
   _globals['_GETEXPERIMENTRESULTREQUEST'].fields_by_name['experiment_id']._options = None
   _globals['_GETEXPERIMENTRESULTREQUEST'].fields_by_name['experiment_id']._serialized_options = b'\272H\014r\n2\010^[0-9]+$'
-  _globals['_PARAMETERS']._serialized_start=193
-  _globals['_PARAMETERS']._serialized_end=454
-  _globals['_EXPERIMENT']._serialized_start=457
-  _globals['_EXPERIMENT']._serialized_end=587
-  _globals['_EXPERIMENTENTRY']._serialized_start=590
-  _globals['_EXPERIMENTENTRY']._serialized_end=791
-  _globals['_GETEXPERIMENTREQUEST']._serialized_start=793
-  _globals['_GETEXPERIMENTREQUEST']._serialized_end=852
-  _globals['_GETEXPERIMENTRESPONSE']._serialized_start=854
-  _globals['_GETEXPERIMENTRESPONSE']._serialized_end=956
-  _globals['_LISTEXPERIMENTSREQUEST']._serialized_start=958
-  _globals['_LISTEXPERIMENTSREQUEST']._serialized_end=1007
-  _globals['_LISTEXPERIMENTSRESPONSE']._serialized_start=1009
-  _globals['_LISTEXPERIMENTSRESPONSE']._serialized_end=1117
-  _globals['_CREATEEXPERIMENTREQUEST']._serialized_start=1120
-  _globals['_CREATEEXPERIMENTREQUEST']._serialized_end=1326
-  _globals['_CREATEEXPERIMENTRESPONSE']._serialized_start=1328
-  _globals['_CREATEEXPERIMENTRESPONSE']._serialized_end=1433
-  _globals['_DELETEEXPERIMENTREQUEST']._serialized_start=1435
-  _globals['_DELETEEXPERIMENTREQUEST']._serialized_end=1476
-  _globals['_DELETEEXPERIMENTRESPONSE']._serialized_start=1478
-  _globals['_DELETEEXPERIMENTRESPONSE']._serialized_end=1504
-  _globals['_GETEXPERIMENTRESULTREQUEST']._serialized_start=1506
-  _globals['_GETEXPERIMENTRESULTREQUEST']._serialized_end=1588
-  _globals['_GETEXPERIMENTRESULTRESPONSE']._serialized_start=1590
-  _globals['_GETEXPERIMENTRESULTRESPONSE']._serialized_end=1650
-  _globals['_EXPERIMENTSERVICE']._serialized_start=1653
-  _globals['_EXPERIMENTSERVICE']._serialized_end=2224
+  _globals['_PARAMETERS']._serialized_start=223
+  _globals['_PARAMETERS']._serialized_end=484
+  _globals['_EXPERIMENT']._serialized_start=487
+  _globals['_EXPERIMENT']._serialized_end=617
+  _globals['_EXPERIMENTENTRY']._serialized_start=620
+  _globals['_EXPERIMENTENTRY']._serialized_end=883
+  _globals['_GETEXPERIMENTREQUEST']._serialized_start=885
+  _globals['_GETEXPERIMENTREQUEST']._serialized_end=944
+  _globals['_GETEXPERIMENTRESPONSE']._serialized_start=946
+  _globals['_GETEXPERIMENTRESPONSE']._serialized_end=1048
+  _globals['_LISTEXPERIMENTSREQUEST']._serialized_start=1050
+  _globals['_LISTEXPERIMENTSREQUEST']._serialized_end=1099
+  _globals['_LISTEXPERIMENTSRESPONSE']._serialized_start=1101
+  _globals['_LISTEXPERIMENTSRESPONSE']._serialized_end=1209
+  _globals['_CREATEEXPERIMENTREQUEST']._serialized_start=1212
+  _globals['_CREATEEXPERIMENTREQUEST']._serialized_end=1418
+  _globals['_CREATEEXPERIMENTRESPONSE']._serialized_start=1420
+  _globals['_CREATEEXPERIMENTRESPONSE']._serialized_end=1525
+  _globals['_DELETEEXPERIMENTREQUEST']._serialized_start=1527
+  _globals['_DELETEEXPERIMENTREQUEST']._serialized_end=1568
+  _globals['_DELETEEXPERIMENTRESPONSE']._serialized_start=1570
+  _globals['_DELETEEXPERIMENTRESPONSE']._serialized_end=1596
+  _globals['_GETEXPERIMENTRESULTREQUEST']._serialized_start=1598
+  _globals['_GETEXPERIMENTRESULTREQUEST']._serialized_end=1680
+  _globals['_GETEXPERIMENTRESULTRESPONSE']._serialized_start=1682
+  _globals['_GETEXPERIMENTRESULTRESPONSE']._serialized_end=1742
+  _globals['_EXPERIMENTSERVICE']._serialized_start=1745
+  _globals['_EXPERIMENTSERVICE']._serialized_end=2316
 # @@protoc_insertion_point(module_scope)
```

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from buf.validate import validate_pb2 as _validate_pb2
 from corvic_generated.algorithm.graph.v1 import graph_pb2 as _graph_pb2
 from corvic_generated.embedding.v1 import models_pb2 as _models_pb2
+from corvic_generated.status.v1 import event_pb2 as _event_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -26,24 +27,26 @@
     PARAMS_FIELD_NUMBER: _ClassVar[int]
     name: str
     description: str
     params: _containers.RepeatedCompositeFieldContainer[Parameters]
     def __init__(self, name: _Optional[str] = ..., description: _Optional[str] = ..., params: _Optional[_Iterable[_Union[Parameters, _Mapping]]] = ...) -> None: ...
 
 class ExperimentEntry(_message.Message):
-    __slots__ = ("room_id", "experiment_id", "created_at", "experiment")
+    __slots__ = ("room_id", "experiment_id", "created_at", "experiment", "recent_events")
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     EXPERIMENT_ID_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     EXPERIMENT_FIELD_NUMBER: _ClassVar[int]
+    RECENT_EVENTS_FIELD_NUMBER: _ClassVar[int]
     room_id: str
     experiment_id: str
     created_at: _timestamp_pb2.Timestamp
     experiment: Experiment
-    def __init__(self, room_id: _Optional[str] = ..., experiment_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., experiment: _Optional[_Union[Experiment, _Mapping]] = ...) -> None: ...
+    recent_events: _containers.RepeatedCompositeFieldContainer[_event_pb2.Event]
+    def __init__(self, room_id: _Optional[str] = ..., experiment_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., experiment: _Optional[_Union[Experiment, _Mapping]] = ..., recent_events: _Optional[_Iterable[_Union[_event_pb2.Event, _Mapping]]] = ...) -> None: ...
 
 class GetExperimentRequest(_message.Message):
     __slots__ = ("experiment_id",)
     EXPERIMENT_ID_FIELD_NUMBER: _ClassVar[int]
     experiment_id: str
     def __init__(self, experiment_id: _Optional[str] = ...) -> None: ...
```

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/experiment_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/experiment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/feature/v1/space_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/feature/v1/space_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v1/service_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/resource_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/resource_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/room_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/room_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/source_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/source_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/ingest/v2/table_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/ingest/v2/table_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/orm/v1/table_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/orm/v1/table_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/status/v1/event_pb2.pyi` & `corvic_engine-0.1.9/python/corvic_generated/status/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2.py` & `corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2_grpc.py` & `corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/python/corvic_generated/status/v1/service_pb2_grpc.pyi` & `corvic_engine-0.1.9/python/corvic_generated/status/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/Cargo.lock` & `corvic_engine-0.1.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "corvic-engine"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "numpy",
  "pyo3",
  "rayon",
  "thread_local",
 ]
 
@@ -59,15 +59,15 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "engine-walk"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
@@ -331,23 +331,23 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `corvic_engine-0.1.8/Cargo.toml` & `corvic_engine-0.1.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 resolver = "2"
 members = ["python"]
 
 [workspace.package]
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 license-file = "LICENSE"
 publish = false
 
 [workspace.dependencies]
 arrow-array = { version = ">=41", default-features = false }
 arrow-buffer = { version = ">=41", default-features = false }
```

### Comparing `corvic_engine-0.1.8/pyproject.toml` & `corvic_engine-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
 license = { file = "LICENSE" }
 authors = [
   { name = "Corvic Team", email = "contact@corvic.ai" },
 ]
-version = "0.1.8" # sync this with tool.poetry.version below
+version = "0.1.9" # sync this with tool.poetry.version below
 
 # TODO(ddn): Pull dependencies from tool.poetry.dependencies. We use maturin as
 # the build system but poetry for the development environment.
 #
 #   https://github.com/python-poetry/poetry/issues/3332
 #
 # Dependencies here are generally looser than their Poetry counterparts so we
@@ -47,15 +47,15 @@
 packages = [
   { include = "corvic", from = "python" },
   { include = "corvic_generated", from = "python" },
   { include = "buf", from = "python" },
 ]
 description = ""
 authors = []
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.scripts]
 check = "corvic_check.cli:main"
 
 [tool.poetry.dependencies]
 duckdb = "^0.10.0"
 more-itertools = "^10.2.0"
```

### Comparing `corvic_engine-0.1.8/LICENSE` & `corvic_engine-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `corvic_engine-0.1.8/PKG-INFO` & `corvic_engine-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: corvic-engine
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: duckdb >=0.10
```

