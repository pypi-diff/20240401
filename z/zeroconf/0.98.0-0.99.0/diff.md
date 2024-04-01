# Comparing `tmp/zeroconf-0.98.0.tar.gz` & `tmp/zeroconf-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.98.0.tar", max compression
+gzip compressed data, was "zeroconf-0.99.0.tar", max compression
```

## Comparing `zeroconf-0.98.0.tar` & `zeroconf-0.99.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    66794 2023-09-06 15:55:54.410210 zeroconf-0.98.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-09-06 15:55:53.342190 zeroconf-0.98.0/COPYING
--rw-r--r--   0        0        0     4407 2023-09-06 15:55:53.342190 zeroconf-0.98.0/README.rst
--rw-r--r--   0        0        0     1417 2023-09-06 15:55:53.342190 zeroconf-0.98.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-09-06 15:55:53.342190 zeroconf-0.98.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-09-06 15:55:53.342190 zeroconf-0.98.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-09-06 15:55:53.342190 zeroconf-0.98.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-09-06 15:55:53.342190 zeroconf-0.98.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-09-06 15:55:54.494212 zeroconf-0.98.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-09-06 15:55:54.422211 zeroconf-0.98.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0     1609 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0     9455 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    28030 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2602 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18409 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     5899 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_engine.py
--rw-r--r--   0        0        0     2167 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0      971 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/__init__.py
--rw-r--r--   0        0        0     3315 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/answers.py
--rw-r--r--   0        0        0     4489 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/multicast_outgoing_queue.py
--rw-r--r--   0        0        0     2067 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/query_handler.pxd
--rw-r--r--   0        0        0    11937 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/query_handler.py
--rw-r--r--   0        0        0      830 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/record_manager.pxd
--rw-r--r--   0        0        0     8596 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_handlers/record_manager.py
--rw-r--r--   0        0        0      574 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_history.pxd
--rw-r--r--   0        0        0     3177 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0      883 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_listener.pxd
--rw-r--r--   0        0        0     8295 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_listener.py
--rw-r--r--   0        0        0     2980 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2884 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14475 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17896 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2419 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    23370 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    29880 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0      530 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/registry.pxd
--rw-r--r--   0        0        0     4089 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2053 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_transport.py
--rw-r--r--   0        0        0     2910 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4987 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6928 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0       69 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/time.pxd
--rw-r--r--   0        0        0     1325 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11450 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4560 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-09-06 15:55:53.346191 zeroconf-0.98.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2708 2023-09-06 15:55:53.346191 zeroconf-0.98.0/tests/__init__.py
--rw-r--r--   0        0        0     1018 2023-09-06 15:55:53.346191 zeroconf-0.98.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/services/__init__.py
--rw-r--r--   0        0        0    44213 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    51451 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     4677 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/services/test_types.py
--rw-r--r--   0        0        0    46404 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_cache.py
--rw-r--r--   0        0        0    23549 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_dns.py
--rw-r--r--   0        0        0     3396 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_engine.py
--rw-r--r--   0        0        0     5021 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    67805 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_init.py
--rw-r--r--   0        0        0     7643 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_listener.py
--rw-r--r--   0        0        0     3396 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5103 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     3214 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-09-06 15:55:53.350190 zeroconf-0.98.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 zeroconf-0.98.0/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.98.0/PKG-INFO
+-rw-r--r--   0        0        0    67073 2023-09-06 20:03:59.706131 zeroconf-0.99.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-09-06 20:03:58.886131 zeroconf-0.99.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-09-06 20:03:58.886131 zeroconf-0.99.0/README.rst
+-rw-r--r--   0        0        0     1417 2023-09-06 20:03:58.886131 zeroconf-0.99.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-09-06 20:03:58.886131 zeroconf-0.99.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-09-06 20:03:58.886131 zeroconf-0.99.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-09-06 20:03:58.886131 zeroconf-0.99.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-09-06 20:03:58.886131 zeroconf-0.99.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-09-06 20:03:59.790130 zeroconf-0.99.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-09-06 20:03:59.722131 zeroconf-0.99.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0     1609 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0     9455 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    28030 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2602 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18409 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     5899 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_engine.py
+-rw-r--r--   0        0        0     2167 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0      971 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_handlers/__init__.py
+-rw-r--r--   0        0        0     3315 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_handlers/answers.py
+-rw-r--r--   0        0        0     4489 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_handlers/multicast_outgoing_queue.py
+-rw-r--r--   0        0        0     2067 2023-09-06 20:03:58.886131 zeroconf-0.99.0/src/zeroconf/_handlers/query_handler.pxd
+-rw-r--r--   0        0        0    11937 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_handlers/query_handler.py
+-rw-r--r--   0        0        0      830 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_handlers/record_manager.pxd
+-rw-r--r--   0        0        0     8596 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_handlers/record_manager.py
+-rw-r--r--   0        0        0      574 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_history.pxd
+-rw-r--r--   0        0        0     3177 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0      883 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_listener.pxd
+-rw-r--r--   0        0        0     8295 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_listener.py
+-rw-r--r--   0        0        0     2980 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2884 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14475 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17896 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2419 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    23370 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    30317 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0      530 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/registry.pxd
+-rw-r--r--   0        0        0     4089 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2053 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_transport.py
+-rw-r--r--   0        0        0     2910 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4987 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6928 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0       69 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/time.pxd
+-rw-r--r--   0        0        0     1325 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11450 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4560 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-09-06 20:03:58.890131 zeroconf-0.99.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2708 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/__init__.py
+-rw-r--r--   0        0        0     1018 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    44213 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    51451 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4677 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    46404 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-09-06 20:03:58.890131 zeroconf-0.99.0/tests/test_cache.py
+-rw-r--r--   0        0        0    23549 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_dns.py
+-rw-r--r--   0        0        0     3396 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_engine.py
+-rw-r--r--   0        0        0     5021 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67805 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_init.py
+-rw-r--r--   0        0        0     7643 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_listener.py
+-rw-r--r--   0        0        0     3396 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5103 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     3214 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-09-06 20:03:58.894131 zeroconf-0.99.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 zeroconf-0.99.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.99.0/PKG-INFO
```

### Comparing `zeroconf-0.98.0/CHANGELOG.md` & `zeroconf-0.99.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.99.0 (2023-09-06)
+
+### Feature
+
+* Reduce IP Address parsing overhead in ServiceInfo ([#1257](https://github.com/python-zeroconf/python-zeroconf/issues/1257)) ([`83d0b7f`](https://github.com/python-zeroconf/python-zeroconf/commit/83d0b7fda2eb09c9c6e18b85f329d1ddc701e3fb))
+
 ## v0.98.0 (2023-09-06)
 
 ### Feature
 
 * Speed up decoding incoming packets ([#1256](https://github.com/python-zeroconf/python-zeroconf/issues/1256)) ([`ac081cf`](https://github.com/python-zeroconf/python-zeroconf/commit/ac081cf00addde1ceea2c076f73905fdb293de3a))
 
 ## v0.97.0 (2023-09-03)
```

### Comparing `zeroconf-0.98.0/COPYING` & `zeroconf-0.99.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/README.rst` & `zeroconf-0.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/build_ext.py` & `zeroconf-0.99.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/docs/Makefile` & `zeroconf-0.99.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/docs/conf.py` & `zeroconf-0.99.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/docs/index.rst` & `zeroconf-0.99.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/pyproject.toml` & `zeroconf-0.99.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.98.0"
+version = "0.99.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.98.0/src/zeroconf/__init__.py` & `zeroconf-0.99.0/src/zeroconf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.98.0'
+__version__ = '0.99.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.98.0/src/zeroconf/_cache.pxd` & `zeroconf-0.99.0/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_cache.py` & `zeroconf-0.99.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_core.py` & `zeroconf-0.99.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_dns.pxd` & `zeroconf-0.99.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_dns.py` & `zeroconf-0.99.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_engine.py` & `zeroconf-0.99.0/src/zeroconf/_engine.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_exceptions.py` & `zeroconf-0.99.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/__init__.py` & `zeroconf-0.99.0/src/zeroconf/_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/answers.py` & `zeroconf-0.99.0/src/zeroconf/_handlers/answers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/multicast_outgoing_queue.py` & `zeroconf-0.99.0/src/zeroconf/_handlers/multicast_outgoing_queue.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/query_handler.pxd` & `zeroconf-0.99.0/src/zeroconf/_handlers/query_handler.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/query_handler.py` & `zeroconf-0.99.0/src/zeroconf/_handlers/query_handler.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/record_manager.pxd` & `zeroconf-0.99.0/src/zeroconf/_handlers/record_manager.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_handlers/record_manager.py` & `zeroconf-0.99.0/src/zeroconf/_handlers/record_manager.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_history.pxd` & `zeroconf-0.99.0/src/zeroconf/_history.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_history.py` & `zeroconf-0.99.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_listener.pxd` & `zeroconf-0.99.0/src/zeroconf/_listener.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_listener.py` & `zeroconf-0.99.0/src/zeroconf/_listener.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_logger.py` & `zeroconf-0.99.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.99.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.99.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.99.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.99.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.99.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.99.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/browser.py` & `zeroconf-0.99.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/info.py` & `zeroconf-0.99.0/src/zeroconf/_services/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,21 @@
     # need to make subtypes a first class citizen
     service_name = service_type_name(info.name, strict=strict)
     if not info.type.endswith(service_name):
         raise BadTypeInNameException
     return info.name[: -len(service_name) - 1]
 
 
-_cached_ip_addresses = lru_cache(maxsize=256)(ip_address)
+@lru_cache(maxsize=512)
+def _cached_ip_addresses(address: Union[str, bytes, int]) -> Optional[Union[IPv4Address, IPv6Address]]:
+    """Cache IP addresses."""
+    try:
+        return ip_address(address)
+    except ValueError:
+        return None
 
 
 class ServiceInfo(RecordUpdateListener):
     """Service information.
 
     Constructor parameters are as follows:
 
@@ -223,24 +229,27 @@
         """
         self._ipv4_addresses.clear()
         self._ipv6_addresses.clear()
         self._dns_address_cache = None
         self._get_address_and_nsec_records_cache = None
 
         for address in value:
-            try:
-                addr = _cached_ip_addresses(address)
-            except ValueError:
+            addr = _cached_ip_addresses(address)
+            if addr is None:
                 raise TypeError(
                     "Addresses must either be IPv4 or IPv6 strings, bytes, or integers;"
                     f" got {address!r}. Hint: convert string addresses with socket.inet_pton"
                 )
             if addr.version == 4:
+                if TYPE_CHECKING:
+                    assert isinstance(addr, IPv4Address)
                 self._ipv4_addresses.append(addr)
             else:
+                if TYPE_CHECKING:
+                    assert isinstance(addr, IPv6Address)
                 self._ipv6_addresses.append(addr)
 
     @property
     def properties(self) -> Dict[Union[str, bytes], Optional[Union[str, bytes]]]:
         """If properties were set in the constructor this property returns the original dictionary
         of type `Dict[Union[bytes, str], Any]`.
 
@@ -390,19 +399,16 @@
         self, zc: 'Zeroconf', now: float, type: int
     ) -> List[Union[IPv4Address, IPv6Address]]:
         """Set IPv6 addresses from the cache."""
         address_list: List[Union[IPv4Address, IPv6Address]] = []
         for record in self._get_address_records_from_cache_by_type(zc, type):
             if record.is_expired(now):
                 continue
-            try:
-                ip_addr = _cached_ip_addresses(record.address)
-            except ValueError:
-                continue
-            else:
+            ip_addr = _cached_ip_addresses(record.address)
+            if ip_addr is not None:
                 address_list.append(ip_addr)
         address_list.reverse()  # Reverse to get LIFO order
         return address_list
 
     def _set_ipv6_addresses_from_cache(self, zc: 'Zeroconf', now: float) -> None:
         """Set IPv6 addresses from the cache."""
         if TYPE_CHECKING:
@@ -442,31 +448,34 @@
             return False
 
         record_key = record.key
         record_type = type(record)
         if record_key == self.server_key and record_type is DNSAddress:
             if TYPE_CHECKING:
                 assert isinstance(record, DNSAddress)
-            try:
-                ip_addr = _cached_ip_addresses(record.address)
-            except ValueError as ex:
-                log.warning("Encountered invalid address while processing %s: %s", record, ex)
+            ip_addr = _cached_ip_addresses(record.address)
+            if ip_addr is None:
+                log.warning("Encountered invalid address while processing %s: %s", record, record.address)
                 return False
 
-            if type(ip_addr) is IPv4Address:
+            if ip_addr.version == 4:
+                if TYPE_CHECKING:
+                    assert isinstance(ip_addr, IPv4Address)
                 ipv4_addresses = self._ipv4_addresses
                 if ip_addr not in ipv4_addresses:
                     ipv4_addresses.insert(0, ip_addr)
                     return True
                 elif ip_addr != ipv4_addresses[0]:
                     ipv4_addresses.remove(ip_addr)
                     ipv4_addresses.insert(0, ip_addr)
 
                 return False
 
+            if TYPE_CHECKING:
+                assert isinstance(ip_addr, IPv6Address)
             ipv6_addresses = self._ipv6_addresses
             if ip_addr not in self._ipv6_addresses:
                 ipv6_addresses.insert(0, ip_addr)
                 return True
             elif ip_addr != self._ipv6_addresses[0]:
                 ipv6_addresses.remove(ip_addr)
                 ipv6_addresses.insert(0, ip_addr)
@@ -512,15 +521,15 @@
         name = self.server or self._name
         ttl = override_ttl if override_ttl is not None else self.host_ttl
         class_ = _CLASS_IN_UNIQUE
         version_value = version.value
         records = [
             DNSAddress(
                 name,
-                _TYPE_AAAA if type(ip_addr) is IPv6Address else _TYPE_A,
+                _TYPE_AAAA if ip_addr.version == 6 else _TYPE_A,
                 class_,
                 ttl,
                 ip_addr.packed,
                 created=0.0,
             )
             for ip_addr in self._ip_addresses_by_version_value(version_value)
         ]
```

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/registry.pxd` & `zeroconf-0.99.0/src/zeroconf/_services/registry.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/registry.py` & `zeroconf-0.99.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_services/types.py` & `zeroconf-0.99.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_transport.py` & `zeroconf-0.99.0/src/zeroconf/_transport.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_updates.py` & `zeroconf-0.99.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.99.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.99.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_utils/name.py` & `zeroconf-0.99.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_utils/net.py` & `zeroconf-0.99.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/_utils/time.py` & `zeroconf-0.99.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/asyncio.py` & `zeroconf-0.99.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/src/zeroconf/const.py` & `zeroconf-0.99.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/__init__.py` & `zeroconf-0.99.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/conftest.py` & `zeroconf-0.99.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/services/__init__.py` & `zeroconf-0.99.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/services/test_browser.py` & `zeroconf-0.99.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/services/test_info.py` & `zeroconf-0.99.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/services/test_registry.py` & `zeroconf-0.99.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/services/test_types.py` & `zeroconf-0.99.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_asyncio.py` & `zeroconf-0.99.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_cache.py` & `zeroconf-0.99.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_core.py` & `zeroconf-0.99.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_dns.py` & `zeroconf-0.99.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_engine.py` & `zeroconf-0.99.0/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_exceptions.py` & `zeroconf-0.99.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_handlers.py` & `zeroconf-0.99.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_history.py` & `zeroconf-0.99.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_init.py` & `zeroconf-0.99.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_listener.py` & `zeroconf-0.99.0/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_logger.py` & `zeroconf-0.99.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_protocol.py` & `zeroconf-0.99.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_services.py` & `zeroconf-0.99.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/test_updates.py` & `zeroconf-0.99.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/utils/__init__.py` & `zeroconf-0.99.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/utils/test_asyncio.py` & `zeroconf-0.99.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/utils/test_name.py` & `zeroconf-0.99.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/tests/utils/test_net.py` & `zeroconf-0.99.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.98.0/setup.py` & `zeroconf-0.99.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.98.0',
+    'version': '0.99.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.98.0/PKG-INFO` & `zeroconf-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.98.0
+Version: 0.99.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

