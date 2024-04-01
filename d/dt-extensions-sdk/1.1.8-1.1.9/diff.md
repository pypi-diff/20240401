# Comparing `tmp/dt_extensions_sdk-1.1.8.tar.gz` & `tmp/dt_extensions_sdk-1.1.9.tar.gz`

## Comparing `dt_extensions_sdk-1.1.8.tar` & `dt_extensions_sdk-1.1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/.github/workflows/gh-pages-docs.yml
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/conf.py
--rw-r--r--   0        0        0    12420 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/index.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/requirements.txt
--rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/dt-sdk-header.png
--rw-r--r--   0        0        0    27116 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/dt-sdk-logo.png
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0        0        0    43607 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-01-new-extension.png
--rw-r--r--   0        0        0    22268 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-02-type.png
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-03-import.png
--rw-r--r--   0        0        0    21720 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-04-import-remote.png
--rw-r--r--   0        0        0    34759 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-05-activation.png
--rw-r--r--   0        0        0   110687 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/_static/img/migrate-06-activation-config.png
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/extension.rst
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/events/event_severity.rst
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/events/event_type.rst
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/events/index.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/metrics/index.rst
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/metrics/metric.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/api/metrics/metric_type.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/assemble.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/build.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/create.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/gencerts.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/help.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/run.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/sign.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/upload.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/cli/wheel.rst
--rw-r--r--   0        0        0     9642 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/guides/extension_structure.rst
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/guides/installation.rst
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/docs/guides/migration.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/__about__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/__init__.py
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/main.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/schema.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/__init__.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/create.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/.gitignore.template
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/README.md.template
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/activation.json.template
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/setup.py.template
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension/activationSchema.json.template
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension/extension.yaml.template
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension_name/__init__.py.template
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension_name/__main__.py.template
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/activation.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/callback.py
--rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/communication.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/event.py
--rw-r--r--   0        0        0    41064 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/extension.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/helper.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/metric.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/runtime.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/mureq/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/mureq/__init__.py
--rw-r--r--   0        0        0    15102 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/mureq/mureq.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/cli/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/cli/test_dt_sdk.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/cli/test_templates.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/cli/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/__init__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_activation.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_callback.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_communication.py
--rw-r--r--   0        0        0    31483 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_extension.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_metric.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_runtime_properties.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/tests/sdk/test_status.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/README.md
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/.github/workflows/gh-pages-docs.yml
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/conf.py
+-rw-r--r--   0        0        0    12420 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/index.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/requirements.txt
+-rw-r--r--   0        0        0    13169 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/dt-sdk-header.png
+-rw-r--r--   0        0        0    27116 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/dt-sdk-logo.png
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0        0        0    43607 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-01-new-extension.png
+-rw-r--r--   0        0        0    22268 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-02-type.png
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-03-import.png
+-rw-r--r--   0        0        0    21720 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-04-import-remote.png
+-rw-r--r--   0        0        0    34759 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-05-activation.png
+-rw-r--r--   0        0        0   110687 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/_static/img/migrate-06-activation-config.png
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/extension.rst
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/events/event_severity.rst
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/events/event_type.rst
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/events/index.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/metrics/index.rst
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/metrics/metric.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/api/metrics/metric_type.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/assemble.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/build.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/create.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/gencerts.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/help.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/run.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/sign.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/upload.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/cli/wheel.rst
+-rw-r--r--   0        0        0     9642 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/guides/extension_structure.rst
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/guides/installation.rst
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/docs/guides/migration.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/__about__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/__init__.py
+-rw-r--r--   0        0        0    17163 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/main.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/schema.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/__init__.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/create.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/.gitignore.template
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/README.md.template
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/activation.json.template
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/setup.py.template
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension/activationSchema.json.template
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension/extension.yaml.template
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension_name/__init__.py.template
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension_name/__main__.py.template
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/activation.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/callback.py
+-rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/communication.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/event.py
+-rw-r--r--   0        0        0    41064 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/extension.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/helper.py
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/metric.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/runtime.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/mureq/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/mureq/__init__.py
+-rw-r--r--   0        0        0    15102 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/mureq/mureq.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/cli/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/cli/test_dt_sdk.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/cli/test_templates.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/cli/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/__init__.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_activation.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_callback.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_communication.py
+-rw-r--r--   0        0        0    31483 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_extension.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_metric.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_runtime_properties.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/tests/sdk/test_status.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/README.md
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 dt_extensions_sdk-1.1.9/PKG-INFO
```

### Comparing `dt_extensions_sdk-1.1.8/.github/workflows/gh-pages-docs.yml` & `dt_extensions_sdk-1.1.9/.github/workflows/gh-pages-docs.yml`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/conf.py` & `dt_extensions_sdk-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/index.rst` & `dt_extensions_sdk-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/dt-sdk-header.png` & `dt_extensions_sdk-1.1.9/docs/_static/dt-sdk-header.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/dt-sdk-logo.png` & `dt_extensions_sdk-1.1.9/docs/_static/dt-sdk-logo.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/favicon.ico` & `dt_extensions_sdk-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-01-new-extension.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-01-new-extension.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-02-type.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-02-type.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-03-import.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-03-import.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-04-import-remote.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-04-import-remote.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-05-activation.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-05-activation.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/_static/img/migrate-06-activation-config.png` & `dt_extensions_sdk-1.1.9/docs/_static/img/migrate-06-activation-config.png`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/api/metrics/metric.rst` & `dt_extensions_sdk-1.1.9/docs/api/metrics/metric.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/api/metrics/metric_type.rst` & `dt_extensions_sdk-1.1.9/docs/api/metrics/metric_type.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/guides/extension_structure.rst` & `dt_extensions_sdk-1.1.9/docs/guides/extension_structure.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/guides/installation.rst` & `dt_extensions_sdk-1.1.9/docs/guides/installation.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/docs/guides/migration.rst` & `dt_extensions_sdk-1.1.9/docs/guides/migration.rst`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/__init__.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/main.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,34 +75,36 @@
     target_directory: Optional[Path] = typer.Option(None, "--target-directory", "-t"),
     extra_platforms: Optional[list[str]] = typer.Option(
         None, "--extra-platform", "-e", help="Download wheels for an extra platform"
     ),
     extra_index_url: Optional[str] = typer.Option(
         None, "--extra-index-url", "-i", help="Extra index url to use when downloading dependencies"
     ),
+    find_links: Optional[str] = typer.Option( None, "--find-links", "-f", help="Extra index url to use when downloading dependencies" ),
 ):
     """
     Builds and signs an extension using the developer fused key-certificate
 
     :param extension_dir: The directory of the extension, by default this is the current directory
     :param private_key: The path to the developer fused key-certificate, if not specified, we try to locate the file developer.pem under the environment
     variable DT_CERTIFICATES_FOLDER
     :param target_directory: The directory to put the extension zip file in, if not specified, we put it in the dist
     folder
     :param extra_platforms: Attempt to also download wheels for an extra platform (e.g. manylinux1_x86_64 or win_amd64)
     :param extra_index_url: Extra index url to use when downloading dependencies
+    :param find_links: Extra index url to use when downloading dependencies
     """
     console.print(f"Building and signing extension from {extension_dir} to {target_directory}", style="cyan")
     if target_directory is None:
         target_directory = extension_dir / "dist"
     if not target_directory.exists():
         target_directory.mkdir()
 
     console.print("Stage 1 - Download and build dependencies", style="bold blue")
-    wheel(extension_dir, extra_platforms, extra_index_url)
+    wheel(extension_dir, extra_platforms, extra_index_url, find_links)
 
     console.print("Stage 2 - Create the extension zip file", style="bold blue")
     built_zip = assemble(extension_dir, target_directory)
 
     console.print("Stage 3 - Sign the extension", style="bold blue")
     extension_yaml = ExtensionYaml(Path(extension_dir) / "extension" / "extension.yaml")
     output = target_directory / extension_yaml.zip_file_name()
@@ -159,33 +161,37 @@
     extension_dir: Path = typer.Argument(".", help="Path to the python extension"),
     extra_platforms: Optional[list[str]] = typer.Option(
         None, "--extra-platform", "-e", help="Download wheels for an extra platform"
     ),
     extra_index_url: Optional[str] = typer.Option(
         None, "--extra-index-url", "-i", help="Extra index url to use when downloading dependencies"
     ),
+    find_links: Optional[str] = typer.Option( None, "--find-links", "-f", help="Extra index url to use when downloading dependencies" ),
 ):
     """
     Builds the extension and it's dependencies into wheel files
     Places these files in the lib folder
 
     :param extension_dir: The directory of the extension, by default this is the current directory
     :param extra_platforms: Attempt to also download wheels for an extra platform (e.g. manylinux1_x86_64 or win_amd64)
     :param extra_index_url: Extra index url to use when downloading dependencies
+    :param find_links: Extra index url to use when downloading dependencies
     """
     relative_lib_folder_dir = "extension/lib"
     lib_folder: Path = extension_dir / relative_lib_folder_dir
     _clean_directory(lib_folder)
 
     console.print(f"Downloading dependencies to {lib_folder}", style="cyan")
 
     # Downloads the dependencies and places them in the lib folder
     command = [sys.executable, "-m", "pip", "wheel", "-w", relative_lib_folder_dir]
     if extra_index_url is not None:
         command.extend(["--extra-index-url", extra_index_url])
+    if find_links is not None:
+        command.extend(["--find-links", find_links])
     command.append(".")
     run_process(command, cwd=extension_dir)
 
     if extra_platforms:
         for extra_platform in extra_platforms:
             console.print(f"Downloading wheels for platform {extra_platform}", style="cyan")
             command = [
@@ -197,14 +203,16 @@
                 relative_lib_folder_dir,
                 "--only-binary=:all:",
                 "--platform",
                 extra_platform,
             ]
             if extra_index_url:
                 command.extend(["--extra-index-url", extra_index_url])
+            if find_links:
+                command.extend(["--find-links", find_links])
             command.append(".")
 
             run_process(command, cwd=extension_dir)
 
     console.print(f"Installed dependencies to {lib_folder}", style="bold green")
```

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/schema.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/schema.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/create.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/create.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/.gitignore.template` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/.gitignore.template`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/README.md.template` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/README.md.template`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension/activationSchema.json.template` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension/activationSchema.json.template`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/cli/create/extension_template/extension_name/__main__.py.template` & `dt_extensions_sdk-1.1.9/dynatrace_extension/cli/create/extension_template/extension_name/__main__.py.template`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/activation.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/activation.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/callback.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/callback.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/communication.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/communication.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/extension.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/extension.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/helper.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/helper.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/metric.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/metric.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/runtime.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/runtime.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/mureq/LICENSE` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/mureq/LICENSE`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/dynatrace_extension/sdk/vendor/mureq/mureq.py` & `dt_extensions_sdk-1.1.9/dynatrace_extension/sdk/vendor/mureq/mureq.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/cli/test_dt_sdk.py` & `dt_extensions_sdk-1.1.9/tests/cli/test_dt_sdk.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/cli/test_templates.py` & `dt_extensions_sdk-1.1.9/tests/cli/test_templates.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/cli/test_types.py` & `dt_extensions_sdk-1.1.9/tests/cli/test_types.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_activation.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_activation.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_callback.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_callback.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_communication.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_communication.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_extension.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_extension.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_metric.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_metric.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_runtime_properties.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_runtime_properties.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/tests/sdk/test_status.py` & `dt_extensions_sdk-1.1.9/tests/sdk/test_status.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/.gitignore` & `dt_extensions_sdk-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/LICENSE.txt` & `dt_extensions_sdk-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/README.md` & `dt_extensions_sdk-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/pyproject.toml` & `dt_extensions_sdk-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dt_extensions_sdk-1.1.8/PKG-INFO` & `dt_extensions_sdk-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dt-extensions-sdk
-Version: 1.1.8
+Version: 1.1.9
 Project-URL: Documentation, https://github.com/dynatrace-extensions/dt-extensions-python-sdk#readme
 Project-URL: Issues, https://github.com/dynatrace-extensions/dt-extensions-python-sdk/issues
 Project-URL: Source, https://github.com/dynatrace-extensions/dt-extensions-python-sdk
 Author-email: dlopes7 <davidribeirolopes@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

