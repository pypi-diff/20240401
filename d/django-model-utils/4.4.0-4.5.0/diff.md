# Comparing `tmp/django-model-utils-4.4.0.tar.gz` & `tmp/django-model-utils-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-utils-4.4.0.tar", last modified: Sat Feb 10 16:20:30 2024, max compression
+gzip compressed data, was "django-model-utils-4.5.0.tar", last modified: Mon Apr  1 19:06:55 2024, max compression
```

## Comparing `django-model-utils-4.4.0.tar` & `django-model-utils-4.5.0.tar`

### file list

```diff
@@ -1,119 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.099238 django-model-utils-4.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.099238 django-model-utils-4.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/django_model_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-10 16:20:30.000000 django-model-utils-4.4.0/django_model_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/managers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/setup.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/docs/utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.095238 django-model-utils-4.4.0/model_utils/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.091238 django-model-utils-4.4.0/model_utils/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.091238 django-model-utils-4.4.0/model_utils/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.091238 django-model-utils-4.4.0/model_utils/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.091238 django-model-utils-4.4.0/model_utils/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.091238 django-model-utils-4.4.0/model_utils/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.103238 django-model-utils-4.4.0/model_utils/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.095238 django-model-utils-4.4.0/model_utils/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.107238 django-model-utils-4.4.0/model_utils/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.095238 django-model-utils-4.4.0/model_utils/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.107238 django-model-utils-4.4.0/model_utils/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.095238 django-model-utils-4.4.0/model_utils/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.107238 django-model-utils-4.4.0/model_utils/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/model_utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.107238 django-model-utils-4.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.107238 django-model-utils-4.4.0/tests/test_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_field_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_monitor_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_split_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_status_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_urlsafe_token_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_fields/test_uuid_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_inheritance_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/tests/test_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23165 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/test_inheritance_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/test_join_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/test_query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/test_softdelete_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_managers/test_status_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:30.111238 django-model-utils-4.4.0/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_deferred_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_softdeletable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_timeframed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_timestamped_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tests/test_models/test_uuid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      870 2024-02-10 16:20:10.000000 django-model-utils-4.4.0/translations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/issue-manager.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/django_model_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/managers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.668269 django-model-utils-4.5.0/model_utils/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.668269 django-model-utils-4.5.0/model_utils/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/test_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35143 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_field_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_monitor_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_split_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_status_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_urlsafe_token_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_uuid_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_inheritance_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/test_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23165 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_inheritance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_join_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_softdelete_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_status_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_miscellaneous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_deferred_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_softdeletable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_timeframed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_timestamped_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_uuid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      870 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/translations.py
```

### Comparing `django-model-utils-4.4.0/.github/workflows/release.yml` & `django-model-utils-4.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/.github/workflows/test.yml` & `django-model-utils-4.5.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 name: Test
 
 on: [push, pull_request]
 
 env:
+  POSTGRES_USER: postgres
+  POSTGRES_PASSWORD: postgres
+  POSTGRES_DB: postgres
   FORCE_COLOR: 1
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12-dev']
 
     services:
       postgres:
-        image: postgres:12
+        image: postgres:13-alpine
         env:
-          POSTGRES_USER: postgres
-          POSTGRES_PASSWORD: postgres
-          POSTGRES_DB: postgres
+          POSTGRES_USER: ${{ env.POSTGRES_USER }}
+          POSTGRES_PASSWORD: ${{ env.POSTGRES_PASSWORD }}
+          POSTGRES_DB: ${{ env.POSTGRES_DB }}
         ports:
         - 5432:5432
         options: >-
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
@@ -56,17 +59,15 @@
         python -m pip install --upgrade pip
         python -m pip install --upgrade tox tox-gh-actions
 
     - name: Tox tests
       run: |
         tox -v -- --cov --cov-append --cov-report term-missing --cov-report xml
       env:
-        DB_NAME: postgres
-        DB_USER: postgres
-        DB_PASSWORD: postgres
-        DB_HOST: localhost
-        DB_PORT: 5432
+        POSTGRES_DB: ${{ env.POSTGRES_DB }}
+        POSTGRES_USER: ${{ env.POSTGRES_USER }}
+        POSTGRES_PASSWORD: ${{ env.POSTGRES_PASSWORD }}
 
     - name: Upload coverage
       uses: codecov/codecov-action@v3
       with:
         name: Python ${{ matrix.python-version }}
```

### Comparing `django-model-utils-4.4.0/AUTHORS.rst` & `django-model-utils-4.5.0/AUTHORS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 | Eugene Kuznetsov <atorich@gmail.com>
 | Felipe Prenholato <felipe.rafael@pdg.com.br>
 | Filipe Ximenes <filipeximenes@gmail.com>
 | Florian Alu <fla@grapps.fr>
 | Germano Massullo <github.com/Germano0>
 | Gregor Müllegger <gregor@muellegger.de>
 | Guilherme Devincenzi <github.com/gdevincenzi>
+| Guilherme Crocetti <github.com/gmcrocetti>
 | Hanley <hanley@wayup.com>
 | Hanley Hansen <hanleyhansen@gmail.com>
 | Harry Moreno <morenoh149@gmail.com>
 | Hasan Ramezani <hasan.r67@gmail.com>
 | Ivan Virabyan <i.virabyan@gmail.com>
 | JMP <josemarfyl@gmail.com>
 | Jack Cushman <jcushman@law.harvard.edu>
@@ -100,7 +101,8 @@
 | romgar <romain.garrigues.cs@gmail.com>
 | silonov <mike@silonov.pro>
 | smacker <max@smacker.ru>
 | zyegfryed <zyegfryed@gmail.com>
 | Éric Araujo <merwok@netwok.org>
 | Őry Máté <ory.mate@cloud.bme.hu>
 | Nafees Anwar <h.nafees.anwar@gmail.com>
+| meanmail <github@meanmail.dev>
```

### Comparing `django-model-utils-4.4.0/CHANGES.rst` & `django-model-utils-4.5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Changelog
 =========
 
+To be released
+--------------
+- Add deprecation warning for MonitorField. The default value will be `None`
+  instead of `django.utils.timezone.now` - when nullable and without a default.
+- Add Brazilian Portuguese translation (GH-#578)
+- Don't use `post_init` signal for initialize tracker
+
 4.4.0 (2024-02-10)
 ------------------
 
-- Add support for `Python 3.11` 
-- Add support for `Python 3.12`
-- Drop support for `Python 3.7`
+- Add support for `Python 3.11` (GH-#545)
+- Add support for `Python 3.12` (GH-#545)
+- Drop support for `Python 3.7` (GH-#545)
 - Add support for `Django 4.2`
 - Add support for `Django 5.0`
 - Remove ``SaveSignalHandlingModel``. This model used a modified copy of the internal Django method `Model.save_base()`
   and had not been updated for upstream bug fixes changes since its addition.
 - Add Swedish translation
-- Use proper column name instead of attname
+- Use proper column name instead of attname (GH-#573)
 - Fix ValueError when calling prefetch_related for tracked ForeignKey fields
 
 4.3.1 (2022-11-15)
 ------------------
 
 - Confirm support for `Django 4.0`
 - Add Spanish translation
```

### Comparing `django-model-utils-4.4.0/CODE_OF_CONDUCT.md` & `django-model-utils-4.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/CONTRIBUTING.rst` & `django-model-utils-4.5.0/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,26 @@
 
     pip install tox coverage
 
 To run tox and generate a coverage report (in ``htmlcov`` directory)::
 
     make test
 
+A database is required to run the tests. For convince there is a ``docker-compose.yml`` file for spinning up a
+database container. To start the database container run:
+
+    docker-compose up -d
+
+Another way to run the tests with a sqlite database is to export the `SQLITE` variable::
+
+    export SQLITE=1
+    make test
+    # or
+    SQLITE=1 python setup.py test
+
 **Please note**: Before a pull request can be merged, all tests must pass and
 code/branch coverage in tests must be 100%.
 
 Code Formatting
 ---------------
 We make use of `isort`_ to sort imports.
```

### Comparing `django-model-utils-4.4.0/LICENSE.txt` & `django-model-utils-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/Makefile` & `django-model-utils-4.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/PKG-INFO` & `django-model-utils-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-utils
-Version: 4.4.0
+Version: 4.5.0
 Summary: Django model mixins and utilities
 Home-page: https://github.com/jazzband/django-model-utils
 Author: Carl Meyer
 Author-email: carl@oddbird.net
 Maintainer: JazzBand
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
@@ -86,26 +86,33 @@
 .. _issue tracker: https://github.com/jazzband/django-model-utils/issues
 .. _CONTRIBUTING.rst: https://github.com/jazzband/django-model-utils/blob/master/CONTRIBUTING.rst
 
 
 Changelog
 =========
 
+To be released
+--------------
+- Add deprecation warning for MonitorField. The default value will be `None`
+  instead of `django.utils.timezone.now` - when nullable and without a default.
+- Add Brazilian Portuguese translation (GH-#578)
+- Don't use `post_init` signal for initialize tracker
+
 4.4.0 (2024-02-10)
 ------------------
 
-- Add support for `Python 3.11` 
-- Add support for `Python 3.12`
-- Drop support for `Python 3.7`
+- Add support for `Python 3.11` (GH-#545)
+- Add support for `Python 3.12` (GH-#545)
+- Drop support for `Python 3.7` (GH-#545)
 - Add support for `Django 4.2`
 - Add support for `Django 5.0`
 - Remove ``SaveSignalHandlingModel``. This model used a modified copy of the internal Django method `Model.save_base()`
   and had not been updated for upstream bug fixes changes since its addition.
 - Add Swedish translation
-- Use proper column name instead of attname
+- Use proper column name instead of attname (GH-#573)
 - Fix ValueError when calling prefetch_related for tracked ForeignKey fields
 
 4.3.1 (2022-11-15)
 ------------------
 
 - Confirm support for `Django 4.0`
 - Add Spanish translation
```

### Comparing `django-model-utils-4.4.0/README.rst` & `django-model-utils-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/django_model_utils.egg-info/PKG-INFO` & `django-model-utils-4.5.0/django_model_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-utils
-Version: 4.4.0
+Version: 4.5.0
 Summary: Django model mixins and utilities
 Home-page: https://github.com/jazzband/django-model-utils
 Author: Carl Meyer
 Author-email: carl@oddbird.net
 Maintainer: JazzBand
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
@@ -86,26 +86,33 @@
 .. _issue tracker: https://github.com/jazzband/django-model-utils/issues
 .. _CONTRIBUTING.rst: https://github.com/jazzband/django-model-utils/blob/master/CONTRIBUTING.rst
 
 
 Changelog
 =========
 
+To be released
+--------------
+- Add deprecation warning for MonitorField. The default value will be `None`
+  instead of `django.utils.timezone.now` - when nullable and without a default.
+- Add Brazilian Portuguese translation (GH-#578)
+- Don't use `post_init` signal for initialize tracker
+
 4.4.0 (2024-02-10)
 ------------------
 
-- Add support for `Python 3.11` 
-- Add support for `Python 3.12`
-- Drop support for `Python 3.7`
+- Add support for `Python 3.11` (GH-#545)
+- Add support for `Python 3.12` (GH-#545)
+- Drop support for `Python 3.7` (GH-#545)
 - Add support for `Django 4.2`
 - Add support for `Django 5.0`
 - Remove ``SaveSignalHandlingModel``. This model used a modified copy of the internal Django method `Model.save_base()`
   and had not been updated for upstream bug fixes changes since its addition.
 - Add Swedish translation
-- Use proper column name instead of attname
+- Use proper column name instead of attname (GH-#573)
 - Fix ValueError when calling prefetch_related for tracked ForeignKey fields
 
 4.3.1 (2022-11-15)
 ------------------
 
 - Confirm support for `Django 4.0`
 - Add Spanish translation
```

### Comparing `django-model-utils-4.4.0/django_model_utils.egg-info/SOURCES.txt` & `django-model-utils-4.5.0/django_model_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 CHANGES.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
+docker-compose.yml
 requirements-test.txt
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 translations.py
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
+.github/workflows/issue-manager.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 django_model_utils.egg-info/PKG-INFO
 django_model_utils.egg-info/SOURCES.txt
 django_model_utils.egg-info/dependency_links.txt
 django_model_utils.egg-info/not-zip-safe
 django_model_utils.egg-info/requires.txt
@@ -50,26 +52,27 @@
 model_utils/locale/de/LC_MESSAGES/django.po
 model_utils/locale/es/LC_MESSAGES/django.mo
 model_utils/locale/es/LC_MESSAGES/django.po
 model_utils/locale/fa/LC_MESSAGES/django.mo
 model_utils/locale/fa/LC_MESSAGES/django.po
 model_utils/locale/fr/LC_MESSAGES/django.mo
 model_utils/locale/fr/LC_MESSAGES/django.po
+model_utils/locale/pt_BR/LC_MESSAGES/django.mo
+model_utils/locale/pt_BR/LC_MESSAGES/django.po
 model_utils/locale/ru/LC_MESSAGES/django.mo
 model_utils/locale/ru/LC_MESSAGES/django.po
 model_utils/locale/sv/LC_MESSAGES/django.mo
 model_utils/locale/sv/LC_MESSAGES/django.po
 model_utils/locale/zh_Hans/LC_MESSAGES/django.mo
 model_utils/locale/zh_Hans/LC_MESSAGES/django.po
 tests/__init__.py
 tests/fields.py
 tests/managers.py
 tests/models.py
 tests/settings.py
-tests/signals.py
 tests/test_choices.py
 tests/test_inheritance_iterable.py
 tests/test_miscellaneous.py
 tests/test_fields/__init__.py
 tests/test_fields/test_field_tracker.py
 tests/test_fields/test_monitor_field.py
 tests/test_fields/test_split_field.py
```

### Comparing `django-model-utils-4.4.0/docs/Makefile` & `django-model-utils-4.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/conf.py` & `django-model-utils-4.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/fields.rst` & `django-model-utils-4.5.0/docs/fields.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/index.rst` & `django-model-utils-4.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/make.bat` & `django-model-utils-4.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/managers.rst` & `django-model-utils-4.5.0/docs/managers.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/docs/models.rst` & `django-model-utils-4.5.0/docs/models.rst`

 * *Files 10% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
 This abstract base class just provides a field ``is_removed`` which is
 set to True instead of removing the instance. Entities returned in
 manager ``available_objects`` are limited to not-deleted instances.
 
 Note that relying on the default ``objects`` manager to filter out not-deleted
 instances is deprecated. ``objects`` will include deleted objects in a future
-release.
-
+release. Until then, the recommended course of action is to use the manager
+``all_objects`` when you want to include all instances.
 
 UUIDModel
 ------------------
 
 This abstract base class provides ``id`` field on any model that inherits from it
 which will be the primary key.
```

### Comparing `django-model-utils-4.4.0/docs/utilities.rst` & `django-model-utils-4.5.0/docs/utilities.rst`

 * *Files 1% similar despite different names*

```diff
@@ -324,17 +324,17 @@
 
     instance = MyModel.objects.first()
     instance.name = 'new'
     instance.save(update_fields={'name'})
 
 This is how ``FieldTracker`` tracks field changes on ``instance.save`` call.
 
-1. In ``class_prepared`` handler ``FieldTracker`` patches ``save_base`` and
-   ``refresh_from_db`` methods to reset initial state for tracked fields.
-2. In ``post_init`` handler ``FieldTracker`` saves initial values for tracked
+1. In ``class_prepared`` handler ``FieldTracker`` patches ``save_base``,
+   ``refresh_from_db`` and ``__init__`` methods to reset initial state for tracked fields.
+2. In the patched ``__init__`` method ``FieldTracker`` saves initial values for tracked
    fields.
 3. ``MyModel.save`` changes ``update_fields`` in order to store auto updated
    ``modified`` timestamp. Complete list of saved fields is now known.
 4. ``Model.save`` does nothing interesting except calling ``save_base``.
 5. Decorated ``save_base()`` method calls ``super().save_base`` and all fields
    that have values different to initial are considered as changed.
 6. ``Model.save_base`` sends ``pre_save`` signal, saves instance to database and
```

### Comparing `django-model-utils-4.4.0/model_utils/choices.py` & `django-model-utils-4.5.0/model_utils/choices.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/model_utils/fields.py` & `django-model-utils-4.5.0/model_utils/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import secrets
 import uuid
+import warnings
 from collections.abc import Callable
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.timezone import now
 
@@ -103,14 +104,24 @@
     A DateTimeField that monitors another field on the same model and
     sets itself to the current date/time whenever the monitored field
     changes.
 
     """
 
     def __init__(self, *args, **kwargs):
+        if kwargs.get("null") and kwargs.get("default") is None:
+            warning_message = (
+                "{}.default is set to 'django.utils.timezone.now' - when nullable"
+                " and no default. This behavior will be deprecated in the next"
+                " major release in favor of 'None'. See"
+                " https://django-model-utils.readthedocs.io/en/stable/fields.html"
+                "#monitorfield for more information."
+            ).format(self.__class__.__name__)
+            warnings.warn(warning_message, DeprecationWarning)
+
         kwargs.setdefault('default', now)
         monitor = kwargs.pop('monitor', None)
         if not monitor:
             raise TypeError(
                 '%s requires a "monitor" argument' % self.__class__.__name__)
         self.monitor = monitor
         when = kwargs.pop('when', None)
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/cs/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-05-04 13:40+0200\n"
 "PO-Revision-Date: 2018-05-04 13:46+0200\n"
+"Last-Translator: Václav Dohnal <vaclav.dohnal@gmail.com>\n"
+"Language-Team: N/A\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"Last-Translator: Václav Dohnal <vaclav.dohnal@gmail.com>\n"
-"Language-Team: \n"
 "X-Generator: Poedit 2.0.7\n"
 
 msgid "created"
 msgstr "vytvořeno"
 
 msgid "end"
 msgstr "konec"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/cs/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 # Translators:
 # ------------
 # Václav Dohnal <vaclav.dohnal@gmail.com>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
-"Report-Msgid-Bugs-To: https://github.com/jazzband/django-model-utils/issues\n"
-"POT-Creation-Date: 2018-05-04 13:40+0200\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: 2018-05-04 13:46+0200\n"
+"Last-Translator: Václav Dohnal <vaclav.dohnal@gmail.com>\n"
+"Language-Team: N/A\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"Last-Translator: Václav Dohnal <vaclav.dohnal@gmail.com>\n"
-"Language-Team: N/A\n"
 "X-Generator: Poedit 2.0.7\n"
 
-#: .\models.py:24
+#: models.py:24
 msgid "created"
 msgstr "vytvořeno"
 
-#: .\models.py:25
+#: models.py:25
 msgid "modified"
 msgstr "upraveno"
 
-#: .\models.py:37
+#: models.py:49
 msgid "start"
 msgstr "začátek"
 
-#: .\models.py:38
+#: models.py:50
 msgid "end"
 msgstr "konec"
 
-#: .\models.py:53
+#: models.py:65
 msgid "status"
 msgstr "stav"
 
-#: .\models.py:54
+#: models.py:66
 msgid "status changed"
 msgstr "změna stavu"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/de/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,52 +2,49 @@
 #
 # Translators:
 # Philipp Steinhardt <steinhardt@myvision.de>, 2015.
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2015-07-20 10:17-0600\n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: 2015-07-01 10:12+0200\n"
 "Last-Translator: Philipp Steinhardt <steinhardt@myvision.de>\n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: models.py:20
+#: models.py:24
 msgid "created"
 msgstr "erstellt"
 
-#: models.py:21
+#: models.py:25
 msgid "modified"
 msgstr "bearbeitet"
 
-#: models.py:33
+#: models.py:49
 msgid "start"
 msgstr "Beginn"
 
-#: models.py:34
+#: models.py:50
 msgid "end"
 msgstr "Ende"
 
-#: models.py:49
+#: models.py:65
 msgid "status"
 msgstr "Status"
 
-#: models.py:50
+#: models.py:66
 msgid "status changed"
 msgstr "Status geändert"
 
-#: tests/models.py:106 tests/models.py:115 tests/models.py:124
-msgid "active"
-msgstr "aktiv"
-
-#: tests/models.py:107 tests/models.py:116 tests/models.py:125
-msgid "deleted"
-msgstr "gelöscht"
-
-#: tests/models.py:108 tests/models.py:117 tests/models.py:126
-msgid "on hold"
-msgstr "wartend"
+#~ msgid "active"
+#~ msgstr "aktiv"
+
+#~ msgid "deleted"
+#~ msgstr "gelöscht"
+
+#~ msgid "on hold"
+#~ msgstr "wartend"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/es/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/model_utils/locale/es/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # This file is distributed under the same license as the django-model-utils package.
 #
 # Translators:
-# Enrique Matías Sánchez <cronopios@gmail.com>, 2020.
+# Tomas Walch <tomas@alternaliv.se>, 2022.
 msgid ""
 msgstr ""
-"Project-Id-Version: django-model-utils\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-03-29 10:59+0200\n"
-"PO-Revision-Date: 2020-03-29 11:14+0100\n"
-"Last-Translator: Enrique Matías Sánchez <cronopios@gmail.com>\n"
-"Language-Team: \n"
-"Language: es\n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Lokalize 2.0\n"
 
-#: models.py:28
+#: models.py:24
 msgid "created"
-msgstr "creado"
+msgstr "skapad"
 
-#: models.py:29
+#: models.py:25
 msgid "modified"
-msgstr "modificado"
+msgstr "ändrad"
 
-#: models.py:51
+#: models.py:49
 msgid "start"
-msgstr "inicio"
+msgstr "start"
 
-#: models.py:52
+#: models.py:50
 msgid "end"
-msgstr "fin"
+msgstr "slut"
 
-#: models.py:67
+#: models.py:65
 msgid "status"
-msgstr "estado"
+msgstr "status"
 
-#: models.py:68
+#: models.py:66
 msgid "status changed"
-msgstr "estado modificado"
+msgstr "status ändrad"
 
+#~ msgid "active"
+#~ msgstr "aktiv"
+
+#~ msgid "deleted"
+#~ msgstr "borttagen"
+
+#~ msgid "on hold"
+#~ msgstr "väntande"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/fa/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/model_utils/locale/fa/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 #
 # Translators:
 # Hasan Ramezani <hasan.r67@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-19 13:00+0200\n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: models.py:28
+#: models.py:24
 msgid "created"
 msgstr "ایجاد شد"
 
-#: models.py:29
+#: models.py:25
 msgid "modified"
 msgstr "اصلاح شد"
 
-#: models.py:51
+#: models.py:49
 msgid "start"
 msgstr "شروع"
 
-#: models.py:52
+#: models.py:50
 msgid "end"
 msgstr "پایان"
 
-#: models.py:67
+#: models.py:65
 msgid "status"
 msgstr "وضعیت"
 
-#: models.py:68
+#: models.py:66
 msgid "status changed"
 msgstr "وضعیت تغییر کرد"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/fr/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,31 +1,30 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: django-model-utils\n"
-"Report-Msgid-Bugs-To: https://github.com/jazzband/django-model-utils/issues\n"
-"PO-Revision-Date: 2021-01-11 11:45+0100\n"
-"Last-Translator: Florian Alu <fla@grapps.fr>\n"
-"Language-Team: \n"
-"Language: fr\n"
+"Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Poedit 2.4.2\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "created"
-msgstr "créé"
+msgstr "skapad"
 
 msgid "end"
-msgstr "fin"
+msgstr "slut"
 
 msgid "modified"
-msgstr "modifié"
+msgstr "ändrad"
 
 msgid "start"
-msgstr "début"
+msgstr "start"
 
 msgid "status"
-msgstr "statut"
+msgstr "status"
 
 msgid "status changed"
-msgstr "statut modifié"
+msgstr "status ändrad"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/fr/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 # Translators:
 # ------------
 # Florian Alu <fla@grapps.fr>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
-"Report-Msgid-Bugs-To: https://github.com/jazzband/django-model-utils/issues\n"
-"POT-Creation-Date: 2021-01-11 11:39+0100\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: 2021-01-11 11:45+0100\n"
 "Last-Translator: Florian Alu <fla@grapps.fr>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 2.4.2\n"
 
-#: .\models.py:25
+#: models.py:24
 msgid "created"
 msgstr "créé"
 
-#: .\models.py:26
+#: models.py:25
 msgid "modified"
 msgstr "modifié"
 
-#: .\models.py:50
+#: models.py:49
 msgid "start"
 msgstr "début"
 
-#: .\models.py:51
+#: models.py:50
 msgid "end"
 msgstr "fin"
 
-#: .\models.py:66
+#: models.py:65
 msgid "status"
 msgstr "statut"
 
-#: .\models.py:67
+#: models.py:66
 msgid "status changed"
 msgstr "statut modifié"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/ru/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-05-22 19:46+0300\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"PO-Revision-Date: 2017-05-22 19:46+0300\n"
 "Last-Translator: Arseny Sysolyatin <arseny.sysolyatin@gmail.com>\n"
 "Language-Team: \n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/ru/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 #
 # Translators:
 # Arseny Sysolyatin <arseny.sysolyatin@gmail.com>, 2017.
 msgid ""
 msgstr ""
 "Project-Id-Version: django-model-utils\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-05-22 19:46+0300\n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: 2017-05-22 19:46+0300\n"
 "Last-Translator: Arseny Sysolyatin <arseny.sysolyatin@gmail.com>\n"
 "Language-Team: \n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: models.py:24
 msgid "created"
 msgstr "создано"
 
 #: models.py:25
 msgid "modified"
 msgstr "изменено"
 
-#: models.py:37
+#: models.py:49
 msgid "start"
 msgstr "начало"
 
-#: models.py:38
+#: models.py:50
 msgid "end"
 msgstr "конец"
 
-#: models.py:53
+#: models.py:65
 msgid "status"
 msgstr "статус"
 
-#: models.py:54
+#: models.py:66
 msgid "status changed"
 msgstr "статус изменен"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-10-23 15:12+0800\n"
 "PO-Revision-Date: 2018-10-23 15:26+0800\n"
 "Last-Translator: Zach Cheung <kuroro.zhang@gmail.com>\n"
 "Language-Team: \n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `django-model-utils-4.4.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po` & `django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Translators:
 # Zach Cheung <kuroro.zhang@gmail.com>, 2018.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-10-23 15:12+0800\n"
+"POT-Creation-Date: 2024-04-01 15:01+0200\n"
 "PO-Revision-Date: 2018-10-23 15:26+0800\n"
 "Last-Translator: Zach Cheung <kuroro.zhang@gmail.com>\n"
 "Language-Team: \n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -20,22 +20,22 @@
 msgid "created"
 msgstr "创建时间"
 
 #: models.py:25
 msgid "modified"
 msgstr "修改时间"
 
-#: models.py:37
+#: models.py:49
 msgid "start"
 msgstr "开始时间"
 
-#: models.py:38
+#: models.py:50
 msgid "end"
 msgstr "结束时间"
 
-#: models.py:53
+#: models.py:65
 msgid "status"
 msgstr "状态"
 
-#: models.py:54
+#: models.py:66
 msgid "status changed"
 msgstr "状态修改时间"
```

### Comparing `django-model-utils-4.4.0/model_utils/managers.py` & `django-model-utils-4.5.0/model_utils/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             if hasattr(self, name):
                 update[name] = getattr(self, name)
 
         chained = super()._chain(**kwargs)
         chained.__dict__.update(update)
         return chained
 
-    def _clone(self, klass=None, setup=False, **kwargs):
+    def _clone(self):
         qs = super()._clone()
         for name in ['subclasses', '_annotated']:
             if hasattr(self, name):
                 setattr(qs, name, getattr(self, name))
         return qs
 
     def annotate(self, *args, **kwargs):
```

### Comparing `django-model-utils-4.4.0/model_utils/models.py` & `django-model-utils-4.5.0/model_utils/models.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/model_utils/tracker.py` & `django-model-utils-4.5.0/model_utils/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from copy import deepcopy
 from functools import wraps
 
 from django.core.exceptions import FieldError
 from django.db import models
-from django.db.models.fields.files import FieldFile, FileDescriptor
-from django.db.models.query_utils import DeferredAttribute
+from django.db.models.fields.files import FieldFile
 
 
 class LightStateFieldFile(FieldFile):
     """
     FieldFile subclass with the only aim to remove the instance from the state.
 
     The change introduced in Django 3.1 on FieldFile subclasses results in pickling the
@@ -36,34 +35,14 @@
             instance=value.instance,
             field=value.field,
             name=value.name,
         )
     return deepcopy(value)
 
 
-class DescriptorMixin:
-    tracker_instance = None
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            return self
-        was_deferred = False
-        field_name = self._get_field_name()
-        if field_name in instance._deferred_fields:
-            instance._deferred_fields.remove(field_name)
-            was_deferred = True
-        value = super().__get__(instance, owner)
-        if was_deferred:
-            self.tracker_instance.saved_data[field_name] = lightweight_deepcopy(value)
-        return value
-
-    def _get_field_name(self):
-        return self.field_name
-
-
 class DescriptorWrapper:
 
     def __init__(self, field_name, descriptor, tracker_attname):
         self.field_name = field_name
         self.descriptor = descriptor
         self.tracker_attname = tracker_attname
 
@@ -270,38 +249,14 @@
         """Returns dict of fields that changed since save (with old values)"""
         return {
             field: self.previous(field)
             for field in self.fields
             if self.has_changed(field)
         }
 
-    def init_deferred_fields(self):
-        self.instance._deferred_fields = set()
-        if hasattr(self.instance, '_deferred') and not self.instance._deferred:
-            return
-
-        class DeferredAttributeTracker(DescriptorMixin, DeferredAttribute):
-            tracker_instance = self
-
-        class FileDescriptorTracker(DescriptorMixin, FileDescriptor):
-            tracker_instance = self
-
-            def _get_field_name(self):
-                return self.field.name
-
-        self.instance._deferred_fields = self.instance.get_deferred_fields()
-        for field in self.instance._deferred_fields:
-            field_obj = self.instance.__class__.__dict__.get(field)
-            if isinstance(field_obj, FileDescriptor):
-                field_tracker = FileDescriptorTracker(field_obj.field)
-                setattr(self.instance.__class__, field, field_tracker)
-            else:
-                field_tracker = DeferredAttributeTracker(field)
-                setattr(self.instance.__class__, field, field_tracker)
-
 
 class FieldTracker:
 
     tracker_class = FieldInstanceTracker
 
     def __init__(self, fields=None):
         self.fields = fields
@@ -339,27 +294,37 @@
         self.fields = set(self.fields)
         for field_name in self.fields:
             descriptor = getattr(sender, field_name)
             wrapper_cls = DescriptorWrapper.cls_for_descriptor(descriptor)
             wrapped_descriptor = wrapper_cls(field_name, descriptor, self.attname)
             setattr(sender, field_name, wrapped_descriptor)
         self.field_map = self.get_field_map(sender)
-        models.signals.post_init.connect(self.initialize_tracker)
+        self.patch_init(sender)
         self.model_class = sender
         setattr(sender, self.name, self)
         self.patch_save(sender)
 
     def initialize_tracker(self, sender, instance, **kwargs):
         if not isinstance(instance, self.model_class):
             return  # Only init instances of given model (including children)
         tracker = self.tracker_class(instance, self.fields, self.field_map)
         setattr(instance, self.attname, tracker)
         tracker.set_saved_fields()
         instance._instance_initialized = True
 
+    def patch_init(self, model):
+        original = getattr(model, '__init__')
+
+        @wraps(original)
+        def inner(instance, *args, **kwargs):
+            original(instance, *args, **kwargs)
+            self.initialize_tracker(model, instance)
+
+        setattr(model, '__init__', inner)
+
     def patch_save(self, model):
         self._patch(model, 'save_base', 'update_fields')
         self._patch(model, 'refresh_from_db', 'fields')
 
     def _patch(self, model, method, fields_kwarg):
         original = getattr(model, method)
```

### Comparing `django-model-utils-4.4.0/setup.py` & `django-model-utils-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/fields.py` & `django-model-utils-4.5.0/tests/fields.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/models.py` & `django-model-utils-4.5.0/tests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db import models
 from django.db.models import Manager
 from django.db.models.query_utils import DeferredAttribute
 from django.utils.translation import gettext_lazy as _
 
 from model_utils import Choices
 from model_utils.fields import MonitorField, SplitField, StatusField, UUIDField
-from model_utils.managers import InheritanceManager, JoinManagerMixin, QueryManager
+from model_utils.managers import InheritanceManager, JoinManager, QueryManager
 from model_utils.models import (
     SoftDeletableModel,
     StatusModel,
     TimeFramedModel,
     TimeStampedModel,
     UUIDModel,
 )
@@ -141,27 +141,31 @@
     )
 
 
 class StatusCustomManager(Manager):
     pass
 
 
-class AbstractStatusCustomManager(StatusModel):
+class AbstractCustomManagerStatusModel(StatusModel):
+    """An abstract status model with a custom manager."""
+
     STATUS = Choices(
         ("first_choice", _("First choice")),
         ("second_choice", _("Second choice")),
     )
 
     objects = StatusCustomManager()
 
     class Meta:
         abstract = True
 
 
-class StatusCustomManager(AbstractStatusCustomManager):
+class CustomManagerStatusModel(AbstractCustomManagerStatusModel):
+    """A concrete status model with a custom manager."""
+
     title = models.CharField(max_length=50)
 
 
 class Post(models.Model):
     published = models.BooleanField(default=False)
     confirmed = models.BooleanField(default=False)
     order = models.IntegerField()
@@ -184,49 +188,14 @@
 class SplitFieldAbstractParent(models.Model):
     content = SplitField()
 
     class Meta:
         abstract = True
 
 
-class NoRendered(models.Model):
-    """
-    Test that the no_excerpt_field keyword arg works. This arg should
-    never be used except by the South model-freezing.
-
-    """
-    body = SplitField(no_excerpt_field=True)
-
-
-class AuthorMixin:
-    def by_author(self, name):
-        return self.filter(author=name)
-
-
-class PublishedMixin:
-    def published(self):
-        return self.filter(published=True)
-
-
-def unpublished(self):
-    return self.filter(published=False)
-
-
-class ByAuthorQuerySet(models.query.QuerySet, AuthorMixin):
-    pass
-
-
-class FeaturedManager(models.Manager):
-    def get_queryset(self):
-        kwargs = {}
-        if hasattr(self, "_db"):
-            kwargs["using"] = self._db
-        return ByAuthorQuerySet(self.model, **kwargs).filter(feature=True)
-
-
 class AbstractTracked(models.Model):
     number = 1
 
     class Meta:
         abstract = True
 
 
@@ -414,18 +383,14 @@
     tracked_custom_field = CustomDescriptorField()
     regular_field = models.IntegerField()
     tracked_regular_field = models.IntegerField()
 
     tracker = FieldTracker(fields=['tracked_custom_field', 'tracked_regular_field'])
 
 
-class JoinManager(JoinManagerMixin, models.Manager):
-    pass
-
-
 class BoxJoinModel(models.Model):
     name = models.CharField(max_length=32)
     objects = JoinManager()
 
 
 class JoinItemForeignKey(models.Model):
     weight = models.IntegerField()
```

### Comparing `django-model-utils-4.4.0/tests/settings.py` & `django-model-utils-4.5.0/tests/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import os
 
 INSTALLED_APPS = (
     'model_utils',
     'tests',
 )
-DATABASES = {
-    "default": {
-        "ENGINE": "django.db.backends.postgresql_psycopg2",
-        "NAME": os.environ.get("DB_NAME", "modelutils"),
-        "USER": os.environ.get("DB_USER", 'postgres'),
-        "PASSWORD": os.environ.get("DB_PASSWORD", ""),
-        "HOST": os.environ.get("DB_HOST", "localhost"),
-        "PORT": os.environ.get("DB_PORT", 5432)
-    },
-}
+
+if os.environ.get('SQLITE'):
+    DATABASES = {
+        'default': {
+            'ENGINE': 'django.db.backends.sqlite3',
+        },
+    }
+else:
+    DATABASES = {
+        "default": {
+            "ENGINE": "django.db.backends.postgresql",
+            "NAME": os.environ.get("POSTGRES_DB", "modelutils"),
+            "USER": os.environ.get("POSTGRES_USER", 'postgres'),
+            "PASSWORD": os.environ.get("POSTGRES_PASSWORD", ""),
+            "HOST": os.environ.get("POSTGRES_HOST", "localhost"),
+            "PORT": os.environ.get("POSTGRES_PORT", 5432)
+        },
+    }
 SECRET_KEY = 'dummy'
 
 CACHES = {
     'default': {
         'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
     }
 }
 
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 
-USE_TZ = False
+USE_TZ = True
```

### Comparing `django-model-utils-4.4.0/tests/test_choices.py` & `django-model-utils-4.5.0/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_field_tracker.py` & `django-model-utils-4.5.0/tests/test_fields/test_field_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,15 +866,15 @@
 
     def test_child_fields_not_tracked(self):
         self.name2 = 'test'
         self.assertEqual(self.tracker.previous('name2'), None)
         self.assertTrue(self.tracker.has_changed('name2'))
 
 
-@skip
+@skip("has known failures")
 class AbstractModelTrackerTests(ModelTrackerTests):
 
     tracked_class = TrackedAbstract
 
 
 class TrackerContextDecoratorTests(TestCase):
```

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_monitor_field.py` & `django-model-utils-4.5.0/tests/test_fields/test_monitor_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-from datetime import datetime
+from datetime import datetime, timezone
 
+import time_machine
 from django.test import TestCase
-from freezegun import freeze_time
 
 from model_utils.fields import MonitorField
 from tests.models import DoubleMonitored, Monitored, MonitorWhen, MonitorWhenEmpty
 
 
 class MonitorFieldTests(TestCase):
     def setUp(self):
-        with freeze_time(datetime(2016, 1, 1, 10, 0, 0)):
+        with time_machine.travel(datetime(2016, 1, 1, 10, 0, 0, tzinfo=timezone.utc)):
             self.instance = Monitored(name='Charlie')
             self.created = self.instance.name_changed
 
     def test_save_no_change(self):
         self.instance.save()
         self.assertEqual(self.instance.name_changed, self.created)
 
     def test_save_changed(self):
-        with freeze_time(datetime(2016, 1, 1, 12, 0, 0)):
+        with time_machine.travel(datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc)):
             self.instance.name = 'Maria'
             self.instance.save()
-        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0))
+        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc))
 
     def test_double_save(self):
         self.instance.name = 'Jose'
         self.instance.save()
         changed = self.instance.name_changed
         self.instance.save()
         self.assertEqual(self.instance.name_changed, changed)
 
     def test_no_monitor_arg(self):
         with self.assertRaises(TypeError):
             MonitorField()
 
+    def test_nullable_without_default_deprecation(self):
+        warning_message = (
+            "{}.default is set to 'django.utils.timezone.now' - when nullable"
+            " and no default. This behavior will be deprecated in the next"
+            " major release in favor of 'None'. See"
+            " https://django-model-utils.readthedocs.io/en/stable/fields.html"
+            "#monitorfield for more information."
+        ).format(MonitorField.__name__)
+
+        with self.assertWarns(DeprecationWarning, msg=warning_message):
+            MonitorField(monitor="foo", null=True, default=None)
+
 
 class MonitorWhenFieldTests(TestCase):
     """
     Will record changes only when name is 'Jose' or 'Maria'
     """
     def setUp(self):
-        with freeze_time(datetime(2016, 1, 1, 10, 0, 0)):
+        with time_machine.travel(datetime(2016, 1, 1, 10, 0, 0, tzinfo=timezone.utc)):
             self.instance = MonitorWhen(name='Charlie')
             self.created = self.instance.name_changed
 
     def test_save_no_change(self):
         self.instance.save()
         self.assertEqual(self.instance.name_changed, self.created)
 
     def test_save_changed_to_Jose(self):
-        with freeze_time(datetime(2016, 1, 1, 12, 0, 0)):
+        with time_machine.travel(datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc)):
             self.instance.name = 'Jose'
             self.instance.save()
-        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0))
+        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc))
 
     def test_save_changed_to_Maria(self):
-        with freeze_time(datetime(2016, 1, 1, 12, 0, 0)):
+        with time_machine.travel(datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc)):
             self.instance.name = 'Maria'
             self.instance.save()
-        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0))
+        self.assertEqual(self.instance.name_changed, datetime(2016, 1, 1, 12, 0, 0, tzinfo=timezone.utc))
 
     def test_save_changed_to_Pedro(self):
         self.instance.name = 'Pedro'
         self.instance.save()
         self.assertEqual(self.instance.name_changed, self.created)
 
     def test_double_save(self):
@@ -107,11 +119,11 @@
 
     def test_recursion_error_with_defer(self):
         # Only monitored fields passed to defer() are failing
         list(DoubleMonitored.objects.defer('name'))
 
     def test_monitor_still_works_with_deferred_fields_filtered_out_of_save_initial(self):
         obj = DoubleMonitored.objects.defer('name').get(name='Charlie')
-        with freeze_time("2016-12-01"):
+        with time_machine.travel(datetime(2016, 12, 1, tzinfo=timezone.utc)):
             obj.name = 'Charlie2'
             obj.save()
-        self.assertEqual(obj.name_changed, datetime(2016, 12, 1))
+        self.assertEqual(obj.name_changed, datetime(2016, 12, 1, tzinfo=timezone.utc))
```

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_split_field.py` & `django-model-utils-4.5.0/tests/test_fields/test_split_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_status_field.py` & `django-model-utils-4.5.0/tests/test_fields/test_status_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_urlsafe_token_field.py` & `django-model-utils-4.5.0/tests/test_fields/test_urlsafe_token_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_fields/test_uuid_field.py` & `django-model-utils-4.5.0/tests/test_fields/test_uuid_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_inheritance_iterable.py` & `django-model-utils-4.5.0/tests/test_inheritance_iterable.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_managers/test_inheritance_manager.py` & `django-model-utils-4.5.0/tests/test_managers/test_inheritance_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_managers/test_join_manager.py` & `django-model-utils-4.5.0/tests/test_managers/test_join_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_managers/test_query_manager.py` & `django-model-utils-4.5.0/tests/test_managers/test_query_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_managers/test_softdelete_manager.py` & `django-model-utils-4.5.0/tests/test_managers/test_softdelete_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_managers/test_status_manager.py` & `django-model-utils-4.5.0/tests/test_managers/test_status_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_miscellaneous.py` & `django-model-utils-4.5.0/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_models/test_deferred_fields.py` & `django-model-utils-4.5.0/tests/test_models/test_deferred_fields.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_models/test_softdeletable_model.py` & `django-model-utils-4.5.0/tests/test_models/test_softdeletable_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from django.db.utils import ConnectionDoesNotExist
 from django.test import TestCase
+from django.utils.connection import ConnectionDoesNotExist
 
 from tests.models import SoftDeletable
 
 
 class SoftDeletableModelTests(TestCase):
     def test_can_only_see_not_removed_entries(self):
         SoftDeletable.available_objects.create(name='a', is_removed=True)
```

### Comparing `django-model-utils-4.4.0/tests/test_models/test_status_model.py` & `django-model-utils-4.5.0/tests/test_models/test_status_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from datetime import datetime
+from datetime import datetime, timezone
 
+import time_machine
 from django.test.testcases import TestCase
-from freezegun import freeze_time
 
-from tests.models import Status, StatusCustomManager, StatusPlainTuple
+from tests.models import CustomManagerStatusModel, Status, StatusPlainTuple
 
 
 class StatusModelTests(TestCase):
     def setUp(self):
         self.model = Status
         self.on_hold = Status.STATUS.on_hold
         self.active = Status.STATUS.active
 
     def test_created(self):
-        with freeze_time(datetime(2016, 1, 1)):
+        with time_machine.travel(datetime(2016, 1, 1)):
             c1 = self.model.objects.create()
         self.assertTrue(c1.status_changed, datetime(2016, 1, 1))
 
         self.model.objects.create()
         self.assertEqual(self.model.active.count(), 2)
         self.assertEqual(self.model.deleted.count(), 0)
 
@@ -39,37 +39,37 @@
 
     def test_save_with_update_fields_overrides_status_changed_provided(self):
         '''
         Tests if the save method updated status_changed field
         accordingly when update_fields is used as an argument
         and status_changed is provided
         '''
-        with freeze_time(datetime(2020, 1, 1)):
+        with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
             t1 = Status.objects.create()
 
-        with freeze_time(datetime(2020, 1, 2)):
+        with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
             t1.status = Status.on_hold
             t1.save(update_fields=['status', 'status_changed'])
 
-        self.assertEqual(t1.status_changed, datetime(2020, 1, 2))
+        self.assertEqual(t1.status_changed, datetime(2020, 1, 2, tzinfo=timezone.utc))
 
     def test_save_with_update_fields_overrides_status_changed_not_provided(self):
         '''
         Tests if the save method updated status_changed field
         accordingly when update_fields is used as an argument
         with status and status_changed is not provided
         '''
-        with freeze_time(datetime(2020, 1, 1)):
+        with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
             t1 = Status.objects.create()
 
-        with freeze_time(datetime(2020, 1, 2)):
+        with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
             t1.status = Status.on_hold
             t1.save(update_fields=['status'])
 
-        self.assertEqual(t1.status_changed, datetime(2020, 1, 2))
+        self.assertEqual(t1.status_changed, datetime(2020, 1, 2, tzinfo=timezone.utc))
 
 
 class StatusModelPlainTupleTests(StatusModelTests):
     def setUp(self):
         self.model = StatusPlainTuple
         self.on_hold = StatusPlainTuple.STATUS[2][0]
         self.active = StatusPlainTuple.STATUS[0][0]
@@ -83,17 +83,17 @@
         # and affects default manager.
         # This code was previously failing because the first custom manager (which filters
         # with first Choice value, here 'first_choice') generated by StatusModel was
         # considered as default manager...
         # This situation only happens when we define a model inheriting from an "abstract"
         # class which defines an "objects" manager.
 
-        StatusCustomManager.objects.create(status='first_choice')
-        StatusCustomManager.objects.create(status='second_choice')
-        StatusCustomManager.objects.create(status='second_choice')
+        CustomManagerStatusModel.objects.create(status='first_choice')
+        CustomManagerStatusModel.objects.create(status='second_choice')
+        CustomManagerStatusModel.objects.create(status='second_choice')
 
         # ...which made this count() equal to 1 (only 1 element with status='first_choice')...
-        self.assertEqual(StatusCustomManager._default_manager.count(), 3)
+        self.assertEqual(CustomManagerStatusModel._default_manager.count(), 3)
 
         # ...and this one equal to 0, because of 2 successive filters of 'first_choice'
         # (default manager) and 'second_choice' (explicit filter below).
-        self.assertEqual(StatusCustomManager._default_manager.filter(status='second_choice').count(), 2)
+        self.assertEqual(CustomManagerStatusModel._default_manager.filter(status='second_choice').count(), 2)
```

### Comparing `django-model-utils-4.4.0/tests/test_models/test_timeframed_model.py` & `django-model-utils-4.5.0/tests/test_models/test_timeframed_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tests/test_models/test_timestamped_model.py` & `django-model-utils-4.5.0/tests/test_models/test_timestamped_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
+import time_machine
 from django.test import TestCase
-from freezegun import freeze_time
 
 from tests.models import TimeStamp, TimeStampWithStatusModel
 
 
 class TimeStampedModelTests(TestCase):
     def test_created(self):
-        with freeze_time(datetime(2016, 1, 1)):
+        with time_machine.travel(datetime(2016, 1, 1, tzinfo=timezone.utc)):
             t1 = TimeStamp.objects.create()
-        self.assertEqual(t1.created, datetime(2016, 1, 1))
+        self.assertEqual(t1.created, datetime(2016, 1, 1, tzinfo=timezone.utc))
 
     def test_created_sets_modified(self):
         '''
         Ensure that on creation that modified is set exactly equal to created.
         '''
         t1 = TimeStamp.objects.create()
         self.assertEqual(t1.created, t1.modified)
 
     def test_modified(self):
-        with freeze_time(datetime(2016, 1, 1)):
+        with time_machine.travel(datetime(2016, 1, 1, tzinfo=timezone.utc)):
             t1 = TimeStamp.objects.create()
 
-        with freeze_time(datetime(2016, 1, 2)):
+        with time_machine.travel(datetime(2016, 1, 2, tzinfo=timezone.utc)):
             t1.save()
 
-        self.assertEqual(t1.modified, datetime(2016, 1, 2))
+        self.assertEqual(t1.modified, datetime(2016, 1, 2, tzinfo=timezone.utc))
 
     def test_overriding_created_via_object_creation_also_uses_creation_date_for_modified(self):
         """
         Setting the created date when first creating an object
         should be permissible.
         """
         different_date = datetime.today() - timedelta(weeks=52)
@@ -100,51 +100,51 @@
             ['modified'],  # list
             ('modified',),  # tuple
             {'modified'},  # set
         )
 
         for update_fields in tests:
             with self.subTest(update_fields=update_fields):
-                with freeze_time(datetime(2020, 1, 1)):
+                with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
                     t1 = TimeStamp.objects.create()
 
-                with freeze_time(datetime(2020, 1, 2)):
+                with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
                     t1.save(update_fields=update_fields)
-                self.assertEqual(t1.modified, datetime(2020, 1, 2))
+                self.assertEqual(t1.modified, datetime(2020, 1, 2, tzinfo=timezone.utc))
 
     def test_save_is_skipped_for_empty_update_fields_iterable(self):
         tests = (
             [],  # list
             (),  # tuple
             set(),  # set
         )
 
         for update_fields in tests:
             with self.subTest(update_fields=update_fields):
-                with freeze_time(datetime(2020, 1, 1)):
+                with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
                     t1 = TimeStamp.objects.create()
 
-                with freeze_time(datetime(2020, 1, 2)):
+                with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
                     t1.test_field = 1
                     t1.save(update_fields=update_fields)
 
                 t1.refresh_from_db()
                 self.assertEqual(t1.test_field, 0)
-                self.assertEqual(t1.modified, datetime(2020, 1, 1))
+                self.assertEqual(t1.modified, datetime(2020, 1, 1, tzinfo=timezone.utc))
 
     def test_save_updates_modified_value_when_update_fields_explicitly_set_to_none(self):
-        with freeze_time(datetime(2020, 1, 1)):
+        with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
             t1 = TimeStamp.objects.create()
 
-        with freeze_time(datetime(2020, 1, 2)):
+        with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
             t1.save(update_fields=None)
 
-        self.assertEqual(t1.modified, datetime(2020, 1, 2))
+        self.assertEqual(t1.modified, datetime(2020, 1, 2, tzinfo=timezone.utc))
 
     def test_model_inherit_timestampmodel_and_statusmodel(self):
-        with freeze_time(datetime(2020, 1, 1)):
+        with time_machine.travel(datetime(2020, 1, 1, tzinfo=timezone.utc)):
             t1 = TimeStampWithStatusModel.objects.create()
 
-        with freeze_time(datetime(2020, 1, 2)):
+        with time_machine.travel(datetime(2020, 1, 2, tzinfo=timezone.utc)):
             t1.save(update_fields=['test_field', 'status'])
 
-        self.assertEqual(t1.modified, datetime(2020, 1, 2))
+        self.assertEqual(t1.modified, datetime(2020, 1, 2, tzinfo=timezone.utc))
```

### Comparing `django-model-utils-4.4.0/tests/test_models/test_uuid_model.py` & `django-model-utils-4.5.0/tests/test_models/test_uuid_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.4.0/tox.ini` & `django-model-utils-4.5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     3.9: py39
     3.10: py310
     3.11: py311
     3.12: py312
 
 [testenv]
 deps =
-    freezegun==0.3.12
+    time-machine==2.4.1
     -rrequirements-test.txt
     dj32: Django==3.2.*
     dj40: Django==4.0.*
     dj41: Django==4.1.*
     dj42: Django==4.2.*
     dj50: Django==5.0.*
     djmain: https://github.com/django/django/archive/main.tar.gz
@@ -32,15 +32,15 @@
     djmain: True
 ignore_errors =
     djmain: True
 passenv =
     CI
     FORCE_COLOR
     GITHUB_*
-    DB_*
+    POSTGRES_*
 usedevelop = True
 commands =
     python -m pytest {posargs}
 
 [testenv:flake8]
 basepython =
     python3.8
```

### Comparing `django-model-utils-4.4.0/translations.py` & `django-model-utils-4.5.0/translations.py`

 * *Files identical despite different names*

