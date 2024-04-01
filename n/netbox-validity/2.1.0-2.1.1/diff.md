# Comparing `tmp/netbox-validity-2.1.0.tar.gz` & `tmp/netbox-validity-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-2.1.0.tar", last modified: Mon Mar 11 16:22:25 2024, max compression
+gzip compressed data, was "netbox-validity-2.1.1.tar", last modified: Mon Apr  1 20:30:56 2024, max compression
```

## Comparing `netbox-validity-2.1.0.tar` & `netbox-validity-2.1.1.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.848213 netbox-validity-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-03-11 16:22:25.848213 netbox-validity-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.848213 netbox-validity-2.1.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-03-11 16:22:25.000000 netbox-validity-2.1.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-11 16:22:25.000000 netbox-validity-2.1.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 16:22:25.000000 netbox-validity-2.1.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-11 16:22:25.000000 netbox-validity-2.1.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 16:22:25.000000 netbox-validity-2.1.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.820213 netbox-validity-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 16:22:25.848213 netbox-validity-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.820213 netbox-validity-2.1.0/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.824213 netbox-validity-2.1.0/validity/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.824213 netbox-validity-2.1.0/validity/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.824213 netbox-validity-2.1.0/validity/compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.824213 netbox-validity-2.1.0/validity/compliance/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/routeros.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/textfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/ttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/serialization/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/compliance/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/data_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.824213 netbox-validity-2.1.0/validity/fields/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/fields/encrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.828213 netbox-validity-2.1.0/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/j2_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.828213 netbox-validity-2.1.0/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0005_rename_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0006_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0007_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0008_script_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/0009_serializer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.832213 netbox-validity-2.1.0/validity/models/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/netbox_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.832213 netbox-validity-2.1.0/validity/pollers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/default_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/netconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/pollers/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.832213 netbox-validity-2.1.0/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.832213 netbox-validity-2.1.0/validity/scripts/install/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/scripts/install/validity_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/scripts/script_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/scripts/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.816213 netbox-validity-2.1.0/validity/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.832213 netbox-validity-2.1.0/validity/static/validity/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/static/validity/connection-type-select.js
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/static/validity/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/static/validity/prism-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/static/validity/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/subforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.816213 netbox-validity-2.1.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.836213 netbox-validity-2.1.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/aux_tab_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/command.html
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/device_state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.836213 netbox-validity-2.1.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/configcontext_format.html
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/datasource_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/prism.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/inc/yaml_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/poller.html
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/poller_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/report_devices.html
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templates/validity/serializer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.840213 netbox-validity-2.1.0/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.840213 netbox-validity-2.1.0/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.840213 netbox-validity-2.1.0/validity/tests/test_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_compliance/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_compliance/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_data_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.844213 netbox-validity-2.1.0/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_compliancetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_vdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_models/test_vdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_pollers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.844213 netbox-validity-2.1.0/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_scripts/test_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_scripts/test_script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.844213 netbox-validity-2.1.0/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_utils/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.844213 netbox-validity-2.1.0/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/utils/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 16:22:25.848213 netbox-validity-2.1.0/validity/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-11 16:22:13.000000 netbox-validity-2.1.0/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 20:30:56.000000 netbox-validity-2.1.1/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:30:56.749223 netbox-validity-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.725223 netbox-validity-2.1.1/validity/compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/compliance/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/textfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/serialization/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/compliance/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/data_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/fields/encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/j2_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.729223 netbox-validity-2.1.1/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0005_rename_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0006_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0007_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0008_script_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/0009_serializer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/netbox_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/pollers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/default_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/netconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/pollers/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.733223 netbox-validity-2.1.1/validity/scripts/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/install/validity_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/script_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/scripts/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/validity/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/static/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/connection-type-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/static/validity/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/subforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.721223 netbox-validity-2.1.1/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/device_state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.737223 netbox-validity-2.1.1/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/configcontext_format.html
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/datasource_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/inc/yaml_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/poller.html
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/poller_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/report_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templates/validity/serializer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/test_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_compliance/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_data_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.741223 netbox-validity-2.1.1/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_compliancetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_vdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_models/test_vdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_pollers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/test_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_scripts/test_script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_utils/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:30:56.745223 netbox-validity-2.1.1/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-01 20:30:45.000000 netbox-validity-2.1.1/validity/views/test_result.py
```

### Comparing `netbox-validity-2.1.0/LICENSE` & `netbox-validity-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/PKG-INFO` & `netbox-validity-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.1.0
-Summary: NetBox plugin for vendor-agnostic configuration compliance
+Version: 2.1.1
+Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,50 +28,46 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Framework :: Django
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: deepdiff<7,>=6.2.0
 Requires-Dist: django-bootstrap-v5==1.0.*
-Requires-Dist: pydantic<3,>=2.0.0
-Requires-Dist: ttp==0.9.*
+Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
-Requires-Dist: deepdiff<7,>=6.2.0
-Requires-Dist: simpleeval==0.9.*
 Requires-Dist: netmiko<5,>=4.0.0
+Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
+Requires-Dist: simpleeval==0.9.*
 Requires-Dist: textfsm<2,>=1.1.3
+Requires-Dist: ttp==0.9.*
 Requires-Dist: xmltodict<1
-Requires-Dist: dulwich
 Provides-Extra: dev
-Requires-Dist: isort[colors]==5.10.1; extra == "dev"
-Requires-Dist: black==22.12.0; extra == "dev"
-Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: Flake8-pyproject==1.2.2; extra == "dev"
-Requires-Dist: flake8-bugbear==22.12.6; extra == "dev"
-Requires-Dist: flake8-print==5.0.0; extra == "dev"
-Requires-Dist: factory_boy==3.2.1; extra == "dev"
-Requires-Dist: pytest==7.2.2; extra == "dev"
-Requires-Dist: pytest-django==4.5.2; extra == "dev"
-Requires-Dist: pytest-subtests==0.10.0; extra == "dev"
-Requires-Dist: pytest-cov==4.0.0; extra == "dev"
+Requires-Dist: debugpy==1.8.1; extra == "dev"
+Requires-Dist: factory_boy==3.3.0; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
-Requires-Dist: debugpy==1.6.7; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: pytest-django==4.8.0; extra == "dev"
+Requires-Dist: pytest-subtests==0.12.1; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.4.2; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra == "docs"
 
 <div align="center">
     <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/images/validity_logo.png" alt="Click to view Validity docs"/></a>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.0 Summary: NetBox
-plugin for vendor-agnostic configuration compliance Author-email: Anton
-Miasnikov
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.1 Summary: NetBox
+plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -16,34 +15,31 @@
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Classifier: Development Status :: 5 - Production/
 Stable Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Intended Audience :: System
-Administrators Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: Unix Classifier: Operating System :: POSIX :: Linux Classifier: Framework ::
-Django Classifier: Topic :: System :: Networking Classifier: Topic :: Internet
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
-pydantic<3,>=2.0.0 Requires-Dist: ttp==0.9.* Requires-Dist: jq<2,>=1.4.0
-Requires-Dist: deepdiff<7,>=6.2.0 Requires-Dist: simpleeval==0.9.* Requires-
-Dist: netmiko<5,>=4.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
-Dist: textfsm<2,>=1.1.3 Requires-Dist: xmltodict<1 Requires-Dist: dulwich
-Provides-Extra: dev Requires-Dist: isort[colors]==5.10.1; extra == "dev"
-Requires-Dist: black==22.12.0; extra == "dev" Requires-Dist: flake8==6.0.0;
-extra == "dev" Requires-Dist: Flake8-pyproject==1.2.2; extra == "dev" Requires-
-Dist: flake8-bugbear==22.12.6; extra == "dev" Requires-Dist: flake8-
-print==5.0.0; extra == "dev" Requires-Dist: factory_boy==3.2.1; extra == "dev"
-Requires-Dist: pytest==7.2.2; extra == "dev" Requires-Dist: pytest-
-django==4.5.2; extra == "dev" Requires-Dist: pytest-subtests==0.10.0; extra ==
-"dev" Requires-Dist: pytest-cov==4.0.0; extra == "dev" Requires-Dist: ipython;
-extra == "dev" Requires-Dist: debugpy==1.6.7; extra == "dev" Requires-Dist:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: System Administrators Classifier: Intended
+Audience :: Telecommunications Industry Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: Unix Classifier: Operating System
+:: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
+:: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
+dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
+Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
+Dist: simpleeval==0.9.* Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
+ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
+debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
+"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pytest==8.1.1;
+extra == "dev" Requires-Dist: pytest-cov==5.0.0; extra == "dev" Requires-Dist:
+pytest-django==4.8.0; extra == "dev" Requires-Dist: pytest-subtests==0.12.1;
+extra == "dev" Requires-Dist: ruff==0.3.4; extra == "dev" Requires-Dist:
 tomli==2.0.1; extra == "dev" Provides-Extra: docs Requires-Dist: mkdocs==1.4.2;
 extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra ==
 "docs"
                          _[_C_l_i_c_k_ _t_o_ _v_i_e_w_ _V_a_l_i_d_i_t_y_ _d_o_c_s_]
        ************ VVaalliiddiittyy:: vveennddoorr--aaggnnoossttiicc ccoonnffiigguurraattiioonn ccoommpplliiaannccee ************
                 [CI][Coverage][Python version][NetBox version]
 ## What? Validity is the [NetBox](https://netbox.dev) plugin to write "auto
```

### Comparing `netbox-validity-2.1.0/README.md` & `netbox-validity-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-2.1.1/netbox_validity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.1.0
-Summary: NetBox plugin for vendor-agnostic configuration compliance
+Version: 2.1.1
+Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,50 +28,46 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Framework :: Django
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: deepdiff<7,>=6.2.0
 Requires-Dist: django-bootstrap-v5==1.0.*
-Requires-Dist: pydantic<3,>=2.0.0
-Requires-Dist: ttp==0.9.*
+Requires-Dist: dulwich
 Requires-Dist: jq<2,>=1.4.0
-Requires-Dist: deepdiff<7,>=6.2.0
-Requires-Dist: simpleeval==0.9.*
 Requires-Dist: netmiko<5,>=4.0.0
+Requires-Dist: pydantic<3,>=2.0.0
 Requires-Dist: scrapli_netconf==2024.1.30
+Requires-Dist: simpleeval==0.9.*
 Requires-Dist: textfsm<2,>=1.1.3
+Requires-Dist: ttp==0.9.*
 Requires-Dist: xmltodict<1
-Requires-Dist: dulwich
 Provides-Extra: dev
-Requires-Dist: isort[colors]==5.10.1; extra == "dev"
-Requires-Dist: black==22.12.0; extra == "dev"
-Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: Flake8-pyproject==1.2.2; extra == "dev"
-Requires-Dist: flake8-bugbear==22.12.6; extra == "dev"
-Requires-Dist: flake8-print==5.0.0; extra == "dev"
-Requires-Dist: factory_boy==3.2.1; extra == "dev"
-Requires-Dist: pytest==7.2.2; extra == "dev"
-Requires-Dist: pytest-django==4.5.2; extra == "dev"
-Requires-Dist: pytest-subtests==0.10.0; extra == "dev"
-Requires-Dist: pytest-cov==4.0.0; extra == "dev"
+Requires-Dist: debugpy==1.8.1; extra == "dev"
+Requires-Dist: factory_boy==3.3.0; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
-Requires-Dist: debugpy==1.6.7; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: pytest-django==4.8.0; extra == "dev"
+Requires-Dist: pytest-subtests==0.12.1; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.4.2; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra == "docs"
 
 <div align="center">
     <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/images/validity_logo.png" alt="Click to view Validity docs"/></a>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.0 Summary: NetBox
-plugin for vendor-agnostic configuration compliance Author-email: Anton
-Miasnikov
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.1.1 Summary: NetBox
+plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -16,34 +15,31 @@
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Classifier: Development Status :: 5 - Production/
 Stable Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Intended Audience :: System
-Administrators Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: Unix Classifier: Operating System :: POSIX :: Linux Classifier: Framework ::
-Django Classifier: Topic :: System :: Networking Classifier: Topic :: Internet
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
-pydantic<3,>=2.0.0 Requires-Dist: ttp==0.9.* Requires-Dist: jq<2,>=1.4.0
-Requires-Dist: deepdiff<7,>=6.2.0 Requires-Dist: simpleeval==0.9.* Requires-
-Dist: netmiko<5,>=4.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
-Dist: textfsm<2,>=1.1.3 Requires-Dist: xmltodict<1 Requires-Dist: dulwich
-Provides-Extra: dev Requires-Dist: isort[colors]==5.10.1; extra == "dev"
-Requires-Dist: black==22.12.0; extra == "dev" Requires-Dist: flake8==6.0.0;
-extra == "dev" Requires-Dist: Flake8-pyproject==1.2.2; extra == "dev" Requires-
-Dist: flake8-bugbear==22.12.6; extra == "dev" Requires-Dist: flake8-
-print==5.0.0; extra == "dev" Requires-Dist: factory_boy==3.2.1; extra == "dev"
-Requires-Dist: pytest==7.2.2; extra == "dev" Requires-Dist: pytest-
-django==4.5.2; extra == "dev" Requires-Dist: pytest-subtests==0.10.0; extra ==
-"dev" Requires-Dist: pytest-cov==4.0.0; extra == "dev" Requires-Dist: ipython;
-extra == "dev" Requires-Dist: debugpy==1.6.7; extra == "dev" Requires-Dist:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: System Administrators Classifier: Intended
+Audience :: Telecommunications Industry Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: Unix Classifier: Operating System
+:: POSIX :: Linux Classifier: Framework :: Django Classifier: Topic :: System
+:: Networking Classifier: Topic :: Internet Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+deepdiff<7,>=6.2.0 Requires-Dist: django-bootstrap-v5==1.0.* Requires-Dist:
+dulwich Requires-Dist: jq<2,>=1.4.0 Requires-Dist: netmiko<5,>=4.0.0 Requires-
+Dist: pydantic<3,>=2.0.0 Requires-Dist: scrapli_netconf==2024.1.30 Requires-
+Dist: simpleeval==0.9.* Requires-Dist: textfsm<2,>=1.1.3 Requires-Dist:
+ttp==0.9.* Requires-Dist: xmltodict<1 Provides-Extra: dev Requires-Dist:
+debugpy==1.8.1; extra == "dev" Requires-Dist: factory_boy==3.3.0; extra ==
+"dev" Requires-Dist: ipython; extra == "dev" Requires-Dist: pytest==8.1.1;
+extra == "dev" Requires-Dist: pytest-cov==5.0.0; extra == "dev" Requires-Dist:
+pytest-django==4.8.0; extra == "dev" Requires-Dist: pytest-subtests==0.12.1;
+extra == "dev" Requires-Dist: ruff==0.3.4; extra == "dev" Requires-Dist:
 tomli==2.0.1; extra == "dev" Provides-Extra: docs Requires-Dist: mkdocs==1.4.2;
 extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin==4.0.4; extra ==
 "docs"
                          _[_C_l_i_c_k_ _t_o_ _v_i_e_w_ _V_a_l_i_d_i_t_y_ _d_o_c_s_]
        ************ VVaalliiddiittyy:: vveennddoorr--aaggnnoossttiicc ccoonnffiigguurraattiioonn ccoommpplliiaannccee ************
                 [CI][Coverage][Python version][NetBox version]
 ## What? Validity is the [NetBox](https://netbox.dev) plugin to write "auto
```

### Comparing `netbox-validity-2.1.0/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-2.1.1/netbox_validity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/pyproject.toml` & `netbox-validity-2.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "2.1.0"
-description = "NetBox plugin for vendor-agnostic configuration compliance"
+version = "2.1.1"
+description = "NetBox plugin for network devices validation"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
     "Operating System :: POSIX :: Linux",
     "Framework :: Django",
     "Topic :: System :: Networking",
@@ -44,37 +45,14 @@
 [tool.setuptools.dynamic.dependencies]
 file = ["requirements/base.txt"]
 
 [tool.setuptools.dynamic.optional-dependencies]
 dev = {file = ["requirements/dev.txt"]}
 docs = {file = ["requirements/docs.txt"]}
 
-
-[tool.black]
-line-length = 120
-skip_glob = ["*/migrations/*"]
-
-
-[tool.isort]
-profile = "black"
-line_length = 120
-no_lines_before = "LOCALFOLDER"
-lines_after_imports = 2
-skip_glob = ["*/migrations/*"]
-skip_gitignore = true
-known_first_party = ["validity"]
-
-
-[tool.flake8]
-max-line-length = 120
-exclude = ["migrations", "__pycache__"]
-per-file-ignores = ["__init__.py:F401", "validity/netbox_changes.py:F401"]
-extend-ignore = "E203"
-
-
 [tool.pytest.ini_options]
 addopts = "-p no:warnings -vv --no-migrations"
 testpaths = ["validity/tests"]
 DJANGO_SETTINGS_MODULE = "netbox.settings"
 pythonpath = ["/opt/netbox/netbox"]
 
 [tool.coverage.run]
@@ -84,7 +62,35 @@
         "validity/migrations/*",
 ]
 source = ["validity"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 75
+
+
+[tool.ruff]
+include = ["validity/**.py"]
+exclude = ["migrations", "__pycache__", "development"]
+line-length = 120
+indent-width = 4
+force-exclude = true
+
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "B", "T", "I"]
+ignore = ["B905"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401"]
+"validity/netbox_changes.py" = ["F401"]
+
+[tool.ruff.lint.isort]
+known-first-party = ["validity"]
+no-lines-before = ["local-folder"]
+lines-after-imports = 2
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+skip-magic-trailing-comma = false
+line-ending = "auto"
+docstring-code-format = false
```

### Comparing `netbox-validity-2.1.0/validity/__init__.py` & `netbox-validity-2.1.1/validity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity"
     description = "Write and run auto tests for network devices"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "2.1.0"
+    version = "2.1.1"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.5.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
```

### Comparing `netbox-validity-2.1.0/validity/api/helpers.py` & `netbox-validity-2.1.1/validity/api/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,18 +69,19 @@
 
 class SubformValidationMixin:
     """
     Serializer Mixin. Validates JSON field according to a subform
     """
 
     def validate(self, attrs):
-        instance = self.instance or self.Meta.model()
-        for field, field_value in attrs.items():
-            if not isinstance(instance._meta.get_field(field), ManyToManyField):
-                setattr(instance, field, field_value)
-        subform = instance.subform_cls(instance.subform_json)
-        if not subform.is_valid():
-            errors = [
-                ": ".join((field, err[0])) if field != "__all__" else err for field, err in subform.errors.items()
-            ]
-            raise ValidationError({instance.subform_json_field: errors})
+        if isinstance(attrs, dict):
+            instance = self.instance or self.Meta.model()
+            for field, field_value in attrs.items():
+                if not isinstance(instance._meta.get_field(field), ManyToManyField):
+                    setattr(instance, field, field_value)
+            subform = instance.subform_cls(instance.subform_json)
+            if not subform.is_valid():
+                errors = [
+                    ": ".join((field, err[0])) if field != "__all__" else err for field, err in subform.errors.items()
+                ]
+                raise ValidationError({instance.subform_json_field: errors})
         return attrs
```

### Comparing `netbox-validity-2.1.0/validity/api/serializers.py` & `netbox-validity-2.1.1/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/api/urls.py` & `netbox-validity-2.1.1/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/api/views.py` & `netbox-validity-2.1.1/validity/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
 
 class SerializedStateView(APIView):
     queryset = models.VDevice.objects.prefetch_datasource().prefetch_serializer().prefetch_poller()
 
     def get_object(self, pk):
         try:
             return self.queryset.get(pk=pk)
-        except models.VDevice.DoesNotExist:
-            raise NotFound
+        except models.VDevice.DoesNotExist as err:
+            raise NotFound from err
 
     @extend_schema(
         responses={200: serializers.SerializedStateSerializer()},
         operation_id="dcim_devices_serialized_state",
         parameters=[
             OpenApiParameter(name="fields", type=str, many=True),
             OpenApiParameter(name="name", type=str, many=True),
```

### Comparing `netbox-validity-2.1.0/validity/choices.py` & `netbox-validity-2.1.1/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/dynamic_pairs.py` & `netbox-validity-2.1.1/validity/compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/eval/default_nameset.py` & `netbox-validity-2.1.1/validity/compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/eval/eval.py` & `netbox-validity-2.1.1/validity/compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/eval/eval_defaults.py` & `netbox-validity-2.1.1/validity/compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/exceptions.py` & `netbox-validity-2.1.1/validity/compliance/exceptions.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/serialization/backend.py` & `netbox-validity-2.1.1/validity/compliance/serialization/backend.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/serialization/routeros.py` & `netbox-validity-2.1.1/validity/compliance/serialization/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/serialization/serializable.py` & `netbox-validity-2.1.1/validity/compliance/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/serialization/xml.py` & `netbox-validity-2.1.1/validity/compliance/serialization/xml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/compliance/state.py` & `netbox-validity-2.1.1/validity/compliance/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     @property
     def verbose_name(self) -> str:
         return _("Config") if self.contains_config else self.command.name
 
     @property
     def error(self) -> SerializationError | None:
         try:
-            self.serialized
+            self.serialized  # noqa: B018
             return
         except SerializationError as exc:
             return exc
 
     @property
     def serialized(self):
         try:
@@ -64,15 +64,15 @@
                 config_label = command.label
             items.append(StateItem.from_command(command))
         return cls(((item.name, item) for item in items), config_label)
 
     def with_config(self, serializable: Serializable):
         state_item = StateItem(serializer=serializable.serializer, data_file=serializable.data_file, command=None)
         with suppress(SerializationError):
-            state_item.serialized
+            state_item.serialized  # noqa: B018
             super().__setitem__("config", state_item)
             self.config_command_label = None
         return self
 
     def _blocked_op(self, *_):
         raise AttributeError("State is read only")
```

### Comparing `netbox-validity-2.1.0/validity/custom_validators.py` & `netbox-validity-2.1.1/validity/custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/data_backends.py` & `netbox-validity-2.1.1/validity/data_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
     def start_polling(self, devices) -> tuple[list[Generator], set[DescriptiveError]]:
         result_generators = []
         no_poller_errors = set()
         for poller, device_group in groupby(devices, key=lambda device: device.poller):
             if poller is None:
                 no_poller_errors.update(
-                    DescriptiveError(device=str(device), error="No poller bound") for device in device_group
+                    DescriptiveError(device=str(device), error="No poller bound")
+                    for device in device_group  # noqa: B031
                 )
             else:
                 result_generators.append(poller.get_backend().poll(device_group))
         return result_generators, no_poller_errors
 
     @contextmanager
     def fetch(self, device_filter: Q | None = None):
```

### Comparing `netbox-validity-2.1.0/validity/fields/encrypted.py` & `netbox-validity-2.1.1/validity/fields/encrypted.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/filtersets.py` & `netbox-validity-2.1.1/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/forms/filterset.py` & `netbox-validity-2.1.1/validity/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/forms/general.py` & `netbox-validity-2.1.1/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/forms/helpers.py` & `netbox-validity-2.1.1/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/graphql.py` & `netbox-validity-2.1.1/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/managers.py` & `netbox-validity-2.1.1/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/migrations/0001_initial.py` & `netbox-validity-2.1.1/validity/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         ("extras", "0084_staging"),
         ("tenancy", "0009_standardize_description_comments"),
-        ("dcim", "0167_module_status"),
+        ("dcim", "0167_module_status")
     ]
 
     operations = [
         migrations.CreateModel(
             name="ComplianceReport",
             fields=[
                 ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
```

### Comparing `netbox-validity-2.1.0/validity/migrations/0002_custom_fields.py` & `netbox-validity-2.1.1/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/migrations/0004_netbox35_scripts.py` & `netbox-validity-2.1.1/validity/migrations/0008_script_change.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 from pathlib import Path
-import sys
 
-from django.db import IntegrityError, migrations, transaction
-from django.utils.translation import gettext_lazy as _
+from django.db import migrations
+from django.utils.translation import gettext_lazy as __
 from validity import scripts
-from validity import config
 
 
-SCRIPTS_FOLDER = str(Path(scripts.__file__).parent.resolve())
+SCRIPTS_INSTALL_FOLDER = Path(scripts.__file__).parent.resolve() / "install"
 DATASOURCE_NAME = "validity_scripts"
+SCRIPT_NAME = "validity_scripts.py"
 
 
 def forward_func(apps, schema_editor):
-    if config.netbox_version < "3.5.0":
-        return
-
     from validity.models import VDataSource
     from extras.models import ScriptModule
 
-    db_alias = schema_editor.connection.alias
-    data_source = VDataSource.objects.using(db_alias).create(
-        name=DATASOURCE_NAME, type="local", source_url="file://" + SCRIPTS_FOLDER, description=_("Required by Validity")
-    )
     DataFile = apps.get_model("core", "DataFile")
-    data_source.sync_in_migration(DataFile)
-    for data_file in data_source.datafiles.using(db_alias).all():
-        if data_file.path.endswith("__init__.py") or data_file.path.endswith(".pyc"):
-            continue
-        module = ScriptModule(data_source=data_source, data_file=data_file, file_root="scripts", auto_sync_enabled=True)
-        module.clean()
-        try:
-            with transaction.atomic():
-                module.save()
-        except IntegrityError:
-            print(f"\n{module.full_path} already exists, ignoring", file=sys.stderr)  # noqa
+    datasource, _ = VDataSource.objects.get_or_create(
+        name=DATASOURCE_NAME,
+        type="local",
+        defaults={"source_url": f"file://{SCRIPTS_INSTALL_FOLDER.parent}", "description": __("Required by Validity")},
+    )
+    apps.get_model("core", "AutoSyncRecord").objects.filter(datafile__source__pk=datasource.pk).delete()
+    ScriptModule.objects.filter(data_source=datasource).delete()
+    datasource.source_url = f"file://{SCRIPTS_INSTALL_FOLDER}"
+    datasource.save()
+    datasource.sync_in_migration(DataFile)
+    module = ScriptModule(
+        data_source=datasource,
+        data_file=datasource.datafiles.get(path=SCRIPT_NAME),
+        file_root="scripts",
+        auto_sync_enabled=True,
+    )
+    module.clean()
+    module.save()
 
 
 def reverse_func(apps, schema_editor):
-    if config.netbox_version < "3.5.0":
-        return
     DataSource = apps.get_model("core", "DataSource")
     ScriptModule = apps.get_model("extras", "ScriptModule")
     db_alias = schema_editor.connection.alias
     ScriptModule.objects.using(db_alias).filter(data_source__name=DATASOURCE_NAME).delete()
     DataSource.objects.using(db_alias).filter(name=DATASOURCE_NAME).delete()
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("validity", "0003_complianceselector_dp_tag_prefix"),
+        ("validity", "0007_polling"),
     ]
 
     operations = [
         migrations.RunPython(forward_func, reverse_func),
     ]
```

### Comparing `netbox-validity-2.1.0/validity/migrations/0005_rename_serializer.py` & `netbox-validity-2.1.1/validity/migrations/0005_rename_serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/migrations/0006_datasources.py` & `netbox-validity-2.1.1/validity/migrations/0006_datasources.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/migrations/0007_polling.py` & `netbox-validity-2.1.1/validity/migrations/0007_polling.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/base.py` & `netbox-validity-2.1.1/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/data.py` & `netbox-validity-2.1.1/validity/models/data.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/device.py` & `netbox-validity-2.1.1/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/nameset.py` & `netbox-validity-2.1.1/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/polling.py` & `netbox-validity-2.1.1/validity/models/polling.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/report.py` & `netbox-validity-2.1.1/validity/models/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/selector.py` & `netbox-validity-2.1.1/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/serializer.py` & `netbox-validity-2.1.1/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/test.py` & `netbox-validity-2.1.1/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/models/test_result.py` & `netbox-validity-2.1.1/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/navigation.py` & `netbox-validity-2.1.1/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/netbox_changes.py` & `netbox-validity-2.1.1/validity/netbox_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module is going to contain all duct tape stuff which is required to support
 different versions of NetBox together
 """
+
 from validity import config
 
 
 DEVICE_ROLE_RELATION = "device_role" if config.netbox_version < "3.6.0" else "role"
 
 
 if config.netbox_version < "3.7.0":
```

### Comparing `netbox-validity-2.1.0/validity/pollers/base.py` & `netbox-validity-2.1.1/validity/pollers/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/pollers/default_credentials.py` & `netbox-validity-2.1.1/validity/pollers/default_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Models from this module are used by js script to render default credentials for a new poller in UI
 """
+
 from typing import Any
 
 from pydantic import BaseModel
 
 
 class EmptyCredentials(BaseModel):
     pass
```

### Comparing `netbox-validity-2.1.0/validity/pollers/factory.py` & `netbox-validity-2.1.1/validity/pollers/factory.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/pollers/http.py` & `netbox-validity-2.1.1/validity/pollers/http.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/pollers/result.py` & `netbox-validity-2.1.1/validity/pollers/result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/scripts/run_tests.py` & `netbox-validity-2.1.1/validity/scripts/run_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         tests_qs: QuerySet[ComplianceTest],
         device: VDevice,
         report: ComplianceReport | None,
     ) -> Generator[ComplianceTestResult, None, None]:
         for test in tests_qs:
             explanation = []
             try:
-                device.state
+                device.state  # noqa: B018
                 passed, explanation = self.run_test(device, test)
             except EvalError as exc:
                 self.log_failure(f"Failed to execute test **{test}** for device **{device}**, `{exc}`")
                 passed = False
                 explanation.append((str(exc), None))
             self.results_count += 1
             self.results_passed += int(passed)
```

### Comparing `netbox-validity-2.1.0/validity/scripts/script_data.py` & `netbox-validity-2.1.1/validity/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/search.py` & `netbox-validity-2.1.1/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/static/validity/connection-type-select.js` & `netbox-validity-2.1.1/validity/static/validity/connection-type-select.js`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/static/validity/prism-dark.css` & `netbox-validity-2.1.1/validity/static/validity/prism-dark.css`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/static/validity/prism-light.css` & `netbox-validity-2.1.1/validity/static/validity/prism-light.css`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/static/validity/prism.js` & `netbox-validity-2.1.1/validity/static/validity/prism.js`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/subforms.py` & `netbox-validity-2.1.1/validity/subforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Subforms are needed to
     1. Render part of the main form for JSON Field
     2. Validate JSON Field
 """
+
 import textwrap
 import xml.etree.ElementTree as ET
 
 from django import forms
 from django.utils.translation import gettext_lazy as _
 from utilities.forms import BootstrapMixin
```

### Comparing `netbox-validity-2.1.0/validity/tables.py` & `netbox-validity-2.1.1/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/template_content.py` & `netbox-validity-2.1.1/validity/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/aux_tab_table.html` & `netbox-validity-2.1.1/validity/templates/validity/aux_tab_table.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/command.html` & `netbox-validity-2.1.1/validity/templates/validity/command.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/compliancereport.html` & `netbox-validity-2.1.1/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/complianceselector.html` & `netbox-validity-2.1.1/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/compliancetest.html` & `netbox-validity-2.1.1/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/compliancetestresult.html` & `netbox-validity-2.1.1/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/device_state.html` & `netbox-validity-2.1.1/validity/templates/validity/device_state.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/inc/parameters.html` & `netbox-validity-2.1.1/validity/templates/validity/inc/parameters.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
         <td colspan="2" class="text-muted">
           No {{ title }} defined
         </td>
       </tr>
       {% endfor %}
     </table>
   </div>
-</div>
+</div>
```

### Comparing `netbox-validity-2.1.0/validity/templates/validity/nameset.html` & `netbox-validity-2.1.1/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/poller.html` & `netbox-validity-2.1.1/validity/templates/validity/poller.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templates/validity/serializer.html` & `netbox-validity-2.1.1/validity/templates/validity/serializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/templatetags/validity.py` & `netbox-validity-2.1.1/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/base.py` & `netbox-validity-2.1.1/validity/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self._test_get(admin_client, obj_id)
 
 
 class ApiPostGetTest(PostMixin, ApiBaseTest):
     def _test_post(self, client):
         self.resolve_post_body()
         resp = client.post(self.url(), self.post_body, content_type="application/json")
-        assert resp.status_code == HTTPStatus.CREATED, resp.data
+        assert resp.status_code == HTTPStatus.CREATED, resp.content
         return resp.json()["id"]
 
     @pytest.mark.django_db
     def test_post_get(self, admin_client):
         obj_id = self._test_post(admin_client)
         self._test_get(admin_client)
         self._test_get(admin_client, obj_id)
```

### Comparing `netbox-validity-2.1.0/validity/tests/conftest.py` & `netbox-validity-2.1.1/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/factories.py` & `netbox-validity-2.1.1/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_api.py` & `netbox-validity-2.1.1/validity/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     DeviceFactory,
     DeviceTypeFactory,
     LocationFactory,
     ManufacturerFactory,
     PlatformFactory,
     ReportFactory,
     SelectorFactory,
+    SerializerDBFactory,
     SiteFactory,
     TagFactory,
     TenantFactory,
     state_item,
 )
 
 from validity.models import VDevice
@@ -149,14 +150,15 @@
 
 class TestCommand(ApiPostGetTest):
     entity = "commands"
     post_body = {
         "name": "command-1",
         "label": "command_1",
         "type": "CLI",
+        "serializer": SerializerDBFactory,
         "parameters": {"cli_command": "show version"},
     }
 
 
 class TestPoller(ApiPostGetTest):
     entity = "pollers"
     post_body = {
```

### Comparing `netbox-validity-2.1.0/validity/tests/test_choices.py` & `netbox-validity-2.1.1/validity/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_compliance/test_dynamic_pairs.py` & `netbox-validity-2.1.1/validity/tests/test_compliance/test_dynamic_pairs.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ("NO", NoneFilter),
         ("TAG", DynamicPairTagFilter),
     ],
 )
 def test_dpf_factory(dynamic_pairs, filter_cls):
     selector = Mock(dynamic_pairs=dynamic_pairs)
     obj = dpf_factory(selector=selector, device=Mock())
-    assert type(obj) == filter_cls
+    assert isinstance(obj, filter_cls)
 
 
 @pytest.mark.parametrize(
     "name_filter, device_name, dp_filter",
     [
         pytest.param("asw[0-9]+-([ab])", "asw01-a.london", "asw01-([ab]).london", id="asw01-([ab]).london"),
         pytest.param("sw[0-9]+-(first|second)", "sw05-second", "sw05-(first|second)", id="sw05-(first|second)"),
```

### Comparing `netbox-validity-2.1.0/validity/tests/test_compliance/test_eval.py` & `netbox-validity-2.1.1/validity/tests/test_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_compliance/test_serialization.py` & `netbox-validity-2.1.1/validity/tests/test_compliance/test_serialization.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_compliance/test_state.py` & `netbox-validity-2.1.1/validity/tests/test_compliance/test_state.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_custom_validators.py` & `netbox-validity-2.1.1/validity/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_data_backends.py` & `netbox-validity-2.1.1/validity/tests/test_data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_fields.py` & `netbox-validity-2.1.1/validity/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_graphql.py` & `netbox-validity-2.1.1/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_managers.py` & `netbox-validity-2.1.1/validity/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_clean.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_compliancetest.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_compliancetest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_git_link.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_selector.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_vdatasource.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_vdatasource.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_models/test_vdevice.py` & `netbox-validity-2.1.1/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_pollers.py` & `netbox-validity-2.1.1/validity/tests/test_pollers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-2.1.1/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_scripts/test_script_data.py` & `netbox-validity-2.1.1/validity/tests/test_scripts/test_script_data.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_utils/test_json.py` & `netbox-validity-2.1.1/validity/tests/test_utils/test_json.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_utils/test_misc.py` & `netbox-validity-2.1.1/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_utils/test_orm.py` & `netbox-validity-2.1.1/validity/tests/test_utils/test_orm.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/tests/test_views.py` & `netbox-validity-2.1.1/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/urls.py` & `netbox-validity-2.1.1/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/utils/json.py` & `netbox-validity-2.1.1/validity/utils/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import jq as pyjq
 
 
 Json = dict[str, "Json"] | list["Json"] | int | float | str | None
 
 
 class TransformFn(Protocol):
-    def __call__(self, key: int | str, value: Json, /) -> tuple[int | str, Json] | None:
-        ...
+    def __call__(self, key: int | str, value: Json, /) -> tuple[int | str, Json] | None: ...
 
 
 def transform_json(data: Json, match_fn: Callable[[int | str, Json], bool], transform_fn: TransformFn) -> Json:
     """
     Traverse JSON-like struct recursively and apply "tranform_fn" to keys and values matched by "match_fn"
     """
```

### Comparing `netbox-validity-2.1.0/validity/utils/misc.py` & `netbox-validity-2.1.1/validity/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/utils/orm.py` & `netbox-validity-2.1.1/validity/utils/orm.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/utils/version.py` & `netbox-validity-2.1.1/validity/utils/version.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/__init__.py` & `netbox-validity-2.1.1/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/base.py` & `netbox-validity-2.1.1/validity/views/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/command.py` & `netbox-validity-2.1.1/validity/views/command.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/device.py` & `netbox-validity-2.1.1/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/nameset.py` & `netbox-validity-2.1.1/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/poller.py` & `netbox-validity-2.1.1/validity/views/poller.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/report.py` & `netbox-validity-2.1.1/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/selector.py` & `netbox-validity-2.1.1/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/serializer.py` & `netbox-validity-2.1.1/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/test.py` & `netbox-validity-2.1.1/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-2.1.0/validity/views/test_result.py` & `netbox-validity-2.1.1/validity/views/test_result.py`

 * *Files identical despite different names*

