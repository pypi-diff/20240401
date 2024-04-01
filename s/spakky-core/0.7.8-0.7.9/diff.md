# Comparing `tmp/spakky_core-0.7.8.tar.gz` & `tmp/spakky_core-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spakky_core-0.7.8.tar", max compression
+gzip compressed data, was "spakky_core-0.7.9.tar", max compression
```

## Comparing `spakky_core-0.7.8.tar` & `spakky_core-0.7.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1057 2024-03-08 11:16:45.266992 spakky_core-0.7.8/README.md
--rw-r--r--   0        0        0     2149 2024-03-08 11:16:45.266992 spakky_core-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/__init__.py
--rw-r--r--   0        0        0      553 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/advice.py
--rw-r--r--   0        0        0     1223 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/advisor.py
--rw-r--r--   0        0        0     2747 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/aspect.py
--rw-r--r--   0        0        0       95 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/error.py
--rw-r--r--   0        0        0     5894 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/aop/post_processor.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/__init__.py
--rw-r--r--   0        0        0     7925 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/application_context.py
--rw-r--r--   0        0        0     1298 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/autowired.py
--rw-r--r--   0        0        0     1754 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/bean.py
--rw-r--r--   0        0        0       96 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/error.py
--rw-r--r--   0        0        0      688 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/inject.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/__init__.py
--rw-r--r--   0        0        0     1363 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/bean_container.py
--rw-r--r--   0        0        0      317 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/bean_processor.py
--rw-r--r--   0        0        0      333 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/bean_processor_registry.py
--rw-r--r--   0        0        0      627 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/bean_registry.py
--rw-r--r--   0        0        0      239 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/interfaces/bean_scanner.py
--rw-r--r--   0        0        0      139 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/bean/primary.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/__init__.py
--rw-r--r--   0        0        0     3339 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/annotation.py
--rw-r--r--   0        0        0      151 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/error.py
--rw-r--r--   0        0        0     1531 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/importing.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/interfaces/__init__.py
--rw-r--r--   0        0        0      409 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/interfaces/cloneable.py
--rw-r--r--   0        0        0      663 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/interfaces/comparable.py
--rw-r--r--   0        0        0     1096 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/interfaces/disposable.py
--rw-r--r--   0        0        0      489 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/interfaces/equatable.py
--rw-r--r--   0        0        0      742 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/mutability.py
--rw-r--r--   0        0        0     2098 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/proxy.py
--rw-r--r--   0        0        0      606 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/core/types.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/__init__.py
--rw-r--r--   0        0        0     1197 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/base64_encoder.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/cryptor/__init__.py
--rw-r--r--   0        0        0     1853 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/cryptor/aes.py
--rw-r--r--   0        0        0     2304 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/cryptor/gcm.py
--rw-r--r--   0        0        0      297 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/cryptor/interface.py
--rw-r--r--   0        0        0     2485 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/cryptor/rsa.py
--rw-r--r--   0        0        0      768 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/error.py
--rw-r--r--   0        0        0     1745 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/hash.py
--rw-r--r--   0        0        0     1916 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/hmac.py
--rw-r--r--   0        0        0     7232 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/jwt.py
--rw-r--r--   0        0        0     1642 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/key.py
--rw-r--r--   0        0        0     3477 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/cryptography/password.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/domain/__init__.py
--rw-r--r--   0        0        0      156 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/domain/error.py
--rw-r--r--   0        0        0      918 2024-03-08 11:16:45.266992 spakky_core-0.7.8/spakky/domain/models/aggregate_root.py
--rw-r--r--   0        0        0     1435 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/models/domain_event.py
--rw-r--r--   0        0        0     1361 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/models/entity.py
--rw-r--r--   0        0        0     1035 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/models/value_object.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/event/__init__.py
--rw-r--r--   0        0        0      651 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/event/event_publisher.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/external/__init__.py
--rw-r--r--   0        0        0     1766 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/external/proxy.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/persistency/__init__.py
--rw-r--r--   0        0        0     2585 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/persistency/repository.py
--rw-r--r--   0        0        0     2159 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/ports/persistency/transaction.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/usecases/__init__.py
--rw-r--r--   0        0        0      695 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/usecases/command.py
--rw-r--r--   0        0        0      679 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/domain/usecases/query.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/extensions/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/extensions/logging.py
--rw-r--r--   0        0        0     1344 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/extensions/transactional.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/py.typed
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/stereotype/__init__.py
--rw-r--r--   0        0        0      117 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/stereotype/configuration.py
--rw-r--r--   0        0        0      122 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/stereotype/controller.py
--rw-r--r--   0        0        0      114 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/stereotype/repository.py
--rw-r--r--   0        0        0      111 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/stereotype/usecase.py
--rw-r--r--   0        0        0        0 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/utils/__init__.py
--rw-r--r--   0        0        0      280 2024-03-08 11:16:45.270992 spakky_core-0.7.8/spakky/utils/casing.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 spakky_core-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-03-10 11:39:56.328840 spakky_core-0.7.9/README.md
+-rw-r--r--   0        0        0     2149 2024-03-10 11:39:56.328840 spakky_core-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/__init__.py
+-rw-r--r--   0        0        0      553 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/advice.py
+-rw-r--r--   0        0        0     1223 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/advisor.py
+-rw-r--r--   0        0        0     2747 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/aspect.py
+-rw-r--r--   0        0        0       95 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/error.py
+-rw-r--r--   0        0        0     6009 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/aop/post_processor.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/__init__.py
+-rw-r--r--   0        0        0     7925 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/application_context.py
+-rw-r--r--   0        0        0     1298 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/autowired.py
+-rw-r--r--   0        0        0     1754 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/bean.py
+-rw-r--r--   0        0        0       96 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/error.py
+-rw-r--r--   0        0        0      688 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/inject.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/__init__.py
+-rw-r--r--   0        0        0     1363 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/bean_container.py
+-rw-r--r--   0        0        0      317 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/bean_processor.py
+-rw-r--r--   0        0        0      333 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/bean_processor_registry.py
+-rw-r--r--   0        0        0      627 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/bean_registry.py
+-rw-r--r--   0        0        0      239 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/interfaces/bean_scanner.py
+-rw-r--r--   0        0        0      139 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/bean/primary.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/__init__.py
+-rw-r--r--   0        0        0     3339 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/annotation.py
+-rw-r--r--   0        0        0      151 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/error.py
+-rw-r--r--   0        0        0     1531 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/importing.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/interfaces/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/interfaces/cloneable.py
+-rw-r--r--   0        0        0      663 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/interfaces/comparable.py
+-rw-r--r--   0        0        0     1096 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/interfaces/disposable.py
+-rw-r--r--   0        0        0      489 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/interfaces/equatable.py
+-rw-r--r--   0        0        0      742 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/mutability.py
+-rw-r--r--   0        0        0     2098 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/proxy.py
+-rw-r--r--   0        0        0      606 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/core/types.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/__init__.py
+-rw-r--r--   0        0        0     1197 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/base64_encoder.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/cryptor/__init__.py
+-rw-r--r--   0        0        0     1853 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/cryptor/aes.py
+-rw-r--r--   0        0        0     2304 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/cryptor/gcm.py
+-rw-r--r--   0        0        0      297 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/cryptor/interface.py
+-rw-r--r--   0        0        0     2485 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/cryptor/rsa.py
+-rw-r--r--   0        0        0      768 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/error.py
+-rw-r--r--   0        0        0     1745 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/hash.py
+-rw-r--r--   0        0        0     1916 2024-03-10 11:39:56.328840 spakky_core-0.7.9/spakky/cryptography/hmac.py
+-rw-r--r--   0        0        0     7232 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/cryptography/jwt.py
+-rw-r--r--   0        0        0     1642 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/cryptography/key.py
+-rw-r--r--   0        0        0     3477 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/cryptography/password.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/__init__.py
+-rw-r--r--   0        0        0      156 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/error.py
+-rw-r--r--   0        0        0      918 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/models/aggregate_root.py
+-rw-r--r--   0        0        0     1435 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/models/domain_event.py
+-rw-r--r--   0        0        0     1361 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/models/entity.py
+-rw-r--r--   0        0        0     1035 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/models/value_object.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/event/__init__.py
+-rw-r--r--   0        0        0      651 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/event/event_publisher.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/external/__init__.py
+-rw-r--r--   0        0        0     1766 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/external/proxy.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/persistency/__init__.py
+-rw-r--r--   0        0        0     2585 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/persistency/repository.py
+-rw-r--r--   0        0        0     2159 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/ports/persistency/transaction.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/usecases/__init__.py
+-rw-r--r--   0        0        0      695 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/usecases/command.py
+-rw-r--r--   0        0        0      671 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/domain/usecases/query.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/extensions/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/extensions/logging.py
+-rw-r--r--   0        0        0     1344 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/extensions/transactional.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/py.typed
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/stereotype/__init__.py
+-rw-r--r--   0        0        0      117 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/stereotype/configuration.py
+-rw-r--r--   0        0        0      122 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/stereotype/controller.py
+-rw-r--r--   0        0        0      114 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/stereotype/repository.py
+-rw-r--r--   0        0        0      111 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/stereotype/usecase.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/utils/__init__.py
+-rw-r--r--   0        0        0      280 2024-03-10 11:39:56.332840 spakky_core-0.7.9/spakky/utils/casing.py
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 spakky_core-0.7.9/PKG-INFO
```

### Comparing `spakky_core-0.7.8/README.md` & `spakky_core-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/pyproject.toml` & `spakky_core-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spakky-core"
-version = "0.7.8"
+version = "0.7.9"
 description = "Highly abstracted Framework core to use DDD & DI/IoC & AOP & Etc..."
 authors = ["Spakky <sejong418@icloud.com>"]
 packages = [{ include = "spakky" }]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `spakky_core-0.7.8/spakky/aop/advice.py` & `spakky_core-0.7.9/spakky/aop/advice.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/aop/advisor.py` & `spakky_core-0.7.9/spakky/aop/advisor.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/aop/aspect.py` & `spakky_core-0.7.9/spakky/aop/aspect.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/aop/post_processor.py` & `spakky_core-0.7.9/spakky/aop/post_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -103,55 +103,61 @@
                 self.__container.single(required_type=advisor), runnable
             )
         return await runnable(*args, **kwargs)
 
 
 class AspectBeanPostProcessor(IBeanPostProcessor):
     __logger: Logger
+    __cache: dict[type, object]
 
     def __init__(self, logger: Logger) -> None:
         super().__init__()
         self.__logger = logger
+        self.__cache = {}
+
+    def __set_cache(self, type_: type, bean: object) -> None:
+        self.__cache[type_] = bean
+
+    def __get_cache(self, type_: type) -> object | None:
+        return self.__cache.get(type_, None)
 
     def post_process_bean(self, container: IBeanContainer, bean: object) -> object:
+        if (cached := self.__get_cache(type(bean))) is not None:
+            return cached
         if Aspect.contains(bean) or AsyncAspect.contains(bean):
+            self.__set_cache(type(bean), bean)
             return bean
         annotation: Bean | None = Bean.single_or_none(bean)
         if annotation is None:
+            self.__set_cache(type(bean), bean)
             return bean
         matched_advisors: Sequence[type[IAdvisor | IAsyncAdvisor]] = []
         advisors: Sequence[type] = container.filter_bean_types(
             lambda x: Aspect.contains(x) or AsyncAspect.contains(x)
         )
-        self.__logger.info(
-            f"[{type(self).__name__}] Advisors found: {[x.__name__ for x in advisors]!r}"
-        )
-        self.__logger.info(
-            f"[{type(self).__name__}] Searching advisors for '{type(bean).__name__}'"
-        )
         for advisor in advisors:
             aspect: Aspect | None = Aspect.single_or_none(advisor)
             async_aspect: AsyncAspect | None = AsyncAspect.single_or_none(advisor)
-            self.__logger.info(
-                f"[{type(self).__name__}] {advisor.__name__} -> ({type(aspect).__name__}, {type(async_aspect).__name__})"
-            )
             if aspect is not None and aspect.matches(bean):
                 matched_advisors.append(cast(type[IAdvisor], advisor))
                 continue
             if async_aspect is not None and async_aspect.matches(bean):
                 matched_advisors.append(cast(type[IAsyncAdvisor], advisor))
                 continue
         self.__logger.info(
-            f"[{type(self).__name__}] Matched advisors found for '{type(bean).__name__}': {[x.__name__ for x in matched_advisors]!r}"
+            f"[{type(self).__name__}] {[x.__name__ for x in matched_advisors]!r} -> {type(bean).__name__}"
         )
         if not any(matched_advisors):
+            self.__cache[type(bean)] = bean
             return bean
         dependencies: dict[str, object] = {}
         for name, required_type in annotation.dependencies.items():
             if required_type == Unknown:
                 dependencies[name] = container.single(name=name)
                 continue
             dependencies[name] = container.single(required_type=required_type)
-        return Enhancer(
+        proxy: object = Enhancer(
             superclass=type(bean),
             callback=AspectMethodInterceptor(container, matched_advisors),
         ).create(**dependencies)
+        self.__set_cache(type(bean), proxy)
+        return proxy
```

### Comparing `spakky_core-0.7.8/spakky/bean/application_context.py` & `spakky_core-0.7.9/spakky/bean/application_context.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/bean/autowired.py` & `spakky_core-0.7.9/spakky/bean/autowired.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/bean/bean.py` & `spakky_core-0.7.9/spakky/bean/bean.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/bean/inject.py` & `spakky_core-0.7.9/spakky/bean/inject.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/bean/interfaces/bean_container.py` & `spakky_core-0.7.9/spakky/bean/interfaces/bean_container.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/bean/interfaces/bean_registry.py` & `spakky_core-0.7.9/spakky/bean/interfaces/bean_registry.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/annotation.py` & `spakky_core-0.7.9/spakky/core/annotation.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/importing.py` & `spakky_core-0.7.9/spakky/core/importing.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/interfaces/comparable.py` & `spakky_core-0.7.9/spakky/core/interfaces/comparable.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/interfaces/disposable.py` & `spakky_core-0.7.9/spakky/core/interfaces/disposable.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/mutability.py` & `spakky_core-0.7.9/spakky/core/mutability.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/proxy.py` & `spakky_core-0.7.9/spakky/core/proxy.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/core/types.py` & `spakky_core-0.7.9/spakky/core/types.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/base64_encoder.py` & `spakky_core-0.7.9/spakky/cryptography/base64_encoder.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/cryptor/aes.py` & `spakky_core-0.7.9/spakky/cryptography/cryptor/aes.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/cryptor/gcm.py` & `spakky_core-0.7.9/spakky/cryptography/cryptor/gcm.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/cryptor/rsa.py` & `spakky_core-0.7.9/spakky/cryptography/cryptor/rsa.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/error.py` & `spakky_core-0.7.9/spakky/cryptography/error.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/hash.py` & `spakky_core-0.7.9/spakky/cryptography/hash.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/hmac.py` & `spakky_core-0.7.9/spakky/cryptography/hmac.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/jwt.py` & `spakky_core-0.7.9/spakky/cryptography/jwt.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/key.py` & `spakky_core-0.7.9/spakky/cryptography/key.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/cryptography/password.py` & `spakky_core-0.7.9/spakky/cryptography/password.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/models/aggregate_root.py` & `spakky_core-0.7.9/spakky/domain/models/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/models/domain_event.py` & `spakky_core-0.7.9/spakky/domain/models/domain_event.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/models/entity.py` & `spakky_core-0.7.9/spakky/domain/models/entity.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/models/value_object.py` & `spakky_core-0.7.9/spakky/domain/models/value_object.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/ports/event/event_publisher.py` & `spakky_core-0.7.9/spakky/domain/ports/event/event_publisher.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/ports/external/proxy.py` & `spakky_core-0.7.9/spakky/domain/ports/external/proxy.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/ports/persistency/repository.py` & `spakky_core-0.7.9/spakky/domain/ports/persistency/repository.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/ports/persistency/transaction.py` & `spakky_core-0.7.9/spakky/domain/ports/persistency/transaction.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/usecases/command.py` & `spakky_core-0.7.9/spakky/domain/usecases/command.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/domain/usecases/query.py` & `spakky_core-0.7.9/spakky/domain/usecases/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any, Generic, TypeVar, Protocol, runtime_checkable
+from typing import Any, TypeVar, Protocol, runtime_checkable
 
 from spakky.core.mutability import immutable
 
 
 @immutable
 class Query(ABC):
     ...
@@ -17,11 +17,11 @@
 class IQueryUseCase(Protocol[QueryT_contra, ResultT_co]):
     @abstractmethod
     def execute(self, query: QueryT_contra) -> ResultT_co:
         ...
 
 
 @runtime_checkable
-class IAsyncQueryUseCase(Generic[QueryT_contra, ResultT_co]):
+class IAsyncQueryUseCase(Protocol[QueryT_contra, ResultT_co]):
     @abstractmethod
     async def execute(self, query: QueryT_contra) -> ResultT_co:
         ...
```

### Comparing `spakky_core-0.7.8/spakky/extensions/logging.py` & `spakky_core-0.7.9/spakky/extensions/logging.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/spakky/extensions/transactional.py` & `spakky_core-0.7.9/spakky/extensions/transactional.py`

 * *Files identical despite different names*

### Comparing `spakky_core-0.7.8/PKG-INFO` & `spakky_core-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spakky-core
-Version: 0.7.8
+Version: 0.7.9
 Summary: Highly abstracted Framework core to use DDD & DI/IoC & AOP & Etc...
 Author: Spakky
 Author-email: sejong418@icloud.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spakky-core Version: 0.7.8 Summary: Highly
+Metadata-Version: 2.1 Name: spakky-core Version: 0.7.9 Summary: Highly
 abstracted Framework core to use DDD & DI/IoC & AOP & Etc... Author: Spakky
 Author-email: sejong418@icloud.com Requires-Python: >=3.10 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: pycryptodome
 (>=3.20.0,<4.0.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
```

