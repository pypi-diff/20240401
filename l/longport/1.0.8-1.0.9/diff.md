# Comparing `tmp/longport-1.0.8.tar.gz` & `tmp/longport-1.0.9.tar.gz`

## Comparing `longport-1.0.8.tar` & `longport-1.0.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport-candlesticks/Cargo.toml
--rw-r--r--   0      501       20      174 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-candlesticks/src/lib.rs
--rw-r--r--   0      501       20     3423 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-candlesticks/src/market.rs
--rw-r--r--   0      501       20    21444 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-candlesticks/src/merger.rs
--rw-r--r--   0      501       20      556 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-candlesticks/src/types.rs
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport-proto/Cargo.toml
--rw-r--r--   0      501       20       96 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/error/error.proto
--rw-r--r--   0      501       20      282 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/.gitignore
--rw-r--r--   0      501       20       51 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/README.md
--rw-r--r--   0      501       20      257 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/buf.gen.yaml
--rw-r--r--   0      501       20     1022 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/control/control.proto
--rw-r--r--   0      501       20      108 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/control/error.proto
--rw-r--r--   0      501       20    67241 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.cc
--rw-r--r--   0      501       20    64169 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.h
--rw-r--r--   0      501       20    13071 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.cc
--rw-r--r--   0      501       20    11600 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.h
--rw-r--r--   0      501       20  1038612 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.cc
--rw-r--r--   0      501       20  1199727 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.h
--rw-r--r--   0      501       20    63373 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.cc
--rw-r--r--   0      501       20    84723 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.h
--rw-r--r--   0      501       20    22451 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/control.pb.go
--rw-r--r--   0      501       20     5856 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/error.pb.go
--rw-r--r--   0      501       20      108 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.mod
--rw-r--r--   0      501       20      739 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.sum
--rw-r--r--   0      501       20   278532 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/quote/api.pb.go
--rw-r--r--   0      501       20    23115 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/trade/subscribe.pb.go
--rw-r--r--   0      501       20     3638 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/control_pb2.py
--rw-r--r--   0      501       20     1717 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/error_pb2.py
--rw-r--r--   0      501       20    34401 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/quote/api_pb2.py
--rw-r--r--   0      501       20     3660 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/trade/subscribe_pb2.py
--rw-r--r--   0      501       20    14370 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/quote/api.proto
--rw-r--r--   0      501       20     1183 2024-02-29 15:16:55.000000 longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/trade/subscribe.proto
--rw-r--r--   0      501       20      287 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/src/lib.rs
--rw-r--r--   0      501       20     2246 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/src/longportapp.control.v1.rs
--rw-r--r--   0      501       20    35478 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/src/longportapp.quote.v1.rs
--rw-r--r--   0      501       20     2691 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/src/longportapp.trade.v1.rs
--rw-r--r--   0      501       20      191 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-proto/src/qop.error.rs
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport-python-macros/Cargo.toml
--rw-r--r--   0      501       20      541 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-python-macros/src/error.rs
--rw-r--r--   0      501       20      692 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-python-macros/src/lib.rs
--rw-r--r--   0      501       20     2561 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-python-macros/src/pyenum.rs
--rw-r--r--   0      501       20     3356 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-python-macros/src/pyobject.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport/Cargo.toml
--rw-r--r--   0      501       20      251 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/CHANGELOG.md
--rw-r--r--   0      501       20      795 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/Makefile.toml
--rw-r--r--   0      501       20     4139 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/README.md
--rw-r--r--   0      501       20      147 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/blocking/error.rs
--rw-r--r--   0      501       20      182 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/blocking/mod.rs
--rw-r--r--   0      501       20    28831 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/blocking/quote.rs
--rw-r--r--   0      501       20     3890 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/blocking/runtime.rs
--rw-r--r--   0      501       20    13183 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/blocking/trade.rs
--rw-r--r--   0      501       20     7532 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/config.rs
--rw-r--r--   0      501       20     3644 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/error.rs
--rw-r--r--   0      501       20      593 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/lib.rs
--rw-r--r--   0      501       20     1518 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/macros.rs
--rw-r--r--   0      501       20     1934 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/cache.rs
--rw-r--r--   0      501       20     2083 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/cmd_code.rs
--rw-r--r--   0      501       20    49869 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/context.rs
--rw-r--r--   0      501       20    34534 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/core.rs
--rw-r--r--   0      501       20     1129 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/mod.rs
--rw-r--r--   0      501       20     5455 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/push_types.rs
--rw-r--r--   0      501       20     4082 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/store.rs
--rw-r--r--   0      501       20     1547 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/sub_flags.rs
--rw-r--r--   0      501       20    44392 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/types.rs
--rw-r--r--   0      501       20      350 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/quote/utils.rs
--rw-r--r--   0      501       20     7128 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/serde_utils.rs
--rw-r--r--   0      501       20      282 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/cmd_code.rs
--rw-r--r--   0      501       20    21658 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/context.rs
--rw-r--r--   0      501       20     8478 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/core.rs
--rw-r--r--   0      501       20     1057 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/mod.rs
--rw-r--r--   0      501       20     3512 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/push_types.rs
--rw-r--r--   0      501       20     1561 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/estimate_max_purchase_quantity.rs
--rw-r--r--   0      501       20     1660 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_cash_flow.rs
--rw-r--r--   0      501       20      682 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_fund_positions.rs
--rw-r--r--   0      501       20     1374 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_history_executions.rs
--rw-r--r--   0      501       20     2281 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_history_orders.rs
--rw-r--r--   0      501       20      687 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_stock_positions.rs
--rw-r--r--   0      501       20      909 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_today_executions.rs
--rw-r--r--   0      501       20     1806 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/get_today_orders.rs
--rw-r--r--   0      501       20      775 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/mod.rs
--rw-r--r--   0      501       20     2539 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/replace_order.rs
--rw-r--r--   0      501       20     3673 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/requests/submit_order.rs
--rw-r--r--   0      501       20    38596 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/trade/types.rs
--rw-r--r--   0      501       20      378 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport/src/types.rs
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport-wscli/Cargo.toml
--rw-r--r--   0      501       20    13801 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-wscli/src/client.rs
--rw-r--r--   0      501       20     6818 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-wscli/src/codec.rs
--rw-r--r--   0      501       20     1785 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-wscli/src/error.rs
--rw-r--r--   0      501       20      320 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-wscli/src/event.rs
--rw-r--r--   0      501       20      396 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-wscli/src/lib.rs
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 longport-1.0.8/local_dependencies/longport-httpcli/Cargo.toml
--rw-r--r--   0      501       20     2578 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/client.rs
--rw-r--r--   0      501       20     2619 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/config.rs
--rw-r--r--   0      501       20     1622 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/error.rs
--rw-r--r--   0      501       20     2343 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/geo.rs
--rw-r--r--   0      501       20      488 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/lib.rs
--rw-r--r--   0      501       20    27363 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/qs.rs
--rw-r--r--   0      501       20     9790 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/request.rs
--rw-r--r--   0      501       20     1910 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/signature.rs
--rw-r--r--   0      501       20      695 2024-02-29 15:16:53.000000 longport-1.0.8/local_dependencies/longport-httpcli/src/timestamp.rs
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 longport-1.0.8/Cargo.toml
--rw-r--r--   0      501       20      210 2024-02-29 15:16:53.000000 longport-1.0.8/.cargo/config.toml
--rw-r--r--   0      501       20        4 2024-02-29 15:16:53.000000 longport-1.0.8/.gitignore
--rw-r--r--   0      501       20      252 2024-02-29 15:16:53.000000 longport-1.0.8/CHANGELOG.md
--rw-r--r--   0      501       20      358 2024-02-29 15:16:53.000000 longport-1.0.8/Makefile.toml
--rw-r--r--   0      501       20     2370 2024-02-29 15:16:53.000000 longport-1.0.8/README.md
--rw-r--r--   0      501       20       71 2024-02-29 15:16:53.000000 longport-1.0.8/build.rs
--rw-r--r--   0      501       20       38 2024-02-29 15:16:53.000000 longport-1.0.8/docs/config.md
--rw-r--r--   0      501       20     2330 2024-02-29 15:16:53.000000 longport-1.0.8/docs/index.md
--rw-r--r--   0      501       20       50 2024-02-29 15:16:53.000000 longport-1.0.8/docs/quote_context.md
--rw-r--r--   0      501       20       39 2024-02-29 15:16:53.000000 longport-1.0.8/docs/reference_all.md
--rw-r--r--   0      501       20       91 2024-02-29 15:16:53.000000 longport-1.0.8/docs/requirements.txt
--rw-r--r--   0      501       20       50 2024-02-29 15:16:53.000000 longport-1.0.8/docs/trade_context.md
--rw-r--r--   0      501       20      811 2024-02-29 15:16:53.000000 longport-1.0.8/mkdocs.yml
--rw-r--r--   0      501       20      803 2024-02-29 15:16:53.000000 longport-1.0.8/pyproject.toml
--rw-r--r--   0      501       20      473 2024-02-29 15:16:53.000000 longport-1.0.8/pysrc/longport/__init__.py
--rw-r--r--   0      501       20        0 2024-02-29 15:16:53.000000 longport-1.0.8/pysrc/longport/openapi.py
--rw-r--r--   0      501       20    82923 2024-02-29 15:16:53.000000 longport-1.0.8/pysrc/longport/openapi.pyi
--rw-r--r--   0      501       20        0 2024-02-29 15:16:53.000000 longport-1.0.8/pysrc/longport/py.typed
--rw-r--r--   0      501       20     1817 2024-02-29 15:16:53.000000 longport-1.0.8/src/config.rs
--rw-r--r--   0      501       20     2205 2024-02-29 15:16:53.000000 longport-1.0.8/src/decimal.rs
--rw-r--r--   0      501       20      375 2024-02-29 15:16:53.000000 longport-1.0.8/src/error.rs
--rw-r--r--   0      501       20     2583 2024-02-29 15:16:53.000000 longport-1.0.8/src/http_client.rs
--rw-r--r--   0      501       20      546 2024-02-29 15:16:53.000000 longport-1.0.8/src/lib.rs
--rw-r--r--   0      501       20    15210 2024-02-29 15:16:53.000000 longport-1.0.8/src/quote/context.rs
--rw-r--r--   0      501       20     1924 2024-02-29 15:16:53.000000 longport-1.0.8/src/quote/mod.rs
--rw-r--r--   0      501       20     2610 2024-02-29 15:16:53.000000 longport-1.0.8/src/quote/push.rs
--rw-r--r--   0      501       20    24604 2024-02-29 15:16:53.000000 longport-1.0.8/src/quote/types.rs
--rw-r--r--   0      501       20     3554 2024-02-29 15:16:53.000000 longport-1.0.8/src/time.rs
--rw-r--r--   0      501       20    12571 2024-02-29 15:16:53.000000 longport-1.0.8/src/trade/context.rs
--rw-r--r--   0      501       20     1232 2024-02-29 15:16:53.000000 longport-1.0.8/src/trade/mod.rs
--rw-r--r--   0      501       20      692 2024-02-29 15:16:53.000000 longport-1.0.8/src/trade/push.rs
--rw-r--r--   0      501       20    18297 2024-02-29 15:16:53.000000 longport-1.0.8/src/trade/types.rs
--rw-r--r--   0      501       20      561 2024-02-29 15:16:53.000000 longport-1.0.8/src/types.rs
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 longport-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport-proto/Cargo.toml
+-rw-r--r--   0      501       20       96 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/error/error.proto
+-rw-r--r--   0      501       20      282 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/.gitignore
+-rw-r--r--   0      501       20       51 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/README.md
+-rw-r--r--   0      501       20      257 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/buf.gen.yaml
+-rw-r--r--   0      501       20     1022 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/control/control.proto
+-rw-r--r--   0      501       20      108 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/control/error.proto
+-rw-r--r--   0      501       20    67241 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.cc
+-rw-r--r--   0      501       20    64169 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.h
+-rw-r--r--   0      501       20    13071 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.cc
+-rw-r--r--   0      501       20    11600 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.h
+-rw-r--r--   0      501       20  1038612 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.cc
+-rw-r--r--   0      501       20  1199727 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.h
+-rw-r--r--   0      501       20    63373 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.cc
+-rw-r--r--   0      501       20    84723 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.h
+-rw-r--r--   0      501       20    22451 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/control.pb.go
+-rw-r--r--   0      501       20     5856 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/error.pb.go
+-rw-r--r--   0      501       20      108 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.mod
+-rw-r--r--   0      501       20      739 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.sum
+-rw-r--r--   0      501       20   278532 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/quote/api.pb.go
+-rw-r--r--   0      501       20    23115 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/trade/subscribe.pb.go
+-rw-r--r--   0      501       20     3638 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/control_pb2.py
+-rw-r--r--   0      501       20     1717 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/error_pb2.py
+-rw-r--r--   0      501       20    34401 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/quote/api_pb2.py
+-rw-r--r--   0      501       20     3660 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/trade/subscribe_pb2.py
+-rw-r--r--   0      501       20    14370 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/quote/api.proto
+-rw-r--r--   0      501       20     1183 2024-02-29 15:53:55.000000 longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/trade/subscribe.proto
+-rw-r--r--   0      501       20      287 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/src/lib.rs
+-rw-r--r--   0      501       20     2246 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/src/longportapp.control.v1.rs
+-rw-r--r--   0      501       20    35478 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/src/longportapp.quote.v1.rs
+-rw-r--r--   0      501       20     2691 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/src/longportapp.trade.v1.rs
+-rw-r--r--   0      501       20      191 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-proto/src/qop.error.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport/Cargo.toml
+-rw-r--r--   0      501       20      251 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/CHANGELOG.md
+-rw-r--r--   0      501       20      795 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/Makefile.toml
+-rw-r--r--   0      501       20     4139 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/README.md
+-rw-r--r--   0      501       20      147 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/blocking/error.rs
+-rw-r--r--   0      501       20      182 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/blocking/mod.rs
+-rw-r--r--   0      501       20    28831 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/blocking/quote.rs
+-rw-r--r--   0      501       20     3890 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/blocking/runtime.rs
+-rw-r--r--   0      501       20    13183 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/blocking/trade.rs
+-rw-r--r--   0      501       20     7532 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/config.rs
+-rw-r--r--   0      501       20     3644 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/error.rs
+-rw-r--r--   0      501       20      593 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/lib.rs
+-rw-r--r--   0      501       20     1518 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/macros.rs
+-rw-r--r--   0      501       20     1934 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/cache.rs
+-rw-r--r--   0      501       20     2083 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/cmd_code.rs
+-rw-r--r--   0      501       20    49869 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/context.rs
+-rw-r--r--   0      501       20    34534 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/core.rs
+-rw-r--r--   0      501       20     1129 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/mod.rs
+-rw-r--r--   0      501       20     5455 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/push_types.rs
+-rw-r--r--   0      501       20     4082 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/store.rs
+-rw-r--r--   0      501       20     1547 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/sub_flags.rs
+-rw-r--r--   0      501       20    44392 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/types.rs
+-rw-r--r--   0      501       20      350 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/quote/utils.rs
+-rw-r--r--   0      501       20     7128 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/serde_utils.rs
+-rw-r--r--   0      501       20      282 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/cmd_code.rs
+-rw-r--r--   0      501       20    21658 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/context.rs
+-rw-r--r--   0      501       20     8478 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/core.rs
+-rw-r--r--   0      501       20     1057 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/mod.rs
+-rw-r--r--   0      501       20     3512 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/push_types.rs
+-rw-r--r--   0      501       20     1561 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/estimate_max_purchase_quantity.rs
+-rw-r--r--   0      501       20     1660 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_cash_flow.rs
+-rw-r--r--   0      501       20      682 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_fund_positions.rs
+-rw-r--r--   0      501       20     1374 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_history_executions.rs
+-rw-r--r--   0      501       20     2281 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_history_orders.rs
+-rw-r--r--   0      501       20      687 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_stock_positions.rs
+-rw-r--r--   0      501       20      909 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_today_executions.rs
+-rw-r--r--   0      501       20     1806 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/get_today_orders.rs
+-rw-r--r--   0      501       20      775 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/mod.rs
+-rw-r--r--   0      501       20     2539 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/replace_order.rs
+-rw-r--r--   0      501       20     3673 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/requests/submit_order.rs
+-rw-r--r--   0      501       20    38596 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/trade/types.rs
+-rw-r--r--   0      501       20      378 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport/src/types.rs
+-rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport-candlesticks/Cargo.toml
+-rw-r--r--   0      501       20      174 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-candlesticks/src/lib.rs
+-rw-r--r--   0      501       20     3423 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-candlesticks/src/market.rs
+-rw-r--r--   0      501       20    21444 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-candlesticks/src/merger.rs
+-rw-r--r--   0      501       20      556 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-candlesticks/src/types.rs
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport-httpcli/Cargo.toml
+-rw-r--r--   0      501       20     2578 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/client.rs
+-rw-r--r--   0      501       20     2619 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/config.rs
+-rw-r--r--   0      501       20     1622 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/error.rs
+-rw-r--r--   0      501       20     2343 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/geo.rs
+-rw-r--r--   0      501       20      488 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/lib.rs
+-rw-r--r--   0      501       20    27363 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/qs.rs
+-rw-r--r--   0      501       20     9790 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/request.rs
+-rw-r--r--   0      501       20     1910 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/signature.rs
+-rw-r--r--   0      501       20      695 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-httpcli/src/timestamp.rs
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport-wscli/Cargo.toml
+-rw-r--r--   0      501       20    13801 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-wscli/src/client.rs
+-rw-r--r--   0      501       20     6818 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-wscli/src/codec.rs
+-rw-r--r--   0      501       20     1785 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-wscli/src/error.rs
+-rw-r--r--   0      501       20      320 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-wscli/src/event.rs
+-rw-r--r--   0      501       20      396 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-wscli/src/lib.rs
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 longport-1.0.9/local_dependencies/longport-python-macros/Cargo.toml
+-rw-r--r--   0      501       20      541 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-python-macros/src/error.rs
+-rw-r--r--   0      501       20      692 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-python-macros/src/lib.rs
+-rw-r--r--   0      501       20     2561 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-python-macros/src/pyenum.rs
+-rw-r--r--   0      501       20     3356 2024-02-29 15:53:54.000000 longport-1.0.9/local_dependencies/longport-python-macros/src/pyobject.rs
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 longport-1.0.9/Cargo.toml
+-rw-r--r--   0      501       20      210 2024-02-29 15:53:54.000000 longport-1.0.9/.cargo/config.toml
+-rw-r--r--   0      501       20        4 2024-02-29 15:53:54.000000 longport-1.0.9/.gitignore
+-rw-r--r--   0      501       20      252 2024-02-29 15:53:54.000000 longport-1.0.9/CHANGELOG.md
+-rw-r--r--   0      501       20      358 2024-02-29 15:53:54.000000 longport-1.0.9/Makefile.toml
+-rw-r--r--   0      501       20     2370 2024-02-29 15:53:54.000000 longport-1.0.9/README.md
+-rw-r--r--   0      501       20       71 2024-02-29 15:53:54.000000 longport-1.0.9/build.rs
+-rw-r--r--   0      501       20       38 2024-02-29 15:53:54.000000 longport-1.0.9/docs/config.md
+-rw-r--r--   0      501       20     2330 2024-02-29 15:53:54.000000 longport-1.0.9/docs/index.md
+-rw-r--r--   0      501       20       50 2024-02-29 15:53:54.000000 longport-1.0.9/docs/quote_context.md
+-rw-r--r--   0      501       20       39 2024-02-29 15:53:54.000000 longport-1.0.9/docs/reference_all.md
+-rw-r--r--   0      501       20       91 2024-02-29 15:53:54.000000 longport-1.0.9/docs/requirements.txt
+-rw-r--r--   0      501       20       50 2024-02-29 15:53:54.000000 longport-1.0.9/docs/trade_context.md
+-rw-r--r--   0      501       20      811 2024-02-29 15:53:54.000000 longport-1.0.9/mkdocs.yml
+-rw-r--r--   0      501       20      803 2024-02-29 15:53:54.000000 longport-1.0.9/pyproject.toml
+-rw-r--r--   0      501       20      473 2024-02-29 15:53:54.000000 longport-1.0.9/pysrc/longport/__init__.py
+-rw-r--r--   0      501       20        0 2024-02-29 15:53:54.000000 longport-1.0.9/pysrc/longport/openapi.py
+-rw-r--r--   0      501       20    82923 2024-02-29 15:53:54.000000 longport-1.0.9/pysrc/longport/openapi.pyi
+-rw-r--r--   0      501       20        0 2024-02-29 15:53:54.000000 longport-1.0.9/pysrc/longport/py.typed
+-rw-r--r--   0      501       20     1817 2024-02-29 15:53:54.000000 longport-1.0.9/src/config.rs
+-rw-r--r--   0      501       20     2205 2024-02-29 15:53:54.000000 longport-1.0.9/src/decimal.rs
+-rw-r--r--   0      501       20      375 2024-02-29 15:53:54.000000 longport-1.0.9/src/error.rs
+-rw-r--r--   0      501       20     2583 2024-02-29 15:53:54.000000 longport-1.0.9/src/http_client.rs
+-rw-r--r--   0      501       20      546 2024-02-29 15:53:54.000000 longport-1.0.9/src/lib.rs
+-rw-r--r--   0      501       20    15210 2024-02-29 15:53:54.000000 longport-1.0.9/src/quote/context.rs
+-rw-r--r--   0      501       20     1924 2024-02-29 15:53:54.000000 longport-1.0.9/src/quote/mod.rs
+-rw-r--r--   0      501       20     2610 2024-02-29 15:53:54.000000 longport-1.0.9/src/quote/push.rs
+-rw-r--r--   0      501       20    24604 2024-02-29 15:53:54.000000 longport-1.0.9/src/quote/types.rs
+-rw-r--r--   0      501       20     3554 2024-02-29 15:53:54.000000 longport-1.0.9/src/time.rs
+-rw-r--r--   0      501       20    12571 2024-02-29 15:53:54.000000 longport-1.0.9/src/trade/context.rs
+-rw-r--r--   0      501       20     1232 2024-02-29 15:53:54.000000 longport-1.0.9/src/trade/mod.rs
+-rw-r--r--   0      501       20      692 2024-02-29 15:53:54.000000 longport-1.0.9/src/trade/push.rs
+-rw-r--r--   0      501       20    18297 2024-02-29 15:53:54.000000 longport-1.0.9/src/trade/types.rs
+-rw-r--r--   0      501       20      561 2024-02-29 15:53:54.000000 longport-1.0.9/src/types.rs
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 longport-1.0.9/PKG-INFO
```

### Comparing `longport-1.0.8/local_dependencies/longport-candlesticks/src/market.rs` & `longport-1.0.9/local_dependencies/longport-candlesticks/src/market.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-candlesticks/src/merger.rs` & `longport-1.0.9/local_dependencies/longport-candlesticks/src/merger.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-candlesticks/src/types.rs` & `longport-1.0.9/local_dependencies/longport-candlesticks/src/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/control/control.proto` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/control/control.proto`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.cc` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.cc`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.h` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/control.pb.h`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.cc` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.cc`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.h` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/control/error.pb.h`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.cc` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.cc`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.h` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/quote/api.pb.h`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.cc` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.cc`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.h` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/cpp/trade/subscribe.pb.h`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/control.pb.go` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/control.pb.go`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/error.pb.go` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/control/error.pb.go`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.sum` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/go.sum`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/quote/api.pb.go` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/quote/api.pb.go`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/go/trade/subscribe.pb.go` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/go/trade/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/control_pb2.py` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/control_pb2.py`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/error_pb2.py` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/control/error_pb2.py`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/quote/api_pb2.py` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/quote/api_pb2.py`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/gen/python/trade/subscribe_pb2.py` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/gen/python/trade/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/quote/api.proto` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/quote/api.proto`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/openapi-protobufs/trade/subscribe.proto` & `longport-1.0.9/local_dependencies/longport-proto/openapi-protobufs/trade/subscribe.proto`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/src/longportapp.control.v1.rs` & `longport-1.0.9/local_dependencies/longport-proto/src/longportapp.control.v1.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/src/longportapp.quote.v1.rs` & `longport-1.0.9/local_dependencies/longport-proto/src/longportapp.quote.v1.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-proto/src/longportapp.trade.v1.rs` & `longport-1.0.9/local_dependencies/longport-proto/src/longportapp.trade.v1.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-python-macros/src/error.rs` & `longport-1.0.9/local_dependencies/longport-python-macros/src/error.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-python-macros/src/lib.rs` & `longport-1.0.9/local_dependencies/longport-python-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-python-macros/src/pyenum.rs` & `longport-1.0.9/local_dependencies/longport-python-macros/src/pyenum.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-python-macros/src/pyobject.rs` & `longport-1.0.9/local_dependencies/longport-python-macros/src/pyobject.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/Cargo.toml` & `longport-1.0.9/local_dependencies/longport/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [package]
 edition = "2021"
 name = "longport"
-version = "1.0.8"
+version = "1.0.9"
 description = "LongPort OpenAPI SDK for Rust"
 homepage = "https://open.longportapp.com/en/"
 readme = "README.md"
 repository = "https://github.com/longportapp/openapi-sdk"
 license = "MIT OR Apache-2.0"
 keywords = ["longport", "openapi", "sdk"]
 categories = ["api-bindings"]
 
 [features]
 blocking = ["flume"]
 
 [dependencies]
-longport-wscli = { path = "../longport-wscli", version = "1.0.8" }
-longport-httpcli = { path = "../longport-httpcli", version = "1.0.8" }
-longport-proto = { path = "../longport-proto", version = "1.0.8" }
-longport-candlesticks = { path = "../longport-candlesticks", version = "1.0.8" }
+longport-wscli = { path = "../longport-wscli", version = "1.0.9" }
+longport-httpcli = { path = "../longport-httpcli", version = "1.0.9" }
+longport-proto = { path = "../longport-proto", version = "1.0.9" }
+longport-candlesticks = { path = "../longport-candlesticks", version = "1.0.9" }
 
 tokio = { version = "1.18.2", features = [
   "time",
   "rt",
   "macros",
   "sync",
   "net",
```

### Comparing `longport-1.0.8/local_dependencies/longport/Makefile.toml` & `longport-1.0.9/local_dependencies/longport/Makefile.toml`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/README.md` & `longport-1.0.9/local_dependencies/longport/README.md`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/blocking/quote.rs` & `longport-1.0.9/local_dependencies/longport/src/blocking/quote.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/blocking/runtime.rs` & `longport-1.0.9/local_dependencies/longport/src/blocking/runtime.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/blocking/trade.rs` & `longport-1.0.9/local_dependencies/longport/src/blocking/trade.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/config.rs` & `longport-1.0.9/local_dependencies/longport/src/config.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/error.rs` & `longport-1.0.9/local_dependencies/longport/src/error.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/lib.rs` & `longport-1.0.9/local_dependencies/longport/src/lib.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/macros.rs` & `longport-1.0.9/local_dependencies/longport/src/macros.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/cache.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/cache.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/cmd_code.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/cmd_code.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/context.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/context.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/core.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/core.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/mod.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/mod.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/push_types.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/push_types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/store.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/store.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/sub_flags.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/sub_flags.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/quote/types.rs` & `longport-1.0.9/local_dependencies/longport/src/quote/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/serde_utils.rs` & `longport-1.0.9/local_dependencies/longport/src/serde_utils.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/context.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/context.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/core.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/core.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/mod.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/mod.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/push_types.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/push_types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/estimate_max_purchase_quantity.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/estimate_max_purchase_quantity.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_cash_flow.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_cash_flow.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_fund_positions.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_fund_positions.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_history_executions.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_history_executions.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_history_orders.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_history_orders.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_stock_positions.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_stock_positions.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_today_executions.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_today_executions.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/get_today_orders.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/get_today_orders.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/mod.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/mod.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/replace_order.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/replace_order.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/requests/submit_order.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/requests/submit_order.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport/src/trade/types.rs` & `longport-1.0.9/local_dependencies/longport/src/trade/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-wscli/Cargo.toml` & `longport-1.0.9/local_dependencies/longport-wscli/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [package]
 name = "longport-wscli"
-version = "1.0.8"
+version = "1.0.9"
 edition = "2021"
 description = "LongPort Websocket SDK for Rust"
 license = "MIT OR Apache-2.0"
 
 [dependencies]
-longport-proto = { path = "../longport-proto", version = "1.0.8" }
+longport-proto = { path = "../longport-proto", version = "1.0.9" }
 
 tokio = { version = "1.18.2", features = [
   "time",
   "rt",
   "macros",
   "sync",
   "net",
```

### Comparing `longport-1.0.8/local_dependencies/longport-wscli/src/client.rs` & `longport-1.0.9/local_dependencies/longport-wscli/src/client.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-wscli/src/codec.rs` & `longport-1.0.9/local_dependencies/longport-wscli/src/codec.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-wscli/src/error.rs` & `longport-1.0.9/local_dependencies/longport-wscli/src/error.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/Cargo.toml` & `longport-1.0.9/local_dependencies/longport-httpcli/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "longport-httpcli"
-version = "1.0.8"
+version = "1.0.9"
 description = "LongPort HTTP SDK for Rust"
 license = "MIT OR Apache-2.0"
 
 [dependencies]
 futures-util = "0.3.21"
 hmac = "0.12.1"
 parking_lot = "0.12.0"
```

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/client.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/client.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/config.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/config.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/error.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/error.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/geo.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/geo.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/qs.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/qs.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/request.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/request.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/signature.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/signature.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/local_dependencies/longport-httpcli/src/timestamp.rs` & `longport-1.0.9/local_dependencies/longport-httpcli/src/timestamp.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/Cargo.toml` & `longport-1.0.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "longport-python"
-version = "1.0.8"
+version = "1.0.9"
 description = "LongPort OpenAPI SDK for Python"
 homepage = "https://open.longportapp.com/en/"
 readme = "README.md"
 repository = "https://github.com/longportapp/openapi-sdk"
 license = "MIT OR Apache-2.0"
 keywords = ["longport", "openapi", "sdk"]
 categories = ["api-bindings"]
```

### Comparing `longport-1.0.8/README.md` & `longport-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/docs/index.md` & `longport-1.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/mkdocs.yml` & `longport-1.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/pyproject.toml` & `longport-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/pysrc/longport/openapi.pyi` & `longport-1.0.9/pysrc/longport/openapi.pyi`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/config.rs` & `longport-1.0.9/src/config.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/decimal.rs` & `longport-1.0.9/src/decimal.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/http_client.rs` & `longport-1.0.9/src/http_client.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/lib.rs` & `longport-1.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/quote/context.rs` & `longport-1.0.9/src/quote/context.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/quote/mod.rs` & `longport-1.0.9/src/quote/mod.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/quote/push.rs` & `longport-1.0.9/src/quote/push.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/quote/types.rs` & `longport-1.0.9/src/quote/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/time.rs` & `longport-1.0.9/src/time.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/trade/context.rs` & `longport-1.0.9/src/trade/context.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/trade/mod.rs` & `longport-1.0.9/src/trade/mod.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/trade/push.rs` & `longport-1.0.9/src/trade/push.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/trade/types.rs` & `longport-1.0.9/src/trade/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/src/types.rs` & `longport-1.0.9/src/types.rs`

 * *Files identical despite different names*

### Comparing `longport-1.0.8/PKG-INFO` & `longport-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: longport
-Version: 1.0.8
+Version: 1.0.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Summary: A Python library for LongPort Open API
 Keywords: longport,openapi,sdk
 Home-Page: https://open.longportapp.com/en/
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://open.longportapp.com/en/docs
-Project-URL: repository, https://github.com/longportapp/openapi-sdk
 Project-URL: homepage, https://open.longportapp.com/en/
+Project-URL: documentation, https://open.longportapp.com/en/docs
 Project-URL: changelog, https://github.com/longportapp/openapi-sdk/blob/master/python/CHANGELOG.md
+Project-URL: repository, https://github.com/longportapp/openapi-sdk
 
 # LongPort OpenAPI SDK for Python
 
 `longport` provides an easy-to-use interface for invokes [`LongPort OpenAPI`](https://open.longportapp.com/en/).
 
 ## Quickstart
```

