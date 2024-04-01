# Comparing `tmp/gigachain_cli-0.0.22rc0.tar.gz` & `tmp/gigachain_cli-0.0.22rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_cli-0.0.22rc0.tar", max compression
+gzip compressed data, was "gigachain_cli-0.0.22rc1.tar", max compression
```

## Comparing `gigachain_cli-0.0.22rc0.tar` & `gigachain_cli-0.0.22rc1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1067 2024-03-14 13:23:45.960439 gigachain_cli-0.0.22rc0/LICENSE
--rw-r--r--   0        0        0      341 2024-03-14 13:23:45.960776 gigachain_cli-0.0.22rc0/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.960932 gigachain_cli-0.0.22rc0/langchain_cli/__init__.py
--rw-r--r--   0        0        0     2765 2024-03-27 13:04:35.265021 gigachain_cli-0.0.22rc0/langchain_cli/cli.py
--rw-r--r--   0        0        0      168 2024-03-14 13:23:45.961280 gigachain_cli-0.0.22rc0/langchain_cli/constants.py
--rw-r--r--   0        0        0     1247 2024-03-27 08:44:31.177342 gigachain_cli-0.0.22rc0/langchain_cli/dev_scripts.py
--rw-r--r--   0        0        0       12 2024-03-14 13:23:45.962211 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/.gitignore
--rw-r--r--   0        0        0     1072 2024-03-14 13:23:45.962393 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/LICENSE
--rw-r--r--   0        0        0     1830 2024-03-14 13:23:45.962627 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/Makefile
--rw-r--r--   0        0        0      923 2024-03-14 13:23:45.962833 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/README.md
--rw-r--r--   0        0        0     2109 2024-03-14 13:23:45.963210 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/chat.ipynb
--rw-r--r--   0        0        0     2114 2024-03-14 13:23:45.963387 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/llms.ipynb
--rw-r--r--   0        0        0      970 2024-03-14 13:23:45.963898 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/provider.ipynb
--rw-r--r--   0        0        0     2661 2024-03-14 13:23:45.964339 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/text_embedding.ipynb
--rw-r--r--   0        0        0     1741 2024-03-14 13:23:45.964576 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/vectorstores.ipynb
--rw-r--r--   0        0        0      372 2024-03-14 13:23:45.965024 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/__init__.py
--rw-r--r--   0        0        0     2297 2024-03-14 13:23:45.965332 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/chat_models.py
--rw-r--r--   0        0        0     1091 2024-03-14 13:23:45.965644 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/embeddings.py
--rw-r--r--   0        0        0     2093 2024-03-14 13:23:45.966064 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/llms.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.966161 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/py.typed
--rw-r--r--   0        0        0     5567 2024-03-14 13:23:45.966662 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/vectorstores.py
--rw-r--r--   0        0        0     2305 2024-03-14 13:23:45.967243 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/pyproject.toml
--rw-r--r--   0        0        0      447 2024-03-14 13:23:45.967778 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/scripts/check_imports.py
--rwxr-xr-x   0        0        0      849 2024-03-14 13:23:45.968052 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/scripts/check_pydantic.sh
--rwxr-xr-x   0        0        0      497 2024-03-14 13:23:45.968343 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/scripts/lint_imports.sh
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.968578 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.968809 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0     1814 2024-03-14 13:23:45.969109 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_chat_models.py
--rw-r--r--   0        0        0      157 2024-03-14 13:23:45.969376 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_compile.py
--rw-r--r--   0        0        0      601 2024-03-14 13:23:45.969565 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_embeddings.py
--rw-r--r--   0        0        0     1730 2024-03-14 13:23:45.969757 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_llms.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.969953 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0      200 2024-03-14 13:23:45.970280 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/test_chat_models.py
--rw-r--r--   0        0        0      221 2024-03-14 13:23:45.970588 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/test_embeddings.py
--rw-r--r--   0        0        0      257 2024-03-14 13:23:45.970847 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/test_imports.py
--rw-r--r--   0        0        0      194 2024-03-14 13:23:45.971154 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/test_llms.py
--rw-r--r--   0        0        0      191 2024-03-14 13:23:45.971415 gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/unit_tests/test_vectorstores.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.971694 gigachain_cli-0.0.22rc0/langchain_cli/namespaces/__init__.py
--rw-r--r--   0        0        0    10982 2024-03-14 13:23:45.972782 gigachain_cli-0.0.22rc0/langchain_cli/namespaces/app.py
--rw-r--r--   0        0        0     3892 2024-03-14 13:23:45.973101 gigachain_cli-0.0.22rc0/langchain_cli/namespaces/integration.py
--rw-r--r--   0        0        0     4378 2024-03-27 16:21:54.872273 gigachain_cli-0.0.22rc0/langchain_cli/namespaces/template.py
--rw-r--r--   0        0        0       12 2024-03-14 13:23:45.974203 gigachain_cli-0.0.22rc0/langchain_cli/package_template/.gitignore
--rw-r--r--   0        0        0     1072 2024-03-14 13:23:45.974471 gigachain_cli-0.0.22rc0/langchain_cli/package_template/LICENSE
--rw-r--r--   0        0        0     1680 2024-03-14 13:23:45.975308 gigachain_cli-0.0.22rc0/langchain_cli/package_template/README.md
--rw-r--r--   0        0        0       61 2024-03-14 13:23:45.975700 gigachain_cli-0.0.22rc0/langchain_cli/package_template/package_template/__init__.py
--rw-r--r--   0        0        0      446 2024-03-14 13:23:45.975945 gigachain_cli-0.0.22rc0/langchain_cli/package_template/package_template/chain.py
--rw-r--r--   0        0        0      487 2024-03-14 13:23:45.976280 gigachain_cli-0.0.22rc0/langchain_cli/package_template/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.976496 gigachain_cli-0.0.22rc0/langchain_cli/package_template/tests/__init__.py
--rw-r--r--   0        0        0       12 2024-03-14 13:23:45.976901 gigachain_cli-0.0.22rc0/langchain_cli/project_template/.gitignore
--rw-r--r--   0        0        0      391 2024-03-14 13:23:45.977156 gigachain_cli-0.0.22rc0/langchain_cli/project_template/Dockerfile
--rw-r--r--   0        0        0     1936 2024-03-14 13:23:45.977424 gigachain_cli-0.0.22rc0/langchain_cli/project_template/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.977590 gigachain_cli-0.0.22rc0/langchain_cli/project_template/app/__init__.py
--rw-r--r--   0        0        0      388 2024-03-14 13:23:45.978671 gigachain_cli-0.0.22rc0/langchain_cli/project_template/app/server.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.978868 gigachain_cli-0.0.22rc0/langchain_cli/project_template/packages/README.md
--rw-r--r--   0        0        0      462 2024-03-14 13:23:45.979075 gigachain_cli-0.0.22rc0/langchain_cli/project_template/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-14 13:23:45.979233 gigachain_cli-0.0.22rc0/langchain_cli/utils/__init__.py
--rw-r--r--   0        0        0      994 2024-03-14 13:23:45.979432 gigachain_cli-0.0.22rc0/langchain_cli/utils/events.py
--rw-r--r--   0        0        0      877 2024-03-14 13:23:45.979624 gigachain_cli-0.0.22rc0/langchain_cli/utils/find_replace.py
--rw-r--r--   0        0        0     6286 2024-03-27 08:44:31.177923 gigachain_cli-0.0.22rc0/langchain_cli/utils/git.py
--rw-r--r--   0        0        0      784 2024-03-14 13:23:45.980075 gigachain_cli-0.0.22rc0/langchain_cli/utils/github.py
--rw-r--r--   0        0        0     1518 2024-03-14 13:23:45.980240 gigachain_cli-0.0.22rc0/langchain_cli/utils/packages.py
--rw-r--r--   0        0        0     1622 2024-03-27 08:44:31.178190 gigachain_cli-0.0.22rc0/langchain_cli/utils/pyproject.py
--rw-r--r--   0        0        0     1840 2024-03-27 16:19:10.677010 gigachain_cli-0.0.22rc0/pyproject.toml
--rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 gigachain_cli-0.0.22rc0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-14 13:23:45.960439 gigachain_cli-0.0.22rc1/LICENSE
+-rw-r--r--   0        0        0      341 2024-03-14 13:23:45.960776 gigachain_cli-0.0.22rc1/README.md
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.960932 gigachain_cli-0.0.22rc1/langchain_cli/__init__.py
+-rw-r--r--   0        0        0     2765 2024-03-28 09:36:51.294150 gigachain_cli-0.0.22rc1/langchain_cli/cli.py
+-rw-r--r--   0        0        0      168 2024-03-14 13:23:45.961280 gigachain_cli-0.0.22rc1/langchain_cli/constants.py
+-rw-r--r--   0        0        0     1247 2024-03-28 09:36:51.295963 gigachain_cli-0.0.22rc1/langchain_cli/dev_scripts.py
+-rw-r--r--   0        0        0       12 2024-03-14 13:23:45.962211 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/.gitignore
+-rw-r--r--   0        0        0     1072 2024-03-14 13:23:45.962393 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/LICENSE
+-rw-r--r--   0        0        0     1830 2024-03-14 13:23:45.962627 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/Makefile
+-rw-r--r--   0        0        0      923 2024-03-14 13:23:45.962833 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/README.md
+-rw-r--r--   0        0        0     2109 2024-03-14 13:23:45.963210 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/chat.ipynb
+-rw-r--r--   0        0        0     2114 2024-03-14 13:23:45.963387 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/llms.ipynb
+-rw-r--r--   0        0        0      970 2024-03-14 13:23:45.963898 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/provider.ipynb
+-rw-r--r--   0        0        0     2661 2024-03-14 13:23:45.964339 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/text_embedding.ipynb
+-rw-r--r--   0        0        0     1741 2024-03-14 13:23:45.964576 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/vectorstores.ipynb
+-rw-r--r--   0        0        0      372 2024-03-14 13:23:45.965024 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/__init__.py
+-rw-r--r--   0        0        0     2297 2024-03-14 13:23:45.965332 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/chat_models.py
+-rw-r--r--   0        0        0     1091 2024-03-14 13:23:45.965644 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/embeddings.py
+-rw-r--r--   0        0        0     2093 2024-03-14 13:23:45.966064 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/llms.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.966161 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/py.typed
+-rw-r--r--   0        0        0     5567 2024-03-14 13:23:45.966662 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/vectorstores.py
+-rw-r--r--   0        0        0     2305 2024-03-14 13:23:45.967243 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/pyproject.toml
+-rw-r--r--   0        0        0      447 2024-03-14 13:23:45.967778 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/scripts/check_imports.py
+-rwxr-xr-x   0        0        0      849 2024-03-14 13:23:45.968052 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/scripts/check_pydantic.sh
+-rwxr-xr-x   0        0        0      497 2024-03-14 13:23:45.968343 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/scripts/lint_imports.sh
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.968578 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.968809 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0     1814 2024-03-14 13:23:45.969109 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_chat_models.py
+-rw-r--r--   0        0        0      157 2024-03-14 13:23:45.969376 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_compile.py
+-rw-r--r--   0        0        0      601 2024-03-14 13:23:45.969565 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_embeddings.py
+-rw-r--r--   0        0        0     1730 2024-03-14 13:23:45.969757 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_llms.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.969953 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0      200 2024-03-14 13:23:45.970280 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/test_chat_models.py
+-rw-r--r--   0        0        0      221 2024-03-14 13:23:45.970588 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/test_embeddings.py
+-rw-r--r--   0        0        0      257 2024-03-14 13:23:45.970847 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/test_imports.py
+-rw-r--r--   0        0        0      194 2024-03-14 13:23:45.971154 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/test_llms.py
+-rw-r--r--   0        0        0      191 2024-03-14 13:23:45.971415 gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/unit_tests/test_vectorstores.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.971694 gigachain_cli-0.0.22rc1/langchain_cli/namespaces/__init__.py
+-rw-r--r--   0        0        0    10982 2024-03-14 13:23:45.972782 gigachain_cli-0.0.22rc1/langchain_cli/namespaces/app.py
+-rw-r--r--   0        0        0     3892 2024-03-14 13:23:45.973101 gigachain_cli-0.0.22rc1/langchain_cli/namespaces/integration.py
+-rw-r--r--   0        0        0     4378 2024-03-28 09:36:51.299459 gigachain_cli-0.0.22rc1/langchain_cli/namespaces/template.py
+-rw-r--r--   0        0        0       12 2024-03-14 13:23:45.974203 gigachain_cli-0.0.22rc1/langchain_cli/package_template/.gitignore
+-rw-r--r--   0        0        0     1072 2024-03-14 13:23:45.974471 gigachain_cli-0.0.22rc1/langchain_cli/package_template/LICENSE
+-rw-r--r--   0        0        0     1680 2024-03-14 13:23:45.975308 gigachain_cli-0.0.22rc1/langchain_cli/package_template/README.md
+-rw-r--r--   0        0        0       61 2024-03-14 13:23:45.975700 gigachain_cli-0.0.22rc1/langchain_cli/package_template/package_template/__init__.py
+-rw-r--r--   0        0        0      446 2024-03-14 13:23:45.975945 gigachain_cli-0.0.22rc1/langchain_cli/package_template/package_template/chain.py
+-rw-r--r--   0        0        0      487 2024-03-28 09:36:51.302260 gigachain_cli-0.0.22rc1/langchain_cli/package_template/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.976496 gigachain_cli-0.0.22rc1/langchain_cli/package_template/tests/__init__.py
+-rw-r--r--   0        0        0       12 2024-03-14 13:23:45.976901 gigachain_cli-0.0.22rc1/langchain_cli/project_template/.gitignore
+-rw-r--r--   0        0        0      391 2024-03-14 13:23:45.977156 gigachain_cli-0.0.22rc1/langchain_cli/project_template/Dockerfile
+-rw-r--r--   0        0        0     1936 2024-03-14 13:23:45.977424 gigachain_cli-0.0.22rc1/langchain_cli/project_template/README.md
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.977590 gigachain_cli-0.0.22rc1/langchain_cli/project_template/app/__init__.py
+-rw-r--r--   0        0        0      388 2024-03-14 13:23:45.978671 gigachain_cli-0.0.22rc1/langchain_cli/project_template/app/server.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.978868 gigachain_cli-0.0.22rc1/langchain_cli/project_template/packages/README.md
+-rw-r--r--   0        0        0      462 2024-03-14 13:23:45.979075 gigachain_cli-0.0.22rc1/langchain_cli/project_template/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-14 13:23:45.979233 gigachain_cli-0.0.22rc1/langchain_cli/utils/__init__.py
+-rw-r--r--   0        0        0      994 2024-03-14 13:23:45.979432 gigachain_cli-0.0.22rc1/langchain_cli/utils/events.py
+-rw-r--r--   0        0        0      877 2024-03-14 13:23:45.979624 gigachain_cli-0.0.22rc1/langchain_cli/utils/find_replace.py
+-rw-r--r--   0        0        0     6286 2024-03-28 09:36:51.303001 gigachain_cli-0.0.22rc1/langchain_cli/utils/git.py
+-rw-r--r--   0        0        0      784 2024-03-14 13:23:45.980075 gigachain_cli-0.0.22rc1/langchain_cli/utils/github.py
+-rw-r--r--   0        0        0     1518 2024-03-14 13:23:45.980240 gigachain_cli-0.0.22rc1/langchain_cli/utils/packages.py
+-rw-r--r--   0        0        0     1622 2024-03-28 09:36:51.303753 gigachain_cli-0.0.22rc1/langchain_cli/utils/pyproject.py
+-rw-r--r--   0        0        0     1840 2024-04-01 09:28:06.017803 gigachain_cli-0.0.22rc1/pyproject.toml
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 gigachain_cli-0.0.22rc1/PKG-INFO
```

### Comparing `gigachain_cli-0.0.22rc0/LICENSE` & `gigachain_cli-0.0.22rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/cli.py` & `gigachain_cli-0.0.22rc1/langchain_cli/cli.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/dev_scripts.py` & `gigachain_cli-0.0.22rc1/langchain_cli/dev_scripts.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/LICENSE` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/Makefile` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/Makefile`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/README.md` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/chat.ipynb` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/chat.ipynb`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/llms.ipynb` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/llms.ipynb`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/provider.ipynb` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/provider.ipynb`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/text_embedding.ipynb` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/text_embedding.ipynb`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/docs/vectorstores.ipynb` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/docs/vectorstores.ipynb`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/chat_models.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/chat_models.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/embeddings.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/embeddings.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/llms.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/llms.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/integration_template/vectorstores.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/integration_template/vectorstores.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/pyproject.toml` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/scripts/check_pydantic.sh` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/scripts/check_pydantic.sh`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_chat_models.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_chat_models.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_embeddings.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/integration_template/tests/integration_tests/test_llms.py` & `gigachain_cli-0.0.22rc1/langchain_cli/integration_template/tests/integration_tests/test_llms.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/namespaces/app.py` & `gigachain_cli-0.0.22rc1/langchain_cli/namespaces/app.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/namespaces/integration.py` & `gigachain_cli-0.0.22rc1/langchain_cli/namespaces/integration.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/namespaces/template.py` & `gigachain_cli-0.0.22rc1/langchain_cli/namespaces/template.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/package_template/LICENSE` & `gigachain_cli-0.0.22rc1/langchain_cli/package_template/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/package_template/README.md` & `gigachain_cli-0.0.22rc1/langchain_cli/package_template/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/project_template/README.md` & `gigachain_cli-0.0.22rc1/langchain_cli/project_template/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/events.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/events.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/find_replace.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/find_replace.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/git.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/github.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/github.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/packages.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/packages.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/langchain_cli/utils/pyproject.py` & `gigachain_cli-0.0.22rc1/langchain_cli/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `gigachain_cli-0.0.22rc0/pyproject.toml` & `gigachain_cli-0.0.22rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gigachain-cli"
-version = "0.0.22rc0"
+version = "0.0.22rc1"
 description = "CLI for interacting with GigaChain"
 authors = ["Erick Friis <erick@langchain.dev>"]
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 packages = [
     {include = "langchain_cli"}
```

### Comparing `gigachain_cli-0.0.22rc0/PKG-INFO` & `gigachain_cli-0.0.22rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain-cli
-Version: 0.0.22rc0
+Version: 0.0.22rc1
 Summary: CLI for interacting with GigaChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Author: Erick Friis
 Author-email: erick@langchain.dev
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

