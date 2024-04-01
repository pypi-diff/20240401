# Comparing `tmp/keystone_api-0.3.1.tar.gz` & `tmp/keystone_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.1.tar", max compression
+gzip compressed data, was "keystone_api-0.3.2.tar", max compression
```

## Comparing `keystone_api-0.3.1.tar` & `keystone_api-0.3.2.tar`

### file list

```diff
@@ -1,105 +1,110 @@
--rw-r--r--   0        0        0    12621 2024-03-26 20:06:12.537990 keystone_api-0.3.1/README.md
--rw-r--r--   0        0        0      428 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     3500 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/tests/__init__.py
--rw-r--r--   0        0        0      625 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/admin_utils/tests/test_managment.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     4723 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1777 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4711 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      346 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/docs/__init__.py
--rw-r--r--   0        0        0      337 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/docs/urls.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     1344 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1747 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1469 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0      868 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0      278 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0      949 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1518 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1758 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1661 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0      868 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      296 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0      804 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      128 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0     1029 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0      487 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1399 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2302 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      884 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      817 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     1966 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-03-26 20:06:12.537990 keystone_api-0.3.1/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1252 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     8095 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1002 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/main/wsgi.py
--rw-r--r--   0        0        0      442 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     5642 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3015 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3102 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0     2981 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2013 2024-03-26 20:06:12.541990 keystone_api-0.3.1/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      959 2024-03-26 20:06:31.462076 keystone_api-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    13824 1970-01-01 00:00:00.000000 keystone_api-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-04-01 21:46:47.669141 keystone_api-0.3.2/README.md
+-rw-r--r--   0        0        0      428 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3479 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/test_managment.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     4837 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     4324 2024-04-01 21:46:47.669141 keystone_api-0.3.2/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      346 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/docs/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/docs/urls.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/tests/test_views.py
+-rw-r--r--   0        0        0      244 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     2066 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     1344 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1759 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1469 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0      868 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      709 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0      278 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0      949 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1758 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0      868 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      296 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0      804 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0     1096 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2370 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2102 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     7768 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1002 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3015 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     3102 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0        0 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2014 2024-04-01 21:46:47.673141 keystone_api-0.3.2/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      958 2024-04-01 21:47:02.201265 keystone_api-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14780 1970-01-01 00:00:00.000000 keystone_api-0.3.2/PKG-INFO
```

### Comparing `keystone_api-0.3.1/README.md` & `keystone_api-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,32 @@
 If the installation was successful, the packaged CLI tool will be available in your working environment.
 Use the `--help` option to view the available commands.
 
 ```bash
 keystone-api --help
 ```
 
-The following example will setup the project database, create an admin user account, and launch the
+The following example will set up the project database, create an admin user account, and launch the
 API server in debug mode. As a general rule, debug mode should **never** be enabled in production.
 
 ```bash
 keystone-api migrate
 keystone-api createsuperuser
 DEBUG=true keystone-api runserver
 ```
 
+#### Enabling Autocomplete
+
+The `keystone-api` utility does not support tab autocompletion by default.
+To enable this feature, use the `enable_autocomplete` command:
+
+```bash
+keystone-api enable_autocomplete
+```
+
 ## Settings
 
 Application settings are configurable as environmental variables.
 Individual settings are listed below by category and use case.
 
 ### Security
 
@@ -203,27 +212,39 @@
 
 Running the application in debug mode enables/disables various features to aid in the development process.
 In addition to enabling the standard debugging behavior provided by Django:
 
 - A `/docs` page is enabled with full API documentation for the parent application
 - Tracebacks are provided in the browser when an exception occurs (a Django standard)
 
+### Admin Utilities
+
+The `keystone-api` utility includes a series of admin utilities.
+These utilities are useful for automating various development tasks.
+A brief summary is provided below.
+Use the `keystone-api <command> --help` option for specific usage information.
+
+| Command                   | Description                                                                              |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `clean`                   | Clean up files generated when launching a new application instance.                      |
+| `quickstart`              | A helper utility for quickly migrating/deploying an application instance.                |
+
 ### Tests and System Checks
 
 Application tests are run using the `test` command:
 
 ```bash
 keystone-api test
 ```
 
 Specific subsets of tests are run by specifying an app label.
-For example, tests for the `admin_utils` application are executed as:
+For example, tests for the `users` application are executed as:
 
 ```bash
-keystone-api test apps.admin_utils
+keystone-api test apps.users
 ```
 
 The default django system checks can also be executed as standard:
 
 ```bash
 keystone-api check                   # Check for system configuration errors
 keystone-api makemigrations --check  # Check for missing database migrations
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.2/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 from argparse import ArgumentParser
 
 from django.core.management import call_command
 from django.core.management.base import BaseCommand
 
 
 class Command(BaseCommand):
-    """A helper utility that wraps other common Django commands for easier development"""
+    """A helper utility for quickly migrating/deploying an application instance."""
 
-    help = 'A helper utility that wraps other common Django commands for easier development'
+    help = __doc__
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         """Add command-line arguments to the parser
 
         Args:
           parser: The argument parser instance
         """
 
-        parser.add_argument('--static', action='store_true', help='Collect static files.')
-        parser.add_argument('--migrate', action='store_true', help='Run database migrations.')
-        parser.add_argument('--celery', action='store_true', help='Launch a background Celery worker.')
-        parser.add_argument('--gunicorn', action='store_true', help='Run a web server using Gunicorn.')
-        parser.add_argument('--no-input', action='store_false', help='Do not prompt for user input of any kind.')
+        group = parser.add_argument_group('quickstart options')
+        group.add_argument('--static', action='store_true', help='Collect static files.')
+        group.add_argument('--migrate', action='store_true', help='Run database migrations.')
+        group.add_argument('--celery', action='store_true', help='Launch a background Celery worker.')
+        group.add_argument('--gunicorn', action='store_true', help='Run a web server using Gunicorn.')
+        group.add_argument('--no-input', action='store_false', help='Do not prompt for user input of any kind.')
 
     def handle(self, *args, **options) -> None:
         """Handle the command execution
 
         Args:
           *args: Additional positional arguments
           **options: Additional keyword arguments
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/admin_utils/tests/test_managment.py` & `keystone_api-0.3.2/keystone_api/apps/admin_utils/tests/test_managment.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         return f'{self.cluster} allocation for {self.request.group}'
 
 
 class AllocationRequest(RGModelInterface, models.Model):
     """User request for additional service units on one or more clusters"""
 
     class StatusChoices(models.TextChoices):
+        """Enumerated choices for the `status` field"""
+
         PENDING = 'PD', 'Pending'
         APPROVED = 'AP', 'Approved'
         DECLINED = 'DC', 'Declined'
         CHANGES = 'CR', 'Changes Requested'
 
     title = models.CharField(max_length=250)
     description = models.TextField(max_length=1600)
@@ -88,14 +90,16 @@
         return truncatechars(self.title, 100)
 
 
 class AllocationRequestReview(RGModelInterface, models.Model):
     """Reviewer feedback for an allocation request"""
 
     class StatusChoices(models.TextChoices):
+        """Enumerated choices for the `status` field"""
+
         APPROVED = 'AP', 'Approved'
         DECLINED = 'DC', 'Declined'
         CHANGES = 'CR', 'Changes Requested'
 
     status = models.CharField(max_length=2, choices=StatusChoices.choices)
     public_comments = models.TextField(max_length=1600, null=True, blank=True)
     private_comments = models.TextField(max_length=1600, null=True, blank=True)
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,30 +19,36 @@
 ]
 
 
 class AllocationSerializer(serializers.ModelSerializer):
     """Object serializer for the `Allocation` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = Allocation
         fields = '__all__'
 
 
 class AllocationRequestSerializer(serializers.ModelSerializer):
     """Object serializer for the `AllocationRequest` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = AllocationRequest
         fields = '__all__'
 
 
 class AllocationRequestReviewSerializer(serializers.ModelSerializer):
     """Object serializer for the `AllocationRequestReview` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = AllocationRequestReview
         fields = '__all__'
         extra_kwargs = {'reviewer': {'required': False}}  # Default reviewer value is set by the view class
 
     def validate_reviewer(self, value: User) -> User:
         """Validate the reviewer matches the user submitting the request"""
 
@@ -52,9 +58,11 @@
         return value
 
 
 class ClusterSerializer(serializers.ModelSerializer):
     """Object serializer for the `Cluster` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = Cluster
         fields = '__all__'
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,84 +17,83 @@
 from keystone_api.plugins.slurm import get_cluster_limit, get_cluster_usage, get_slurm_account_names, set_cluster_limit
 
 log = logging.getLogger(__name__)
 
 
 @shared_task()
 def update_limits() -> None:
-    """Adjust per Slurm account TRES billing hours usage limits on all enabled clusters"""
-    log.info(f"Begin updating TRES billing hour limits for all Slurm Accounts")
+    """Adjust TRES billing limits for all Slurm accounts on all enabled clusters"""
 
+    log.info(f"Begin updating TRES billing hour limits for all Slurm Accounts")
     for cluster in Cluster.objects.filter(enabled=True).all():
         log.info(f"Updating TRES billing hour limits for cluster {cluster.name}")
         update_limits_for_cluster(cluster)
 
 
 @shared_task()
 def update_limits_for_cluster(cluster: Cluster) -> None:
-    """Update the TRES billing usage limits of each account on a given cluster, excluding the root account"""
+    """Adjust TRES billing limits for all Slurm accounts on a given Slurm cluster
+
+    The account `root` is automatically ignored.
+
+    Args:
+        cluster: The name of the Slurm cluster
+    """
 
     for account_name in get_slurm_account_names(cluster.name):
-        # Do not adjust limits for root
         if account_name in ['root']:
             continue
-        log.info(f"Updating TRES billing hour limits for account {account_name}")
+
+        log.debug(f"Updating TRES billing hour limits for account {account_name}")
         update_limit_for_account(account_name, cluster)
 
 
 @shared_task()
 def update_limit_for_account(account_name: str, cluster: Cluster) -> None:
     """Update the TRES billing usage limits for an individual Slurm account, closing out any expired allocations"""
 
-    # Check that the Slurm account has an entry in the keystone database
     try:
+        # Check the Slurm account has a database entry
         account = ResearchGroup.objects.get(name=account_name)
+
     except ResearchGroup.DoesNotExist:
-        #  Set the usage limit to the current usage (lock on this cluster) and continue
+        #  Lock the missing user by setting their usage limit to their current usage
         log.warning(f"No existing ResearchGroup for account {account_name}, locking {account_name} on {cluster.name}")
         set_cluster_limit(account_name, cluster.name, get_cluster_usage(account_name, cluster.name))
         return
 
-    # Base query for approved Allocations under the account on this cluster
+    # Base query for approved Allocations under the given account on the given cluster
     acct_alloc_query = Allocation.objects.filter(request__group=account, cluster=cluster, request__status='AP')
 
-    # Filter on the base query for allocations that have expired but do not have a final usage value
-    # (still contributing to current limit as active SUs instead of historical usage)
-    closing_query = acct_alloc_query.filter(final=None, request__expire__lte=date.today()) \
-                                    .order_by("request__expire")
-
-    # Filter account's allocations to those that are active, and determine their total service unit contribution
-    active_sus = acct_alloc_query.filter(request__active__lte=date.today(), request__expire__gt=date.today()) \
-                                 .aggregate(Sum("awarded"))['awarded__sum'] or 0
+    # Query for allocations that have expired but do not have a final usage value
+    closing_query = acct_alloc_query \
+        .filter(final=None, request__expire__lte=date.today()) \
+        .order_by("request__expire")
+
+    # Query for allocations that are active, and determine their total service unit contribution
+    active_sus = acct_alloc_query \
+        .filter(request__active__lte=date.today(), request__expire__gt=date.today()) \
+        .aggregate(Sum("awarded"))['awarded__sum'] or 0
 
-    # Determine usage that can be covered:
-    # total usage on the cluster (from slurm) - historical usage (current limit from slurm - active SUs - closing SUs)
+    # Calculate the total usage to count against expiring allocations and close them
     closing_sus = closing_query.aggregate(Sum("awarded"))['awarded__sum'] or 0
-
     historical_usage_from_limit = get_cluster_limit(account.name, cluster.name) - active_sus - closing_sus
     current_usage = get_cluster_usage(account.name, cluster.name) - historical_usage_from_limit
-
     close_expired_allocations(closing_query.all(), current_usage)
 
-    # Gather the updated historical usage from expired allocations (including any newly expired allocations)
+    # Set the new account usage limit using the updated historical usage from expired allocations
     updated_historical_usage = acct_alloc_query.filter(request__expire__lte=date.today()).aggregate(Sum("final"))['final__sum'] or 0
-
-    # Set the new limit to the calculated limit
     set_cluster_limit(account_name, cluster.name, limit=updated_historical_usage + active_sus)
 
 
 def close_expired_allocations(closing_allocations: Collection[Allocation], current_usage: int) -> None:
-    """Set the final usage for expired allocations that have not yet been closed out
+    """Set the final usage for expired allocations that have not been closed out yet
 
     Args:
-        closing_allocations: list of Allocations to set final usage for
-        current_usage: TRES billing hour usage to apply to allocations being closed out
+        closing_allocations: list of `Allocation` objects to set the final usage for
+        current_usage: The total TRES billing hour usage to apply across all allocations being closed out
     """
 
     for allocation in closing_allocations:
         log.debug(f"Closing allocation {allocation.id}")
-
-        # Set the final usage for the expired allocation
         allocation.final = min(current_usage, allocation.awarded)
-
-        # Update the usage needing to be covered, so it is not double counted (can only ever be >= 0)
         current_usage -= allocation.final
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.2/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/health/tests/test_views.py` & `keystone_api-0.3.2/keystone_api/apps/health/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/health/views.py` & `keystone_api-0.3.2/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.2/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.2/keystone_api/apps/logging/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
         if not request.user.is_anonymous:
             request_log.user = request.user
 
         request_log.save()
         return response
 
-    def get_client_ip(self, request: HttpRequest) -> str:
+    @staticmethod
+    def get_client_ip(request: HttpRequest) -> str:
         """Return the client IP for the incoming request
 
         Args:
             request: The incoming HTTP request
 
         Return:
             The requesting IP address
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.2/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/models.py` & `keystone_api-0.3.2/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.2/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.2/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/logging/views.py` & `keystone_api-0.3.2/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.2/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.2/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.2/keystone_api/apps/research_products/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.2/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.2/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.2/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/admin.py` & `keystone_api-0.3.2/keystone_api/apps/users/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,29 +20,24 @@
 ])
 
 
 @admin.register(User)
 class UserAdmin(auth.admin.UserAdmin):
     """Admin interface for managing user accounts"""
 
-    readonly_fields = ("last_login", "date_joined")
+    readonly_fields = ("last_login", "date_joined", "is_ldap_user")
     fieldsets = (
-        (None, {"fields": ("username", "password")}),
-        ("Personal info", {"fields": ("first_name", "last_name", "email")}),
-        (
-            "Permissions",
-            {
-                "fields": (
-                    "is_active",
-                    "is_staff",
-                    "is_superuser",
-                ),
-            },
-        ),
-        ("Important dates", {"fields": ("last_login", "date_joined")}),
+        ("User Info", {"fields": ("first_name", "last_name", "email", "last_login", "date_joined", 'is_ldap_user')}),
+        ("Credentials", {"fields": ("username", "password")}),
+        ("Permissions",
+         {"fields": (
+             "is_active",
+             "is_staff",
+             "is_superuser",
+         )})
     )
 
 
 @admin.register(ResearchGroup)
 class ResearchGroupAdmin(admin.ModelAdmin):
     """Admin interface for managing research group delegates"""
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.2/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/managers.py` & `keystone_api-0.3.2/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.2/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/models.py` & `keystone_api-0.3.2/keystone_api/apps/users/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     last_name = models.CharField('last name', max_length=150)
     email = models.EmailField('email address')
 
     is_active = models.BooleanField(default=True)
     is_staff = models.BooleanField('staff status', default=False)
     date_joined = models.DateTimeField('date joined', default=timezone.now)
 
+    is_ldap_user = models.BooleanField('LDAP User', default=False)
+
     objects = UserManager()
 
     USERNAME_FIELD = 'username'
     EMAIL_FIELD = "email"
     REQUIRED_FIELDS = ['email', 'first_name', 'last_name']
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.2/keystone_api/apps/users/permissions.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
     def has_permission(self, request, view) -> bool:
         """Return whether the request has permissions to access the requested resource"""
 
         if request.method in permissions.SAFE_METHODS:
             return request.user.is_authenticated
 
-        return request.user.is_staff
+        return request.user.is_staff or request.user.is_superuser
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.2/keystone_api/apps/users/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 ]
 
 
 class ResearchGroupSerializer(serializers.ModelSerializer):
     """Object serializer for the `ResearchGroup` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = ResearchGroup
         fields = '__all__'
 
 
 class UserSerializer(serializers.ModelSerializer):
     """Object serializer for the `User` class"""
 
     class Meta:
+        """Serializer settings"""
+
         model = User
         exclude = ['password']
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.2/keystone_api/apps/users/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def ldap_update_users(prune=False) -> None:
     """Update the user database with the latest data from LDAP
 
     This function performs no action if the `AUTH_LDAP_SERVER_URI` setting
     is not configured in the application settings.
 
     Args:
-        prune: Optionally delete any accounts with usernames not found in LDAP
+        prune: Optionally delete old LDAP accounts with usernames no longer found in LDAP
     """
 
     if not settings.AUTH_LDAP_SERVER_URI:
         return
 
     # Search LDAP for all users
     conn = get_ldap_connection()
@@ -48,12 +48,15 @@
 
     # Fetch keystone usernames using the LDAP attribute map defined in settings
     ldap_username_attr = settings.AUTH_LDAP_USER_ATTR_MAP.get('username', 'uid')
     ldap_names = {uid.decode() for result in search for uid in result[1][ldap_username_attr]}
 
     for username in tqdm(ldap_names):
         LDAPBackend().populate_user(username)
+        user = User.objects.get(username=username)
+        user.is_ldap_user = True
+        user.save()
 
     if prune:
-        usernames = set(User.objects.values_list('username', flat=True))
+        usernames = set(User.objects.filter(is_ldap=True).values_list('username', flat=True))
         users_to_delete = usernames - ldap_names
         User.objects.filter(username__in=users_to_delete).delete()
```

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.2/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.2/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.2/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/apps/users/views.py` & `keystone_api-0.3.2/keystone_api/apps/users/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 __all__ = [
     'ResearchGroupViewSet',
     'UserViewSet',
 ]
 
 
 class ResearchGroupViewSet(viewsets.ModelViewSet):
-    """View ResearchGroups"""
+    """Manage user membership in research groups"""
 
     permission_classes = [permissions.IsAuthenticated, StaffWriteAuthenticatedRead]
     serializer_class = ResearchGroupSerializer
     filterset_fields = '__all__'
 
     def get_queryset(self) -> list[ResearchGroup]:
         """Return a list of all research groups to admins, or the requesting users research groups"""
@@ -29,12 +29,13 @@
         if self.request.user.is_superuser or self.request.user.is_staff:
             return ResearchGroup.objects.all()
 
         return ResearchGroup.objects.groups_for_user(self.request.user)
 
 
 class UserViewSet(viewsets.ModelViewSet):
-    """View Users"""
+    """Read only access to user datta."""
 
+    queryset = User.objects.all()
     permission_classes = [permissions.IsAuthenticated, StaffWriteAuthenticatedRead]
     serializer_class = UserSerializer
     filterset_fields = '__all__'
```

### Comparing `keystone_api-0.3.1/keystone_api/main/settings.py` & `keystone_api-0.3.2/keystone_api/main/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import importlib.metadata
 import os
 import sys
 from datetime import timedelta
 from pathlib import Path
 
 import environ
-from celery.schedules import crontab
 from django.core.management.utils import get_random_secret_key
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 sys.path.insert(0, str(BASE_DIR))
 
 # Application metadata
 
@@ -162,28 +161,18 @@
 
 _redis_host = env.url('REDIS_HOST', '127.0.0.1').geturl()
 _redis_port = env.int('REDIS_PORT', 6379)
 _redis_db = env.int('REDIS_DB', 0)
 _redis_pass = env.str('REDIS_PASSWORD', '')
 
 REDIS_URL = f'redis://:{_redis_pass}@{_redis_host}:{_redis_port}'
-CELERY_BROKER_URL = REDIS_URL + f'/{_redis_db}'
 
+CELERY_BROKER_URL = REDIS_URL + f'/{_redis_db}'
 CELERY_RESULT_BACKEND = 'django-db'
 CELERY_CACHE_BACKEND = 'django-cache'
-CELERY_BEAT_SCHEDULE = {
-    "Update LDAP users": {
-        "task": "apps.users.tasks.ldap_update",
-        "schedule": crontab(minute='0'),
-    },
-    "Rotate Log Entries": {
-        "task": "apps.logging.tasks.rotate_log_files",
-        "schedule": crontab(hour='0', minute='0'),
-    }
-}
 
 # Database
 
 DATABASES = dict()
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 _db_name = env.str('DB_NAME', 'keystone')
```

### Comparing `keystone_api-0.3.1/keystone_api/main/urls.py` & `keystone_api-0.3.2/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/plugins/slurm.py` & `keystone_api-0.3.2/keystone_api/plugins/slurm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Plugin for providing command line functionality to a Slurm installation"""
+"""Plugin providing wrappers around command line calls to a local Slurm installation"""
 
 import logging
 import re
 from shlex import split
 from subprocess import PIPE, Popen
 
 log = logging.getLogger(__name__)
@@ -11,44 +11,43 @@
 def subprocess_call(args: list[str]) -> str:
     """Wrapper method for executing shell commands via ``Popen.communicate``
 
     Args:
         args: A sequence of program arguments
 
     Returns:
-        The piped output to STDOUT and STDERR as strings
+        The piped output to STDOUT
     """
 
     process = Popen(args, stdout=PIPE, stderr=PIPE)
     out, err = process.communicate()
 
     if process.returncode != 0:
         message = f"Error executing shell command: {' '.join(args)} \n {err.decode('utf-8').strip()}"
         log.error(message)
         raise RuntimeError(message)
 
     return out.decode("utf-8").strip()
 
 
 def get_slurm_account_names(cluster_name: str | None = None) -> set[str]:
-    """Gather a list of account names defined on either all clusters or a given cluster from `sacctmgr`
+    """Return a list of Slurm account names from `sacctmgr`
 
     Args:
-        cluster_name: Optionally provide the name of the cluster to get account names on
+        cluster_name: Optionally return account names on a specific Slurm cluster
 
     Returns:
-        A set of unique Slurm account name strings
+        A set of unique Slurm account names
     """
 
-    cmd = split(f"sacctmgr show -nP account withassoc where parents=root format=Account")
+    cmd = split("sacctmgr show -nP account withassoc where parents=root format=Account")
     if cluster_name:
         cmd.append(f"cluster={cluster_name}")
 
-    out = subprocess_call(cmd)
-    return set(out.split())
+    return set(subprocess_call(cmd).split())
 
 
 def get_slurm_account_principal_investigator(account_name: str) -> str:
     """Return the Principal Investigator (PI) username (Slurm account description field) for a Slurm account given the
     account name
 
     Args:
@@ -59,95 +58,89 @@
     """
 
     cmd = split(f"sacctmgr show -nP account where account={account_name} format=Descr")
     return subprocess_call(cmd)
 
 
 def get_slurm_account_users(account_name: str, cluster_name: str | None = None) -> set[str]:
-    """Return the usernames of users under a Slurm account given the account name
+    """Return all usernames tied to a Slurm account
 
     Args:
         account_name: The Slurm account name
         cluster_name: Optionally provide the name of the cluster to get usernames on
 
     Returns:
         The account PI username
     """
 
     cmd = split(f"sacctmgr show -nP association where account={account_name} format=user")
     if cluster_name:
         cmd.append(f"cluster={cluster_name}")
 
-    out = subprocess_call(cmd)
-    return set(out.split())
+    return set(subprocess_call(cmd).split())
 
 
-def set_cluster_limit(account_name: str, cluster_name: str, limit: int, in_hours: bool = True) -> None:
-    """Update the current TRES Billing usage limit to the provided limit on a given cluster for a given account
-    with sacctmgr. The default expected limit unit is Hours, and a conversion takes place as Slurm uses minutes.
+def set_cluster_limit(account_name: str, cluster_name: str, limit: int) -> None:
+    """Update the TRES Billing usage limit for a given Slurm account and cluster
+
+    The default expected limit unit is Hours, and a conversion takes place as Slurm uses minutes.
 
     Args:
-        account_name: The name of the account to get usage for
-        cluster_name: The name of the cluster to get usage on
-        limit: Number of billing TRES hours to set the usage limit to
-        in_hours: Boolean value for whether (True) or not (False) the limit provided is in Hours (Default: True)
+        account_name: The name of the Slurm account
+        cluster_name: The name of the Slurm cluster
+        limit: The new TRES usage limit in hours
     """
 
-    # Convert the input hours to minutes
-    if in_hours:
-        limit *= 60
-
+    limit *= 60  # Convert the input hours to minutes
     cmd = split(f"sacctmgr modify -i account where account={account_name} cluster={cluster_name} set GrpTresMins=billing={limit}")
     subprocess_call(cmd)
 
 
-def get_cluster_limit(account_name: str, cluster_name: str, in_hours: bool = True) -> int:
-    """Get the current TRES Billing usage limit on a given cluster for a given account with sacctmgr.
+def get_cluster_limit(account_name: str, cluster_name: str) -> int:
+    """Return the current TRES Billing usage limit for a given Slurm account and cluster
+
     The limit unit coming out of Slurm is minutes, and the default behavior is to convert this to hours.
     This can be skipped with in_hours = False.
 
     Args:
-        account_name: The name of the account to get usage for
-        cluster_name: The name of the cluster to get usage on
-        in_hours: Boolean value for whether (True) or not (False) the returned limit is in Hours (Default: True)
+        account_name: The name of the Slurm account
+        cluster_name: The name of the Slurm cluster
 
     Returns:
-        An integer representing the total (historical + current) billing TRES limit
+        The current TRES Billing usage limit in hours
     """
 
     cmd = split(f"sacctmgr show -nP association where account={account_name} cluster={cluster_name} format=GrpTRESMins")
 
     try:
         limit = re.findall(r'billing=(.*)', subprocess_call(cmd))[0]
+
     except IndexError:
         log.debug(f"'billing' limit not found in command output from {cmd}, assuming zero for current limit")
         return 0
 
     limit = int(limit) if limit.isnumeric() else 0
-    return limit // 60 if in_hours else limit
+    return limit // 60  # convert from minutes to hours
 
 
-def get_cluster_usage(account_name: str, cluster_name: str, in_hours: bool = True) -> int:
-    """Get the total billable usage in Hours on a given cluster for a given account. Slurm provides a usage in minutes
-    and that values is converted to Hours by default. This can be skipped with in_hours = False.
+def get_cluster_usage(account_name: str, cluster_name: str) -> int:
+    """Return the total billable usage in hours for a given Slurm account
 
     Args:
         account_name: The name of the account to get usage for
         cluster_name: The name of the cluster to get usage on
-        in_hours: Boolean value for whether (True) or not (False) the returned Usage is in hours (Default: True)
 
     Returns:
         An integer representing the total (historical + current) billing TRES hours usage from sshare
     """
 
     cmd = split(f"sshare -nP -A {account_name} -M {cluster_name} --format=GrpTRESRaw")
 
     try:
         usage = re.findall(r'billing=(.*),fs', subprocess_call(cmd))[0]
+
     except IndexError:
         log.debug(f"'billing' usage not found in command output from {cmd}, assuming zero for current usage")
         return 0
 
     usage = int(usage) if usage.isnumeric() else 0
-
-    # Billing TRES comes out of Slurm in minutes, needs to be converted to hours
-    return usage // 60 if in_hours else usage
+    return usage // 60  # convert from minutes to hours
```

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.2/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.2/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/health/test.py` & `keystone_api-0.3.2/keystone_api/tests/health/test.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.2/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.2/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.2/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.2/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.2/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.1/keystone_api/tests/utils.py` & `keystone_api-0.3.2/keystone_api/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def assert_http_responses(self, endpoint: str, **kwargs) -> None:
         """Execute a series of API calls and assert the returned status matches the given values
 
         Args:
             endpoint: The URL to perform requests against
             **<request>: The integer status code expected by the given request type (get, post, etc.)
             **<request>_body: The data to include in the request (get_body, post_body, etc.)
-            **<request>_headers: Header vaues to include in the request (get_headers, post_headers, etc.)
+            **<request>_headers: Header values to include in the request (get_headers, post_headers, etc.)
         """
 
         http_methods = ['get', 'head', 'options', 'post', 'put', 'patch', 'delete', 'trace']
         for method in http_methods:
             expected_status = kwargs.get(method, None)
             http_method = getattr(self.client, method)
             http_args = self._build_request_args(method, kwargs)
```

### Comparing `keystone_api-0.3.1/pyproject.toml` & `keystone_api-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-django = "4.2.11"
-django-auth-ldap = "4.6.0"
+django = "5.0.3"
+django-auth-ldap = "4.7.0"
 django-celery-beat = "2.6.0"
 django-celery-results = "2.5.1"
 django-cors-headers = "^4.3.1"
 django-environ = "0.11.2"
-django-filter = "24.1"
+django-filter = "24.2"
 django-health-check = "3.18.1"
-django-jazzmin = "2.6.0"
-djangorestframework = "3.14.0"
+django-jazzmin = "2.6.1"
+djangorestframework = "3.15.1"
 djangorestframework-simplejwt = "5.3.1"
 drf_spectacular = { version = "0.27.1", extras = ["sidecar"] }
 gunicorn = "21.2.0"
 psycopg2-binary = "2.9.9"
 pyyaml = "6.0.1"
 redis = "5.0.3"
 tqdm = "4.66.2"
```

### Comparing `keystone_api-0.3.1/PKG-INFO` & `keystone_api-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: django (==4.2.11)
-Requires-Dist: django-auth-ldap (==4.6.0)
+Requires-Dist: django (==5.0.3)
+Requires-Dist: django-auth-ldap (==4.7.0)
 Requires-Dist: django-celery-beat (==2.6.0)
 Requires-Dist: django-celery-results (==2.5.1)
 Requires-Dist: django-cors-headers (>=4.3.1,<5.0.0)
 Requires-Dist: django-environ (==0.11.2)
-Requires-Dist: django-filter (==24.1)
+Requires-Dist: django-filter (==24.2)
 Requires-Dist: django-health-check (==3.18.1)
-Requires-Dist: django-jazzmin (==2.6.0)
-Requires-Dist: djangorestframework (==3.14.0)
+Requires-Dist: django-jazzmin (==2.6.1)
+Requires-Dist: djangorestframework (==3.15.1)
 Requires-Dist: djangorestframework-simplejwt (==5.3.1)
 Requires-Dist: drf_spectacular[sidecar] (==0.27.1)
 Requires-Dist: gunicorn (==21.2.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: redis (==5.0.3)
 Requires-Dist: tqdm (==4.66.2)
@@ -98,23 +98,32 @@
 If the installation was successful, the packaged CLI tool will be available in your working environment.
 Use the `--help` option to view the available commands.
 
 ```bash
 keystone-api --help
 ```
 
-The following example will setup the project database, create an admin user account, and launch the
+The following example will set up the project database, create an admin user account, and launch the
 API server in debug mode. As a general rule, debug mode should **never** be enabled in production.
 
 ```bash
 keystone-api migrate
 keystone-api createsuperuser
 DEBUG=true keystone-api runserver
 ```
 
+#### Enabling Autocomplete
+
+The `keystone-api` utility does not support tab autocompletion by default.
+To enable this feature, use the `enable_autocomplete` command:
+
+```bash
+keystone-api enable_autocomplete
+```
+
 ## Settings
 
 Application settings are configurable as environmental variables.
 Individual settings are listed below by category and use case.
 
 ### Security
 
@@ -234,27 +243,39 @@
 
 Running the application in debug mode enables/disables various features to aid in the development process.
 In addition to enabling the standard debugging behavior provided by Django:
 
 - A `/docs` page is enabled with full API documentation for the parent application
 - Tracebacks are provided in the browser when an exception occurs (a Django standard)
 
+### Admin Utilities
+
+The `keystone-api` utility includes a series of admin utilities.
+These utilities are useful for automating various development tasks.
+A brief summary is provided below.
+Use the `keystone-api <command> --help` option for specific usage information.
+
+| Command                   | Description                                                                              |
+|---------------------------|------------------------------------------------------------------------------------------|
+| `clean`                   | Clean up files generated when launching a new application instance.                      |
+| `quickstart`              | A helper utility for quickly migrating/deploying an application instance.                |
+
 ### Tests and System Checks
 
 Application tests are run using the `test` command:
 
 ```bash
 keystone-api test
 ```
 
 Specific subsets of tests are run by specifying an app label.
-For example, tests for the `admin_utils` application are executed as:
+For example, tests for the `users` application are executed as:
 
 ```bash
-keystone-api test apps.admin_utils
+keystone-api test apps.users
 ```
 
 The default django system checks can also be executed as standard:
 
 ```bash
 keystone-api check                   # Check for system configuration errors
 keystone-api makemigrations --check  # Check for missing database migrations
```

