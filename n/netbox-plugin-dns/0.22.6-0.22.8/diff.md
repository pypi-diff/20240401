# Comparing `tmp/netbox_plugin_dns-0.22.6.tar.gz` & `tmp/netbox_plugin_dns-0.22.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-0.22.6.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-0.22.8.tar", max compression
```

## Comparing `netbox_plugin_dns-0.22.6.tar` & `netbox_plugin_dns-0.22.8.tar`

### file list

```diff
@@ -1,116 +1,117 @@
--rw-r--r--   0        0        0     1076 2024-03-22 23:49:15.174060 netbox_plugin_dns-0.22.6/LICENSE
--rw-r--r--   0        0        0     3696 2024-03-22 23:49:15.174060 netbox_plugin_dns-0.22.6/README.md
--rw-r--r--   0        0        0     1287 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/__init__.py
--rw-r--r--   0        0        0     3291 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0     8183 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0      575 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3527 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/apps.py
--rw-r--r--   0        0        0       69 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0     1494 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3592 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/fields/network.py
--rw-r--r--   0        0        0     2521 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/fields/rfc2317.py
--rw-r--r--   0        0        0      136 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/__init__.py
--rw-r--r--   0        0        0     1027 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/contact.py
--rwxr-xr-x   0        0        0      522 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/nameserver.py
--rwxr-xr-x   0        0        0     1691 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/record.py
--rw-r--r--   0        0        0      911 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/registrar.py
--rw-r--r--   0        0        0      497 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/view.py
--rwxr-xr-x   0        0        0     3556 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/filters/zone.py
--rw-r--r--   0        0        0      136 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/__init__.py
--rw-r--r--   0        0        0     4492 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/contact.py
--rwxr-xr-x   0        0        0     2027 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     6171 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/record.py
--rw-r--r--   0        0        0     2636 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/registrar.py
--rw-r--r--   0        0        0     1627 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    21702 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      811 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0      497 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/contact.py
--rw-r--r--   0        0        0      527 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/nameserver.py
--rw-r--r--   0        0        0      487 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/record.py
--rw-r--r--   0        0        0      517 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/registrar.py
--rw-r--r--   0        0        0      221 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0      467 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/view.py
--rw-r--r--   0        0        0      467 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/graphql/zone.py
--rw-r--r--   0        0        0     6050 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0     2077 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/management/commands/cleanup_rrset_ttl.py
--rw-r--r--   0        0        0     4580 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/management/commands/setup_coupling.py
--rw-r--r--   0        0        0      661 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0     4153 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0001_initial.py
--rw-r--r--   0        0        0    11466 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0      437 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0002_zone_default_ttl.py
--rw-r--r--   0        0        0     3716 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0003_soa_managed_records.py
--rw-r--r--   0        0        0     2287 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
--rw-r--r--   0        0        0     1156 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0005_update_ns_records.py
--rw-r--r--   0        0        0      861 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0006_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      399 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      527 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0008_zone_status_names.py
--rw-r--r--   0        0        0     2176 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0009_netbox32.py
--rw-r--r--   0        0        0     1543 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0010_update_soa_records.py
--rw-r--r--   0        0        0     2201 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0011_add_view_model.py
--rw-r--r--   0        0        0      402 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0012_adjust_zone_and_record.py
--rw-r--r--   0        0        0      733 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
--rw-r--r--   0        0        0      428 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0014_add_view_description.py
--rw-r--r--   0        0        0      393 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0015_add_record_status.py
--rw-r--r--   0        0        0     1053 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0016_cleanup_ptr_records.py
--rw-r--r--   0        0        0      405 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0017_alter_record_ttl.py
--rw-r--r--   0        0        0     1553 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0018_zone_arpa_network.py
--rw-r--r--   0        0        0      433 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0019_update_ns_ttl.py
--rw-r--r--   0        0        0     1260 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3243 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      172 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0      378 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0023_alter_record_value.py
--rw-r--r--   0        0        0     1745 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0024_tenancy.py
--rw-r--r--   0        0        0      620 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0025_ipam_coupling_cf.py
--rw-r--r--   0        0        0     5796 2024-03-22 23:49:15.206060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0026_domain_registration.py
--rw-r--r--   0        0        0      404 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0027_alter_registrar_iana_id.py
--rw-r--r--   0        0        0     1364 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/0028_rfc2317_fields.py
--rw-r--r--   0        0        0        0 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0      182 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/__init__.py
--rw-r--r--   0        0        0     2849 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/contact.py
--rw-r--r--   0        0        0     2941 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/nameserver.py
--rw-r--r--   0        0        0    23896 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/record.py
--rw-r--r--   0        0        0     1416 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/registrar.py
--rw-r--r--   0        0        0      920 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/view.py
--rw-r--r--   0        0        0    26333 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/models/zone.py
--rw-r--r--   0        0        0     4587 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/navigation.py
--rw-r--r--   0        0        0        0 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/signals/__init__.py
--rw-r--r--   0        0        0     5727 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/signals/ipam_coupling.py
--rw-r--r--   0        0        0      136 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      747 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/contact.py
--rw-r--r--   0        0        0      819 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3162 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      621 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/registrar.py
--rw-r--r--   0        0        0      501 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1886 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     3936 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/template_content.py
--rw-r--r--   0        0        0     2858 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/contact.html
--rw-r--r--   0        0        0     1623 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      742 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     5835 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0     2130 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/registrar.html
--rw-r--r--   0        0        0      806 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/related_dns_objects.html
--rw-r--r--   0        0        0     1350 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      460 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2171 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      524 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2218 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0     1283 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/registration.html
--rw-r--r--   0        0        0      527 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
--rw-r--r--   0        0        0     7187 2024-03-22 23:49:15.210060 netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0     9172 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/urls.py
--rw-r--r--   0        0        0     1967 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/utilities/__init__.py
--rw-r--r--   0        0        0     3573 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/utilities/ipam_coupling.py
--rw-r--r--   0        0        0       47 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/validators/__init__.py
--rw-r--r--   0        0        0     2232 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/validators/dns_name.py
--rw-r--r--   0        0        0      503 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/validators/rfc2317.py
--rw-r--r--   0        0        0      136 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0     2235 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/contact.py
--rw-r--r--   0        0        0     2990 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     4896 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/record.py
--rw-r--r--   0        0        0     2072 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/registrar.py
--rw-r--r--   0        0        0     1895 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/view.py
--rw-r--r--   0        0        0     4587 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      741 2024-03-22 23:49:15.214060 netbox_plugin_dns-0.22.6/pyproject.toml
--rw-r--r--   0        0        0     4572 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.22.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-01 17:13:14.517036 netbox_plugin_dns-0.22.8/LICENSE
+-rw-r--r--   0        0        0     3696 2024-04-01 17:13:14.517036 netbox_plugin_dns-0.22.8/README.md
+-rw-r--r--   0        0        0     1314 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/__init__.py
+-rw-r--r--   0        0        0     3291 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0     8203 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0      575 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/apps.py
+-rw-r--r--   0        0        0       69 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1494 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3592 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0     2521 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/__init__.py
+-rw-r--r--   0        0        0     1027 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/contact.py
+-rwxr-xr-x   0        0        0      522 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/nameserver.py
+-rwxr-xr-x   0        0        0     2256 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/record.py
+-rw-r--r--   0        0        0      911 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/registrar.py
+-rw-r--r--   0        0        0      497 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/view.py
+-rwxr-xr-x   0        0        0     3564 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/zone.py
+-rw-r--r--   0        0        0      136 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/__init__.py
+-rw-r--r--   0        0        0     4492 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/contact.py
+-rwxr-xr-x   0        0        0     2027 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     6266 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0     2832 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/registrar.py
+-rw-r--r--   0        0        0     1627 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    21740 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      811 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0      497 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/contact.py
+-rw-r--r--   0        0        0      527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/nameserver.py
+-rw-r--r--   0        0        0      487 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/record.py
+-rw-r--r--   0        0        0      517 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/registrar.py
+-rw-r--r--   0        0        0      221 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0      467 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/view.py
+-rw-r--r--   0        0        0      467 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/zone.py
+-rw-r--r--   0        0        0     6050 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0     2077 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_rrset_ttl.py
+-rw-r--r--   0        0        0     4580 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/setup_coupling.py
+-rw-r--r--   0        0        0      661 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0     4153 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_initial.py
+-rw-r--r--   0        0        0    11466 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0      437 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0002_zone_default_ttl.py
+-rw-r--r--   0        0        0     3716 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0003_soa_managed_records.py
+-rw-r--r--   0        0        0     2287 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
+-rw-r--r--   0        0        0     1156 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0005_update_ns_records.py
+-rw-r--r--   0        0        0      861 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0006_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      399 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
+-rw-r--r--   0        0        0      527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0008_zone_status_names.py
+-rw-r--r--   0        0        0     2176 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0009_netbox32.py
+-rw-r--r--   0        0        0     1543 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0010_update_soa_records.py
+-rw-r--r--   0        0        0     2201 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0011_add_view_model.py
+-rw-r--r--   0        0        0      402 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0012_adjust_zone_and_record.py
+-rw-r--r--   0        0        0      733 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
+-rw-r--r--   0        0        0      428 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0014_add_view_description.py
+-rw-r--r--   0        0        0      393 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0015_add_record_status.py
+-rw-r--r--   0        0        0     1053 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0016_cleanup_ptr_records.py
+-rw-r--r--   0        0        0      405 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0017_alter_record_ttl.py
+-rw-r--r--   0        0        0     1553 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0018_zone_arpa_network.py
+-rw-r--r--   0        0        0      433 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0019_update_ns_ttl.py
+-rw-r--r--   0        0        0     1260 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3243 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      172 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0      378 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0023_alter_record_value.py
+-rw-r--r--   0        0        0     1745 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0024_tenancy.py
+-rw-r--r--   0        0        0      620 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0025_ipam_coupling_cf.py
+-rw-r--r--   0        0        0     5796 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0026_domain_registration.py
+-rw-r--r--   0        0        0      404 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0027_alter_registrar_iana_id.py
+-rw-r--r--   0        0        0     1364 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0028_rfc2317_fields.py
+-rw-r--r--   0        0        0      808 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0029_record_fqdn.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/__init__.py
+-rw-r--r--   0        0        0     2849 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/contact.py
+-rw-r--r--   0        0        0     2941 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/nameserver.py
+-rw-r--r--   0        0        0    23917 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/record.py
+-rw-r--r--   0        0        0     1416 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/registrar.py
+-rw-r--r--   0        0        0      920 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/view.py
+-rw-r--r--   0        0        0    26637 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/zone.py
+-rw-r--r--   0        0        0     4587 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/navigation.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/signals/__init__.py
+-rw-r--r--   0        0        0     5727 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/signals/ipam_coupling.py
+-rw-r--r--   0        0        0      136 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/contact.py
+-rw-r--r--   0        0        0      819 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3162 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      621 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/registrar.py
+-rw-r--r--   0        0        0      501 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1886 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     3936 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     2858 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/contact.html
+-rw-r--r--   0        0        0     1623 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      742 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     5835 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0     2130 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/registrar.html
+-rw-r--r--   0        0        0      806 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/related_dns_objects.html
+-rw-r--r--   0        0        0     1350 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      460 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2171 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      524 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2218 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0     1283 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/registration.html
+-rw-r--r--   0        0        0      527 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
+-rw-r--r--   0        0        0     7187 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0     9172 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1967 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/utilities/__init__.py
+-rw-r--r--   0        0        0     3573 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/utilities/ipam_coupling.py
+-rw-r--r--   0        0        0       47 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/__init__.py
+-rw-r--r--   0        0        0     2232 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/dns_name.py
+-rw-r--r--   0        0        0      503 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2235 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/contact.py
+-rw-r--r--   0        0        0     2990 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     4904 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     2072 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/registrar.py
+-rw-r--r--   0        0        0     1895 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     4587 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      741 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/pyproject.toml
+-rw-r--r--   0        0        0     4572 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.22.8/PKG-INFO
```

### Comparing `netbox_plugin_dns-0.22.6/LICENSE` & `netbox_plugin_dns-0.22.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/README.md` & `netbox_plugin_dns-0.22.8/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/__init__.py` & `netbox_plugin_dns-0.22.8/netbox_dns/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 try:
     # NetBox 3.5.0 - 3.5.7, 3.5.9+
     from extras.plugins import get_plugin_config
 except ImportError:
     # NetBox 3.5.8
     from extras.plugins.utils import get_plugin_config
 
-__version__ = "0.22.6"
+__version__ = "0.22.8"
 
 
 class DNSConfig(PluginConfig):
     name = "netbox_dns"
     verbose_name = "NetBox DNS"
     description = "NetBox plugin for DNS data"
     min_version = "3.5.0"
+    max_version = "3.99.0"
     version = __version__
     author = "Peter Eckel"
     author_email = "pete@netbox-dns.org"
     required_settings = []
     default_settings = {
         "zone_default_ttl": 86400,
         "zone_soa_serial_auto": True,
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-0.22.8/netbox_dns/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/api/serializers.py` & `netbox_plugin_dns-0.22.8/netbox_dns/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
         fields = (
             "id",
             "url",
             "zone",
             "display",
             "type",
             "name",
+            "fqdn",
             "value",
             "status",
             "ttl",
             "description",
             "tags",
             "created",
             "last_updated",
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/api/urls.py` & `netbox_plugin_dns-0.22.8/netbox_dns/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/api/views.py` & `netbox_plugin_dns-0.22.8/netbox_dns/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/fields/address.py` & `netbox_plugin_dns-0.22.8/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/fields/network.py` & `netbox_plugin_dns-0.22.8/netbox_dns/fields/network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/fields/rfc2317.py` & `netbox_plugin_dns-0.22.8/netbox_dns/fields/rfc2317.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/filters/contact.py` & `netbox_plugin_dns-0.22.8/netbox_dns/filters/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/filters/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/filters/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/filters/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/filters/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/filters/zone.py` & `netbox_plugin_dns-0.22.8/netbox_dns/filters/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.filtersets import TenancyFilterSet
 
 from netbox_dns.models import View, Zone, ZoneStatusChoices, Registrar, Contact
 
 
 class ZoneFilter(TenancyFilterSet, NetBoxModelFilterSet):
-    status = django_filters.ChoiceFilter(
+    status = django_filters.MultipleChoiceFilter(
         choices=ZoneStatusChoices,
     )
     view_id = django_filters.ModelMultipleChoiceFilter(
         queryset=View.objects.all(),
         label="View ID",
     )
     view = django_filters.ModelMultipleChoiceFilter(
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/contact.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/record.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,32 +75,39 @@
         )
 
 
 class RecordFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = Record
     fieldsets = (
         (None, ("q", "filter_id", "tag")),
-        ("Attributes", ("view_id", "zone_id", "name", "type", "value", "status")),
+        (
+            "Attributes",
+            ("view_id", "zone_id", "name", "fqdn", "type", "value", "status"),
+        ),
         ("Tenant", ("tenant_group_id", "tenant_id")),
     )
 
     type = forms.MultipleChoiceField(
-        choices=add_blank_choice(RecordTypeChoices),
+        choices=RecordTypeChoices,
         required=False,
     )
     name = forms.CharField(
         required=False,
         label="Name",
     )
+    fqdn = forms.CharField(
+        required=False,
+        label="FQDN",
+    )
     value = forms.CharField(
         required=False,
         label="Value",
     )
-    status = forms.ChoiceField(
-        choices=add_blank_choice(RecordStatusChoices),
+    status = forms.MultipleChoiceField(
+        choices=RecordStatusChoices,
         required=False,
     )
     zone_id = DynamicModelMultipleChoiceField(
         queryset=Zone.objects.all(),
         required=False,
         label="Zone",
     )
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/registrar.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,21 @@
             "tags",
         )
 
 
 class RegistrarBulkEditForm(NetBoxModelBulkEditForm):
     model = Registrar
 
+    iana_id = forms.IntegerField(
+        required=False,
+        label="IANA ID",
+    )
+    address = forms.CharField(
+        required=False,
+    )
     referral_url = forms.CharField(
         required=False,
         label="Referral URL",
     )
     whois_server = forms.CharField(
         required=False,
         label="WHOIS Server",
@@ -100,23 +107,25 @@
         label="Abuse Phone",
     )
 
     fieldsets = (
         (
             None,
             (
+                "iana_id",
                 "address",
                 "referral_url",
                 "whois_server",
                 "abuse_email",
                 "abuse_phone",
             ),
         ),
     )
 
     nullable_fields = (
+        "iana_id",
         "address",
         "referral_url",
         "whois_server",
         "abuse_email",
         "abuse_phone",
     )
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/view.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/forms/zone.py` & `netbox_plugin_dns-0.22.8/netbox_dns/forms/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,16 @@
     )
 
     view_id = DynamicModelMultipleChoiceField(
         queryset=View.objects.all(),
         required=False,
         label="View",
     )
-    status = forms.ChoiceField(
-        choices=add_blank_choice(ZoneStatusChoices),
+    status = forms.MultipleChoiceField(
+        choices=ZoneStatusChoices,
         required=False,
     )
     name = forms.CharField(
         required=False,
         label="Name",
     )
     nameservers = DynamicModelMultipleChoiceField(
@@ -591,16 +591,17 @@
     )
     rfc2317_prefix = RFC2317NetworkFormField(
         required=False,
         label="RFC2317 Prefix",
         help_text="IPv4 network prefix with a mask length of at least 25 bits",
         validators=[validate_ipv4, validate_prefix, validate_rfc2317],
     )
-    rfc2317_parent_managed = forms.BooleanField(
+    rfc2317_parent_managed = forms.NullBooleanField(
         required=False,
+        widget=BulkEditNullBooleanSelect(),
         label="RFC2317 Parent Managed",
         help_text="IPv4 reverse zone for deletgating the RFC2317 PTR records is managed in NetBox DNS",
     )
     registrar = DynamicModelChoiceField(
         queryset=Registrar.objects.all(),
         required=False,
         widget=APISelect(
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/graphql/__init__.py` & `netbox_plugin_dns-0.22.8/netbox_dns/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/graphql/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/graphql/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/graphql/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/graphql/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_database.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/management/commands/cleanup_rrset_ttl.py` & `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_rrset_ttl.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/management/commands/setup_coupling.py` & `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/setup_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/update_soa.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0001_initial.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0003_soa_managed_records.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0003_soa_managed_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0005_update_ns_records.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0005_update_ns_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0006_zone_soa_serial_auto.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0006_zone_soa_serial_auto.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0008_zone_status_names.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0008_zone_status_names.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0009_netbox32.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0009_netbox32.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0010_update_soa_records.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0010_update_soa_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0011_add_view_model.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0011_add_view_model.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0016_cleanup_ptr_records.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0016_cleanup_ptr_records.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0018_zone_arpa_network.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0018_zone_arpa_network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0021_record_ip_address.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0024_tenancy.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0024_tenancy.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0025_ipam_coupling_cf.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0025_ipam_coupling_cf.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0026_domain_registration.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0026_domain_registration.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/migrations/0028_rfc2317_fields.py` & `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0028_rfc2317_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/contact.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/record.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,25 +110,31 @@
     ACTIVE_STATUS_LIST = (RecordStatusChoices.STATUS_ACTIVE,)
 
     unique_ptr_qs = Q(
         Q(disable_ptr=False),
         Q(Q(type=RecordTypeChoices.A) | Q(type=RecordTypeChoices.AAAA)),
     )
 
+    name = models.CharField(
+        max_length=255,
+    )
     zone = models.ForeignKey(
         "Zone",
         on_delete=models.CASCADE,
     )
+    fqdn = models.CharField(
+        max_length=255,
+        null=True,
+        blank=True,
+        default=None,
+    )
     type = models.CharField(
         choices=RecordTypeChoices,
         max_length=10,
     )
-    name = models.CharField(
-        max_length=255,
-    )
     value = models.CharField(
         max_length=65535,
     )
     status = models.CharField(
         max_length=50,
         choices=RecordStatusChoices,
         default=RecordStatusChoices.STATUS_ACTIVE,
@@ -205,22 +211,15 @@
     ]
 
     class Meta:
         ordering = ("zone", "name", "type", "value", "status")
 
     def __str__(self):
         try:
-            name = (
-                dns_name.from_text(
-                    str(self.name),
-                    origin=dns_name.from_text(self.zone.name, origin=None),
-                )
-                .relativize(dns_name.root)
-                .to_unicode()
-            )
+            name = dns_name.from_text(self.fqdn).relativize(dns_name.root).to_unicode()
         except dns_name.IDNAException:
             name = self.name
         except dns_name.LabelTooLong as exc:
             name = f"{self.name[:59]}..."
 
         return f"{name} [{self.type}]"
 
@@ -231,21 +230,14 @@
     def get_status_color(self):
         return RecordStatusChoices.colors.get(self.status)
 
     def get_absolute_url(self):
         return reverse("plugins:netbox_dns:record", kwargs={"pk": self.id})
 
     @property
-    def fqdn(self):
-        zone = dns_name.from_text(self.zone.name)
-        name = dns_name.from_text(self.name, origin=zone)
-
-        return name.to_text()
-
-    @property
     def value_fqdn(self):
         if self.type != RecordTypeChoices.CNAME:
             return None
 
         zone = dns_name.from_text(self.zone.name)
         value_fqdn = dns_name.from_text(self.value, origin=zone)
 
@@ -389,63 +381,87 @@
                 ptr_record.save(
                     update_rfc2317_cname=update_rfc2317_cname,
                     save_zone_serial=save_zone_serial,
                 )
 
         self.ptr_record = ptr_record
 
+    def remove_from_rfc2317_cname_record(self, save_zone_serial=True):
+        if self.rfc2317_cname_record.pk:
+            rfc2317_ptr_records = self.rfc2317_cname_record.rfc2317_ptr_records.exclude(
+                pk=self.pk
+            )
+
+            if rfc2317_ptr_records:
+                self.rfc2317_cname_record.ttl = rfc2317_ptr_records.aggregate(
+                    Min("ttl")
+                ).get("ttl__min")
+                self.rfc2317_cname_record.save(
+                    update_fields=["ttl"], save_zone_serial=save_zone_serial
+                )
+            else:
+                self.rfc2317_cname_record.delete()
+
     def update_rfc2317_cname_record(self, save_zone_serial=True):
         if self.zone.rfc2317_parent_managed:
             cname_name = dns_name.from_text(
                 ipaddress.ip_address(self.ip_address).reverse_pointer
             ).relativize(dns_name.from_text(self.zone.rfc2317_parent_zone.name))
 
             if self.rfc2317_cname_record is not None:
-                self.rfc2317_cname_record.name = cname_name
-                self.rfc2317_cname_record.zone = self.zone.rfc2317_parent_zone
-                self.rfc2317_cname_record.value = self.fqdn
-                self.rfc2317_cname_record.ttl = min_ttl(
-                    self.rfc2317_cname_record.rfc2317_ptr_records.exclude(pk=self.pk)
+                if self.rfc2317_cname_record.name == cname_name.to_text():
+                    self.rfc2317_cname_record.zone = self.zone.rfc2317_parent_zone
+                    self.rfc2317_cname_record.value = self.fqdn
+                    self.rfc2317_cname_record.ttl = min_ttl(
+                        self.rfc2317_cname_record.rfc2317_ptr_records.exclude(
+                            pk=self.pk
+                        )
+                        .aggregate(Min("ttl"))
+                        .get("ttl__min"),
+                        self.ttl,
+                    )
+                    self.rfc2317_cname_record.save(save_zone_serial=save_zone_serial)
+
+                    return
+                else:
+                    self.remove_from_rfc2317_cname_record(
+                        save_zone_serial=save_zone_serial
+                    )
+
+            rfc2317_cname_record = Record.objects.filter(
+                name=cname_name,
+                type=RecordTypeChoices.CNAME,
+                zone=self.zone.rfc2317_parent_zone,
+                managed=True,
+                value=self.fqdn,
+            ).first()
+
+            if rfc2317_cname_record is not None:
+                rfc2317_cname_record.ttl = min_ttl(
+                    rfc2317_cname_record.rfc2317_ptr_records.exclude(pk=self.pk)
                     .aggregate(Min("ttl"))
                     .get("ttl__min"),
                     self.ttl,
                 )
-                self.rfc2317_cname_record.save(save_zone_serial=save_zone_serial)
+                rfc2317_cname_record.save(
+                    update_fields=["ttl"], save_zone_serial=save_zone_serial
+                )
+
             else:
-                rfc2317_cname_record = Record.objects.filter(
+                rfc2317_cname_record = Record(
                     name=cname_name,
                     type=RecordTypeChoices.CNAME,
                     zone=self.zone.rfc2317_parent_zone,
                     managed=True,
                     value=self.fqdn,
-                ).first()
-
-                if rfc2317_cname_record is not None:
-                    rfc2317_cname_record.ttl = min_ttl(
-                        rfc2317_cname_record.rfc2317_ptr_records.exclude(pk=self.pk)
-                        .aggregate(Min("ttl"))
-                        .get("ttl__min"),
-                        self.ttl,
-                    )
-                    rfc2317_cname_record.save(
-                        update_fields=["ttl"], save_zone_serial=save_zone_serial
-                    )
-
-                else:
-                    rfc2317_cname_record = Record(
-                        name=cname_name,
-                        type=RecordTypeChoices.CNAME,
-                        zone=self.zone.rfc2317_parent_zone,
-                        managed=True,
-                        value=self.fqdn,
-                        ttl=self.ttl,
-                    )
-                    rfc2317_cname_record.save(save_zone_serial=save_zone_serial)
+                    ttl=self.ttl,
+                )
+                rfc2317_cname_record.save(save_zone_serial=save_zone_serial)
 
-                self.rfc2317_cname_record = rfc2317_cname_record
+            self.rfc2317_cname_record = rfc2317_cname_record
 
         else:
             if self.rfc2317_cname_record is not None:
                 self.rfc2317_cname_record.delete(save_zone_serial=save_zone_serial)
                 self.rfc2317_cname_record = None
 
     def validate_name(self):
@@ -454,14 +470,15 @@
             name = dns_name.from_text(self.name, origin=None)
             fqdn = dns_name.from_text(self.name, origin=zone)
 
             zone.to_unicode()
             name.to_unicode()
 
             self.name = name.relativize(zone).to_text()
+            self.fqdn = fqdn.to_text()
 
         except dns.exception.DNSException as exc:
             raise ValidationError(
                 {
                     "name": str(exc),
                 }
             )
@@ -721,28 +738,15 @@
 
         zone = self.zone
         if self.type != RecordTypeChoices.SOA and zone.soa_serial_auto:
             zone.update_serial(save_zone_serial=save_zone_serial)
 
     def delete(self, *args, save_zone_serial=True, **kwargs):
         if self.rfc2317_cname_record:
-            if self.rfc2317_cname_record.pk:
-                if self.rfc2317_cname_record.rfc2317_ptr_records.count() == 1:
-                    self.rfc2317_cname_record.delete()
-                else:
-                    self.rfc2317_cname_record.ttl = (
-                        self.rfc2317_cname_record.rfc2317_ptr_records.exclude(
-                            pk=self.pk
-                        )
-                        .aggregate(Min("ttl"))
-                        .get("ttl__min")
-                    )
-                    self.rfc2317_cname_record.save(
-                        update_fields=["ttl"], save_zone_serial=save_zone_serial
-                    )
+            self.remove_from_rfc2317_cname_record(save_zone_serial=save_zone_serial)
 
         if self.ptr_record:
             self.ptr_record.delete()
 
         super().delete(*args, **kwargs)
 
         zone = self.zone
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/view.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/models/zone.py` & `netbox_plugin_dns-0.22.8/netbox_dns/models/zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -734,14 +734,23 @@
             ):
                 for ip in IPAddress.objects.filter(
                     custom_field_data__ipaddress_dns_zone_id=self.pk
                 ):
                     ip.dns_name = f'{ip.custom_field_data["ipaddress_dns_record_name"]}.{self.name}'
                     ip.save(update_fields=["dns_name"])
 
+        if name_changed:
+            for _record in self.record_set.all():
+                _record.save(
+                    update_fields=["fqdn"],
+                    save_zone_serial=False,
+                    update_rrset_ttl=False,
+                    update_rfc2317_cname=False,
+                )
+
         self.save_soa_serial()
         self.update_soa_record()
 
     def delete(self, *args, **kwargs):
         with transaction.atomic():
             address_records = self.record_set.filter(
                 ptr_record__isnull=False
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/navigation.py` & `netbox_plugin_dns-0.22.8/netbox_dns/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/signals/ipam_coupling.py` & `netbox_plugin_dns-0.22.8/netbox_dns/signals/ipam_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/tables/contact.py` & `netbox_plugin_dns-0.22.8/netbox_dns/tables/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/tables/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/tables/record.py` & `netbox_plugin_dns-0.22.8/netbox_dns/tables/record.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,32 +57,32 @@
         linkify=True,
     )
 
     class Meta(NetBoxTable.Meta):
         model = Record
         fields = (
             "pk",
-            "zone",
             "name",
+            "zone",
             "ttl",
             "type",
             "value",
             "unicode_value",
             "status",
             "disable_ptr",
             "ptr_record",
             "tags",
             "active",
             "description",
             "tenant",
             "tenant_group",
         )
         default_columns = (
-            "zone",
             "name",
+            "zone",
             "ttl",
             "type",
             "value",
             "tags",
             "active",
         )
 
@@ -97,27 +97,27 @@
         linkify=True,
     )
     actions = ActionsColumn(actions=("changelog",))
 
     class Meta(NetBoxTable.Meta):
         model = Record
         fields = (
-            "zone",
             "name",
+            "zone",
             "ttl",
             "type",
             "value",
             "unicode_value",
             "address_record",
             "ipam_ip_address",
             "active",
         )
         default_columns = (
-            "zone",
             "name",
+            "zone",
             "ttl",
             "type",
             "value",
             "active",
         )
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/tables/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/tables/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/tables/zone.py` & `netbox_plugin_dns-0.22.8/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/template_content.py` & `netbox_plugin_dns-0.22.8/netbox_dns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/contact.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/contact.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/record/related.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/related.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/registrar.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/registrar.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/related_dns_objects.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/related_dns_objects.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/view.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/managed_record.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/managed_record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/registration.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/registration.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/urls.py` & `netbox_plugin_dns-0.22.8/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/utilities/__init__.py` & `netbox_plugin_dns-0.22.8/netbox_dns/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/utilities/ipam_coupling.py` & `netbox_plugin_dns-0.22.8/netbox_dns/utilities/ipam_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/validators/dns_name.py` & `netbox_plugin_dns-0.22.8/netbox_dns/validators/dns_name.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/contact.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/record.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class RecordView(generic.ObjectView):
     queryset = Record.objects.all().prefetch_related("zone", "ptr_record")
 
     def get_value_records(self, instance):
         value_fqdn = dns_name.from_text(instance.value_fqdn)
         value_zone_names = [
             value_fqdn.split(length)[1].to_text().rstrip(".")
-            for length in range(2, len(value_fqdn))
+            for length in range(2, len(value_fqdn) + 1)
         ]
 
         value_zone = (
             Zone.objects.filter(instance.zone.view_filter, name__in=value_zone_names)
             .order_by(Length("name").desc())
             .first()
         )
@@ -76,15 +76,15 @@
                 view_filter, value=instance.fqdn, type=RecordTypeChoices.CNAME
             )
         )
 
         fqdn = dns_name.from_text(instance.fqdn)
         parent_zone_names = [
             fqdn.split(length)[1].to_text().rstrip(".")
-            for length in range(1, len(fqdn))
+            for length in range(1, len(fqdn) + 1)
         ]
 
         parent_zones = Zone.objects.filter(
             instance.zone.view_filter, name__in=parent_zone_names
         )
 
         for parent_zone in parent_zones:
```

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/registrar.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/view.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/netbox_dns/views/zone.py` & `netbox_plugin_dns-0.22.8/netbox_dns/views/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.6/pyproject.toml` & `netbox_plugin_dns-0.22.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-plugin-dns"
-version = "0.22.6"
+version = "0.22.8"
 description = "NetBox DNS is a NetBox plugin for managing DNS data."
 authors = ["Peter Eckel <pete@netbox-dns.org>"]
 homepage = "https://github.com/peteeckel/netbox-plugin-dns"
 repository = "https://github.com/peteeckel/netbox-plugin-dns"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_dns"}]
```

### Comparing `netbox_plugin_dns-0.22.6/PKG-INFO` & `netbox_plugin_dns-0.22.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-dns
-Version: 0.22.6
+Version: 0.22.8
 Summary: NetBox DNS is a NetBox plugin for managing DNS data.
 Home-page: https://github.com/peteeckel/netbox-plugin-dns
 License: MIT
 Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel
 Author-email: pete@netbox-dns.org
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.22.6 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.22.8 Summary: NetBox
 DNS is a NetBox plugin for managing DNS data. Home-page: https://github.com/
 peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel Author-email: pete@netbox-dns.org Requires-Python:
 >=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

