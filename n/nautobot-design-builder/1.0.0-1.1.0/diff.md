# Comparing `tmp/nautobot_design_builder-1.0.0.tar.gz` & `tmp/nautobot_design_builder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_design_builder-1.0.0.tar", max compression
+gzip compressed data, was "nautobot_design_builder-1.1.0.tar", max compression
```

## Comparing `nautobot_design_builder-1.0.0.tar` & `nautobot_design_builder-1.1.0.tar`

### file list

```diff
@@ -1,76 +1,83 @@
--rw-r--r--   0        0        0      591 2024-02-10 15:02:06.673480 nautobot_design_builder-1.0.0/LICENSE
--rw-r--r--   0        0        0     3305 2024-02-10 15:02:06.673480 nautobot_design_builder-1.0.0/README.md
--rw-r--r--   0        0        0     1270 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/__init__.py
--rw-r--r--   0        0        0    13472 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/context.py
--rw-r--r--   0        0        0        0 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/__init__.py
--rw-r--r--   0        0        0    22045 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/ext.py
--rw-r--r--   0        0        0        0 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/__init__.py
--rw-r--r--   0        0        0     1085 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/test_ext.py
--rw-r--r--   0        0        0      789 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml
--rw-r--r--   0        0        0     2630 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml
--rw-r--r--   0        0        0     1990 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml
--rw-r--r--   0        0        0     1244 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml
--rw-r--r--   0        0        0     1469 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix.yaml
--rw-r--r--   0        0        0      725 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml
--rw-r--r--   0        0        0     2818 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/bgp_extension.yaml
--rw-r--r--   0        0        0     2268 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml
--rw-r--r--   0        0        0     1434 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml
--rw-r--r--   0        0        0     1659 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix.yaml
--rw-r--r--   0        0        0      915 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix_by_role_and_tenant.yaml
--rw-r--r--   0        0        0    22104 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/design.py
--rw-r--r--   0        0        0     8187 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/design_job.py
--rw-r--r--   0        0        0     8182 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/errors.py
--rw-r--r--   0        0        0    11298 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/ext.py
--rw-r--r--   0        0        0     8871 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/fields.py
--rw-r--r--   0        0        0     4030 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/git.py
--rw-r--r--   0        0        0     4013 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/helpers.py
--rw-r--r--   0        0        0     5966 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/jinja2.py
--rw-r--r--   0        0        0     4225 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/logging.py
--rw-r--r--   0        0        0       57 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/management/__init__.py
--rw-r--r--   0        0        0       57 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/management/commands/__init__.py
--rw-r--r--   0        0        0     1288 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/management/commands/build_design.py
--rw-r--r--   0        0        0      630 2024-02-10 15:02:06.681480 nautobot_design_builder-1.0.0/nautobot_design_builder/management/commands/install_demo_designs.py
--rw-r--r--   0        0        0     2734 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/__init__.py
--rw-r--r--   0        0        0      227 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/context.py
--rw-r--r--   0        0        0      311 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/sub_designs/__init__.py
--rw-r--r--   0        0        0       71 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/templates/design_with_ref_error.yaml.j2
--rw-r--r--   0        0        0       30 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/templates/design_with_validation_error.yaml.j2
--rw-r--r--   0        0        0       49 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/templates/simple_design.yaml.j2
--rw-r--r--   0        0        0       51 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/templates/simple_design_2.yaml.j2
--rw-r--r--   0        0        0       13 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/templates/simple_report.md.j2
--rw-r--r--   0        0        0     2284 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/test_designs.py
--rw-r--r--   0        0        0     5941 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_builder.py
--rw-r--r--   0        0        0     6940 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_context.py
--rw-r--r--   0        0        0     8224 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_data_sources.py
--rw-r--r--   0        0        0     4440 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_design_job.py
--rw-r--r--   0        0        0     3802 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_errors.py
--rw-r--r--   0        0        0     3853 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_ext.py
--rw-r--r--   0        0        0     2760 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_jinja.py
--rw-r--r--   0        0        0      669 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/many_to_many.yaml
--rw-r--r--   0        0        0      422 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_name.yaml
--rw-r--r--   0        0        0      412 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_ref.yaml
--rw-r--r--   0        0        0     6639 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/complex_design1.yaml
--rw-r--r--   0        0        0     2332 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_by_ref.yaml
--rw-r--r--   0        0        0     1510 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_mlag.yaml
--rw-r--r--   0        0        0      800 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_rack.yaml
--rw-r--r--   0        0        0      895 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_relationships.yaml
--rw-r--r--   0        0        0      213 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_tags.yaml
--rw-r--r--   0        0        0     1370 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship.yaml
--rw-r--r--   0        0        0      982 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml
--rw-r--r--   0        0        0     1078 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/interface_addresses.yaml
--rw-r--r--   0        0        0     1039 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_create.yaml
--rw-r--r--   0        0        0     1221 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_update.yaml
--rw-r--r--   0        0        0     1282 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/one_to_one.yaml
--rw-r--r--   0        0        0      505 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/prefixes.yaml
--rw-r--r--   0        0        0     1476 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/interface_addresses.yaml
--rw-r--r--   0        0        0      815 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml
--rw-r--r--   0        0        0     1280 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/nested_create.yaml
--rw-r--r--   0        0        0      665 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml
--rw-r--r--   0        0        0      310 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/roll_back.yaml
--rw-r--r--   0        0        0      632 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/simple_create.yaml
--rw-r--r--   0        0        0      547 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/simple_update.yaml
--rw-r--r--   0        0        0      478 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/update_with_ref.yaml
--rw-r--r--   0        0        0    12482 2024-02-10 15:02:06.685480 nautobot_design_builder-1.0.0/nautobot_design_builder/util.py
--rw-r--r--   0        0        0     3576 2024-02-10 15:02:14.385509 nautobot_design_builder-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 nautobot_design_builder-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-01 19:05:22.854016 nautobot_design_builder-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3305 2024-04-01 19:05:22.854016 nautobot_design_builder-1.1.0/README.md
+-rw-r--r--   0        0        0     1271 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/__init__.py
+-rw-r--r--   0        0        0    13473 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/context.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/__init__.py
+-rw-r--r--   0        0        0    22178 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/ext.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/__init__.py
+-rw-r--r--   0        0        0     1086 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/test_ext.py
+-rw-r--r--   0        0        0      789 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml
+-rw-r--r--   0        0        0     2630 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml
+-rw-r--r--   0        0        0     1990 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml
+-rw-r--r--   0        0        0     1244 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml
+-rw-r--r--   0        0        0     1469 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix.yaml
+-rw-r--r--   0        0        0      725 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml
+-rw-r--r--   0        0        0     2822 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/bgp_extension.yaml
+-rw-r--r--   0        0        0     2268 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml
+-rw-r--r--   0        0        0     1434 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml
+-rw-r--r--   0        0        0     1659 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix.yaml
+-rw-r--r--   0        0        0      915 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix_by_role_and_tenant.yaml
+-rw-r--r--   0        0        0     2246 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/debug.py
+-rw-r--r--   0        0        0    35386 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/design.py
+-rw-r--r--   0        0        0    10636 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/design_job.py
+-rw-r--r--   0        0        0     8244 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/errors.py
+-rw-r--r--   0        0        0    11551 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/ext.py
+-rw-r--r--   0        0        0    14290 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/fields.py
+-rw-r--r--   0        0        0     4030 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/git.py
+-rw-r--r--   0        0        0     4014 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/helpers.py
+-rw-r--r--   0        0        0     5967 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/jinja2.py
+-rw-r--r--   0        0        0     4226 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/logging.py
+-rw-r--r--   0        0        0       57 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/__init__.py
+-rw-r--r--   0        0        0     1297 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/build_design.py
+-rw-r--r--   0        0        0      631 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/install_demo_designs.py
+-rw-r--r--   0        0        0     2867 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/__init__.py
+-rw-r--r--   0        0        0      228 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/context.py
+-rw-r--r--   0        0        0      312 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/sub_designs/__init__.py
+-rw-r--r--   0        0        0       71 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/design_with_ref_error.yaml.j2
+-rw-r--r--   0        0        0       30 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/design_with_validation_error.yaml.j2
+-rw-r--r--   0        0        0       49 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design.yaml.j2
+-rw-r--r--   0        0        0       51 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design_2.yaml.j2
+-rw-r--r--   0        0        0       81 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design_3.yaml.j2
+-rw-r--r--   0        0        0       13 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_report.md.j2
+-rw-r--r--   0        0        0     2972 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/test_designs.py
+-rw-r--r--   0        0        0     6436 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_builder.py
+-rw-r--r--   0        0        0     6941 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_context.py
+-rw-r--r--   0        0        0     8225 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_data_sources.py
+-rw-r--r--   0        0        0     4961 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_design_job.py
+-rw-r--r--   0        0        0     3804 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_errors.py
+-rw-r--r--   0        0        0     3890 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_ext.py
+-rw-r--r--   0        0        0     2761 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_jinja.py
+-rw-r--r--   0        0        0      669 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/many_to_many.yaml
+-rw-r--r--   0        0        0      422 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_name.yaml
+-rw-r--r--   0        0        0      412 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_ref.yaml
+-rw-r--r--   0        0        0     6639 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/complex_design1.yaml
+-rw-r--r--   0        0        0     2332 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_by_ref.yaml
+-rw-r--r--   0        0        0     1510 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_mlag.yaml
+-rw-r--r--   0        0        0      800 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_rack.yaml
+-rw-r--r--   0        0        0      895 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_relationships.yaml
+-rw-r--r--   0        0        0      213 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_tags.yaml
+-rw-r--r--   0        0        0     1360 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_label.yaml
+-rw-r--r--   0        0        0     1370 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_slug.yaml
+-rw-r--r--   0        0        0     1000 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml
+-rw-r--r--   0        0        0      337 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/git_repo.yaml
+-rw-r--r--   0        0        0     1078 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/interface_addresses.yaml
+-rw-r--r--   0        0        0     1039 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_create.yaml
+-rw-r--r--   0        0        0     1221 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_update.yaml
+-rw-r--r--   0        0        0     1282 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/one_to_one.yaml
+-rw-r--r--   0        0        0      505 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/prefixes.yaml
+-rw-r--r--   0        0        0     1615 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/custom_relationship_by_key.yaml
+-rw-r--r--   0        0        0     1605 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/custom_relationship_by_label.yaml
+-rw-r--r--   0        0        0      258 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/git_repo.yaml
+-rw-r--r--   0        0        0     1480 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/interface_addresses.yaml
+-rw-r--r--   0        0        0      815 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml
+-rw-r--r--   0        0        0     1284 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/nested_create.yaml
+-rw-r--r--   0        0        0      703 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml
+-rw-r--r--   0        0        0      310 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/roll_back.yaml
+-rw-r--r--   0        0        0      632 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_create.yaml
+-rw-r--r--   0        0        0      547 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_update.yaml
+-rw-r--r--   0        0        0      478 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/update_with_ref.yaml
+-rw-r--r--   0        0        0    12483 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/util.py
+-rw-r--r--   0        0        0     3599 2024-04-01 19:05:30.169982 nautobot_design_builder-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 nautobot_design_builder-1.1.0/PKG-INFO
```

### Comparing `nautobot_design_builder-1.0.0/LICENSE` & `nautobot_design_builder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/README.md` & `nautobot_design_builder-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/__init__.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plugin declaration for nautobot_design_builder."""
+
 # Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 from importlib import metadata
 
 from django.conf import settings
 from django.utils.functional import classproperty
 
 __version__ = metadata.version(__name__)
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/context.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that contains classes and functions for use with Design Builder context available when using Jinja templating."""
+
 from functools import cached_property
 from collections import UserList, UserDict, UserString
 import inspect
 from typing import Any
 import yaml
 
 from jinja2.nativetypes import NativeEnvironment
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/ext.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Extra action tags that are not part of the core Design Builder."""
+
 from functools import reduce
 import operator
 from typing import Any, Dict, Iterator, Tuple
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist, MultipleObjectsReturned, FieldError
 from django.db.models import Q
 
 from nautobot.circuits import models as circuits
 from nautobot.dcim import models as dcim
 from nautobot.ipam.models import Prefix
 
 import netaddr
-from nautobot_design_builder.design import Builder
-from nautobot_design_builder.design import ModelInstance
+from nautobot_design_builder.design import Environment, ModelInstance, ModelMetadata
 
 from nautobot_design_builder.errors import DesignImplementationError, MultipleObjectsReturnedError, DoesNotExistError
 from nautobot_design_builder.ext import AttributeExtension
 from nautobot_design_builder.jinja2 import network_offset
 
 
 class LookupMixin:
     """A helper mixin that provides a way to lookup objects."""
 
-    builder: Builder
+    environment: Environment
 
     def lookup_by_content_type(self, app_label, model_name, query):
         """Perform a query on a model.
 
         Args:
             app_label: Content type app-label that the model exists in.
             model_name_: Name of the model for the query.
@@ -61,15 +61,18 @@
         Returns:
             Iterator[Tuple[str, Any]]: A generator that yields they key/value pairs.
         """
         for key, value in query.items():
             if isinstance(value, dict):
                 yield from LookupMixin._flatten(value, f"{prefix}{key}__")
             else:
-                yield (f"{prefix}{key}", value)
+                if isinstance(value, ModelInstance):
+                    yield (f"!get:{prefix}{key}", value.instance)
+                else:
+                    yield (f"!get:{prefix}{key}", value)
 
     @staticmethod
     def flatten_query(query: dict) -> Dict[str, Any]:
         """Flatten a dictionary of dictionaries into query params.
 
         Django query arguments are a flat dictionary with the argument
         name being the query parameter and the value being what to match. However,
@@ -92,15 +95,15 @@
             >>>
             >>> LookupMixin.flatten_query(query)
             {'status__name': 'Active'}
             >>>
         """
         return dict(LookupMixin._flatten(query))
 
-    def lookup(self, queryset, query, parent=None):
+    def lookup(self, queryset, query, parent: ModelInstance = None):
         """Perform a single object lookup from a queryset.
 
         Args:
             queryset: Queryset (e.g. Status.objects.all) from which to query.
             query: Query params to filter by.
             parent: Optional field used for better error reporting. Set this
             value to the model instance that is semantically the parent so
@@ -109,18 +112,21 @@
         Raises:
             DoesNotExistError: If either no object is found.
             MultipleObjectsReturnedError: if multiple objects are found.
 
         Returns:
             Any: The object matching the query.
         """
-        query = self.builder.resolve_values(query, unwrap_model_instances=True)
+        query = self.environment.resolve_values(query)
         query = self.flatten_query(query)
         try:
-            return queryset.get(**query)
+            model_class = self.environment.model_class_index[queryset.model]
+            if parent:
+                return parent.create_child(model_class, query, queryset)
+            return model_class(self.environment, query, queryset)
         except ObjectDoesNotExist:
             # pylint: disable=raise-missing-from
             raise DoesNotExistError(queryset.model, query_filter=query, parent=parent)
         except MultipleObjectsReturned:
             # pylint: disable=raise-missing-from
             raise MultipleObjectsReturnedError(queryset.model, query=query, parent=parent)
 
@@ -237,16 +243,15 @@
             builder query lookup.
 
         Raises:
             DesignImplementationError: If no `status` was provided, or no matching
             termination was found.
 
         Returns:
-            None: This tag does not return a value, as it adds a deferred object
-            representing the cable connection.
+            dict: All of the information needed to lookup or create a cable instance.
 
         Example:
             ```yaml
             devices:
             - name: "Device 2"
               site__name: "Site"
               status__name: "Active"
@@ -279,27 +284,22 @@
                 if not query_managers:
                     # pylint:disable=raise-missing-from
                     raise DoesNotExistError(model_instance.model_class, query_filter=termination_query)
 
         cable_attributes.update(
             {
                 "termination_a": model_instance,
-                "!create_or_update:termination_b_type": ContentType.objects.get_for_model(remote_instance),
-                "!create_or_update:termination_b_id": remote_instance.id,
+                "!create_or_update:termination_b_type_id": ContentType.objects.get_for_model(
+                    remote_instance.instance
+                ).id,
+                "!create_or_update:termination_b_id": remote_instance.instance.id,
+                "deferred": True,
             }
         )
-
-        model_instance.deferred.append("cable")
-        model_instance.deferred_attributes["cable"] = [
-            model_instance.__class__(
-                self.builder,
-                model_class=dcim.Cable,
-                attributes=cable_attributes,
-            )
-        ]
+        return ("cable", cable_attributes)
 
 
 class NextPrefixExtension(AttributeExtension):
     """Provision the next prefix for a given set of parent prefixes."""
 
     tag = "next_prefix"
 
@@ -451,53 +451,44 @@
 
 
 class BGPPeeringExtension(AttributeExtension):
     """Create BGP peerings in the BGP Models App."""
 
     tag = "bgp_peering"
 
-    def __init__(self, builder: Builder):
+    def __init__(self, environment: Environment):
         """Initialize the BGPPeeringExtension.
 
         This initializer will import the necessary BGP models. If the
         BGP models app is not installed then it raises a DesignImplementationError.
 
         Raises:
             DesignImplementationError: Raised when the BGP Models App is not installed.
         """
-        super().__init__(builder)
+        super().__init__(environment)
         try:
             from nautobot_bgp_models.models import PeerEndpoint, Peering  # pylint:disable=import-outside-toplevel
 
-            self.PeerEndpoint = PeerEndpoint  # pylint:disable=invalid-name
-            self.Peering = Peering  # pylint:disable=invalid-name
+            self.PeerEndpoint = ModelInstance.factory(PeerEndpoint)  # pylint:disable=invalid-name
+            self.Peering = ModelInstance.factory(Peering)  # pylint:disable=invalid-name
         except ModuleNotFoundError:
             # pylint:disable=raise-missing-from
             raise DesignImplementationError(
                 "the `bgp_peering` tag can only be used when the bgp models app is installed."
             )
 
-    @staticmethod
-    def _post_save(sender, instance, **kwargs) -> None:  # pylint:disable=unused-argument
-        peering_instance: ModelInstance = instance
-        endpoint_a = peering_instance.instance.endpoint_a
-        endpoint_z = peering_instance.instance.endpoint_z
-        endpoint_a.peer, endpoint_z.peer = endpoint_z, endpoint_a
-        endpoint_a.save()
-        endpoint_z.save()
-
     def attribute(self, value, model_instance) -> None:
         """This attribute tag creates or updates a BGP peering for two endpoints.
 
         !bgp_peering will take an `endpoint_a` and `endpoint_z` argument to correctly
         create or update a BGP peering. Both endpoints can be specified using typical
         Design Builder syntax.
 
         Args:
-            value (dict): dictionary containing the keys `entpoint_a`
+            value (dict): dictionary containing the keys `endpoint_a`
             and `endpoint_z`. Both of these keys must be dictionaries
             specifying a way to either lookup or create the appropriate
             peer endpoints.
 
         Raises:
             DesignImplementationError: if the supplied value is not a dictionary
             or it does not include `endpoint_a` and `endpoint_z` as keys.
@@ -528,33 +519,41 @@
             raise DesignImplementationError(
                 "bgp peerings must be supplied a dictionary with `endpoint_a` and `endpoint_z`."
             )
 
         # copy the value so it won't be modified in later
         # use
         retval = {**value}
-        endpoint_a = ModelInstance(self.builder, self.PeerEndpoint, retval.pop("endpoint_a"))
-        endpoint_z = ModelInstance(self.builder, self.PeerEndpoint, retval.pop("endpoint_z"))
+        endpoint_a = self.PeerEndpoint(self.environment, retval.pop("endpoint_a"))
+        endpoint_z = self.PeerEndpoint(self.environment, retval.pop("endpoint_z"))
         peering_a = None
         peering_z = None
         try:
             peering_a = endpoint_a.instance.peering
             peering_z = endpoint_z.instance.peering
-        except self.Peering.DoesNotExist:
+        except self.Peering.model_class.DoesNotExist:
             pass
 
         # try to prevent empty peerings
         if peering_a == peering_z:
             if peering_a:
                 retval["!update:pk"] = peering_a.pk
         else:
             if peering_a:
                 peering_a.delete()
             if peering_z:
                 peering_z.delete()
 
         retval["endpoints"] = [endpoint_a, endpoint_z]
-        endpoint_a.attributes["peering"] = model_instance
-        endpoint_z.attributes["peering"] = model_instance
+        endpoint_a.metadata.attributes["peering"] = model_instance
+        endpoint_z.metadata.attributes["peering"] = model_instance
+
+        def post_save():
+            peering_instance: ModelInstance = model_instance
+            endpoint_a = peering_instance.instance.endpoint_a
+            endpoint_z = peering_instance.instance.endpoint_z
+            endpoint_a.peer, endpoint_z.peer = endpoint_z, endpoint_a
+            endpoint_a.save()
+            endpoint_z.save()
 
-        model_instance.connect(ModelInstance.POST_SAVE, BGPPeeringExtension._post_save)
+        model_instance.connect(ModelMetadata.POST_SAVE, post_save)
         return retval
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/test_ext.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/test_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests related to template extensions."""
+
 import os
 
 from django.test import TestCase
 
 from nautobot_design_builder.tests.test_builder import builder_test_case
 from nautobot_design_builder.util import nautobot_version
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/bgp_extension.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/bgp_extension.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
     location_types:
       - name: "Site"
         content_types:
           - "!get:app_label": "dcim"
             "!get:model": "device"
         locations:
-          name: "Site"
-          status__name: "Active"
+          - name: "Site"
+            status__name: "Active"
 
     manufacturers:
       - "!create_or_update:name": "test-manufacturer"
 
     device_types:
       - manufacturer__name: "test-manufacturer"
         "!create_or_update:model": "test-type"
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix_by_role_and_tenant.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix_by_role_and_tenant.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/design_job.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/design_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Base Design Job class definition."""
+
 import sys
 import traceback
 from abc import ABC, abstractmethod
 from os import path
 from typing import Dict
 import yaml
 
 from django.db import transaction
+from django.core.files.base import ContentFile
 
 from jinja2 import TemplateError
 
 from nautobot.extras.jobs import Job
-
+from nautobot.extras.models import FileProxy
 
 from nautobot_design_builder.errors import DesignImplementationError, DesignModelError
 from nautobot_design_builder.jinja2 import new_template_environment
 from nautobot_design_builder.logging import LoggingMixin
-from nautobot_design_builder.design import Builder
+from nautobot_design_builder.design import Environment
 from nautobot_design_builder.context import Context
 from .util import nautobot_version
 
 
 class DesignJob(Job, ABC, LoggingMixin):  # pylint: disable=too-many-instance-attributes
     """The base Design Job class that all specific Design Builder jobs inherit from.
 
@@ -38,40 +40,46 @@
     @abstractmethod
     def Meta(cls) -> Job.Meta:  # pylint: disable=invalid-name
         """Design jobs must provide either a Meta class method or a Meta class."""
 
     def __init__(self, *args, **kwargs):
         """Initialize the design job."""
         # rendered designs
-        self.builder: Builder = None
+        self.environment: Environment = None
         self.designs = {}
+        # TODO: Remove this when we no longer support Nautobot 1.x
         self.rendered = None
+        self.rendered_design = None
         self.failed = False
+        self.report = None
 
         super().__init__(*args, **kwargs)
 
-    def post_implementation(self, context: Context, builder: Builder):
+    def post_implementation(self, context: Context, environment: Environment):
         """Similar to Nautobot job's `post_run` method, but will be called after a design is implemented.
 
         Any design job that requires additional work to be completed after the design
         has been implemented can provide a `post_implementation` method. This method will be
         called after the entire set of design files has been implemented and the database
         transaction has been committed.
 
         Args:
             context (Context): The render context that was used for rendering the design files.
-            builder (Builder): The builder object that consumed the rendered design files. This is useful for accessing the design journal.
+            environment (Environment): The build environment that consumed the rendered design files. This is useful for accessing the design journal.
         """
 
     def post_run(self):
         """Method that will run after the main Nautobot job has executed."""
+        # TODO: This is not supported in Nautobot 2 and the entire method
+        # should be removed once we no longer support Nautobot 1.
         if self.rendered:
             self.job_result.data["output"] = self.rendered
 
         self.job_result.data["designs"] = self.designs
+        self.job_result.data["report"] = self.report
 
     def render(self, context: Context, filename: str) -> str:
         """High level function to render the Jinja design templates into YAML.
 
         Args:
             context (Context object): a tree of variables that can include templates for values
             filename (str): file name of the Jinja design template
@@ -108,20 +116,22 @@
     def render_design(self, context, design_file):
         """Wrapper function to take in rendered YAML from the design and convert to structured data and assign to the design property of a class instance.
 
         Args:
             context (Context object): a tree of variables that can include templates for values
             design_file (str): Filename of the design file to render.
         """
+        self.rendered_design = design_file
         self.rendered = self.render(context, design_file)
         design = yaml.safe_load(self.rendered)
         self.designs[design_file] = design
 
         # no need to save the rendered content if yaml loaded
         # it okay
+        self.rendered_design = None
         self.rendered = None
         return design
 
     def render_report(self, context: Context, journal: Dict) -> str:
         """Wrapper function to create rendered markdown report from the design job's Jinja report template.
 
         Args:
@@ -138,22 +148,45 @@
             },
             getattr(self.Meta, "report"),
         )
 
     def implement_design(self, context, design_file, commit):
         """Render the design_file template using the provided render context."""
         design = self.render_design(context, design_file)
-        self.builder.implement_design(design, commit)
+        self.environment.implement_design(design, commit)
+
+    def run(self, **kwargs):  # pylint: disable=arguments-differ
+        """Render the design and implement it within a build Environment object."""
+        try:
+            return self._run_in_transaction(**kwargs)
+        finally:
+            if self.rendered:
+                rendered_design = path.basename(self.rendered_design)
+                rendered_design, _ = path.splitext(rendered_design)
+                if not rendered_design.endswith(".yaml") and not rendered_design.endswith(".yml"):
+                    rendered_design = f"{rendered_design}.yaml"
+                self.save_design_file(rendered_design, self.rendered)
+            for design_file, design in self.designs.items():
+                output_file = path.basename(design_file)
+                # this should remove the .j2
+                output_file, _ = path.splitext(output_file)
+                if not output_file.endswith(".yaml") and not output_file.endswith(".yml"):
+                    output_file = f"{output_file}.yaml"
+                self.save_design_file(output_file, yaml.safe_dump(design))
 
     @transaction.atomic
-    def run(self, **kwargs):  # pylint: disable=arguments-differ,too-many-branches
-        """Render the design and implement it with a Builder object."""
+    def _run_in_transaction(self, **kwargs):  # pylint: disable=too-many-branches
+        """Render the design and implement it within a build Environment object.
+
+        This version of `run` is wrapped in a transaction and will roll back database changes
+        on error. In general, this method should only be called by the `run` method.
+        """
         self.log_info(message=f"Building {getattr(self.Meta, 'name')}")
         extensions = getattr(self.Meta, "extensions", [])
-        self.builder = Builder(job_result=self.job_result, extensions=extensions)
+        self.environment = Environment(job_result=self.job_result, extensions=extensions)
 
         design_files = None
 
         if nautobot_version < "2.0.0":
             commit = kwargs["commit"]
             data = kwargs["data"]
         else:
@@ -177,18 +210,20 @@
 
         sid = transaction.savepoint()
 
         try:
             for design_file in design_files:
                 self.implement_design(context, design_file, commit)
             if commit:
-                self.post_implementation(context, self.builder)
+                self.post_implementation(context, self.environment)
                 if hasattr(self.Meta, "report"):
-                    self.job_result.data["report"] = self.render_report(context, self.builder.journal)
-                    self.log_success(message=self.job_result.data["report"])
+                    self.report = self.render_report(context, self.environment.journal)
+                    self.log_success(message=self.report)
+                    if nautobot_version >= "2.0":
+                        self.save_design_file("report.md", self.report)
             else:
                 transaction.savepoint_rollback(sid)
                 self.log_info(
                     message=f"{self.name} can be imported successfully - No database changes made",
                 )
         except (DesignImplementationError, DesignModelError) as ex:
             transaction.savepoint_rollback(sid)
@@ -197,7 +232,25 @@
             self.failed = True
             if nautobot_version >= "2":
                 raise ex
         except Exception as ex:
             transaction.savepoint_rollback(sid)
             self.failed = True
             raise ex
+
+    def save_design_file(self, filename, content):
+        """Save some content to a job file.
+
+        This is only supported on Nautobot 2.0 and greater.
+
+        Args:
+            filename (str): The name of the file to save.
+            content (str): The content to save to the file.
+        """
+        if nautobot_version < "2.0":
+            return
+
+        FileProxy.objects.create(
+            name=filename,
+            job_result=self.job_result,
+            file=ContentFile(content.encode("utf-8"), name=filename),
+        )
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/errors.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing error Exception classes specific to Design Builder."""
+
 from collections import defaultdict
 from inspect import isclass
 
 from django.core.exceptions import ValidationError
 from django.db.models import Model
 
 
@@ -75,15 +76,15 @@
                 instance_str = str(model)
             except Exception:  # pylint: disable=broad-exception-caught
                 # Sometimes when converting a model to a string the __str__
                 # method itself produces an exceptions, like when an attribute
                 # hasn't been set or something. Whatever it is commonly is
                 # the cause of the original exception, we don't want to
                 # cause *another* exception because of that.
-                instance_str = model.__class__.__name__
+                instance_str = "unknown"
         model_str = model_class._meta.verbose_name.capitalize()
         if instance_str:
             model_str = f"{model_str} {instance_str}"
         return model_str
 
     @staticmethod
     def _object_to_markdown(obj, indentation=""):
@@ -107,16 +108,16 @@
     @property
     def path_str(self):
         """List of properly indented parents for the model."""
         path_msg = []
         model = self.model
         while model is not None:
             path_msg.insert(0, DesignModelError._model_str(model))
-            if not isclass(model) and hasattr(model, "parent"):
-                model = model.parent
+            if not isclass(model) and hasattr(model, "_parent"):
+                model = model._parent  # pylint:disable=protected-access
             elif self.parent:
                 model = self.parent
                 self.parent = None
             else:
                 model = None
         # don't include the top level model in the ancestry
         # tree because details about it should be included
@@ -188,15 +189,17 @@
             msg.append(path_msg)
         msg.append(f"{indentation}- {self.model_str}:")
         if hasattr(self.model, "query_filter"):
             msg.append(DesignModelError._object_to_markdown(self.model.query_filter, indentation=f"{indentation}    "))
         elif self.query_filter:
             msg.append(DesignModelError._object_to_markdown(self.query_filter, indentation=f"{indentation}    "))
         else:
-            msg.append(DesignModelError._object_to_markdown(self.model.filter, indentation=f"{indentation}    "))
+            msg.append(
+                DesignModelError._object_to_markdown(self.model.metadata.filter, indentation=f"{indentation}    ")
+            )
         return "\n".join(msg)
 
 
 class DoesNotExistError(DesignQueryError):
     """Raised when a `ModelInstance` underlying database object cannot be found."""
 
     def __str__(self):
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/ext.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/ext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extensions API for the object creator."""
+
 import os
 from abc import ABC, abstractmethod
 from functools import reduce
 from typing import TYPE_CHECKING, Any, List
 
 import inspect
 import sys
@@ -10,15 +11,15 @@
 import yaml
 
 from nautobot_design_builder import NautobotDesignBuilderConfig
 from nautobot_design_builder.errors import DesignImplementationError
 from nautobot_design_builder.git import GitRepo
 
 if TYPE_CHECKING:
-    from design import ModelInstance, Builder
+    from design import ModelInstance, Environment
 
 
 def is_extension(cls):
     """Determine if a class is an Extension."""
     return inspect.isclass(cls) and issubclass(cls, Extension) and cls is not Extension
 
 
@@ -60,35 +61,37 @@
     Likewise, for a value extension the `value_tag` and `value` instance
     method must be provided.
 
     The `__init__` method is called only once. The extension is initialized when the first
     tag matching `tag_name` or `value_name` is encountered.
 
     Args:
-        builder (Builder): The object creator that is implementing the
+        environment (Environment): The object creator that is implementing the
             current design.
     """
 
+    environment: "Environment"
+
     @property
     @abstractmethod
     def tag(self):
         """All Extensions must specify their tag name.
 
-        The `tag` method indicates to the Builder what the
+        The `tag` method indicates to the Environment what the
         tag name is for this extensions. For instance, a `tag`
         of `ref` will match `!ref` in the design.
         """
 
-    def __init__(self, builder: "Builder"):  # noqa: D107
-        self.builder = builder
+    def __init__(self, environment: "Environment"):  # noqa: D107
+        self.environment = environment
 
     def commit(self) -> None:
         """Optional method that is called once a design has been implemented and committed to the database.
 
-        Note: Commit is called once for each time Builder.implement_design is called. For a design job with
+        Note: Commit is called once for each time Environment.implement_design is called. For a design job with
         multiple design files, commit will be called once for each design file. It is up to the extension
         to track internal state so that multiple calls to `commit` don't introduce an inconsistency.
         """
 
     def roll_back(self) -> None:
         """Optional method that is called if the design has failed and the database transaction will be rolled back."""
 
@@ -134,22 +137,22 @@
     When used as a value extension, the syntax is `!ref:name_previously_used` where
     `name_previously_used` matches the string value provided to the original `!ref` attribute. With
     only the reference name, the entire CreatorObject is returned for assignment, when the name is
     followed by a dot and an attribute name, then only that matching attribute is returned from the
     stored creator object.
 
     Args:
-        builder (Builder): The object creator that is implementing the
+        environment (Environment): The object creator that is implementing the
             current design.
     """
 
     tag = "ref"
 
-    def __init__(self, builder: "Builder"):  # noqa: D107
-        super().__init__(builder)
+    def __init__(self, environment: "Environment"):  # noqa: D107
+        super().__init__(environment)
         self._env = {}
 
     def attribute(self, value, model_instance):
         """This method is called when the `!ref` tag is encountered.
 
         Args:
             value (Any): Value should be a string name (the reference) to refer to the object
@@ -191,23 +194,25 @@
             model_instance = self._env[key]
         except KeyError:
             # pylint: disable=raise-missing-from
             raise DesignImplementationError(f"No ref named {key} has been saved in the design.")
         if model_instance.instance and not model_instance.instance._state.adding:  # pylint: disable=protected-access
             model_instance.instance.refresh_from_db()
         if attribute:
+            # TODO: I think the result of the reduce operation needs to (potentially)
+            # be wrapped up in a ModelInstance object
             return reduce(getattr, [model_instance.instance, *attribute.split(".")])
         return model_instance
 
 
 class GitContextExtension(AttributeExtension):
     """Provides the "!git_context" attribute extension that will save content to a git repo.
 
     Args:
-        builder (Builder): The object creator that is implementing the
+        environment (Environment): The object creator that is implementing the
             current design.
 
     Example:
         ```yaml
         devices:
             - name: "My Device"
                 "!git_context":
@@ -220,18 +225,18 @@
         it will marshal the dictionary at `data` to `config/my_device.yml` to the base directory
         of the git repository. TODO: explain how the git repo is configured. Potentially change
         the configuration to have git_slug directly in the tag content?
     """
 
     tag = "git_context"
 
-    def __init__(self, builder: "Builder"):  # noqa: D107
-        super().__init__(builder)
+    def __init__(self, environment: "Environment"):  # noqa: D107
+        super().__init__(environment)
         slug = NautobotDesignBuilderConfig.context_repository
-        self.context_repo = GitRepo(slug, builder.job_result)
+        self.context_repo = GitRepo(slug, environment.job_result)
         self._env = {}
         self._reset()
 
     def _reset(self):
         """Reset the internal state for commit/rollback tracking."""
         self._env = {
             "files": [],
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/git.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/helpers.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module provides some common provisioning helpers that many designs use."""
+
 from typing import List
 
 from nautobot.dcim.models import Device
 from netutils.interface import interface_range_expansion
 
 from nautobot_design_builder.errors import DesignValidationError
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/jinja2.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/jinja2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Jinja2 related filters and environment methods."""
+
 import json
 from typing import TYPE_CHECKING
 import yaml
 
 from django.template import engines
 
 from jinja2 import Environment, FileSystemLoader, StrictUndefined
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/logging.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines logging capability for design builder."""
+
 import logging
 
 from nautobot.extras.choices import LogLevelChoices
 from nautobot.extras.models import JobResult
 
 from .util import nautobot_version
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/management/commands/build_design.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/build_design.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Management command to bootstrap development data for design builder app."""
+
 import sys
 import yaml
 
 from django.core.management.base import BaseCommand, CommandError
 
-from ...design import Builder
+from ...design import Environment
 
 
 def _load_file(filename):
     if filename == "-":
         return yaml.safe_load(sys.stdin)
     try:
         with open(filename) as file:  # pylint: disable=unspecified-encoding
@@ -24,12 +25,12 @@
     def add_arguments(self, parser):
         """Adds the design_file argument to the required command arguments."""
         parser.add_argument("--commit", action="store_true", help="Commit the design to the database.")
         parser.add_argument("design_file", nargs="+", type=str)
 
     def handle(self, *args, **options):
         """Handle the execution of the command."""
-        builder = Builder()
+        builder = Environment()
         for filename in options["design_file"]:
             self.stdout.write(f"Building design from {filename}")
             design = _load_file(filename)
             builder.implement_design(design, commit=options["commit"])
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/management/commands/install_demo_designs.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/install_demo_designs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Set up the demo designs git data source."""
+
 from django.core.management.base import BaseCommand
 
 from nautobot.extras.models import GitRepository
 
 
 class Command(BaseCommand):
     """Create a git datasource pointed to the demo designs repo."""
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/__init__.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,17 +31,19 @@
         git_instance_mock.return_value.path = self.git_path
         self.git_mock.side_effect = git_instance_mock
 
     def get_mocked_job(self, design_class: Type[DesignJob]):
         """Create an instance of design_class and properly mock request and job_result for testing."""
         job = design_class()
         job.job_result = mock.Mock()
+        job.save_design_file = lambda filename, content: None
         if nautobot_version < "2.0.0":
             job.request = mock.Mock()
         else:
+            # TODO: Remove this when we no longer support Nautobot 1.x
             job.job_result.data = {}
             old_run = job.run
 
             def new_run(data, commit):
                 kwargs = {**data}
                 kwargs["dryrun"] = not commit
                 old_run(**kwargs)
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/designs/test_designs.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/test_designs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 """Design jobs used for unit testing."""
+
 from nautobot_design_builder.design_job import DesignJob
 from nautobot_design_builder.ext import Extension
+from nautobot_design_builder.util import nautobot_version
 
 
 class SimpleDesign(DesignJob):
     """Simple design job."""
 
     class Meta:  # pylint: disable=too-few-public-methods
         name = "Simple Design"
         design_file = "templates/simple_design.yaml.j2"
 
 
+class SimpleDesign3(DesignJob):
+    """Simple design job with extra manufacturer."""
+
+    class Meta:  # pylint: disable=too-few-public-methods
+        name = "Simple Design 3"
+        design_file = "templates/simple_design_3.yaml.j2"
+
+
 class SimpleDesignReport(DesignJob):
     """Simple design job that includes a post-implementation report."""
 
     class Meta:  # pylint: disable=too-few-public-methods
-        name = "Simple Design"
+        name = "Simple Design with Report"
         design_file = "templates/simple_design.yaml.j2"
         report = "templates/simple_report.md.j2"
 
 
 class MultiDesignJob(DesignJob):
     """Design job that is implemented from multiple design files."""
 
     class Meta:  # pylint: disable=too-few-public-methods
-        name = "Simple Design"
+        name = "Multi File Design"
         design_files = [
             "templates/simple_design.yaml.j2",
             "templates/simple_design_2.yaml.j2",
         ]
 
 
 class MultiDesignJobWithError(DesignJob):
     """Design job that includes an error (for unit testing)."""
 
     class Meta:  # pylint: disable=too-few-public-methods
-        name = "Simple Design"
+        name = "Multi File Design with Error"
         design_files = [
             "templates/simple_design.yaml.j2",
             "templates/simple_design.yaml.j2",
         ]
 
 
 class CustomExtension(Extension):
@@ -67,7 +77,21 @@
 
 class DesignWithValidationError(DesignJob):
     """Design job that has objects with failing validation."""
 
     class Meta:  # pylint: disable=too-few-public-methods
         name = "Design with validation errors"
         design_file = "templates/design_with_validation_error.yaml.j2"
+
+
+if nautobot_version >= "2.0":
+    from nautobot.apps.jobs import register_jobs  # pylint: disable=import-error, no-name-in-module
+
+    register_jobs(
+        SimpleDesign,
+        SimpleDesignReport,
+        MultiDesignJob,
+        MultiDesignJobWithError,
+        DesignJobWithExtensions,
+        DesignWithRefError,
+        DesignWithValidationError,
+    )
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_builder.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Test object creator methods."""
+
 import importlib
 from operator import attrgetter
 import os
 from unittest.mock import Mock, patch
 import yaml
 
 from django.db.models import Manager, Q
 from django.test import TestCase
 
 from nautobot.dcim.models import Cable
 
-from nautobot_design_builder.design import Builder
+from nautobot_design_builder.design import Environment
 from nautobot_design_builder.util import nautobot_version
 
 
 class BuilderChecks:
     """Collection of static methods for testing designs."""
 
     @staticmethod
@@ -40,14 +41,23 @@
         value0 = _get_value(check[0])
         value1 = _get_value(check[1])
         if len(value0) == 1 and len(value1) == 1:
             test.assertEqual(value0[0], value1[0], msg=f"Check {index}")
         test.assertEqual(value0, value1, msg=f"Check {index}")
 
     @staticmethod
+    def check_count_equal(test, check, index):
+        """Check that two values are equal."""
+        value0 = _get_value(check[0])
+        value1 = _get_value(check[1])
+        if len(value0) == 1 and len(value1) == 1:
+            test.assertEqual(value0[0], value1[0], msg=f"Check {index}")
+        test.assertCountEqual(value0, value1, msg=f"Check {index}")
+
+    @staticmethod
     def check_model_exists(test, check, index):
         """Check that a model exists."""
         values = _get_value(check)
         test.assertEqual(len(values), 1, msg=f"Check {index}")
 
     @staticmethod
     def check_model_not_exist(test, check, index):
@@ -102,28 +112,29 @@
     def class_wrapper(test_class):
         for testcase, filename in _testcases(data_dir):
             # Strip the .yaml extension
             testcase_name = f"test_{filename[:-5]}"
 
             # Create a new closure for testcase
             def test_wrapper(testcase):
-                @patch("nautobot_design_builder.design.Builder.roll_back")
+                @patch("nautobot_design_builder.design.Environment.roll_back")
                 def test_runner(self, roll_back: Mock):
                     if testcase.get("skip", False):
                         self.skipTest("Skipping due to testcase skip=true")
                     extensions = []
                     for extension in testcase.get("extensions", []):
                         extensions.append(_load_class(extension))
 
-                    for design in testcase["designs"]:
-                        builder = Builder(extensions=extensions)
-                        commit = design.pop("commit", True)
-                        builder.implement_design(design=design, commit=commit)
-                        if not commit:
-                            roll_back.assert_called()
+                    with self.captureOnCommitCallbacks(execute=True):
+                        for design in testcase["designs"]:
+                            environment = Environment(extensions=extensions)
+                            commit = design.pop("commit", True)
+                            environment.implement_design(design=design, commit=commit)
+                            if not commit:
+                                roll_back.assert_called()
 
                     for index, check in enumerate(testcase.get("checks", [])):
                         for check_name, args in check.items():
                             _check_name = f"check_{check_name}"
                             if hasattr(BuilderChecks, _check_name):
                                 getattr(BuilderChecks, _check_name)(self, args, index)
                             else:
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_context.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test jinja2 render context."""
+
 import unittest
 
 from nautobot_design_builder.context import Context, _DictNode
 from nautobot_design_builder.tests.designs.context import BaseContext
 from nautobot_design_builder.tests.designs.sub_designs import SubDesignContext
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_data_sources.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_data_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test loading designs from git."""
+
 import inspect
 import os
 import sys
 from collections import namedtuple
 from unittest.mock import Mock
 
 from django.conf import settings
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_design_job.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_design_job.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test running design jobs."""
+
 from unittest.mock import patch, Mock
 
 from django.core.exceptions import ValidationError
 
 from nautobot.dcim.models import Manufacturer
 
 from nautobot_design_builder.errors import DesignImplementationError, DesignValidationError
@@ -10,31 +11,44 @@
 from nautobot_design_builder.tests.designs import test_designs
 from nautobot_design_builder.util import nautobot_version
 
 
 class TestDesignJob(DesignTestCase):
     """Test running design jobs."""
 
-    @patch("nautobot_design_builder.design_job.Builder")
-    def test_simple_design_commit(self, object_creator: Mock):
+    @patch("nautobot_design_builder.design_job.Environment")
+    def test_simple_design_commit(self, environment: Mock):
         job = self.get_mocked_job(test_designs.SimpleDesign)
         job.run(data={}, commit=True)
         self.assertIsNotNone(job.job_result)
-        object_creator.assert_called()
+        environment.assert_called()
         self.assertDictEqual(
             {"manufacturers": {"name": "Test Manufacturer"}},
             job.designs[test_designs.SimpleDesign.Meta.design_file],
         )
-        object_creator.return_value.roll_back.assert_not_called()
+        environment.return_value.roll_back.assert_not_called()
+
+    def test_simple_design_rollback(self):
+        job1 = self.get_mocked_job(test_designs.SimpleDesign)
+        job1.run(data={}, commit=True)
+        self.assertFalse(job1.failed)
+        self.assertEqual(1, Manufacturer.objects.all().count())
+        job2 = self.get_mocked_job(test_designs.SimpleDesign3)
+        if nautobot_version < "2":
+            job2.run(data={}, commit=True)
+        else:
+            self.assertRaises(DesignValidationError, job2.run, data={}, commit=True)
+        self.assertTrue(job2.failed)
+        self.assertEqual(1, Manufacturer.objects.all().count())
 
     def test_simple_design_report(self):
         job = self.get_mocked_job(test_designs.SimpleDesignReport)
         job.run(data={}, commit=True)
         self.assertJobSuccess(job)
-        self.assertEqual("Report output", job.job_result.data["report"])  # pylint: disable=unsubscriptable-object
+        self.assertEqual("Report output", job.report)
 
     def test_multiple_design_files(self):
         job = self.get_mocked_job(test_designs.MultiDesignJob)
         job.run(data={}, commit=True)
         self.assertDictEqual(
             {"manufacturers": {"name": "Test Manufacturer"}},
             job.designs[test_designs.MultiDesignJob.Meta.design_files[0]],
@@ -50,30 +64,30 @@
         if nautobot_version < "2":
             job.run(data={}, commit=True)
         else:
             self.assertRaises(DesignValidationError, job.run, data={}, commit=True)
 
         self.assertEqual(0, Manufacturer.objects.all().count())
 
-    @patch("nautobot_design_builder.design_job.Builder")
-    def test_custom_extensions(self, builder_patch: Mock):
+    @patch("nautobot_design_builder.design_job.Environment")
+    def test_custom_extensions(self, environment: Mock):
         job = self.get_mocked_job(test_designs.DesignJobWithExtensions)
         job.run(data={}, commit=True)
-        builder_patch.assert_called_once_with(
+        environment.assert_called_once_with(
             job_result=job.job_result,
             extensions=test_designs.DesignJobWithExtensions.Meta.extensions,
         )
 
 
 class TestDesignJobLogging(DesignTestCase):
     """Test that the design job logs errors correctly."""
 
-    @patch("nautobot_design_builder.design_job.Builder")
-    def test_simple_design_implementation_error(self, object_creator: Mock):
-        object_creator.return_value.implement_design.side_effect = DesignImplementationError("Broken")
+    @patch("nautobot_design_builder.design_job.Environment")
+    def test_simple_design_implementation_error(self, environment: Mock):
+        environment.return_value.implement_design.side_effect = DesignImplementationError("Broken")
         job = self.get_mocked_job(test_designs.SimpleDesign)
         if nautobot_version < "2":
             job.run(data={}, commit=True)
         else:
             self.assertRaises(DesignImplementationError, job.run, data={}, commit=True)
         self.assertTrue(job.failed)
         job.job_result.log.assert_called()
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_errors.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test design errors."""
+
 import unittest
 
 from django.core.exceptions import ValidationError
 
 from nautobot_design_builder.errors import DesignModelError, DesignValidationError
 
 
@@ -14,15 +15,15 @@
 
         def __init__(self, title="", parent=None):
             self.title = title
             self.instance = self
             self.model_class = self
             self._meta = self
             self.verbose_name = "verbose name"
-            self.parent = parent
+            self._parent = parent
 
         def __str__(self):
             return self.title
 
     def test_str_model(self):
         want = "Error Message"
         got = DesignModelError("Error Message").model_str
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_ext.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Unit tests related to template extensions."""
+
 import sys
 
 from django.test import TestCase
 
 from nautobot_design_builder import ext
-from nautobot_design_builder.design import Builder
+from nautobot_design_builder.design import Environment
 from nautobot_design_builder.ext import DesignImplementationError
 
 
 class Extension(ext.AttributeExtension):
     """An extension for testing."""
 
     tag = "custom_extension"
@@ -40,22 +41,22 @@
         self.assertEqual(extensions, discovered_extensions)
 
 
 class TestCustomExtensions(TestCase):
     """Test that custom extensions are loaded correctly."""
 
     def test_builder_called_with_custom_extensions(self):
-        builder = Builder(extensions=[Extension])
+        environment = Environment(extensions=[Extension])
         self.assertEqual(
-            builder.extensions["attribute"]["custom_extension"]["class"],
+            environment.extensions["attribute"]["custom_extension"]["class"],
             Extension,
         )
 
-    def test_builder_called_with_invalid_extensions(self):
-        self.assertRaises(DesignImplementationError, Builder, extensions=[NotExtension])
+    def test_environment_called_with_invalid_extensions(self):
+        self.assertRaises(DesignImplementationError, Environment, extensions=[NotExtension])
 
 
 class TestExtensionCommitRollback(TestCase):
     """Test that extensions are called correctly."""
 
     @staticmethod
     def run_test(design, commit):
@@ -75,17 +76,17 @@
                 nonlocal committed
                 committed = True
 
             def roll_back(self) -> None:
                 nonlocal rolled_back
                 rolled_back = True
 
-        builder = Builder(extensions=[CommitExtension])
+        environment = Environment(extensions=[CommitExtension])
         try:
-            builder.implement_design(design, commit=commit)
+            environment.implement_design(design, commit=commit)
         except DesignImplementationError:
             pass
         return committed, rolled_back
 
     def test_extension_commit(self):
         design = {
             "manufacturers": [
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/test_jinja.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_jinja.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests related to jinja2 rendering in the Design Builder."""
+
 import unittest
 
 from nautobot_design_builder.context import Context
 from nautobot_design_builder.jinja2 import new_template_environment
 
 
 class TestJinja(unittest.TestCase):
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/many_to_many.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/many_to_many.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/complex_design1.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/complex_design1.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_by_ref.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_by_ref.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_mlag.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_mlag.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_rack.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_rack.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_relationships.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_relationships.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_slug.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_update.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ---
 designs:
+  # Design 1
   - manufacturers:
       - name: "manufacturer1"
 
     device_types:
       - manufacturer__name: "manufacturer1"
         model: "model name"
         u_height: 1
@@ -22,17 +23,25 @@
         device_type__model: "model name"
         device_role__name: "device role"
         interfaces:
           - name: "Ethernet1/1"
             type: "virtual"
             status__name: "Active"
             description: "description for Ethernet1/1"
-            ip_addresses:
-              - address: "192.168.56.1/24"
-                status__name: "Active"
-        primary_ip4: {"!get:address": "192.168.56.1/24"}
+  # Design 2
+  - devices:
+      - "!update:name": "device_1"
+        interfaces:
+          - "!update:name": "Ethernet1/1"
+            description: "new description for Ethernet1/1"
 checks:
   - equal:
+      - model: "nautobot.dcim.models.Interface"
+        query: {name: "Ethernet1/1"}
+        attribute: "device"
       - model: "nautobot.dcim.models.Device"
         query: {name: "device_1"}
-        attribute: "primary_ip4.address.__str__"
-      - value: "192.168.56.1/24"
+  - equal:
+      - model: "nautobot.dcim.models.Interface"
+        query: {name: "Ethernet1/1"}
+        attribute: "description"
+      - value: "new description for Ethernet1/1"
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/interface_addresses.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/interface_addresses.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_create.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_create.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_update.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ---
 designs:
-  # Design 1
   - manufacturers:
       - name: "manufacturer1"
 
     device_types:
       - manufacturer__name: "manufacturer1"
         model: "model name"
         u_height: 1
@@ -23,25 +22,17 @@
         device_type__model: "model name"
         device_role__name: "device role"
         interfaces:
           - name: "Ethernet1/1"
             type: "virtual"
             status__name: "Active"
             description: "description for Ethernet1/1"
-  # Design 2
-  - devices:
-      - "!update:name": "device_1"
-        interfaces:
-          - "!update:name": "Ethernet1/1"
-            description: "new description for Ethernet1/1"
+            ip_addresses:
+              - address: "192.168.56.1/24"
+                status__name: "Active"
+        primary_ip4: {"!get:address": "192.168.56.1/24", "deferred": true}
 checks:
   - equal:
-      - model: "nautobot.dcim.models.Interface"
-        query: {name: "Ethernet1/1"}
-        attribute: "device"
       - model: "nautobot.dcim.models.Device"
         query: {name: "device_1"}
-  - equal:
-      - model: "nautobot.dcim.models.Interface"
-        query: {name: "Ethernet1/1"}
-        attribute: "description"
-      - value: "new description for Ethernet1/1"
+        attribute: "primary_ip4.address.__str__"
+      - value: "192.168.56.1/24"
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v1/one_to_one.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/one_to_one.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/interface_addresses.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/interface_addresses.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     location_types:
       - name: "Site"
         content_types:
           - "!get:app_label": "dcim"
             "!get:model": "device"
         locations:
-          name: "site_1"
-          status__name: "Active"
+          - name: "site_1"
+            status__name: "Active"
 
     prefixes:
       - prefix: "192.168.56.0/24"
         status__name: "Active"
         "!ref": "parent_prefix"
 
     devices:
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/nested_create.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/nested_create.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     location_types:
       - name: "Site"
         content_types:
           - "!get:app_label": "dcim"
             "!get:model": "device"
         locations:
-          name: "site_1"
-          status__name: "Active"
+          - name: "site_1"
+            status__name: "Active"
 
     devices:
       - name: "device_1"
         location__name: "site_1"
         status__name: "Active"
         device_type__model: "model name"
         role__name: "device role"
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 designs:
   - location_types:
       - name: "Site"
         content_types:
           - "!get:app_label": "ipam"
             "!get:model": "prefix"
         locations:
-          name: "site_1"
-          status__name: "Active"
+          - name: "site_1"
+            status__name: "Active"
+            "!ref": "site_1"
 
     prefixes:
-      - location__name: "site_1"
+      - locations:
+          - "!ref:site_1"
         status__name: "Active"
         prefix: "192.168.0.0/24"
-      - "!create_or_update:location__name": "site_1"
-        "!create_or_update:prefix": "192.168.56.0/24"
+      - "!create_or_update:prefix": "192.168.56.0/24"
+        locations:
+          - "!ref:site_1"
         status__name: "Active"
 
 checks:
   - equal:
       - model: "nautobot.ipam.models.Prefix"
-        query: {location__name: "site_1"}
+        query: {locations__name: "site_1"}
         attribute: "__str__"
       - value: ["192.168.0.0/24", "192.168.56.0/24"]
```

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/simple_create.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_create.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/tests/testdata/simple_update.yaml` & `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_update.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.0.0/nautobot_design_builder/util.py` & `nautobot_design_builder-1.1.0/nautobot_design_builder/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main design builder app module, contains DesignJob and base methods and functions."""
+
 import functools
 import importlib
 import inspect
 import logging
 import os
 import pkgutil
 import sys
```

### Comparing `nautobot_design_builder-1.0.0/pyproject.toml` & `nautobot_design_builder-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-design-builder"
-version = "v1.0.0"
+version = "v1.1.0"
 description = "Nautobot app that uses design templates to easily create data objects in Nautobot with minimal input from a user."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-app-design-builder"
 repository = "https://github.com/nautobot/nautobot-app-design-builder"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -22,15 +22,15 @@
     "README.md",
 ]
 packages = [
     { include = "nautobot_design_builder" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8.1,<3.12"
 # Used for local development
 nautobot = ">=1.6.0,<=2.9999"
 nautobot-bgp-models = { version = "*", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 black = "*"
@@ -53,14 +53,15 @@
 mkdocs-material = "9.2.4"
 # Render custom markdown for version added/changed/remove notes
 mkdocs-version-annotations = "1.0.0"
 # Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.22.0"
 mkdocstrings-python = "1.5.2"
 gitpython = "^3.1.41"
+snakeviz = "^2.2.0"
 
 [tool.poetry.extras]
 nautobot = ["nautobot"]
 contrib = ["nautobot-bgp-models"]
 
 [tool.black]
 line-length = 120
@@ -94,15 +95,15 @@
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
 disable = """,
-    line-too-long
+    line-too-long,
     """
 
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
```

### Comparing `nautobot_design_builder-1.0.0/PKG-INFO` & `nautobot_design_builder-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nautobot-design-builder
-Version: 1.0.0
+Version: 1.1.0
 Summary: Nautobot app that uses design templates to easily create data objects in Nautobot with minimal input from a user.
 Home-page: https://github.com/nautobot/nautobot-app-design-builder
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: contrib
 Provides-Extra: nautobot
 Requires-Dist: nautobot (>=1.6.0,<=2.9999) ; extra == "nautobot"
 Requires-Dist: nautobot-bgp-models ; extra == "contrib"
 Project-URL: Repository, https://github.com/nautobot/nautobot-app-design-builder
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nautobot-design-builder Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nautobot-design-builder Version: 1.1.0 Summary:
 Nautobot app that uses design templates to easily create data objects in
 Nautobot with minimal input from a user. Home-page: https://github.com/
 nautobot/nautobot-app-design-builder License: Apache-2.0 Keywords:
 nautobot,nautobot-plugin Author: Network to Code, LLC Author-email:
-opensource@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
+opensource@networktocode.com Requires-Python: >=3.8.1,<3.12 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Provides-Extra: contrib Provides-Extra: nautobot
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.8 Provides-Extra: contrib Provides-Extra: nautobot
 Requires-Dist: nautobot (>=1.6.0,<=2.9999) ; extra == "nautobot" Requires-Dist:
 nautobot-bgp-models ; extra == "contrib" Project-URL: Repository, https://
 github.com/nautobot/nautobot-app-design-builder Description-Content-Type: text/
 markdown # Nautobot Design Builder
    [https://raw.githubusercontent.com/nautobot/nautobot-app-design-builder/
              develop/docs/images/icon-nautobot-design-builder.png]
   _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_s_i_g_n_-_b_u_i_l_d_e_r_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
```

