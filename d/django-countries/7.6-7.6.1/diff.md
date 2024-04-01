# Comparing `tmp/django-countries-7.6.tar.gz` & `tmp/django-countries-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-countries-7.6.tar", last modified: Wed Mar 27 03:22:58 2024, max compression
+gzip compressed data, was "django-countries-7.6.1.tar", last modified: Mon Apr  1 21:01:00 2024, max compression
```

## Comparing `django-countries-7.6.tar` & `django-countries-7.6.1.tar`

### file list

```diff
@@ -1,512 +1,512 @@
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.741777 django-countries-7.6/
--rw-r--r--   0 chris     (1000) chris     (1001)    12687 2024-03-27 03:22:58.000000 django-countries-7.6/CHANGES.rst
--rw-r--r--   0 chris     (1000) chris     (1001)     1072 2024-03-27 03:22:58.000000 django-countries-7.6/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1001)      207 2024-03-27 03:22:58.000000 django-countries-7.6/MANIFEST.in
--rw-r--r--   0 chris     (1000) chris     (1001)    30687 2024-03-27 03:22:58.741777 django-countries-7.6/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1001)    16624 2024-03-27 03:22:58.000000 django-countries-7.6/README.rst
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/
--rw-r--r--   0 chris     (1000) chris     (1001)    20043 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1157 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/base.py
--rw-r--r--   0 chris     (1000) chris     (1001)     2831 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/conf.py
--rwxr-xr-x   0 chris     (1000) chris     (1001)    17739 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/data.py
--rw-r--r--   0 chris     (1000) chris     (1001)    18890 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/fields.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1522 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/filters.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/graphql/
--rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/graphql/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1001)      906 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/graphql/types.py
--rw-r--r--   0 chris     (1000) chris     (1001)     5947 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/ioc_data.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/af/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/af/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12720 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16227 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ar/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/ar/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    15290 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    18794 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/bg/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/bg/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    15695 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    19034 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ca/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/ca/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12944 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16496 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/cs/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/cs/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    13138 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16563 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/da/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/da/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12522 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    15884 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/de/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/de/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12775 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16506 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/el/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/el/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    15885 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    19340 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/en@test/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/en@test/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/en@test/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)      573 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/en@test/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/eo/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/eo/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12563 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16112 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/es/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/es/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12890 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16610 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/et/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/et/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12279 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    15834 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/eu/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/eu/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12715 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16226 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/eu_ES/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12729 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16240 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/eu_ES/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/fa/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/fa/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    14606 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    17978 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/fi/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/fi/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12283 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    15844 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/fr/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/fr/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    13137 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16941 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/he/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/he/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    14493 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    17997 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/he_IL/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.711776 django-countries-7.6/django_countries/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    14508 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/he_IL/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    18012 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/he_IL/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/hr/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/hr/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12858 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16419 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/hu/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/hu/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12597 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16061 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/hy/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/hy/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    16198 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hy/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    19558 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/it/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/it/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12629 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16225 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ja/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/ja/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    14523 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    18088 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ko_KR/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    13395 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16784 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/lt/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/lt/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12702 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16271 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/lv/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/lv/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12867 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16373 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/mn/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/mn/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    15174 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    18497 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/nb/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/nb/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12527 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16050 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/nl/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/nl/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12744 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16273 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/pl/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/pl/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12599 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16243 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/pt_BR/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.715110 django-countries-7.6/django_countries/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12848 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16527 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/pt_PT/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    13015 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16415 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ro/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/ro/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12497 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16000 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/ru/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/ru/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    16173 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    19877 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sk/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sk/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12759 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16250 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sl/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sl/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12494 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16009 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sr/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sr/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    15647 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    18949 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sr@latin/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sr@latin/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12944 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr@latin/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16222 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sr_Latn/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12944 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr_Latn/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16222 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sr_Latn_BA/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12486 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    15950 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.705110 django-countries-7.6/django_countries/locale/sv/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/sv/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12613 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16129 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/th_TH/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12907 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16218 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/tr_TR/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12884 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16296 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/tr_TR/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/uk/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/uk/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    16213 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    19688 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/vi/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/vi/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    13151 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16471 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/zh_CN/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12810 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16492 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/zh_Hans/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12817 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16454 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/locale/zh_Hant/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.718443 django-countries-7.6/django_countries/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 chris     (1000) chris     (1001)    12833 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 chris     (1000) chris     (1001)    16149 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/locale/zh_Hant/LC_MESSAGES/django.po
--rwxr-xr-x   0 chris     (1000) chris     (1001)     2525 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/makesprite.py
--rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/models.py
--rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/py.typed
--rw-r--r--   0 chris     (1000) chris     (1001)      800 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/release.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1294 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/serializer_fields.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1180 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/serializers.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries/static/
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.738443 django-countries-7.6/django_countries/static/flags/
--rw-r--r--   0 chris     (1000) chris     (1001)       53 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/__.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ad.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ae.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/af.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ag.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ai.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/al.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/am.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      236 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ao.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      331 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/aq.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ar.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/as.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/at.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/au.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/aw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ax.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/az.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ba.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bb.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bd.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/be.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bi.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bj.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bo.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      546 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bq.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/br.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      343 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bs.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/by.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/bz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ca.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      235 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cd.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      324 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ch.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ci.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ck.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      345 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/co.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      308 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cx.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cy.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/cz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/de.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/dj.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/dk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/dm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/do.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/dz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ec.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ee.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/eg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/eh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/er.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/es.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/et.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      163 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/eu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fi.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fj.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fo.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/fr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ga.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      252 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gb.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gd.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      371 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ge.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      546 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gi.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gp.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gq.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gs.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/gy.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/hk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/hm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/hn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/hr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ht.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/hu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/id.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ie.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/il.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      544 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/im.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/in.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/io.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/iq.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ir.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/is.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/it.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      579 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/je.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/jm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/jo.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/jp.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ke.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ki.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/km.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kp.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      377 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ky.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/kz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/la.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lb.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      251 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/li.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ls.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/lv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      202 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ly.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ma.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/md.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      330 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/me.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      374 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ml.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      335 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mo.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mp.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      371 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mq.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      538 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ms.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mx.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/my.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/mz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/na.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ne.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ng.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ni.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/no.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      302 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/np.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/nz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/om.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pa.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pe.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ph.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ps.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/pw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/py.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/qa.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/re.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ro.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      230 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/rs.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ru.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/rw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sa.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sb.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      347 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sd.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/se.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sh.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/si.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sj.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/so.gif
--rw-r--r--   0 chris     (1000) chris     (1001)     9738 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sprite-hq.css
--rw-r--r--   0 chris     (1000) chris     (1001)    86727 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sprite-hq.png
--rw-r--r--   0 chris     (1000) chris     (1001)     2253 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sprite.css
--rw-r--r--   0 chris     (1000) chris     (1001)    27692 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sprite.png
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      554 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ss.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/st.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      551 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sx.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sy.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/sz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/td.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/th.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tj.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tl.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/to.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tr.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tv.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tw.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/tz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ua.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ug.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/um.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/us.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/uy.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/uz.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/va.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/vc.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ve.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/vg.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/vi.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/vn.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/vu.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/wf.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ws.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      555 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/xk.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      348 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/ye.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      374 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/yt.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/za.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/zm.gif
--rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/static/flags/zw.gif
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.741777 django-countries-7.6/django_countries/templatetags/
--rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/templatetags/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1001)      262 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/templatetags/countries.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.741777 django-countries-7.6/django_countries/tests/
--rw-r--r--   0 chris     (1000) chris     (1001)       62 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1001)      138 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/apps.py
--rw-r--r--   0 chris     (1000) chris     (1001)      617 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/custom_countries.py
--rw-r--r--   0 chris     (1000) chris     (1001)      445 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/forms.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.741777 django-countries-7.6/django_countries/tests/graphql/
--rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/graphql/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1001)      753 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/graphql/schema.py
--rw-r--r--   0 chris     (1000) chris     (1001)      488 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/graphql/test_country_type.py
--rw-r--r--   0 chris     (1000) chris     (1001)      476 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/graphql/test_model.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1486 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/models.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1136 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/settings.py
--rw-r--r--   0 chris     (1000) chris     (1001)       50 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/settings_noi18n.py
--rw-r--r--   0 chris     (1000) chris     (1001)     2291 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_admin_filters.py
--rw-r--r--   0 chris     (1000) chris     (1001)    15851 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_countries.py
--rw-r--r--   0 chris     (1000) chris     (1001)     7004 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_drf.py
--rw-r--r--   0 chris     (1000) chris     (1001)    27672 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_fields.py
--rw-r--r--   0 chris     (1000) chris     (1001)     2067 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_settings.py
--rw-r--r--   0 chris     (1000) chris     (1001)     1743 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_tags.py
--rw-r--r--   0 chris     (1000) chris     (1001)     2607 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/tests/test_widgets.py
--rw-r--r--   0 chris     (1000) chris     (1001)     3011 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries/widgets.py
-drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-03-27 03:22:58.708443 django-countries-7.6/django_countries.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1001)    30687 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1001)    15986 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1001)        1 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1001)        1 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) chris     (1001)      251 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1001)       17 2024-03-27 03:22:58.000000 django-countries-7.6/django_countries.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1001)      106 2024-03-27 03:22:58.000000 django-countries-7.6/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1001)     2467 2024-03-27 03:22:58.741777 django-countries-7.6/setup.cfg
--rwxr-xr-x   0 chris     (1000) chris     (1001)       60 2024-03-27 03:22:58.000000 django-countries-7.6/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.740693 django-countries-7.6.1/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12811 2024-04-01 21:01:00.000000 django-countries-7.6.1/CHANGES.rst
+-rw-r--r--   0 chris     (1000) chris     (1001)     1072 2024-04-01 21:01:00.000000 django-countries-7.6.1/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1001)      207 2024-04-01 21:01:00.000000 django-countries-7.6.1/MANIFEST.in
+-rw-r--r--   0 chris     (1000) chris     (1001)    30813 2024-04-01 21:01:00.740693 django-countries-7.6.1/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1001)    16624 2024-04-01 21:01:00.000000 django-countries-7.6.1/README.rst
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/
+-rw-r--r--   0 chris     (1000) chris     (1001)    20043 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1188 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/base.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     2831 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/conf.py
+-rwxr-xr-x   0 chris     (1000) chris     (1001)    17739 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/data.py
+-rw-r--r--   0 chris     (1000) chris     (1001)    18890 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/fields.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1544 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/filters.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/graphql/
+-rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/graphql/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      906 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/graphql/types.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     5947 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/ioc_data.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.707360 django-countries-7.6.1/django_countries/locale/af/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/af/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12722 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16229 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ar/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    15292 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    18796 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/bg/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    15697 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    19036 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ca/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12946 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16498 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/cs/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    13140 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16565 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/da/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/da/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12524 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    15886 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/de/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/de/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12777 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16508 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/el/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/el/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    15887 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    19342 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/en@test/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/en@test/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/en@test/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)      573 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/en@test/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/eo/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12565 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16114 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/es/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/es/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12892 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16612 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/et/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/et/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12281 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    15836 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/eu/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12717 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16228 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/eu_ES/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12731 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16242 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/eu_ES/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/fa/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    14608 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    17980 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/fi/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12285 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    15846 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/fr/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    13139 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16943 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/he/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/he/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    14495 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    17999 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/he_IL/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    14510 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/he_IL/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    18014 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/he_IL/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/hr/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12860 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16421 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/hu/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12599 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16063 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/hy/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    16200 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hy/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    19560 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/it/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/it/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12631 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16227 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ja/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    14525 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    18090 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ko_KR/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    13397 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16786 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/lt/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12704 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16273 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/lv/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12869 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16375 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/mn/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    15176 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    18499 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/nb/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12529 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16052 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/nl/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12737 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16294 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/pl/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12601 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16245 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/pt_BR/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12850 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16529 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/pt_PT/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.717360 django-countries-7.6.1/django_countries/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    13017 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16417 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ro/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12499 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16002 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/ru/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    16175 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    19879 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sk/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12761 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16252 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sl/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12496 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16011 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sr/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    15649 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    18951 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sr@latin/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sr@latin/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12946 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr@latin/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16224 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr@latin/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sr_Latn/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12946 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr_Latn/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16224 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sr_Latn_BA/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12488 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    15952 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/sv/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12615 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16131 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/th_TH/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12907 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16218 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/tr_TR/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12886 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16298 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/tr_TR/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/uk/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    16215 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    19690 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/vi/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    13151 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16471 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/zh_CN/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12812 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16494 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/zh_Hans/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12819 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16456 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/locale/zh_Hant/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.720693 django-countries-7.6.1/django_countries/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 chris     (1000) chris     (1001)    12835 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris     (1000) chris     (1001)    16151 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/locale/zh_Hant/LC_MESSAGES/django.po
+-rwxr-xr-x   0 chris     (1000) chris     (1001)     2525 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/makesprite.py
+-rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/models.py
+-rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/py.typed
+-rw-r--r--   0 chris     (1000) chris     (1001)      800 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/release.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1294 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/serializer_fields.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1180 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/serializers.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.710693 django-countries-7.6.1/django_countries/static/
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.740693 django-countries-7.6.1/django_countries/static/flags/
+-rw-r--r--   0 chris     (1000) chris     (1001)       53 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/__.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ad.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ae.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/af.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ag.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ai.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/al.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/am.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      236 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ao.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      331 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/aq.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ar.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/as.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/at.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/au.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/aw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ax.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/az.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ba.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bb.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bd.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/be.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bi.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bj.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bo.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      546 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bq.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/br.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      343 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bs.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/by.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/bz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ca.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      235 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cd.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      324 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ch.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ci.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ck.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      345 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/co.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      308 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cx.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cy.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/cz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/de.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/dj.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/dk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/dm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/do.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/dz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ec.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ee.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/eg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/eh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/er.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/es.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/et.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      163 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/eu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fi.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fj.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fo.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/fr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ga.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      252 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gb.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gd.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      371 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ge.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      546 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gi.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gp.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gq.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gs.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/gy.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/hk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/hm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/hn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/hr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ht.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/hu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/id.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ie.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/il.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      544 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/im.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/in.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/io.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/iq.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ir.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/is.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/it.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      579 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/je.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/jm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/jo.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/jp.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ke.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ki.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/km.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kp.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      377 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ky.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/kz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/la.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lb.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      251 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/li.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ls.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/lv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      202 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ly.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ma.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/md.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      330 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/me.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      374 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ml.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      335 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      370 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mo.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mp.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      371 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mq.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      538 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ms.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mx.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/my.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/mz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/na.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ne.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ng.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ni.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/no.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      302 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/np.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/nz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/om.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pa.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pe.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ph.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ps.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      366 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/pw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/py.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/qa.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/re.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ro.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      230 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/rs.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ru.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/rw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sa.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sb.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      349 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      347 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sd.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/se.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sh.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      354 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/si.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sj.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/so.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)     9738 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sprite-hq.css
+-rw-r--r--   0 chris     (1000) chris     (1001)    86727 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sprite-hq.png
+-rw-r--r--   0 chris     (1000) chris     (1001)     2253 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sprite.css
+-rw-r--r--   0 chris     (1000) chris     (1001)    27692 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sprite.png
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      554 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ss.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/st.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      551 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sx.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sy.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/sz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/td.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/th.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tj.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      364 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tl.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      367 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/to.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tr.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      353 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tv.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tw.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      358 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/tz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      352 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ua.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      351 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ug.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      363 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/um.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      359 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/us.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      365 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/uy.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/uz.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      361 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/va.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/vc.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      356 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ve.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      360 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/vg.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      368 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/vi.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      362 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/vn.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/vu.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      369 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/wf.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ws.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      555 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/xk.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      348 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/ye.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      374 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/yt.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      355 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/za.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      350 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/zm.gif
+-rw-r--r--   0 chris     (1000) chris     (1001)      357 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/static/flags/zw.gif
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.740693 django-countries-7.6.1/django_countries/templatetags/
+-rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/templatetags/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      262 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/templatetags/countries.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.740693 django-countries-7.6.1/django_countries/tests/
+-rw-r--r--   0 chris     (1000) chris     (1001)       62 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      138 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/apps.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      617 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/custom_countries.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      445 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/forms.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.740693 django-countries-7.6.1/django_countries/tests/graphql/
+-rw-r--r--   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/graphql/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      753 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/graphql/schema.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      488 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/graphql/test_country_type.py
+-rw-r--r--   0 chris     (1000) chris     (1001)      476 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/graphql/test_model.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1486 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/models.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1136 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/settings.py
+-rw-r--r--   0 chris     (1000) chris     (1001)       50 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/settings_noi18n.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     2731 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_admin_filters.py
+-rw-r--r--   0 chris     (1000) chris     (1001)    15851 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_countries.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     7004 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_drf.py
+-rw-r--r--   0 chris     (1000) chris     (1001)    27672 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_fields.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     2067 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_settings.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     1743 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_tags.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     2607 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/tests/test_widgets.py
+-rw-r--r--   0 chris     (1000) chris     (1001)     3011 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries/widgets.py
+drwxr-xr-x   0 chris     (1000) chris     (1001)        0 2024-04-01 21:01:00.714027 django-countries-7.6.1/django_countries.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1001)    30813 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1001)    15986 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1001)        1 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1001)        1 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/not-zip-safe
+-rw-r--r--   0 chris     (1000) chris     (1001)      251 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1001)       17 2024-04-01 21:01:00.000000 django-countries-7.6.1/django_countries.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1001)      106 2024-04-01 21:01:00.000000 django-countries-7.6.1/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1001)     2469 2024-04-01 21:01:00.740693 django-countries-7.6.1/setup.cfg
+-rwxr-xr-x   0 chris     (1000) chris     (1001)       60 2024-04-01 21:01:00.000000 django-countries-7.6.1/setup.py
```

### Comparing `django-countries-7.6/CHANGES.rst` & `django-countries-7.6.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 Change Log
 ==========
 
 This log shows interesting changes that happen for each version, latest
 versions first. It can be assumed that translations have been updated each
 release, and any new translations added.
 
+7.6.1 (2 April 2024)
+====================
+
+- Fix a TypeError when no country is selected, introduced in the Django 5 fix.
+
+
 7.6 (27 March 2024)
 ===================
 
 - Replace deprecated ``pkg_resources.iter_entry_points`` with
   ``importlib_metadata``.
 
 - Support Django 5.0.
```

### Comparing `django-countries-7.6/LICENSE` & `django-countries-7.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/PKG-INFO` & `django-countries-7.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-countries
-Version: 7.6
+Version: 7.6.1
 Summary: Provides a country field for Django models.
 Home-page: https://github.com/SmileyChris/django-countries/
 Author: Chris Beaven
 Author-email: smileychris@gmail.com
 License: MIT
 Project-URL: Change Log, https://github.com/SmileyChris/django-countries/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/SmileyChris/django-countries
@@ -628,14 +628,20 @@
 Change Log
 ==========
 
 This log shows interesting changes that happen for each version, latest
 versions first. It can be assumed that translations have been updated each
 release, and any new translations added.
 
+7.6.1 (2 April 2024)
+====================
+
+- Fix a TypeError when no country is selected, introduced in the Django 5 fix.
+
+
 7.6 (27 March 2024)
 ===================
 
 - Replace deprecated ``pkg_resources.iter_entry_points`` with
   ``importlib_metadata``.
 
 - Support Django 5.0.
```

### Comparing `django-countries-7.6/README.rst` & `django-countries-7.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/__init__.py` & `django-countries-7.6.1/django_countries/__init__.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/base.py` & `django-countries-7.6.1/django_countries/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         return message  # type: ignore
 
 
 class CountriesBase:
     COMMON_NAMES = {
         "BN": _("Brunei"),
         "BO": _("Bolivia"),
+        "FM": _("Micronesia"),
         "GB": _("United Kingdom"),
         "IR": _("Iran"),
         "KP": _("North Korea"),
         "KR": _("South Korea"),
         "LA": _("Laos"),
         "MD": _("Moldova"),
         "RU": _("Russia"),
```

### Comparing `django-countries-7.6/django_countries/conf.py` & `django-countries-7.6.1/django_countries/conf.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/data.py` & `django-countries-7.6.1/django_countries/data.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/fields.py` & `django-countries-7.6.1/django_countries/fields.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/filters.py` & `django-countries-7.6.1/django_countries/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         yield {
             "selected": value is None,
             "query_string": changelist.get_query_string({}, [self.field.name]),
             "display": _("All"),
         }
         for lookup, title in self.lookup_choices(changelist):
             if django.VERSION >= (5, 0):
-                selected = force_str(lookup) in value
+                selected = value is not None and force_str(lookup) in value
             else:
                 selected = force_str(lookup) == value
             yield {
                 "selected": selected,
                 "query_string": changelist.get_query_string(
                     {self.field.name: lookup}, []
                 ),
```

### Comparing `django-countries-7.6/django_countries/graphql/types.py` & `django-countries-7.6.1/django_countries/graphql/types.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/ioc_data.py` & `django-countries-7.6.1/django_countries/ioc_data.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/locale/af/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/af/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad en Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisië"
 
-msgid "Turkey"
-msgstr "Turkye"
-
 msgid "Turkmenistan"
 msgstr "Toerkmenië"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- en Caicoseilande"
 
 msgid "Tuvalu"
 msgstr "Toewaloe"
 
+msgid "Türkiye"
+msgstr "Turkye"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Oekraïne"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/af/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/af/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad en Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisië"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkye"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Toerkmenië"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ar/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ar/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -741,26 +741,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "ترينيداد وتوباغو"
 
 msgid "Tunisia"
 msgstr "تونس"
 
-msgid "Turkey"
-msgstr "تركيا"
-
 msgid "Turkmenistan"
 msgstr "تركمانستان"
 
 msgid "Turks and Caicos Islands"
 msgstr "جزر الترك وجايكوس"
 
 msgid "Tuvalu"
 msgstr "توفالو"
 
+msgid "Türkiye"
+msgstr "تركيا"
+
 msgid "Uganda"
 msgstr "أوغندا"
 
 msgid "Ukraine"
 msgstr "أوكرانيا"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ar/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
 msgstr "ترينيداد وتوباغو"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "تونس"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "تركيا"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "تركمانستان"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/bg/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/bg/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Тринидад и Тобаго"
 
 msgid "Tunisia"
 msgstr "Тунис"
 
-msgid "Turkey"
-msgstr "Турция"
-
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 msgid "Turks and Caicos Islands"
 msgstr "Островите Туркс и Кайкос"
 
 msgid "Tuvalu"
 msgstr "Тувалу"
 
+msgid "Türkiye"
+msgstr "Турция"
+
 msgid "Uganda"
 msgstr "Уганда"
 
 msgid "Ukraine"
 msgstr "Украйна"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/bg/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/bg/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Тринидад и Тобаго"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Тунис"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Турция"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ca/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ca/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinitat i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunísia"
 
-msgid "Turkey"
-msgstr "Turquia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Illes Turks i Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucraïna"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ca/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 msgstr "Trinitat i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunísia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turquia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/cs/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sk/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,129 +1,129 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2020-04-22 07:19+0000\n"
-"Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>\n"
-"Language-Team: Czech (http://www.transifex.com/smileychris/django-countries/"
-"language/cs/)\n"
+"PO-Revision-Date: 2020-03-26 01:43+0000\n"
+"Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
+"Language-Team: Slovak (http://www.transifex.com/smileychris/django-countries/"
+"language/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: cs\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Language: sk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Afghanistan"
-msgstr "Afghánistán"
+msgstr "Afganistan"
 
 msgid "Albania"
-msgstr "Albánie"
+msgstr "Albánsko"
 
 msgid "Algeria"
 msgstr "Alžírsko"
 
 msgid "All"
-msgstr "Vše"
+msgstr "Všetko"
 
 msgid "American Samoa"
 msgstr "Americká Samoa"
 
 msgid "Andorra"
 msgstr "Andorra"
 
 msgid "Angola"
 msgstr "Angola"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarktida"
+msgstr "Antarktída"
 
 msgid "Antigua and Barbuda"
 msgstr "Antigua a Barbuda"
 
 msgid "Argentina"
-msgstr "Argentina"
+msgstr "Argentína"
 
 msgid "Armenia"
-msgstr "Arménie"
+msgstr "Arménsko"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
-msgstr "Austrálie"
+msgstr "Austrália"
 
 msgid "Austria"
-msgstr "Rakousko"
+msgstr "Rakúsko"
 
 msgid "Azerbaijan"
-msgstr "Ázerbájdžán"
+msgstr "Azerbajdžan"
 
 msgid "Bahamas"
 msgstr "Bahamy"
 
 msgid "Bahrain"
 msgstr "Bahrajn"
 
 msgid "Bangladesh"
 msgstr "Bangladéš"
 
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Bělorusko"
+msgstr "Bielorusko"
 
 msgid "Belgium"
-msgstr "Belgie"
+msgstr "Belgicko"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
 msgid "Bermuda"
 msgstr "Bermudy"
 
 msgid "Bhutan"
-msgstr "Bhútán"
+msgstr "Bután"
 
 msgid "Bolivia"
-msgstr "Bolívie"
+msgstr "Bolívia"
 
 msgid "Bolivia (Plurinational State of)"
-msgstr "Mnohonárodní stát Bolívie"
+msgstr "Bolívia (Bolívijský mnohonárodný štát)"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Svatý Eustach a Saba"
+msgstr "Bonaire"
 
 msgid "Bosnia and Herzegovina"
 msgstr "Bosna a Hercegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Bouvetův ostrov"
+msgstr "Bouvetov ostrov"
 
 msgid "Brazil"
-msgstr "Brazílie"
+msgstr "Brazília"
 
 msgid "British Indian Ocean Territory"
-msgstr "Britské indickooceánské území"
+msgstr "Britské indickooceánske územie"
 
 msgid "Brunei"
 msgstr "Brunej"
 
 msgid "Brunei Darussalam"
-msgstr "Brunej Darussalam"
+msgstr "Brunej"
 
 msgid "Bulgaria"
 msgstr "Bulharsko"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
@@ -139,159 +139,153 @@
 msgid "Cameroon"
 msgstr "Kamerun"
 
 msgid "Canada"
 msgstr "Kanada"
 
 msgid "Cayman Islands"
-msgstr "Kajmanské ostrovy"
+msgstr "Kajmanie ostrovy"
 
 msgid "Central African Republic"
-msgstr "Středoafrická republika"
+msgstr "Stredoafrická republika"
 
 msgid "Chad"
 msgstr "Čad"
 
 msgid "Chile"
-msgstr "Chile"
+msgstr "Čile"
 
 msgid "China"
 msgstr "Čína"
 
 msgid "Christmas Island"
-msgstr "Vánoční ostrov"
+msgstr "Vianočný ostrov"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Kokosové (Keelingovy) ostrovy"
+msgstr "Kokosové ostrovy"
 
 msgid "Colombia"
-msgstr "Kolumbie"
+msgstr "Kolumbia"
 
 msgid "Comoros"
 msgstr "Komory"
 
 msgid "Congo"
 msgstr "Kongo"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Kongo, demokratická republika"
+msgstr "Kongo"
 
 msgid "Cook Islands"
-msgstr "Cookovy ostrovy"
+msgstr "Cookove ostrovy"
 
 msgid "Costa Rica"
 msgstr "Kostarika"
 
 msgid "Country"
-msgstr "Země"
+msgstr "Krajina"
 
 msgid "Croatia"
-msgstr "Chorvatsko"
+msgstr "Chorvátsko"
 
 msgid "Cuba"
 msgstr "Kuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Kypr"
+msgstr "Cyprus"
 
 msgid "Czech Republic"
 msgstr "Česká republika"
 
 msgid "Czechia"
 msgstr "Česko"
 
 msgid "Côte d'Ivoire"
-msgstr "Pobřeží Slonoviny"
+msgstr "Pobrežie Slonoviny"
 
 msgid "Denmark"
 msgstr "Dánsko"
 
 msgid "Djibouti"
 msgstr "Džibutsko"
 
 msgid "Dominica"
 msgstr "Dominika"
 
 msgid "Dominican Republic"
-msgstr "Dominikánská republika"
+msgstr "Dominikánska republika"
 
 msgid "Ecuador"
 msgstr "Ekvádor"
 
 msgid "Egypt"
 msgstr "Egypt"
 
 msgid "El Salvador"
-msgstr "Salvador"
+msgstr "Salvádor"
 
 msgid "Equatorial Guinea"
 msgstr "Rovníková Guinea"
 
 msgid "Eritrea"
 msgstr "Eritrea"
 
 msgid "Estonia"
-msgstr "Estonsko"
-
-msgid "Eswatini"
-msgstr "Eswatini"
+msgstr "Estónsko"
 
 msgid "Ethiopia"
-msgstr "Etiopie"
+msgstr "Etiópia"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Falklandské ostrovy (Malvíny)"
-
-msgid "Falkland Islands (Malvinas)"
-msgstr "Falklandy (Malvíny)"
+msgstr "Falklandy [Malvíny]"
 
 msgid "Faroe Islands"
 msgstr "Faerské ostrovy"
 
 msgid "Fiji"
 msgstr "Fidži"
 
 msgid "Finland"
-msgstr "Finsko"
+msgstr "Fínsko"
 
 msgid "France"
-msgstr "Francie"
+msgstr "Francúzsko"
 
 msgid "French Guiana"
-msgstr "Francouzská Guyana"
+msgstr "Francúzska Guyana"
 
 msgid "French Polynesia"
-msgstr "Francouzská Polynésie"
+msgstr "Francúzska Polynézia"
 
 msgid "French Southern Territories"
-msgstr "Francouzská jižní a antarktická území"
+msgstr "Francúzske južné a antarktické územia"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
-msgstr "Gambie"
+msgstr "Gambia"
 
 msgid "Georgia"
-msgstr "Gruzie"
+msgstr "Gruzínsko"
 
 msgid "Germany"
-msgstr "Německo"
+msgstr "Nemecko"
 
 msgid "Ghana"
 msgstr "Ghana"
 
 msgid "Gibraltar"
-msgstr "Gibraltar"
+msgstr "Gibraltár"
 
 msgid "Greece"
-msgstr "Řecko"
+msgstr "Grécko"
 
 msgid "Greenland"
 msgstr "Grónsko"
 
 msgid "Grenada"
 msgstr "Grenada"
 
@@ -316,330 +310,327 @@
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Heardův ostrov a McDonaldovy ostrovy"
+msgstr "Heardov ostrov"
 
 msgid "Holy See"
-msgstr "Vatikán"
+msgstr "Svätá stolica"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hongkong"
 
 msgid "Hungary"
 msgstr "Maďarsko"
 
 msgid "Iceland"
 msgstr "Island"
 
 msgid "India"
-msgstr "Indie"
+msgstr "India"
 
 msgid "Indonesia"
-msgstr "Indonésie"
+msgstr "Indonézia"
 
 msgid "Iran"
-msgstr "Írán"
+msgstr "Irán"
 
 msgid "Iran (Islamic Republic of)"
-msgstr "Íránská islámská republika"
+msgstr "Irán (Iránska islamská republika)"
 
 msgid "Iraq"
-msgstr "Irák"
+msgstr "Irak"
 
 msgid "Ireland"
-msgstr "Irsko"
+msgstr "Írsko"
 
 msgid "Isle of Man"
-msgstr "Ostrov Man"
+msgstr "Man"
 
 msgid "Israel"
 msgstr "Izrael"
 
 msgid "Italy"
-msgstr "Itálie"
+msgstr "Taliansko"
 
 msgid "Jamaica"
 msgstr "Jamajka"
 
 msgid "Japan"
 msgstr "Japonsko"
 
 msgid "Jersey"
 msgstr "Jersey"
 
 msgid "Jordan"
 msgstr "Jordánsko"
 
 msgid "Kazakhstan"
-msgstr "Kazachstán"
+msgstr "Kazachstan"
 
 msgid "Kenya"
 msgstr "Keňa"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Korea, lidově demokratická republika"
+msgstr "Kórejská ľudovodemokratická republika (Severná Kórea)"
 
 msgid "Korea (the Republic of)"
-msgstr "Korejská republika"
+msgstr "Kórejská republika (Južná Kórea)"
 
 msgid "Kuwait"
 msgstr "Kuvajt"
 
 msgid "Kyrgyzstan"
-msgstr "Kyrgyzstán"
+msgstr "Kirgizsko"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Laoská lidově demokratická republika"
+msgstr "Laos"
 
 msgid "Laos"
 msgstr "Laos"
 
 msgid "Latvia"
 msgstr "Lotyšsko"
 
 msgid "Lebanon"
 msgstr "Libanon"
 
 msgid "Lesotho"
 msgstr "Lesotho"
 
 msgid "Liberia"
-msgstr "Libérie"
+msgstr "Libéria"
 
 msgid "Libya"
-msgstr "Libye"
+msgstr "Líbya"
 
 msgid "Liechtenstein"
-msgstr "Lichtenštejnsko"
+msgstr "Lichtenštajnsko"
 
 msgid "Lithuania"
 msgstr "Litva"
 
 msgid "Luxembourg"
-msgstr "Lucembursko"
+msgstr "Luxembursko"
 
 msgid "Macao"
 msgstr "Macao"
 
 msgid "Macedonia"
-msgstr "Makedonie"
+msgstr "Macedónsko"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Makedonie, bývalá jugoslávská republika"
+msgstr "Macedónsko"
 
 msgid "Madagascar"
 msgstr "Madagaskar"
 
 msgid "Malawi"
 msgstr "Malawi"
 
 msgid "Malaysia"
-msgstr "Malajsie"
+msgstr "Malajzia"
 
 msgid "Maldives"
-msgstr "Maledivy"
+msgstr "Maldivy"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Marshallovy ostrovy"
+msgstr "Marshallove ostrovy"
 
 msgid "Martinique"
 msgstr "Martinik"
 
 msgid "Mauritania"
-msgstr "Mauritánie"
+msgstr "Mauritánia"
 
 msgid "Mauritius"
-msgstr "Mauricius"
+msgstr "Maurícius"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
 msgstr "Mexiko"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Mikronésie"
+msgstr "Mikronézia (Mikronézske federatívne štáty)"
 
 msgid "Moldova"
 msgstr "Moldavsko"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldavská republika"
+msgstr "Moldavsko"
 
 msgid "Monaco"
 msgstr "Monako"
 
 msgid "Mongolia"
 msgstr "Mongolsko"
 
 msgid "Montenegro"
-msgstr "Černá Hora"
+msgstr "Čierna Hora"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
 msgstr "Maroko"
 
 msgid "Mozambique"
-msgstr "Mosambik"
+msgstr "Mozambik"
 
 msgid "Myanmar"
-msgstr "Myanma"
+msgstr "Mjanmarsko"
 
 msgid "Namibia"
-msgstr "Namibie"
+msgstr "Namíbia"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepál"
 
 msgid "Netherlands"
-msgstr "Nizozemsko"
+msgstr "Holandsko"
 
 msgid "New Caledonia"
-msgstr "Nová Kaledonie"
+msgstr "Nová Kaledónia"
 
 msgid "New Zealand"
 msgstr "Nový Zéland"
 
 msgid "Nicaragua"
 msgstr "Nikaragua"
 
 msgid "Niger"
 msgstr "Niger"
 
 msgid "Nigeria"
-msgstr "Nigérie"
+msgstr "Nigéria"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Ostrov Norfolk"
+msgstr "Norfolk"
 
 msgid "North Korea"
-msgstr "Severní Korea"
-
-msgid "North Macedonia"
-msgstr "Severní Makedonie"
+msgstr "Severná Kórea"
 
 msgid "Northern Mariana Islands"
-msgstr "Ostrovy Severní Mariany"
+msgstr "Mariánske ostrovy"
 
 msgid "Norway"
-msgstr "Norsko"
+msgstr "Nórsko"
 
 msgid "Oman"
 msgstr "Omán"
 
 msgid "Pakistan"
-msgstr "Pákistán"
+msgstr "Pakistan"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestinské území (okupované)"
+msgstr "Palestína"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papua Nová Guinea"
+msgstr "Papua-Nová Guinea"
 
 msgid "Paraguay"
-msgstr "Paraguay"
+msgstr "Paraguaj"
 
 msgid "Peru"
 msgstr "Peru"
 
 msgid "Philippines"
 msgstr "Filipíny"
 
 msgid "Pitcairn"
 msgstr "Pitcairn"
 
 msgid "Poland"
-msgstr "Polsko"
+msgstr "Poľsko"
 
 msgid "Portugal"
 msgstr "Portugalsko"
 
 msgid "Puerto Rico"
 msgstr "Portoriko"
 
 msgid "Qatar"
 msgstr "Katar"
 
 msgid "Romania"
-msgstr "Rumunsko"
+msgstr "Rumúnsko"
 
 msgid "Russia"
 msgstr "Rusko"
 
 msgid "Russian Federation"
-msgstr "Ruská federace"
+msgstr "Ruská federácia"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Réunion"
 msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Svatý Bartoloměj"
+msgstr "Svätý Bartolomej"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Svatá Helena, Ascension a Tristan da Cunha"
+msgstr "Svätá Helena, Ascension a Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Svatý Kryštof a Nevis"
+msgstr "Svätý Krištof a Nevis"
 
 msgid "Saint Lucia"
-msgstr "Svatá Lucie"
+msgstr "Svätá Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Svatý Martin (francouzská část)"
+msgstr "Svätý Martin (francúzska časť)"
 
 msgid "Saint Pierre and Miquelon"
 msgstr "Saint Pierre a Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Svatý Vincenc a Grenadiny"
+msgstr "Svätý Vincent a Grenadíny"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
-msgstr "San Marino"
+msgstr "San Maríno"
 
 msgid "Sao Tome and Principe"
-msgstr "Svatý Tomáš a Princův ostrov"
+msgstr "Svätý Tomáš a Princov ostrov"
 
 msgid "Saudi Arabia"
-msgstr "Saúdská Arábie"
+msgstr "Saudská Arábia"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
 msgstr "Srbsko"
 
@@ -649,90 +640,87 @@
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
 msgstr "Singapur"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Svatý Martin (nizozemská část)"
+msgstr "Svätý Martin (holandská časť)"
 
 msgid "Slovakia"
 msgstr "Slovensko"
 
 msgid "Slovenia"
 msgstr "Slovinsko"
 
 msgid "Solomon Islands"
-msgstr "Šalomounovy ostrovy"
+msgstr "Šalamúnove ostrovy"
 
 msgid "Somalia"
 msgstr "Somálsko"
 
 msgid "South Africa"
-msgstr "Jižní Afrika"
+msgstr "Južná Afrika"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Jižní Georgie a Jižní Sandwichovy ostrovy"
+msgstr "Južná Georgia a Južné Sandwichove ostrovy"
 
 msgid "South Korea"
-msgstr "Jižní Korea"
+msgstr "Južná Kórea"
 
 msgid "South Sudan"
-msgstr "Jižní Súdán"
+msgstr "Južný Sudán"
 
 msgid "Spain"
-msgstr "Španělsko"
+msgstr "Španielsko"
 
 msgid "Sri Lanka"
 msgstr "Srí Lanka"
 
 msgid "Sudan"
-msgstr "Súdán"
+msgstr "Sudán"
 
 msgid "Suriname"
 msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
 msgstr "Svalbard a Jan Mayen"
 
 msgid "Swaziland"
 msgstr "Svazijsko"
 
 msgid "Sweden"
 msgstr "Švédsko"
 
 msgid "Switzerland"
-msgstr "Švýcarsko"
+msgstr "Švajčiarsko"
 
 msgid "Syria"
-msgstr "Sýrie"
+msgstr "Sýria"
 
 msgid "Syrian Arab Republic"
-msgstr "Syrská arabská republika"
+msgstr "Sýria"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Tchaj-wan (čínská provincie)"
+msgstr "Taiwan"
 
 msgid "Tajikistan"
-msgstr "Tádžikistán"
+msgstr "Tadžikistan"
 
 msgid "Tanzania"
-msgstr "Tanzánie"
-
-msgid "Tanzania, the United Republic of"
-msgstr "Tanzanie"
+msgstr "Tanzánia"
 
 msgid "Thailand"
 msgstr "Thajsko"
 
 msgid "Timor-Leste"
-msgstr "Východní Timor"
+msgstr "Východný Timor"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
@@ -741,61 +729,61 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad a Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisko"
 
-msgid "Turkey"
-msgstr "Turecko"
-
 msgid "Turkmenistan"
-msgstr "Turkmenistán"
+msgstr "Turkménsko"
 
 msgid "Turks and Caicos Islands"
-msgstr "Ostrovy Turks a Caicos"
+msgstr "Turks a Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turecko"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
 msgstr "Spojené arabské emiráty"
 
 msgid "United Kingdom"
-msgstr "Spojené království"
+msgstr "Spojené kráľovstvo"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Spojené království Velké Británie a Severního Irska"
+msgstr "Spojené kráľovstvo Veľkej Británie a Severného Írska"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Menší odlehlé ostrovy USA"
+msgstr "Menšie odľahlé ostrovy USA"
 
 msgid "United States of America"
-msgstr "Spojené státy americké"
+msgstr "Spojené štáty americké"
 
 msgid "Uruguay"
-msgstr "Uruguay"
+msgstr "Uruguaj"
 
 msgid "Uzbekistan"
-msgstr "Uzbekistán"
+msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Bolívarovská republika Venezuela"
+msgstr "Venezuela (Venezuelská bolívarovská republika)"
 
 msgid "Viet Nam"
 msgstr "Vietnam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
@@ -805,20 +793,20 @@
 msgid "Virgin Islands (U.S.)"
 msgstr "Americké Panenské ostrovy"
 
 msgid "Wallis and Futuna"
 msgstr "Wallis a Futuna"
 
 msgid "Western Sahara"
-msgstr "Západní Sahara"
+msgstr "Západná Sahara"
 
 msgid "Yemen"
 msgstr "Jemen"
 
 msgid "Zambia"
-msgstr "Zambie"
+msgstr "Zambia"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "Åland Islands"
-msgstr "Alandy"
+msgstr "Ålandy"
```

### Comparing `django-countries-7.6/django_countries/locale/cs/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
 msgstr "Trinidad a Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisko"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turecko"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistán"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/da/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/da/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -737,26 +737,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad og Tobago"
 
 msgid "Tunisia"
 msgstr "Tunesien"
 
-msgid "Turkey"
-msgstr "Tyrkiet"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- og Caicosøerne"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Tyrkiet"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraine"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/da/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/da/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad og Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunesien"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Tyrkiet"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/de/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/de/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -731,26 +731,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad und Tobago"
 
 msgid "Tunisia"
 msgstr "Tunesien"
 
-msgid "Turkey"
-msgstr "Türkei"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- und Caicosinseln"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Türkei"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraine"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/de/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
 msgstr "Trinidad und Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunesien"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Türkei"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/el/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/el/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -731,26 +731,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Τρινιδάδ και Τομπάγκο"
 
 msgid "Tunisia"
 msgstr "Τυνησία"
 
-msgid "Turkey"
-msgstr "Τουρκία"
-
 msgid "Turkmenistan"
 msgstr "Τουρκμενιστάν"
 
 msgid "Turks and Caicos Islands"
 msgstr "Νήσοι Τερκς και Κάικος"
 
 msgid "Tuvalu"
 msgstr "Τουβαλού"
 
+msgid "Türkiye"
+msgstr "Τουρκία"
+
 msgid "Uganda"
 msgstr "Ουγκάντα"
 
 msgid "Ukraine"
 msgstr "Ουκρανία"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/el/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Τρινιδάδ και Τομπάγκο"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Τυνησία"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Τουρκία"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Τουρκμενιστάν"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/en@test/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/en@test/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/locale/eo/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/eo/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidado kaj Tobago"
 
 msgid "Tunisia"
 msgstr "Tunizio"
 
-msgid "Turkey"
-msgstr "Turkio"
-
 msgid "Turkmenistan"
 msgstr "Turkmenio"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turkoj kaj Kajkoj"
 
 msgid "Tuvalu"
 msgstr "Tuvalo"
 
+msgid "Türkiye"
+msgstr "Turkio"
+
 msgid "Uganda"
 msgstr "Ugando"
 
 msgid "Ukraine"
 msgstr "Ukrainio"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/eo/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/eo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
 msgstr "Trinidado kaj Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunizio"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkio"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenio"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/es/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/es/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad yTobago"
 
 msgid "Tunisia"
 msgstr "Túnez"
 
-msgid "Turkey"
-msgstr "Turquía"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistán"
 
 msgid "Turks and Caicos Islands"
 msgstr "Islas Turcas y Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquía"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucrania"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/es/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1008,15 +1008,15 @@
 msgstr "Trinidad yTobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Túnez"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turquía"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistán"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/et/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/et/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad ja Tobago"
 
 msgid "Tunisia"
 msgstr "Tuneesia"
 
-msgid "Turkey"
-msgstr "Türgi"
-
 msgid "Turkmenistan"
 msgstr "Türkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turksi ja Caicose saared"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Türgi"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/et/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/et/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 msgstr "Trinidad ja Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tuneesia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Türgi"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Türkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/eu/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Basque (http://www.transifex.com/smileychris/django-countries/"
-"language/eu/)\n"
+"Language-Team: Basque (Spain) (http://www.transifex.com/smileychris/django-"
+"countries/language/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: eu\n"
+"Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad eta Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Turkia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turk eta Caico uharteak"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turkia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/eu/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/eu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad eta Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/eu_ES/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/eu/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Basque (Spain) (http://www.transifex.com/smileychris/django-"
-"countries/language/eu_ES/)\n"
+"Language-Team: Basque (http://www.transifex.com/smileychris/django-countries/"
+"language/eu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: eu_ES\n"
+"Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Afghanistan"
 msgstr "Afganistan"
 
 msgid "Albania"
 msgstr "Albania"
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad eta Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Turkia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turk eta Caico uharteak"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turkia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/eu_ES/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad eta Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/fa/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/fa/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "ترینیداد و توباگو"
 
 msgid "Tunisia"
 msgstr "تونس"
 
-msgid "Turkey"
-msgstr "ترکیه"
-
 msgid "Turkmenistan"
 msgstr "ترکمنستان"
 
 msgid "Turks and Caicos Islands"
 msgstr "جزایر تورکس و کایکوس"
 
 msgid "Tuvalu"
 msgstr "تووالو"
 
+msgid "Türkiye"
+msgstr "ترکیه"
+
 msgid "Uganda"
 msgstr "اوگاندا"
 
 msgid "Ukraine"
 msgstr "اوکراین"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/fa/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/fa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 msgstr "ترینیداد و توباگو"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "تونس"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "ترکیه"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "ترکمنستان"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/fi/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/fi/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -732,26 +732,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad ja Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Turkki"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- ja Caicossaaret"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turkki"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/fi/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/fi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 msgstr "Trinidad ja Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkki"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/fr/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/fr/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad et Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisie"
 
-msgid "Turkey"
-msgstr "Turquie"
-
 msgid "Turkmenistan"
 msgstr "Turkménistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Îles Turques-et-Caïques"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquie"
+
 msgid "Uganda"
 msgstr "Ouganda"
 
 msgid "Ukraine"
 msgstr "Ukraine"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/fr/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
 msgstr "Trinidad et Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisie"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turquie"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkménistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/he/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/he_IL/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Hebrew (http://www.transifex.com/smileychris/django-countries/"
-"language/he/)\n"
+"Language-Team: Hebrew (Israel) (http://www.transifex.com/smileychris/django-"
+"countries/language/he_IL/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: he\n"
+"Language: he_IL\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "Afghanistan"
 msgstr "אפגניסטן"
 
 msgid "Albania"
@@ -729,26 +729,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "טרינידד וטובגו"
 
 msgid "Tunisia"
 msgstr "טוניסיה"
 
-msgid "Turkey"
-msgstr "טורקיה"
-
 msgid "Turkmenistan"
 msgstr "טורקמניסטן"
 
 msgid "Turks and Caicos Islands"
 msgstr "איי טורקס וקאיקוס"
 
 msgid "Tuvalu"
 msgstr "טובאלו"
 
+msgid "Türkiye"
+msgstr "טורקיה"
+
 msgid "Uganda"
 msgstr "אוגנדה"
 
 msgid "Ukraine"
 msgstr "אוקראינה"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/he/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/he/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "טרינידד וטובגו"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "טוניסיה"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "טורקיה"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "טורקמניסטן"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/he_IL/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/he/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Hebrew (Israel) (http://www.transifex.com/smileychris/django-"
-"countries/language/he_IL/)\n"
+"Language-Team: Hebrew (http://www.transifex.com/smileychris/django-countries/"
+"language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: he_IL\n"
+"Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "Afghanistan"
 msgstr "אפגניסטן"
 
 msgid "Albania"
@@ -729,26 +729,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "טרינידד וטובגו"
 
 msgid "Tunisia"
 msgstr "טוניסיה"
 
-msgid "Turkey"
-msgstr "טורקיה"
-
 msgid "Turkmenistan"
 msgstr "טורקמניסטן"
 
 msgid "Turks and Caicos Islands"
 msgstr "איי טורקס וקאיקוס"
 
 msgid "Tuvalu"
 msgstr "טובאלו"
 
+msgid "Türkiye"
+msgstr "טורקיה"
+
 msgid "Uganda"
 msgstr "אוגנדה"
 
 msgid "Ukraine"
 msgstr "אוקראינה"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/he_IL/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/he_IL/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "טרינידד וטובגו"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "טוניסיה"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "טורקיה"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "טורקמניסטן"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/hr/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/hr/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -732,26 +732,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunis"
 
-msgid "Turkey"
-msgstr "Turska"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Otoci Turks i Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turska"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/hr/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/hr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 msgstr "Trinidad i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunis"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turska"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/hu/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/hu/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad és Tobago"
 
 msgid "Tunisia"
 msgstr "Tunézia"
 
-msgid "Turkey"
-msgstr "Törökország"
-
 msgid "Turkmenistan"
 msgstr "Türkmenisztán"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- és Caicos-szigetek"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Törökország"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajna"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/hu/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/hu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 msgstr "Trinidad és Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunézia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Törökország"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Türkmenisztán"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/hy/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/hy/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Տրինիդադ և Տոբագո"
 
 msgid "Tunisia"
 msgstr "Թունիս"
 
-msgid "Turkey"
-msgstr "Թուրքիա"
-
 msgid "Turkmenistan"
 msgstr "Թուրքմենստան"
 
 msgid "Turks and Caicos Islands"
 msgstr "Թուրքեր և Կայկոս կղզիներ"
 
 msgid "Tuvalu"
 msgstr "Թուվալու"
 
+msgid "Türkiye"
+msgstr "Թուրքիա"
+
 msgid "Uganda"
 msgstr "Ուգանդա"
 
 msgid "Ukraine"
 msgstr "Ուկրաինա"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/hy/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/hy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 msgstr "Տրինիդադ և Տոբագո"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Թունիս"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Թուրքիա"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Թուրքմենստան"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/it/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/it/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -731,26 +731,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad e Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Turchia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Isole Turks e Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turchia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/it/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
 msgstr "Trinidad e Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turchia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ja/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ja/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "トリニダード・トバゴ"
 
 msgid "Tunisia"
 msgstr "チュニジア"
 
-msgid "Turkey"
-msgstr "トルコ"
-
 msgid "Turkmenistan"
 msgstr "トルクメニスタン"
 
 msgid "Turks and Caicos Islands"
 msgstr "タークス・カイコス諸島"
 
 msgid "Tuvalu"
 msgstr "ツバル"
 
+msgid "Türkiye"
+msgstr "トルコ"
+
 msgid "Uganda"
 msgstr "ウガンダ"
 
 msgid "Ukraine"
 msgstr "ウクライナ"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ja/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ja/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
 msgstr "トリニダード・トバゴ"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "チュニジア"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "トルコ"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "トルクメニスタン"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ko_KR/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "트리니다드토바고"
 
 msgid "Tunisia"
 msgstr "튀니지"
 
-msgid "Turkey"
-msgstr "터키"
-
 msgid "Turkmenistan"
 msgstr "투르크메니스탄"
 
 msgid "Turks and Caicos Islands"
 msgstr "터크스 케이커스 제도"
 
 msgid "Tuvalu"
 msgstr "투발루"
 
+msgid "Türkiye"
+msgstr "터키"
+
 msgid "Uganda"
 msgstr "우간다"
 
 msgid "Ukraine"
 msgstr "우크라이나"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ko_KR/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 msgstr "트리니다드토바고"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "튀니지"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "터키"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "투르크메니스탄"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/lt/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/lt/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -730,26 +730,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidadas ir Tobagas"
 
 msgid "Tunisia"
 msgstr "Tunisas"
 
-msgid "Turkey"
-msgstr "Turkija"
-
 msgid "Turkmenistan"
 msgstr "Turkmėnija"
 
 msgid "Turks and Caicos Islands"
 msgstr "Terksas ir Kaikosas"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turkija"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/lt/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/lt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 msgstr "Trinidadas ir Tobagas"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisas"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkija"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmėnija"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/lv/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/lv/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -729,26 +729,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidāda un Tobāgo"
 
 msgid "Tunisia"
 msgstr "Tunisija"
 
-msgid "Turkey"
-msgstr "Turcija"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistāna"
 
 msgid "Turks and Caicos Islands"
 msgstr "Tērksas un Kaikosas"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turcija"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/lv/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/lv/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidāda un Tobāgo"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisija"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turcija"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistāna"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/mn/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/mn/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -737,26 +737,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Тринидад Тобаго"
 
 msgid "Tunisia"
 msgstr "Тунис"
 
-msgid "Turkey"
-msgstr "Турк"
-
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 msgid "Turks and Caicos Islands"
 msgstr "Турк ба Кайкосын Арлууд"
 
 msgid "Tuvalu"
 msgstr "Тувалу"
 
+msgid "Türkiye"
+msgstr "Турк"
+
 msgid "Uganda"
 msgstr "Уганда"
 
 msgid "Ukraine"
 msgstr "Украин"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/mn/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/mn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 msgstr "Тринидад Тобаго"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Тунис"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Турк"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/nb/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/nb/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -737,26 +737,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad og Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Tyrkia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks- og Caicosøyene"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Tyrkia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/nb/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1004,15 +1004,15 @@
 msgstr "Trinidad og Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Tyrkia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/nl/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/nl/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2020-08-06 01:04+0000\n"
-"Last-Translator: Robin van der Vliet <info@robinvandervliet.nl>\n"
-"Language-Team: Dutch (http://www.transifex.com/smileychris/django-countries/"
+"PO-Revision-Date: 2011-06-05 21:30+0000\n"
+"Last-Translator: Jieter Waagmeester, 2024\n"
+"Language-Team: Dutch (http://app.transifex.com/smileychris/django-countries/"
 "language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -687,15 +687,15 @@
 msgid "Sudan"
 msgstr "Soedan"
 
 msgid "Suriname"
 msgstr "Suriname"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Jan Mayen"
+msgstr "Spitsbergen en Jan Mayen"
 
 msgid "Swaziland"
 msgstr "Swaziland"
 
 msgid "Sweden"
 msgstr "Zweden"
```

### Comparing `django-countries-7.6/django_countries/locale/nl/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/nl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Bart de Goede <bart@dispectu.com>, 2013
 # tijs <hello@tijs.org>, 2014
+# Jieter Waagmeester, 2024
 # Remco Wendt <remco.wendt@gmail.com>, 2015
 # Rik Smit <riksmithh@gmail.com>, 2017
-# Robin van der Vliet <info@robinvandervliet.nl>, 2020
+# Robin van der Vliet <info@robinvandervliet.com>, 2020
 # 30074767d5368eda142c1e994fd2139d, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-03-26 14:14+1300\n"
-"PO-Revision-Date: 2020-08-06 01:04+0000\n"
-"Last-Translator: Robin van der Vliet <info@robinvandervliet.nl>\n"
-"Language-Team: Dutch (http://www.transifex.com/smileychris/django-countries/language/nl/)\n"
+"PO-Revision-Date: 2011-06-05 21:30+0000\n"
+"Last-Translator: Jieter Waagmeester, 2024\n"
+"Language-Team: Dutch (http://app.transifex.com/smileychris/django-countries/language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: base.py:11
@@ -953,15 +954,15 @@
 
 #: data.py:244
 msgid "Suriname"
 msgstr "Suriname"
 
 #: data.py:245
 msgid "Svalbard and Jan Mayen"
-msgstr "Jan Mayen"
+msgstr "Spitsbergen en Jan Mayen"
 
 #: data.py:246
 msgid "Sweden"
 msgstr "Zweden"
 
 #: data.py:247
 msgid "Switzerland"
```

### Comparing `django-countries-7.6/django_countries/locale/pl/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/pl/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -733,26 +733,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trynidad i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunezja"
 
-msgid "Turkey"
-msgstr "Turcja"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks i Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turcja"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/pl/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/pl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
 msgstr "Trynidad i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunezja"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turcja"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/pt_BR/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -742,26 +742,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad e Tobago"
 
 msgid "Tunisia"
 msgstr "Tunísia"
 
-msgid "Turkey"
-msgstr "Turquia"
-
 msgid "Turkmenistan"
 msgstr "Turcomenistão"
 
 msgid "Turks and Caicos Islands"
 msgstr "Ilhas Turks e Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucrânia"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/pt_BR/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1006,15 +1006,15 @@
 msgstr "Trinidad e Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunísia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turquia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turcomenistão"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/pt_PT/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidade e Tobago"
 
 msgid "Tunisia"
 msgstr "Tunísia"
 
-msgid "Turkey"
-msgstr "Turquia"
-
 msgid "Turkmenistan"
 msgstr "Turcomenistão"
 
 msgid "Turks and Caicos Islands"
 msgstr "Ilhas Turks e Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turquia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucrânia"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/pt_PT/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 msgstr "Trinidade e Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunísia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turquia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turcomenistão"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ro/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ro/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -729,26 +729,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad şi Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
-msgid "Turkey"
-msgstr "Turcia"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Insulele Turks şi Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turcia"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ucraina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ro/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad şi Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisia"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turcia"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/ru/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/ru/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -742,26 +742,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Тринидад и Тобаго"
 
 msgid "Tunisia"
 msgstr "Тунис"
 
-msgid "Turkey"
-msgstr "Турция"
-
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 msgid "Turks and Caicos Islands"
 msgstr "Острова Теркс и Кайкос"
 
 msgid "Tuvalu"
 msgstr "Тувалу"
 
+msgid "Türkiye"
+msgstr "Турция"
+
 msgid "Uganda"
 msgstr "Уганда"
 
 msgid "Ukraine"
 msgstr "Украина"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/ru/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
 msgstr "Тринидад и Тобаго"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Тунис"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Турция"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sk/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/cs/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,129 +1,129 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2020-03-26 01:43+0000\n"
-"Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Slovak (http://www.transifex.com/smileychris/django-countries/"
-"language/sk/)\n"
+"PO-Revision-Date: 2020-04-22 07:19+0000\n"
+"Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>\n"
+"Language-Team: Czech (http://www.transifex.com/smileychris/django-countries/"
+"language/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: cs\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "Afghanistan"
-msgstr "Afganistan"
+msgstr "Afghánistán"
 
 msgid "Albania"
-msgstr "Albánsko"
+msgstr "Albánie"
 
 msgid "Algeria"
 msgstr "Alžírsko"
 
 msgid "All"
-msgstr "Všetko"
+msgstr "Vše"
 
 msgid "American Samoa"
 msgstr "Americká Samoa"
 
 msgid "Andorra"
 msgstr "Andorra"
 
 msgid "Angola"
 msgstr "Angola"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarktída"
+msgstr "Antarktida"
 
 msgid "Antigua and Barbuda"
 msgstr "Antigua a Barbuda"
 
 msgid "Argentina"
-msgstr "Argentína"
+msgstr "Argentina"
 
 msgid "Armenia"
-msgstr "Arménsko"
+msgstr "Arménie"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
-msgstr "Austrália"
+msgstr "Austrálie"
 
 msgid "Austria"
-msgstr "Rakúsko"
+msgstr "Rakousko"
 
 msgid "Azerbaijan"
-msgstr "Azerbajdžan"
+msgstr "Ázerbájdžán"
 
 msgid "Bahamas"
 msgstr "Bahamy"
 
 msgid "Bahrain"
 msgstr "Bahrajn"
 
 msgid "Bangladesh"
 msgstr "Bangladéš"
 
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Bielorusko"
+msgstr "Bělorusko"
 
 msgid "Belgium"
-msgstr "Belgicko"
+msgstr "Belgie"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
 msgid "Bermuda"
 msgstr "Bermudy"
 
 msgid "Bhutan"
-msgstr "Bután"
+msgstr "Bhútán"
 
 msgid "Bolivia"
-msgstr "Bolívia"
+msgstr "Bolívie"
 
 msgid "Bolivia (Plurinational State of)"
-msgstr "Bolívia (Bolívijský mnohonárodný štát)"
+msgstr "Mnohonárodní stát Bolívie"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire"
+msgstr "Bonaire, Svatý Eustach a Saba"
 
 msgid "Bosnia and Herzegovina"
 msgstr "Bosna a Hercegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Bouvetov ostrov"
+msgstr "Bouvetův ostrov"
 
 msgid "Brazil"
-msgstr "Brazília"
+msgstr "Brazílie"
 
 msgid "British Indian Ocean Territory"
-msgstr "Britské indickooceánske územie"
+msgstr "Britské indickooceánské území"
 
 msgid "Brunei"
 msgstr "Brunej"
 
 msgid "Brunei Darussalam"
-msgstr "Brunej"
+msgstr "Brunej Darussalam"
 
 msgid "Bulgaria"
 msgstr "Bulharsko"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
@@ -139,153 +139,159 @@
 msgid "Cameroon"
 msgstr "Kamerun"
 
 msgid "Canada"
 msgstr "Kanada"
 
 msgid "Cayman Islands"
-msgstr "Kajmanie ostrovy"
+msgstr "Kajmanské ostrovy"
 
 msgid "Central African Republic"
-msgstr "Stredoafrická republika"
+msgstr "Středoafrická republika"
 
 msgid "Chad"
 msgstr "Čad"
 
 msgid "Chile"
-msgstr "Čile"
+msgstr "Chile"
 
 msgid "China"
 msgstr "Čína"
 
 msgid "Christmas Island"
-msgstr "Vianočný ostrov"
+msgstr "Vánoční ostrov"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Kokosové ostrovy"
+msgstr "Kokosové (Keelingovy) ostrovy"
 
 msgid "Colombia"
-msgstr "Kolumbia"
+msgstr "Kolumbie"
 
 msgid "Comoros"
 msgstr "Komory"
 
 msgid "Congo"
 msgstr "Kongo"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Kongo"
+msgstr "Kongo, demokratická republika"
 
 msgid "Cook Islands"
-msgstr "Cookove ostrovy"
+msgstr "Cookovy ostrovy"
 
 msgid "Costa Rica"
 msgstr "Kostarika"
 
 msgid "Country"
-msgstr "Krajina"
+msgstr "Země"
 
 msgid "Croatia"
-msgstr "Chorvátsko"
+msgstr "Chorvatsko"
 
 msgid "Cuba"
 msgstr "Kuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Cyprus"
+msgstr "Kypr"
 
 msgid "Czech Republic"
 msgstr "Česká republika"
 
 msgid "Czechia"
 msgstr "Česko"
 
 msgid "Côte d'Ivoire"
-msgstr "Pobrežie Slonoviny"
+msgstr "Pobřeží Slonoviny"
 
 msgid "Denmark"
 msgstr "Dánsko"
 
 msgid "Djibouti"
 msgstr "Džibutsko"
 
 msgid "Dominica"
 msgstr "Dominika"
 
 msgid "Dominican Republic"
-msgstr "Dominikánska republika"
+msgstr "Dominikánská republika"
 
 msgid "Ecuador"
 msgstr "Ekvádor"
 
 msgid "Egypt"
 msgstr "Egypt"
 
 msgid "El Salvador"
-msgstr "Salvádor"
+msgstr "Salvador"
 
 msgid "Equatorial Guinea"
 msgstr "Rovníková Guinea"
 
 msgid "Eritrea"
 msgstr "Eritrea"
 
 msgid "Estonia"
-msgstr "Estónsko"
+msgstr "Estonsko"
+
+msgid "Eswatini"
+msgstr "Eswatini"
 
 msgid "Ethiopia"
-msgstr "Etiópia"
+msgstr "Etiopie"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Falklandy [Malvíny]"
+msgstr "Falklandské ostrovy (Malvíny)"
+
+msgid "Falkland Islands (Malvinas)"
+msgstr "Falklandy (Malvíny)"
 
 msgid "Faroe Islands"
 msgstr "Faerské ostrovy"
 
 msgid "Fiji"
 msgstr "Fidži"
 
 msgid "Finland"
-msgstr "Fínsko"
+msgstr "Finsko"
 
 msgid "France"
-msgstr "Francúzsko"
+msgstr "Francie"
 
 msgid "French Guiana"
-msgstr "Francúzska Guyana"
+msgstr "Francouzská Guyana"
 
 msgid "French Polynesia"
-msgstr "Francúzska Polynézia"
+msgstr "Francouzská Polynésie"
 
 msgid "French Southern Territories"
-msgstr "Francúzske južné a antarktické územia"
+msgstr "Francouzská jižní a antarktická území"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
-msgstr "Gambia"
+msgstr "Gambie"
 
 msgid "Georgia"
-msgstr "Gruzínsko"
+msgstr "Gruzie"
 
 msgid "Germany"
-msgstr "Nemecko"
+msgstr "Německo"
 
 msgid "Ghana"
 msgstr "Ghana"
 
 msgid "Gibraltar"
-msgstr "Gibraltár"
+msgstr "Gibraltar"
 
 msgid "Greece"
-msgstr "Grécko"
+msgstr "Řecko"
 
 msgid "Greenland"
 msgstr "Grónsko"
 
 msgid "Grenada"
 msgstr "Grenada"
 
@@ -310,327 +316,330 @@
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Heardov ostrov"
+msgstr "Heardův ostrov a McDonaldovy ostrovy"
 
 msgid "Holy See"
-msgstr "Svätá stolica"
+msgstr "Vatikán"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hongkong"
 
 msgid "Hungary"
 msgstr "Maďarsko"
 
 msgid "Iceland"
 msgstr "Island"
 
 msgid "India"
-msgstr "India"
+msgstr "Indie"
 
 msgid "Indonesia"
-msgstr "Indonézia"
+msgstr "Indonésie"
 
 msgid "Iran"
-msgstr "Irán"
+msgstr "Írán"
 
 msgid "Iran (Islamic Republic of)"
-msgstr "Irán (Iránska islamská republika)"
+msgstr "Íránská islámská republika"
 
 msgid "Iraq"
-msgstr "Irak"
+msgstr "Irák"
 
 msgid "Ireland"
-msgstr "Írsko"
+msgstr "Irsko"
 
 msgid "Isle of Man"
-msgstr "Man"
+msgstr "Ostrov Man"
 
 msgid "Israel"
 msgstr "Izrael"
 
 msgid "Italy"
-msgstr "Taliansko"
+msgstr "Itálie"
 
 msgid "Jamaica"
 msgstr "Jamajka"
 
 msgid "Japan"
 msgstr "Japonsko"
 
 msgid "Jersey"
 msgstr "Jersey"
 
 msgid "Jordan"
 msgstr "Jordánsko"
 
 msgid "Kazakhstan"
-msgstr "Kazachstan"
+msgstr "Kazachstán"
 
 msgid "Kenya"
 msgstr "Keňa"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Kórejská ľudovodemokratická republika (Severná Kórea)"
+msgstr "Korea, lidově demokratická republika"
 
 msgid "Korea (the Republic of)"
-msgstr "Kórejská republika (Južná Kórea)"
+msgstr "Korejská republika"
 
 msgid "Kuwait"
 msgstr "Kuvajt"
 
 msgid "Kyrgyzstan"
-msgstr "Kirgizsko"
+msgstr "Kyrgyzstán"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Laos"
+msgstr "Laoská lidově demokratická republika"
 
 msgid "Laos"
 msgstr "Laos"
 
 msgid "Latvia"
 msgstr "Lotyšsko"
 
 msgid "Lebanon"
 msgstr "Libanon"
 
 msgid "Lesotho"
 msgstr "Lesotho"
 
 msgid "Liberia"
-msgstr "Libéria"
+msgstr "Libérie"
 
 msgid "Libya"
-msgstr "Líbya"
+msgstr "Libye"
 
 msgid "Liechtenstein"
-msgstr "Lichtenštajnsko"
+msgstr "Lichtenštejnsko"
 
 msgid "Lithuania"
 msgstr "Litva"
 
 msgid "Luxembourg"
-msgstr "Luxembursko"
+msgstr "Lucembursko"
 
 msgid "Macao"
 msgstr "Macao"
 
 msgid "Macedonia"
-msgstr "Macedónsko"
+msgstr "Makedonie"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Macedónsko"
+msgstr "Makedonie, bývalá jugoslávská republika"
 
 msgid "Madagascar"
 msgstr "Madagaskar"
 
 msgid "Malawi"
 msgstr "Malawi"
 
 msgid "Malaysia"
-msgstr "Malajzia"
+msgstr "Malajsie"
 
 msgid "Maldives"
-msgstr "Maldivy"
+msgstr "Maledivy"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Marshallove ostrovy"
+msgstr "Marshallovy ostrovy"
 
 msgid "Martinique"
 msgstr "Martinik"
 
 msgid "Mauritania"
-msgstr "Mauritánia"
+msgstr "Mauritánie"
 
 msgid "Mauritius"
-msgstr "Maurícius"
+msgstr "Mauricius"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
 msgstr "Mexiko"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Mikronézia (Mikronézske federatívne štáty)"
+msgstr "Mikronésie"
 
 msgid "Moldova"
 msgstr "Moldavsko"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldavsko"
+msgstr "Moldavská republika"
 
 msgid "Monaco"
 msgstr "Monako"
 
 msgid "Mongolia"
 msgstr "Mongolsko"
 
 msgid "Montenegro"
-msgstr "Čierna Hora"
+msgstr "Černá Hora"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
 msgstr "Maroko"
 
 msgid "Mozambique"
-msgstr "Mozambik"
+msgstr "Mosambik"
 
 msgid "Myanmar"
-msgstr "Mjanmarsko"
+msgstr "Myanma"
 
 msgid "Namibia"
-msgstr "Namíbia"
+msgstr "Namibie"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepál"
 
 msgid "Netherlands"
-msgstr "Holandsko"
+msgstr "Nizozemsko"
 
 msgid "New Caledonia"
-msgstr "Nová Kaledónia"
+msgstr "Nová Kaledonie"
 
 msgid "New Zealand"
 msgstr "Nový Zéland"
 
 msgid "Nicaragua"
 msgstr "Nikaragua"
 
 msgid "Niger"
 msgstr "Niger"
 
 msgid "Nigeria"
-msgstr "Nigéria"
+msgstr "Nigérie"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Norfolk"
+msgstr "Ostrov Norfolk"
 
 msgid "North Korea"
-msgstr "Severná Kórea"
+msgstr "Severní Korea"
+
+msgid "North Macedonia"
+msgstr "Severní Makedonie"
 
 msgid "Northern Mariana Islands"
-msgstr "Mariánske ostrovy"
+msgstr "Ostrovy Severní Mariany"
 
 msgid "Norway"
-msgstr "Nórsko"
+msgstr "Norsko"
 
 msgid "Oman"
 msgstr "Omán"
 
 msgid "Pakistan"
-msgstr "Pakistan"
+msgstr "Pákistán"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestína"
+msgstr "Palestinské území (okupované)"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papua-Nová Guinea"
+msgstr "Papua Nová Guinea"
 
 msgid "Paraguay"
-msgstr "Paraguaj"
+msgstr "Paraguay"
 
 msgid "Peru"
 msgstr "Peru"
 
 msgid "Philippines"
 msgstr "Filipíny"
 
 msgid "Pitcairn"
 msgstr "Pitcairn"
 
 msgid "Poland"
-msgstr "Poľsko"
+msgstr "Polsko"
 
 msgid "Portugal"
 msgstr "Portugalsko"
 
 msgid "Puerto Rico"
 msgstr "Portoriko"
 
 msgid "Qatar"
 msgstr "Katar"
 
 msgid "Romania"
-msgstr "Rumúnsko"
+msgstr "Rumunsko"
 
 msgid "Russia"
 msgstr "Rusko"
 
 msgid "Russian Federation"
-msgstr "Ruská federácia"
+msgstr "Ruská federace"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Réunion"
 msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Svätý Bartolomej"
+msgstr "Svatý Bartoloměj"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Svätá Helena, Ascension a Tristan da Cunha"
+msgstr "Svatá Helena, Ascension a Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Svätý Krištof a Nevis"
+msgstr "Svatý Kryštof a Nevis"
 
 msgid "Saint Lucia"
-msgstr "Svätá Lucia"
+msgstr "Svatá Lucie"
 
 msgid "Saint Martin (French part)"
-msgstr "Svätý Martin (francúzska časť)"
+msgstr "Svatý Martin (francouzská část)"
 
 msgid "Saint Pierre and Miquelon"
 msgstr "Saint Pierre a Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Svätý Vincent a Grenadíny"
+msgstr "Svatý Vincenc a Grenadiny"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
-msgstr "San Maríno"
+msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Svätý Tomáš a Princov ostrov"
+msgstr "Svatý Tomáš a Princův ostrov"
 
 msgid "Saudi Arabia"
-msgstr "Saudská Arábia"
+msgstr "Saúdská Arábie"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
 msgstr "Srbsko"
 
@@ -640,87 +649,90 @@
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
 msgstr "Singapur"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Svätý Martin (holandská časť)"
+msgstr "Svatý Martin (nizozemská část)"
 
 msgid "Slovakia"
 msgstr "Slovensko"
 
 msgid "Slovenia"
 msgstr "Slovinsko"
 
 msgid "Solomon Islands"
-msgstr "Šalamúnove ostrovy"
+msgstr "Šalomounovy ostrovy"
 
 msgid "Somalia"
 msgstr "Somálsko"
 
 msgid "South Africa"
-msgstr "Južná Afrika"
+msgstr "Jižní Afrika"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Južná Georgia a Južné Sandwichove ostrovy"
+msgstr "Jižní Georgie a Jižní Sandwichovy ostrovy"
 
 msgid "South Korea"
-msgstr "Južná Kórea"
+msgstr "Jižní Korea"
 
 msgid "South Sudan"
-msgstr "Južný Sudán"
+msgstr "Jižní Súdán"
 
 msgid "Spain"
-msgstr "Španielsko"
+msgstr "Španělsko"
 
 msgid "Sri Lanka"
 msgstr "Srí Lanka"
 
 msgid "Sudan"
-msgstr "Sudán"
+msgstr "Súdán"
 
 msgid "Suriname"
 msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
 msgstr "Svalbard a Jan Mayen"
 
 msgid "Swaziland"
 msgstr "Svazijsko"
 
 msgid "Sweden"
 msgstr "Švédsko"
 
 msgid "Switzerland"
-msgstr "Švajčiarsko"
+msgstr "Švýcarsko"
 
 msgid "Syria"
-msgstr "Sýria"
+msgstr "Sýrie"
 
 msgid "Syrian Arab Republic"
-msgstr "Sýria"
+msgstr "Syrská arabská republika"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Taiwan"
+msgstr "Tchaj-wan (čínská provincie)"
 
 msgid "Tajikistan"
-msgstr "Tadžikistan"
+msgstr "Tádžikistán"
 
 msgid "Tanzania"
-msgstr "Tanzánia"
+msgstr "Tanzánie"
+
+msgid "Tanzania, the United Republic of"
+msgstr "Tanzanie"
 
 msgid "Thailand"
 msgstr "Thajsko"
 
 msgid "Timor-Leste"
-msgstr "Východný Timor"
+msgstr "Východní Timor"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
@@ -729,61 +741,61 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad a Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisko"
 
-msgid "Turkey"
-msgstr "Turecko"
-
 msgid "Turkmenistan"
-msgstr "Turkménsko"
+msgstr "Turkmenistán"
 
 msgid "Turks and Caicos Islands"
-msgstr "Turks a Caicos"
+msgstr "Ostrovy Turks a Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turecko"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
 msgstr "Spojené arabské emiráty"
 
 msgid "United Kingdom"
-msgstr "Spojené kráľovstvo"
+msgstr "Spojené království"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Spojené kráľovstvo Veľkej Británie a Severného Írska"
+msgstr "Spojené království Velké Británie a Severního Irska"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Menšie odľahlé ostrovy USA"
+msgstr "Menší odlehlé ostrovy USA"
 
 msgid "United States of America"
-msgstr "Spojené štáty americké"
+msgstr "Spojené státy americké"
 
 msgid "Uruguay"
-msgstr "Uruguaj"
+msgstr "Uruguay"
 
 msgid "Uzbekistan"
-msgstr "Uzbekistan"
+msgstr "Uzbekistán"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Venezuela (Venezuelská bolívarovská republika)"
+msgstr "Bolívarovská republika Venezuela"
 
 msgid "Viet Nam"
 msgstr "Vietnam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
@@ -793,20 +805,20 @@
 msgid "Virgin Islands (U.S.)"
 msgstr "Americké Panenské ostrovy"
 
 msgid "Wallis and Futuna"
 msgstr "Wallis a Futuna"
 
 msgid "Western Sahara"
-msgstr "Západná Sahara"
+msgstr "Západní Sahara"
 
 msgid "Yemen"
 msgstr "Jemen"
 
 msgid "Zambia"
-msgstr "Zambia"
+msgstr "Zambie"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "Åland Islands"
-msgstr "Ålandy"
+msgstr "Alandy"
```

### Comparing `django-countries-7.6/django_countries/locale/sk/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad a Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisko"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turecko"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkménsko"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sl/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sv/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,812 +1,811 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Slovenian (http://www.transifex.com/smileychris/django-"
-"countries/language/sl/)\n"
+"Language-Team: Swedish (http://www.transifex.com/smileychris/django-"
+"countries/language/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sl\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Language: sv\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Afghanistan"
-msgstr "Afganistan"
+msgstr "Afghanistan"
 
 msgid "Albania"
-msgstr "Albanija"
+msgstr "Albania"
 
 msgid "Algeria"
-msgstr "Alžirija"
+msgstr "Algeriet"
 
 msgid "All"
-msgstr "Vse"
+msgstr "Allt"
 
 msgid "American Samoa"
-msgstr "Ameriška Samoa"
+msgstr "American Samoa"
 
 msgid "Andorra"
-msgstr "Andora"
+msgstr "Andorra"
 
 msgid "Angola"
 msgstr "Angola"
 
 msgid "Anguilla"
-msgstr "Angvila"
+msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarktika"
+msgstr "Antarktis"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigva in Barbuda"
+msgstr "Antigua och Barbuda"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Armenia"
-msgstr "Armenija"
+msgstr "Armenien"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
-msgstr "Avstralija"
+msgstr "Australia"
 
 msgid "Austria"
-msgstr "Avstrija"
+msgstr "Österrike"
 
 msgid "Azerbaijan"
-msgstr "Azerbajdžan"
+msgstr "Azerbajdzjan"
 
 msgid "Bahamas"
-msgstr "Bahami"
+msgstr "Bahamas"
 
 msgid "Bahrain"
-msgstr "Bahrajn"
+msgstr "Bahrain"
 
 msgid "Bangladesh"
-msgstr "Bangladeš"
+msgstr "Bangladesh"
 
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Belorusija"
+msgstr "Belarus"
 
 msgid "Belgium"
-msgstr "Belgija"
+msgstr "Belgien"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
 msgid "Bermuda"
-msgstr "Bermudi"
+msgstr "Bermuda"
 
 msgid "Bhutan"
-msgstr "Butan"
+msgstr "Bhutan"
 
 msgid "Bolivia"
-msgstr "Bolivija"
+msgstr "Bolivia"
 
 msgid "Bolivia (Plurinational State of)"
-msgstr "Bolivija"
+msgstr "Bolivia (Plurinational State of)"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sint Eustatius in Saba"
+msgstr "Bonaire, Sint Eustatius och Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosna in Hercegovina"
+msgstr "Bosnien och Hercegovina"
 
 msgid "Botswana"
-msgstr "Bocvana"
+msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Bouvetov otok"
+msgstr "Bouvet Island"
 
 msgid "Brazil"
-msgstr "Brazilija"
+msgstr "Brazil"
 
 msgid "British Indian Ocean Territory"
-msgstr "Britansko ozemlje v Indijskem oceanu"
+msgstr "Brittiska territoriet i Indiska oceanen"
 
 msgid "Brunei"
-msgstr "Brunej"
+msgstr "Brunei"
 
 msgid "Brunei Darussalam"
-msgstr "Brunej"
+msgstr "Brunei"
 
 msgid "Bulgaria"
-msgstr "Bolgarija"
+msgstr "Bulgarien"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
-msgstr "Zelenortski otoki"
+msgstr "Cabo Verde"
 
 msgid "Cambodia"
-msgstr "Kambodža"
+msgstr "Cambodia"
 
 msgid "Cameroon"
 msgstr "Kamerun"
 
 msgid "Canada"
-msgstr "Kanada"
+msgstr "Canada"
 
 msgid "Cayman Islands"
-msgstr "Kajmanski otoki"
+msgstr "Caymanöarna"
 
 msgid "Central African Republic"
-msgstr "Srednjeafriška republika"
+msgstr "Centralafrikanska republiken"
 
 msgid "Chad"
-msgstr "Čad"
+msgstr "Chad"
 
 msgid "Chile"
-msgstr "Čile"
+msgstr "Chile"
 
 msgid "China"
-msgstr "Kitajska"
+msgstr "Kina"
 
 msgid "Christmas Island"
-msgstr "Velikonočni otok"
+msgstr "Julön"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Kokosovi (Keeling) otoki"
+msgstr "Cocos (Keeling) Islands"
 
 msgid "Colombia"
-msgstr "Kolumbija"
+msgstr "Colombia"
 
 msgid "Comoros"
-msgstr "Komori"
+msgstr "Komorerna"
 
 msgid "Congo"
 msgstr "Kongo"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Kongo (demokratična republika)"
+msgstr "Kongo (Demokratiska republiken)"
 
 msgid "Cook Islands"
-msgstr "Cookovi otoki"
+msgstr "Cooköarna"
 
 msgid "Costa Rica"
-msgstr "Kostarika"
+msgstr "Costa Rica"
 
 msgid "Country"
-msgstr "Država"
+msgstr "Land"
 
 msgid "Croatia"
-msgstr "Hrvaška"
+msgstr "Kroatien"
 
 msgid "Cuba"
-msgstr "Kuba"
+msgstr "Cuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Ciper"
+msgstr "Cypern"
 
 msgid "Czech Republic"
-msgstr "Češka"
+msgstr "Tjeckien"
 
 msgid "Czechia"
-msgstr "Češka"
+msgstr "Tjeckien"
 
 msgid "Côte d'Ivoire"
-msgstr "Slonokoščena obala"
+msgstr "Elfenbenskusten"
 
 msgid "Denmark"
-msgstr "Danska"
+msgstr "Danmark"
 
 msgid "Djibouti"
-msgstr "Džibuti"
+msgstr "Djibouti"
 
 msgid "Dominica"
-msgstr "Dominika"
+msgstr "Dominica"
 
 msgid "Dominican Republic"
-msgstr "Dominikanska republika"
+msgstr "Dominikanska republiken"
 
 msgid "Ecuador"
-msgstr "Ekvador"
+msgstr "Ecuador"
 
 msgid "Egypt"
-msgstr "Egipt"
+msgstr "Egypt"
 
 msgid "El Salvador"
-msgstr "Salvador"
+msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Ekvatorialna Gvineja"
+msgstr "Ekvatorialguinea"
 
 msgid "Eritrea"
-msgstr "Eritreja"
+msgstr "Eritrea"
 
 msgid "Estonia"
-msgstr "Estonija"
+msgstr "Estland"
 
 msgid "Ethiopia"
-msgstr "Etiopija"
+msgstr "Etiopien"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Falklandski otoki"
+msgstr "Falklandsöarna [Malvinas]"
 
 msgid "Faroe Islands"
-msgstr "Ferski otoki"
+msgstr "Färöarna"
 
 msgid "Fiji"
-msgstr "Fidži"
+msgstr "Fiji"
 
 msgid "Finland"
-msgstr "Finska"
+msgstr "Finland"
 
 msgid "France"
-msgstr "Francija"
+msgstr "Frankrike"
 
 msgid "French Guiana"
-msgstr "Francoska Gvajana"
+msgstr "Franska Guyana"
 
 msgid "French Polynesia"
-msgstr "Francoska Polinezija"
+msgstr "Franska Polynesien"
 
 msgid "French Southern Territories"
-msgstr "Francoska južna ozemlja"
+msgstr "Franska Sydterritorierna"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
-msgstr "Gambija"
+msgstr "Gambia"
 
 msgid "Georgia"
-msgstr "Gruzija"
+msgstr "Georgia"
 
 msgid "Germany"
-msgstr "Nemčija"
+msgstr "Tyskland"
 
 msgid "Ghana"
-msgstr "Gana"
+msgstr "Ghana"
 
 msgid "Gibraltar"
 msgstr "Gibraltar"
 
 msgid "Greece"
-msgstr "Grčija"
+msgstr "Grekland"
 
 msgid "Greenland"
-msgstr "Grenlandija"
+msgstr "Grönland"
 
 msgid "Grenada"
 msgstr "Grenada"
 
 msgid "Guadeloupe"
-msgstr "Gvadelupe"
+msgstr "Guadeloupe"
 
 msgid "Guam"
 msgstr "Guam"
 
 msgid "Guatemala"
-msgstr "Gvatemala"
+msgstr "Guatemala"
 
 msgid "Guernsey"
 msgstr "Guernsey"
 
 msgid "Guinea"
-msgstr "Gvineja"
+msgstr "Guinea"
 
 msgid "Guinea-Bissau"
-msgstr "Gvineja Bissau"
+msgstr "Guinea-Bissau"
 
 msgid "Guyana"
-msgstr "Gvajana"
+msgstr "Guyana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Otok Heard in otočje McDonald"
+msgstr "Heard Island och McDonald Islands"
 
 msgid "Holy See"
-msgstr "Sveti sedež"
+msgstr "Heliga stolen"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hong Kong"
 
 msgid "Hungary"
-msgstr "Madžarska"
+msgstr "Ungern"
 
 msgid "Iceland"
-msgstr "Islandija"
+msgstr "Island"
 
 msgid "India"
-msgstr "Indija"
+msgstr "India"
 
 msgid "Indonesia"
-msgstr "Indonezija"
+msgstr "Indonesia"
 
 msgid "Iran"
 msgstr "Iran"
 
 msgid "Iran (Islamic Republic of)"
-msgstr "Iran"
+msgstr "Iran (Islamic Republic of)"
 
 msgid "Iraq"
 msgstr "Irak"
 
 msgid "Ireland"
-msgstr "Irska"
+msgstr "Irland"
 
 msgid "Isle of Man"
-msgstr "Otok Man"
+msgstr "Isle of Man"
 
 msgid "Israel"
-msgstr "Izrael"
+msgstr "Israel"
 
 msgid "Italy"
-msgstr "Italija"
+msgstr "Italien"
 
 msgid "Jamaica"
-msgstr "Jamajka"
+msgstr "Jamaica"
 
 msgid "Japan"
-msgstr "Japonska"
+msgstr "Japan"
 
 msgid "Jersey"
 msgstr "Jersey"
 
 msgid "Jordan"
-msgstr "Jordanija"
+msgstr "Jordan"
 
 msgid "Kazakhstan"
-msgstr "Kazahstan"
+msgstr "Kazakstan"
 
 msgid "Kenya"
-msgstr "Kenija"
+msgstr "Kenya"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Severna Koreja"
+msgstr "Korea (Demokratiska folkrepubliken)"
 
 msgid "Korea (the Republic of)"
-msgstr "Južna Koreja"
+msgstr "Korea (Republiken)"
 
 msgid "Kuwait"
-msgstr "Kuvajt"
+msgstr "Kuwait"
 
 msgid "Kyrgyzstan"
 msgstr "Kirgizistan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Laos"
+msgstr "Laos Demokratiska folkrepubliken"
 
 msgid "Laos"
 msgstr "Laos"
 
 msgid "Latvia"
-msgstr "Latvija"
+msgstr "Lettland"
 
 msgid "Lebanon"
-msgstr "Libanon"
+msgstr "Lebanon"
 
 msgid "Lesotho"
-msgstr "Lesoto"
+msgstr "Lesotho"
 
 msgid "Liberia"
-msgstr "Liberija"
+msgstr "Liberia"
 
 msgid "Libya"
-msgstr "Libija"
+msgstr "Libyen"
 
 msgid "Liechtenstein"
-msgstr "Lihtenštajn"
+msgstr "Liechtenstein"
 
 msgid "Lithuania"
-msgstr "Litva"
+msgstr "Litauen"
 
 msgid "Luxembourg"
-msgstr "Luksemburg"
+msgstr "Luxemburg"
 
 msgid "Macao"
-msgstr "Macau"
+msgstr "Macao"
 
 msgid "Macedonia"
-msgstr "Severna Makedonija"
+msgstr "Makedonien"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Severna Makedonija"
+msgstr "Makedonien (fd jugoslaviska republiken)"
 
 msgid "Madagascar"
 msgstr "Madagaskar"
 
 msgid "Malawi"
-msgstr "Malavi"
+msgstr "Malawi"
 
 msgid "Malaysia"
-msgstr "Malezija"
+msgstr "Malaysia"
 
 msgid "Maldives"
-msgstr "Maldivi"
+msgstr "Maldiverna"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Maršalovi otoki"
+msgstr "Marshallöarna"
 
 msgid "Martinique"
-msgstr "Martinik"
+msgstr "Martinique"
 
 msgid "Mauritania"
-msgstr "Mavretanija"
+msgstr "Mauretanien"
 
 msgid "Mauritius"
-msgstr "Mavricij"
+msgstr "Mauritius"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
-msgstr "Mehika"
+msgstr "Mexiko"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Mikronezija"
+msgstr "Mikronesien (federationen)"
 
 msgid "Moldova"
-msgstr "Moldavija"
+msgstr "Moldavien"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldavija"
+msgstr "Moldavien (Republiken)"
 
 msgid "Monaco"
-msgstr "Monako"
+msgstr "Monaco"
 
 msgid "Mongolia"
-msgstr "Mongolija"
+msgstr "Mongoliet"
 
 msgid "Montenegro"
-msgstr "Črna gora"
+msgstr "Montenegro"
 
 msgid "Montserrat"
-msgstr "Monserat"
+msgstr "Montserrat"
 
 msgid "Morocco"
-msgstr "Maroko"
+msgstr "Marocko"
 
 msgid "Mozambique"
-msgstr "Mozambik"
+msgstr "Moçambique"
 
 msgid "Myanmar"
-msgstr "Mjanmar"
+msgstr "Myanmar"
 
 msgid "Namibia"
-msgstr "Namibija"
+msgstr "Namibia"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Nizozemska"
+msgstr "Nederländerna"
 
 msgid "New Caledonia"
-msgstr "Nova Kaledonija"
+msgstr "Nya Kaledonien"
 
 msgid "New Zealand"
-msgstr "Nova Zelandija"
+msgstr "Nya Zeeland"
 
 msgid "Nicaragua"
-msgstr "Nikaragva"
+msgstr "Nicaragua"
 
 msgid "Niger"
 msgstr "Niger"
 
 msgid "Nigeria"
-msgstr "Nigerija"
+msgstr "Nigeria"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Otok Norfolk"
+msgstr "Norfolk Island"
 
 msgid "North Korea"
-msgstr "Severna Koreja"
+msgstr "Nordkorea"
 
 msgid "Northern Mariana Islands"
-msgstr "Severni Marianski otoki"
+msgstr "Nordmarianerna"
 
 msgid "Norway"
-msgstr "Norveška"
+msgstr "Norge"
 
 msgid "Oman"
 msgstr "Oman"
 
 msgid "Pakistan"
 msgstr "Pakistan"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestina"
+msgstr "Palestina, State of"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papua Nova Gvineja"
+msgstr "Papua Nya Guinea"
 
 msgid "Paraguay"
-msgstr "Paragvaj"
+msgstr "Paraguay"
 
 msgid "Peru"
 msgstr "Peru"
 
 msgid "Philippines"
-msgstr "Filipini"
+msgstr "Philippines"
 
 msgid "Pitcairn"
-msgstr "Pitcairnovi otoki"
+msgstr "Pitcairn"
 
 msgid "Poland"
-msgstr "Polska"
+msgstr "Polen"
 
 msgid "Portugal"
-msgstr "Portugalska"
+msgstr "Portugal"
 
 msgid "Puerto Rico"
-msgstr "Portorika"
+msgstr "Puerto Rico"
 
 msgid "Qatar"
-msgstr "Katar"
+msgstr "Qatar"
 
 msgid "Romania"
-msgstr "Romunija"
+msgstr "Rumänien"
 
 msgid "Russia"
-msgstr "Rusija"
+msgstr "Ryssland"
 
 msgid "Russian Federation"
-msgstr "Ruska federacija"
+msgstr "Ryska federationen"
 
 msgid "Rwanda"
-msgstr "Ruanda"
+msgstr "Rwanda"
 
 msgid "Réunion"
-msgstr "Reunion"
+msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Saint Barthélemy"
+msgstr "Saint-Barthélemy"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Saint Helena, Ascension in Tristan da Cunha"
+msgstr "Saint Helena, Kristi himmelsfärd och Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Saint Kitts in Nevis"
+msgstr "Saint Kitts och Nevis"
 
 msgid "Saint Lucia"
 msgstr "Saint Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Saint Martin (francoski del)"
+msgstr "Saint Martin (franska delen)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Saint Pierre in Miquelon"
+msgstr "Saint Pierre och Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Saint Vincent in Grenadine"
+msgstr "Saint Vincent och Grenadinerna"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
 msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tome in Principe"
+msgstr "Sao Tomé och Principe"
 
 msgid "Saudi Arabia"
-msgstr "Saudova Arabija"
+msgstr "Saudiarabien"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
-msgstr "Srbija"
+msgstr "Serbien"
 
 msgid "Seychelles"
-msgstr "Sejšeli"
+msgstr "Seychellerna"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
-msgstr "Singapur"
+msgstr "Singapore"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sint Maarten (nizozemski del)"
+msgstr "Sint Maarten (nederländska delen)"
 
 msgid "Slovakia"
-msgstr "Slovaška"
+msgstr "Slovakien"
 
 msgid "Slovenia"
-msgstr "Slovenija"
+msgstr "Slovenien"
 
 msgid "Solomon Islands"
-msgstr "Salomonovi otoki"
+msgstr "Salomonöarna"
 
 msgid "Somalia"
-msgstr "Somalija"
+msgstr "Somalia"
 
 msgid "South Africa"
-msgstr "Južna Afrika"
+msgstr "Sydafrika"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Južna Georgia in Južni Sandwichevi otoki"
+msgstr "Sydgeorgien och Sydsandwichöarna"
 
 msgid "South Korea"
-msgstr "Južna Koreja"
+msgstr "Sydkorea"
 
 msgid "South Sudan"
-msgstr "Južni Sudan"
+msgstr "South Sudan"
 
 msgid "Spain"
-msgstr "Španija"
+msgstr "Spanien"
 
 msgid "Sri Lanka"
-msgstr "Šrilanka"
+msgstr "Sri Lanka"
 
 msgid "Sudan"
 msgstr "Sudan"
 
 msgid "Suriname"
 msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard in Jan Mayen"
+msgstr "Svalbard och Jan Mayen"
 
 msgid "Swaziland"
-msgstr "Svazi"
+msgstr "Swaziland"
 
 msgid "Sweden"
-msgstr "Švedska"
+msgstr "Sverige"
 
 msgid "Switzerland"
-msgstr "Švica"
+msgstr "Schweiz"
 
 msgid "Syria"
-msgstr "Sirija"
+msgstr "Syrien"
 
 msgid "Syrian Arab Republic"
-msgstr "Sirija"
+msgstr "Syrien"
 
 msgid "Taiwan"
-msgstr "Tajvan"
+msgstr "Taiwan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Tajvan"
+msgstr "Taiwan (provinsen i Kina)"
 
 msgid "Tajikistan"
-msgstr "Tadžikistan"
+msgstr "Tadzjikistan"
 
 msgid "Tanzania"
-msgstr "Tanzanija"
+msgstr "Tanzania"
 
 msgid "Thailand"
-msgstr "Tajska"
+msgstr "Thailand"
 
 msgid "Timor-Leste"
-msgstr "Timor"
+msgstr "Östtimor"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
 msgstr "Tonga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinidad in Tobago"
+msgstr "Trinidad och Tobago"
 
 msgid "Tunisia"
-msgstr "Tunizija"
-
-msgid "Turkey"
-msgstr "Turčija"
+msgstr "Tunisien"
 
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Otoki Turks in Caicos"
+msgstr "Turks- och Caicosöarna"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turkiet"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
-msgstr "Ukrajina"
+msgstr "Ukraina"
 
 msgid "United Arab Emirates"
-msgstr "Združeni arabski emirati"
+msgstr "Förenade Arabemiraten"
 
 msgid "United Kingdom"
-msgstr "Združeno kraljestvo"
+msgstr "Storbritannien"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Združeno kraljestvo Velike Britanije in Severne Irske"
+msgstr "Förenade konungariket Storbritannien och Nordirland"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Stranski zunanji otoki Združenih držav"
+msgstr "Förenta staternas mindre öar i Oceanien och Västindien"
 
 msgid "United States of America"
-msgstr "Združene države Amerike"
+msgstr "Amerikas förenta stater"
 
 msgid "Uruguay"
-msgstr "Urugvaj"
+msgstr "Uruguay"
 
 msgid "Uzbekistan"
 msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Venezuela"
+msgstr "Venezuela (Bolivarianska republiken)"
 
 msgid "Viet Nam"
-msgstr "Vietnam"
+msgstr "Viet Nam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
 msgid "Virgin Islands (British)"
-msgstr "Britanski Deviški otoki"
+msgstr "Jungfruöarna (Storbritannien)"
 
 msgid "Virgin Islands (U.S.)"
-msgstr "Deviški otoki"
+msgstr "Jungfruöarna (US)"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis in Futuna"
+msgstr "Wallis och Futuna"
 
 msgid "Western Sahara"
-msgstr "Zahodna Sahara"
+msgstr "Västsahara"
 
 msgid "Yemen"
 msgstr "Jemen"
 
 msgid "Zambia"
-msgstr "Zambija"
+msgstr "Zambia"
 
 msgid "Zimbabwe"
-msgstr "Zimbabve"
+msgstr "Zimbabwe"
 
 msgid "Åland Islands"
-msgstr "Alandski otoki"
+msgstr "Åland"
```

### Comparing `django-countries-7.6/django_countries/locale/sl/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad in Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunizija"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turčija"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sr/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sr/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -741,26 +741,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Тринидад и Тобаго"
 
 msgid "Tunisia"
 msgstr "Тунис"
 
-msgid "Turkey"
-msgstr "Турска"
-
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 msgid "Turks and Caicos Islands"
 msgstr "Туркс и Каикос Острва"
 
 msgid "Tuvalu"
 msgstr "Тувалу"
 
+msgid "Türkiye"
+msgstr "Турска"
+
 msgid "Uganda"
 msgstr "Уганда"
 
 msgid "Ukraine"
 msgstr "Украјина"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/sr/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Тринидад и Тобаго"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Тунис"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Турска"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Туркменистан"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sr@latin/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sr@latin/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -741,26 +741,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunis"
 
-msgid "Turkey"
-msgstr "Turska"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks i Kaikos Ostrva"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turska"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/sr@latin/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sr@latin/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 msgstr "Trinidad i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunis"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turska"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sr_Latn/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sr_Latn/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -741,26 +741,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunis"
 
-msgid "Turkey"
-msgstr "Turska"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks i Kaikos Ostrva"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turska"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/sr_Latn/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 msgstr "Trinidad i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunis"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turska"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -729,26 +729,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad i Tobago"
 
 msgid "Tunisia"
 msgstr "Tunis"
 
-msgid "Turkey"
-msgstr "Turska"
-
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Ostrva Turks i Kaikos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turska"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sr_Latn_BA/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -998,15 +998,15 @@
 msgstr "Trinidad i Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunis"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turska"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/sv/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,68 +1,68 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2020-03-26 01:43+0000\n"
-"Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Swedish (http://www.transifex.com/smileychris/django-"
-"countries/language/sv/)\n"
+"PO-Revision-Date: 2011-06-05 21:30+0000\n"
+"Last-Translator: Chinnathan Chongsujiphan, 2023\n"
+"Language-Team: Thai (Thailand) (http://app.transifex.com/smileychris/django-"
+"countries/language/th_TH/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sv\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: th_TH\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Afghanistan"
 msgstr "Afghanistan"
 
 msgid "Albania"
 msgstr "Albania"
 
 msgid "Algeria"
-msgstr "Algeriet"
+msgstr "Algeria"
 
 msgid "All"
-msgstr "Allt"
+msgstr "All"
 
 msgid "American Samoa"
 msgstr "American Samoa"
 
 msgid "Andorra"
 msgstr "Andorra"
 
 msgid "Angola"
 msgstr "Angola"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarktis"
+msgstr "Antarctica"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua och Barbuda"
+msgstr "Antigua and Barbuda"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Armenia"
-msgstr "Armenien"
+msgstr "Armenia"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
 msgstr "Australia"
 
 msgid "Austria"
-msgstr "Österrike"
+msgstr "Austria"
 
 msgid "Azerbaijan"
-msgstr "Azerbajdzjan"
+msgstr "Azerbaijan"
 
 msgid "Bahamas"
 msgstr "Bahamas"
 
 msgid "Bahrain"
 msgstr "Bahrain"
 
@@ -72,15 +72,15 @@
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
 msgstr "Belarus"
 
 msgid "Belgium"
-msgstr "Belgien"
+msgstr "Belgium"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
 msgstr "Benin"
 
@@ -93,201 +93,207 @@
 msgid "Bolivia"
 msgstr "Bolivia"
 
 msgid "Bolivia (Plurinational State of)"
 msgstr "Bolivia (Plurinational State of)"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sint Eustatius och Saba"
+msgstr "Bonaire, Sint Eustatius and Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosnien och Hercegovina"
+msgstr "Bosnia and Herzegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
 msgstr "Bouvet Island"
 
 msgid "Brazil"
 msgstr "Brazil"
 
 msgid "British Indian Ocean Territory"
-msgstr "Brittiska territoriet i Indiska oceanen"
+msgstr "British Indian Ocean Territory"
 
 msgid "Brunei"
 msgstr "Brunei"
 
 msgid "Brunei Darussalam"
-msgstr "Brunei"
+msgstr "Brunei Darussalam"
 
 msgid "Bulgaria"
-msgstr "Bulgarien"
+msgstr "Bulgaria"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
 msgstr "Cabo Verde"
 
 msgid "Cambodia"
 msgstr "Cambodia"
 
 msgid "Cameroon"
-msgstr "Kamerun"
+msgstr "Cameroon"
 
 msgid "Canada"
 msgstr "Canada"
 
 msgid "Cayman Islands"
-msgstr "Caymanöarna"
+msgstr "Cayman Islands"
 
 msgid "Central African Republic"
-msgstr "Centralafrikanska republiken"
+msgstr "Central African Republic"
 
 msgid "Chad"
 msgstr "Chad"
 
 msgid "Chile"
 msgstr "Chile"
 
 msgid "China"
-msgstr "Kina"
+msgstr "China"
 
 msgid "Christmas Island"
-msgstr "Julön"
+msgstr "Christmas Island"
 
 msgid "Cocos (Keeling) Islands"
 msgstr "Cocos (Keeling) Islands"
 
 msgid "Colombia"
 msgstr "Colombia"
 
 msgid "Comoros"
-msgstr "Komorerna"
+msgstr "Comoros"
 
 msgid "Congo"
-msgstr "Kongo"
+msgstr "Congo"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Kongo (Demokratiska republiken)"
+msgstr "Congo (the Democratic Republic of the)"
 
 msgid "Cook Islands"
-msgstr "Cooköarna"
+msgstr "Cook Islands"
 
 msgid "Costa Rica"
 msgstr "Costa Rica"
 
 msgid "Country"
-msgstr "Land"
+msgstr "Country"
 
 msgid "Croatia"
-msgstr "Kroatien"
+msgstr "Croatia"
 
 msgid "Cuba"
 msgstr "Cuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Cypern"
+msgstr "Cyprus"
 
 msgid "Czech Republic"
-msgstr "Tjeckien"
+msgstr "Czech Republic"
 
 msgid "Czechia"
-msgstr "Tjeckien"
+msgstr "Czechia"
 
 msgid "Côte d'Ivoire"
-msgstr "Elfenbenskusten"
+msgstr "Côte d'Ivoire"
 
 msgid "Denmark"
-msgstr "Danmark"
+msgstr "Denmark"
 
 msgid "Djibouti"
 msgstr "Djibouti"
 
 msgid "Dominica"
 msgstr "Dominica"
 
 msgid "Dominican Republic"
-msgstr "Dominikanska republiken"
+msgstr "Dominican Republic"
 
 msgid "Ecuador"
 msgstr "Ecuador"
 
 msgid "Egypt"
 msgstr "Egypt"
 
 msgid "El Salvador"
 msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Ekvatorialguinea"
+msgstr "Equatorial Guinea"
 
 msgid "Eritrea"
 msgstr "Eritrea"
 
 msgid "Estonia"
-msgstr "Estland"
+msgstr "Estonia"
+
+msgid "Eswatini"
+msgstr "Eswatini"
 
 msgid "Ethiopia"
-msgstr "Etiopien"
+msgstr "Ethiopia"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Falklandsöarna [Malvinas]"
+msgstr "Falkland Islands  [Malvinas]"
+
+msgid "Falkland Islands (Malvinas)"
+msgstr "Falkland Islands (Malvinas)"
 
 msgid "Faroe Islands"
-msgstr "Färöarna"
+msgstr "Faroe Islands"
 
 msgid "Fiji"
 msgstr "Fiji"
 
 msgid "Finland"
 msgstr "Finland"
 
 msgid "France"
-msgstr "Frankrike"
+msgstr "France"
 
 msgid "French Guiana"
-msgstr "Franska Guyana"
+msgstr "French Guiana"
 
 msgid "French Polynesia"
-msgstr "Franska Polynesien"
+msgstr "French Polynesia"
 
 msgid "French Southern Territories"
-msgstr "Franska Sydterritorierna"
+msgstr "French Southern Territories"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
 msgstr "Gambia"
 
 msgid "Georgia"
 msgstr "Georgia"
 
 msgid "Germany"
-msgstr "Tyskland"
+msgstr "Germany"
 
 msgid "Ghana"
 msgstr "Ghana"
 
 msgid "Gibraltar"
 msgstr "Gibraltar"
 
 msgid "Greece"
-msgstr "Grekland"
+msgstr "Greece"
 
 msgid "Greenland"
-msgstr "Grönland"
+msgstr "Greenland"
 
 msgid "Grenada"
 msgstr "Grenada"
 
 msgid "Guadeloupe"
 msgstr "Guadeloupe"
 
@@ -309,213 +315,213 @@
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Heard Island och McDonald Islands"
+msgstr "Heard Island and McDonald Islands"
 
 msgid "Holy See"
-msgstr "Heliga stolen"
+msgstr "Holy See"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
 msgstr "Hong Kong"
 
 msgid "Hungary"
-msgstr "Ungern"
+msgstr "Hungary"
 
 msgid "Iceland"
-msgstr "Island"
+msgstr "Iceland"
 
 msgid "India"
 msgstr "India"
 
 msgid "Indonesia"
 msgstr "Indonesia"
 
 msgid "Iran"
 msgstr "Iran"
 
 msgid "Iran (Islamic Republic of)"
 msgstr "Iran (Islamic Republic of)"
 
 msgid "Iraq"
-msgstr "Irak"
+msgstr "Iraq"
 
 msgid "Ireland"
-msgstr "Irland"
+msgstr "Ireland"
 
 msgid "Isle of Man"
 msgstr "Isle of Man"
 
 msgid "Israel"
 msgstr "Israel"
 
 msgid "Italy"
-msgstr "Italien"
+msgstr "Italy"
 
 msgid "Jamaica"
 msgstr "Jamaica"
 
 msgid "Japan"
 msgstr "Japan"
 
 msgid "Jersey"
 msgstr "Jersey"
 
 msgid "Jordan"
 msgstr "Jordan"
 
 msgid "Kazakhstan"
-msgstr "Kazakstan"
+msgstr "Kazakhstan"
 
 msgid "Kenya"
 msgstr "Kenya"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Korea (Demokratiska folkrepubliken)"
+msgstr "Korea (the Democratic People's Republic of)"
 
 msgid "Korea (the Republic of)"
-msgstr "Korea (Republiken)"
+msgstr "Korea (the Republic of)"
 
 msgid "Kuwait"
 msgstr "Kuwait"
 
 msgid "Kyrgyzstan"
-msgstr "Kirgizistan"
+msgstr "Kyrgyzstan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Laos Demokratiska folkrepubliken"
+msgstr "Lao People's Democratic Republic"
 
 msgid "Laos"
 msgstr "Laos"
 
 msgid "Latvia"
-msgstr "Lettland"
+msgstr "Latvia"
 
 msgid "Lebanon"
 msgstr "Lebanon"
 
 msgid "Lesotho"
 msgstr "Lesotho"
 
 msgid "Liberia"
 msgstr "Liberia"
 
 msgid "Libya"
-msgstr "Libyen"
+msgstr "Libya"
 
 msgid "Liechtenstein"
 msgstr "Liechtenstein"
 
 msgid "Lithuania"
-msgstr "Litauen"
+msgstr "Lithuania"
 
 msgid "Luxembourg"
-msgstr "Luxemburg"
+msgstr "Luxembourg"
 
 msgid "Macao"
 msgstr "Macao"
 
 msgid "Macedonia"
-msgstr "Makedonien"
+msgstr "Macedonia"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Makedonien (fd jugoslaviska republiken)"
+msgstr "Macedonia (the former Yugoslav Republic of)"
 
 msgid "Madagascar"
-msgstr "Madagaskar"
+msgstr "Madagascar"
 
 msgid "Malawi"
 msgstr "Malawi"
 
 msgid "Malaysia"
 msgstr "Malaysia"
 
 msgid "Maldives"
-msgstr "Maldiverna"
+msgstr "Maldives"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Marshallöarna"
+msgstr "Marshall Islands"
 
 msgid "Martinique"
 msgstr "Martinique"
 
 msgid "Mauritania"
-msgstr "Mauretanien"
+msgstr "Mauritania"
 
 msgid "Mauritius"
 msgstr "Mauritius"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
-msgstr "Mexiko"
+msgstr "Mexico"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Mikronesien (federationen)"
+msgstr "Micronesia (Federated States of)"
 
 msgid "Moldova"
-msgstr "Moldavien"
+msgstr "Moldova"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldavien (Republiken)"
+msgstr "Moldova (the Republic of)"
 
 msgid "Monaco"
 msgstr "Monaco"
 
 msgid "Mongolia"
-msgstr "Mongoliet"
+msgstr "Mongolia"
 
 msgid "Montenegro"
 msgstr "Montenegro"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
-msgstr "Marocko"
+msgstr "Morocco"
 
 msgid "Mozambique"
-msgstr "Moçambique"
+msgstr "Mozambique"
 
 msgid "Myanmar"
 msgstr "Myanmar"
 
 msgid "Namibia"
 msgstr "Namibia"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Nederländerna"
+msgstr "Netherlands"
 
 msgid "New Caledonia"
-msgstr "Nya Kaledonien"
+msgstr "New Caledonia"
 
 msgid "New Zealand"
-msgstr "Nya Zeeland"
+msgstr "New Zealand"
 
 msgid "Nicaragua"
 msgstr "Nicaragua"
 
 msgid "Niger"
 msgstr "Niger"
 
@@ -525,287 +531,293 @@
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
 msgstr "Norfolk Island"
 
 msgid "North Korea"
-msgstr "Nordkorea"
+msgstr "North Korea"
+
+msgid "North Macedonia"
+msgstr "North Macedonia"
 
 msgid "Northern Mariana Islands"
-msgstr "Nordmarianerna"
+msgstr "Northern Mariana Islands"
 
 msgid "Norway"
-msgstr "Norge"
+msgstr "Norway"
 
 msgid "Oman"
 msgstr "Oman"
 
 msgid "Pakistan"
 msgstr "Pakistan"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestina, State of"
+msgstr "Palestine, State of"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papua Nya Guinea"
+msgstr "Papua New Guinea"
 
 msgid "Paraguay"
 msgstr "Paraguay"
 
 msgid "Peru"
 msgstr "Peru"
 
 msgid "Philippines"
 msgstr "Philippines"
 
 msgid "Pitcairn"
 msgstr "Pitcairn"
 
 msgid "Poland"
-msgstr "Polen"
+msgstr "Poland"
 
 msgid "Portugal"
 msgstr "Portugal"
 
 msgid "Puerto Rico"
 msgstr "Puerto Rico"
 
 msgid "Qatar"
 msgstr "Qatar"
 
 msgid "Romania"
-msgstr "Rumänien"
+msgstr "Romania"
 
 msgid "Russia"
-msgstr "Ryssland"
+msgstr "Russia"
 
 msgid "Russian Federation"
-msgstr "Ryska federationen"
+msgstr "Russian Federation"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Réunion"
 msgstr "Réunion"
 
 msgid "Saint Barthélemy"
-msgstr "Saint-Barthélemy"
+msgstr "Saint Barthélemy"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Saint Helena, Kristi himmelsfärd och Tristan da Cunha"
+msgstr "Saint Helena, Ascension and Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Saint Kitts och Nevis"
+msgstr "Saint Kitts and Nevis"
 
 msgid "Saint Lucia"
 msgstr "Saint Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Saint Martin (franska delen)"
+msgstr "Saint Martin (French part)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Saint Pierre och Miquelon"
+msgstr "Saint Pierre and Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Saint Vincent och Grenadinerna"
+msgstr "Saint Vincent and the Grenadines"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
 msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tomé och Principe"
+msgstr "Sao Tome and Principe"
 
 msgid "Saudi Arabia"
-msgstr "Saudiarabien"
+msgstr "Saudi Arabia"
 
 msgid "Senegal"
 msgstr "Senegal"
 
 msgid "Serbia"
-msgstr "Serbien"
+msgstr "Serbia"
 
 msgid "Seychelles"
-msgstr "Seychellerna"
+msgstr "Seychelles"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
 msgstr "Singapore"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sint Maarten (nederländska delen)"
+msgstr "Sint Maarten (Dutch part)"
 
 msgid "Slovakia"
-msgstr "Slovakien"
+msgstr "Slovakia"
 
 msgid "Slovenia"
-msgstr "Slovenien"
+msgstr "Slovenia"
 
 msgid "Solomon Islands"
-msgstr "Salomonöarna"
+msgstr "Solomon Islands"
 
 msgid "Somalia"
 msgstr "Somalia"
 
 msgid "South Africa"
-msgstr "Sydafrika"
+msgstr "South Africa"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Sydgeorgien och Sydsandwichöarna"
+msgstr "South Georgia and the South Sandwich Islands"
 
 msgid "South Korea"
-msgstr "Sydkorea"
+msgstr "South Korea"
 
 msgid "South Sudan"
 msgstr "South Sudan"
 
 msgid "Spain"
-msgstr "Spanien"
+msgstr "Spain"
 
 msgid "Sri Lanka"
 msgstr "Sri Lanka"
 
 msgid "Sudan"
 msgstr "Sudan"
 
 msgid "Suriname"
-msgstr "Surinam"
+msgstr "Suriname"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard och Jan Mayen"
+msgstr "Svalbard and Jan Mayen"
 
 msgid "Swaziland"
 msgstr "Swaziland"
 
 msgid "Sweden"
-msgstr "Sverige"
+msgstr "Sweden"
 
 msgid "Switzerland"
-msgstr "Schweiz"
+msgstr "Switzerland"
 
 msgid "Syria"
-msgstr "Syrien"
+msgstr "Syria"
 
 msgid "Syrian Arab Republic"
-msgstr "Syrien"
+msgstr "Syrian Arab Republic"
 
 msgid "Taiwan"
 msgstr "Taiwan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Taiwan (provinsen i Kina)"
+msgstr "Taiwan (Province of China)"
 
 msgid "Tajikistan"
-msgstr "Tadzjikistan"
+msgstr "Tajikistan"
 
 msgid "Tanzania"
 msgstr "Tanzania"
 
+msgid "Tanzania, the United Republic of"
+msgstr "Tanzania, the United Republic of"
+
 msgid "Thailand"
 msgstr "Thailand"
 
 msgid "Timor-Leste"
-msgstr "Östtimor"
+msgstr "Timor-Leste"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
 msgstr "Tonga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinidad och Tobago"
+msgstr "Trinidad and Tobago"
 
 msgid "Tunisia"
-msgstr "Tunisien"
+msgstr "Tunisia"
 
 msgid "Turkey"
-msgstr "Turkiet"
+msgstr "Turkey"
 
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Turks- och Caicosöarna"
+msgstr "Turks and Caicos Islands"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
-msgstr "Ukraina"
+msgstr "Ukraine"
 
 msgid "United Arab Emirates"
-msgstr "Förenade Arabemiraten"
+msgstr "United Arab Emirates"
 
 msgid "United Kingdom"
-msgstr "Storbritannien"
+msgstr "United Kingdom"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Förenade konungariket Storbritannien och Nordirland"
+msgstr "United Kingdom of Great Britain and Northern Ireland"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Förenta staternas mindre öar i Oceanien och Västindien"
+msgstr "United States Minor Outlying Islands"
 
 msgid "United States of America"
-msgstr "Amerikas förenta stater"
+msgstr "United States of America"
 
 msgid "Uruguay"
 msgstr "Uruguay"
 
 msgid "Uzbekistan"
 msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Venezuela (Bolivarianska republiken)"
+msgstr "Venezuela (Bolivarian Republic of)"
 
 msgid "Viet Nam"
 msgstr "Viet Nam"
 
 msgid "Vietnam"
 msgstr "Vietnam"
 
 msgid "Virgin Islands (British)"
-msgstr "Jungfruöarna (Storbritannien)"
+msgstr "Virgin Islands (British)"
 
 msgid "Virgin Islands (U.S.)"
-msgstr "Jungfruöarna (US)"
+msgstr "Virgin Islands (U.S.)"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis och Futuna"
+msgstr "Wallis and Futuna"
 
 msgid "Western Sahara"
-msgstr "Västsahara"
+msgstr "Western Sahara"
 
 msgid "Yemen"
-msgstr "Jemen"
+msgstr "Yemen"
 
 msgid "Zambia"
 msgstr "Zambia"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "Åland Islands"
-msgstr "Åland"
+msgstr "Åland Islands"
```

### Comparing `django-countries-7.6/django_countries/locale/sv/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/sv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "Trinidad och Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunisien"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Turkiet"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/th_TH/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/vi/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,122 +1,122 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2011-06-05 21:30+0000\n"
-"Last-Translator: Chinnathan Chongsujiphan, 2023\n"
-"Language-Team: Thai (Thailand) (http://app.transifex.com/smileychris/django-"
-"countries/language/th_TH/)\n"
+"Last-Translator: martin stone, 2024\n"
+"Language-Team: Vietnamese (http://app.transifex.com/smileychris/django-"
+"countries/language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: th_TH\n"
+"Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Afghanistan"
 msgstr "Afghanistan"
 
 msgid "Albania"
 msgstr "Albania"
 
 msgid "Algeria"
 msgstr "Algeria"
 
 msgid "All"
-msgstr "All"
+msgstr "Tất cả"
 
 msgid "American Samoa"
-msgstr "American Samoa"
+msgstr "Samoa thuộc Mỹ"
 
 msgid "Andorra"
 msgstr "Andorra"
 
 msgid "Angola"
-msgstr "Angola"
+msgstr "Ăng-gô-la"
 
 msgid "Anguilla"
 msgstr "Anguilla"
 
 msgid "Antarctica"
-msgstr "Antarctica"
+msgstr "Nam Cực"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua and Barbuda"
+msgstr "Antigua và Barbuda"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Armenia"
 msgstr "Armenia"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
-msgstr "Australia"
+msgstr "Úc"
 
 msgid "Austria"
-msgstr "Austria"
+msgstr "Áo"
 
 msgid "Azerbaijan"
 msgstr "Azerbaijan"
 
 msgid "Bahamas"
-msgstr "Bahamas"
+msgstr "Bahama"
 
 msgid "Bahrain"
 msgstr "Bahrain"
 
 msgid "Bangladesh"
 msgstr "Bangladesh"
 
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Belarus"
+msgstr "Bêlarut"
 
 msgid "Belgium"
-msgstr "Belgium"
+msgstr "Bỉ"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
-msgstr "Benin"
+msgstr "Bénin"
 
 msgid "Bermuda"
 msgstr "Bermuda"
 
 msgid "Bhutan"
 msgstr "Bhutan"
 
 msgid "Bolivia"
 msgstr "Bolivia"
 
 msgid "Bolivia (Plurinational State of)"
-msgstr "Bolivia (Plurinational State of)"
+msgstr "Bolivia (Nhà nước đa quốc gia)"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sint Eustatius and Saba"
+msgstr "Bonaire, Sint Eustatius và Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosnia and Herzegovina"
+msgstr "Bosnia và Herzegovina"
 
 msgid "Botswana"
 msgstr "Botswana"
 
 msgid "Bouvet Island"
-msgstr "Bouvet Island"
+msgstr "Đảo Bouvet"
 
 msgid "Brazil"
 msgstr "Brazil"
 
 msgid "British Indian Ocean Territory"
-msgstr "British Indian Ocean Territory"
+msgstr "Lãnh thổ Ấn Độ Dương thuộc Anh"
 
 msgid "Brunei"
 msgstr "Brunei"
 
 msgid "Brunei Darussalam"
 msgstr "Brunei Darussalam"
 
@@ -129,168 +129,168 @@
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
 msgstr "Cabo Verde"
 
 msgid "Cambodia"
-msgstr "Cambodia"
+msgstr "Campuchia"
 
 msgid "Cameroon"
 msgstr "Cameroon"
 
 msgid "Canada"
 msgstr "Canada"
 
 msgid "Cayman Islands"
-msgstr "Cayman Islands"
+msgstr "Quần đảo Cayman"
 
 msgid "Central African Republic"
-msgstr "Central African Republic"
+msgstr "Cộng hòa Trung Phi"
 
 msgid "Chad"
-msgstr "Chad"
+msgstr "Tchad"
 
 msgid "Chile"
-msgstr "Chile"
+msgstr "Chilê"
 
 msgid "China"
-msgstr "China"
+msgstr "Trung Quốc"
 
 msgid "Christmas Island"
-msgstr "Christmas Island"
+msgstr "Đảo Giáng Sinh"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Cocos (Keeling) Islands"
+msgstr "Quần đảo Cocos (Keeling)"
 
 msgid "Colombia"
 msgstr "Colombia"
 
 msgid "Comoros"
 msgstr "Comoros"
 
 msgid "Congo"
-msgstr "Congo"
+msgstr "Công-gô"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Congo (the Democratic Republic of the)"
+msgstr "Congo (Cộng hòa Dân chủ)"
 
 msgid "Cook Islands"
-msgstr "Cook Islands"
+msgstr "Quần đảo Cook"
 
 msgid "Costa Rica"
 msgstr "Costa Rica"
 
 msgid "Country"
-msgstr "Country"
+msgstr "Quốc gia"
 
 msgid "Croatia"
 msgstr "Croatia"
 
 msgid "Cuba"
 msgstr "Cuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Cyprus"
+msgstr "Síp"
 
 msgid "Czech Republic"
-msgstr "Czech Republic"
+msgstr "Cộng hòa Séc"
 
 msgid "Czechia"
-msgstr "Czechia"
+msgstr "Séc"
 
 msgid "Côte d'Ivoire"
 msgstr "Côte d'Ivoire"
 
 msgid "Denmark"
-msgstr "Denmark"
+msgstr "Đan Mạch"
 
 msgid "Djibouti"
 msgstr "Djibouti"
 
 msgid "Dominica"
 msgstr "Dominica"
 
 msgid "Dominican Republic"
-msgstr "Dominican Republic"
+msgstr "Cộng hòa Dominica"
 
 msgid "Ecuador"
 msgstr "Ecuador"
 
 msgid "Egypt"
-msgstr "Egypt"
+msgstr "Ai Cập"
 
 msgid "El Salvador"
 msgstr "El Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Equatorial Guinea"
+msgstr "Guinea Xích đạo"
 
 msgid "Eritrea"
 msgstr "Eritrea"
 
 msgid "Estonia"
 msgstr "Estonia"
 
 msgid "Eswatini"
-msgstr "Eswatini"
+msgstr "Tiếng Swaziland"
 
 msgid "Ethiopia"
 msgstr "Ethiopia"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Falkland Islands  [Malvinas]"
+msgstr "Quần đảo Falkland [Malvinas]"
 
 msgid "Falkland Islands (Malvinas)"
-msgstr "Falkland Islands (Malvinas)"
+msgstr "Quần đảo Falkland (Malvinas)"
 
 msgid "Faroe Islands"
-msgstr "Faroe Islands"
+msgstr "Quần đảo Faroe"
 
 msgid "Fiji"
 msgstr "Fiji"
 
 msgid "Finland"
-msgstr "Finland"
+msgstr "Phần Lan"
 
 msgid "France"
-msgstr "France"
+msgstr "Pháp"
 
 msgid "French Guiana"
-msgstr "French Guiana"
+msgstr "Guiana thuộc Pháp"
 
 msgid "French Polynesia"
-msgstr "French Polynesia"
+msgstr "Polynesia thuộc Pháp"
 
 msgid "French Southern Territories"
-msgstr "French Southern Territories"
+msgstr "Lãnh thổ phía Nam thuộc Pháp"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
 msgstr "Gambia"
 
 msgid "Georgia"
 msgstr "Georgia"
 
 msgid "Germany"
-msgstr "Germany"
+msgstr "Đức"
 
 msgid "Ghana"
 msgstr "Ghana"
 
 msgid "Gibraltar"
 msgstr "Gibraltar"
 
 msgid "Greece"
-msgstr "Greece"
+msgstr "Hy Lạp"
 
 msgid "Greenland"
 msgstr "Greenland"
 
 msgid "Grenada"
 msgstr "Grenada"
 
@@ -315,189 +315,189 @@
 msgid "Guyana"
 msgstr "Guyana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Heard Island and McDonald Islands"
+msgstr "Đảo Heard và Quần đảo McDonald"
 
 msgid "Holy See"
-msgstr "Holy See"
+msgstr "Tòa Thánh"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
-msgstr "Hong Kong"
+msgstr "Hồng Kông"
 
 msgid "Hungary"
 msgstr "Hungary"
 
 msgid "Iceland"
-msgstr "Iceland"
+msgstr "Ai-len"
 
 msgid "India"
-msgstr "India"
+msgstr "Ấn Độ"
 
 msgid "Indonesia"
 msgstr "Indonesia"
 
 msgid "Iran"
 msgstr "Iran"
 
 msgid "Iran (Islamic Republic of)"
-msgstr "Iran (Islamic Republic of)"
+msgstr "Iran (Cộng hòa Hồi giáo)"
 
 msgid "Iraq"
 msgstr "Iraq"
 
 msgid "Ireland"
-msgstr "Ireland"
+msgstr "Ai-len"
 
 msgid "Isle of Man"
-msgstr "Isle of Man"
+msgstr "Đảo Man"
 
 msgid "Israel"
 msgstr "Israel"
 
 msgid "Italy"
-msgstr "Italy"
+msgstr "Ý"
 
 msgid "Jamaica"
 msgstr "Jamaica"
 
 msgid "Japan"
-msgstr "Japan"
+msgstr "Nhật Bản"
 
 msgid "Jersey"
-msgstr "Jersey"
+msgstr "Áo"
 
 msgid "Jordan"
 msgstr "Jordan"
 
 msgid "Kazakhstan"
 msgstr "Kazakhstan"
 
 msgid "Kenya"
 msgstr "Kenya"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Korea (the Democratic People's Republic of)"
+msgstr "Hàn Quốc (Cộng hòa Dân chủ Nhân dân)"
 
 msgid "Korea (the Republic of)"
-msgstr "Korea (the Republic of)"
+msgstr "Hàn Quốc (Cộng hòa)"
 
 msgid "Kuwait"
 msgstr "Kuwait"
 
 msgid "Kyrgyzstan"
 msgstr "Kyrgyzstan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Lao People's Democratic Republic"
+msgstr "Cộng hòa Dân chủ Nhân dân Lào"
 
 msgid "Laos"
-msgstr "Laos"
+msgstr "Lào"
 
 msgid "Latvia"
 msgstr "Latvia"
 
 msgid "Lebanon"
-msgstr "Lebanon"
+msgstr "Liban"
 
 msgid "Lesotho"
 msgstr "Lesotho"
 
 msgid "Liberia"
 msgstr "Liberia"
 
 msgid "Libya"
-msgstr "Libya"
+msgstr "Lybia"
 
 msgid "Liechtenstein"
 msgstr "Liechtenstein"
 
 msgid "Lithuania"
-msgstr "Lithuania"
+msgstr "Litva"
 
 msgid "Luxembourg"
 msgstr "Luxembourg"
 
 msgid "Macao"
-msgstr "Macao"
+msgstr "Ma Cao"
 
 msgid "Macedonia"
 msgstr "Macedonia"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Macedonia (the former Yugoslav Republic of)"
+msgstr "Macedonia (Cộng hòa Nam Tư cũ)"
 
 msgid "Madagascar"
 msgstr "Madagascar"
 
 msgid "Malawi"
-msgstr "Malawi"
+msgstr "Ma-la-uy"
 
 msgid "Malaysia"
 msgstr "Malaysia"
 
 msgid "Maldives"
 msgstr "Maldives"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Marshall Islands"
+msgstr "Quần đảo Marshall"
 
 msgid "Martinique"
 msgstr "Martinique"
 
 msgid "Mauritania"
-msgstr "Mauritania"
+msgstr "Mauritanie"
 
 msgid "Mauritius"
 msgstr "Mauritius"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
 msgstr "Mexico"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Micronesia (Federated States of)"
+msgstr "Micronesia (Liên bang)"
 
 msgid "Moldova"
-msgstr "Moldova"
+msgstr "Mô-đô-va"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldova (the Republic of)"
+msgstr "Moldova (Cộng hòa)"
 
 msgid "Monaco"
 msgstr "Monaco"
 
 msgid "Mongolia"
-msgstr "Mongolia"
+msgstr "Mông Cổ"
 
 msgid "Montenegro"
 msgstr "Montenegro"
 
 msgid "Montserrat"
 msgstr "Montserrat"
 
 msgid "Morocco"
-msgstr "Morocco"
+msgstr "Maroc"
 
 msgid "Mozambique"
 msgstr "Mozambique"
 
 msgid "Myanmar"
 msgstr "Myanmar"
 
@@ -507,60 +507,60 @@
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Netherlands"
+msgstr "Hà Lan"
 
 msgid "New Caledonia"
-msgstr "New Caledonia"
+msgstr "Tân Caledonia"
 
 msgid "New Zealand"
 msgstr "New Zealand"
 
 msgid "Nicaragua"
 msgstr "Nicaragua"
 
 msgid "Niger"
-msgstr "Niger"
+msgstr "Nigeria"
 
 msgid "Nigeria"
 msgstr "Nigeria"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Norfolk Island"
+msgstr "Đảo Norfolk"
 
 msgid "North Korea"
-msgstr "North Korea"
+msgstr "Bắc Triều Tiên"
 
 msgid "North Macedonia"
-msgstr "North Macedonia"
+msgstr "Bắc Macedonia"
 
 msgid "Northern Mariana Islands"
-msgstr "Northern Mariana Islands"
+msgstr "Quần đảo Bắc Mariana"
 
 msgid "Norway"
-msgstr "Norway"
+msgstr "Na Uy"
 
 msgid "Oman"
-msgstr "Oman"
+msgstr "Ô-man"
 
 msgid "Pakistan"
 msgstr "Pakistan"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestine, State of"
+msgstr "Palestine, Bang"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
 msgstr "Papua New Guinea"
 
@@ -573,251 +573,251 @@
 msgid "Philippines"
 msgstr "Philippines"
 
 msgid "Pitcairn"
 msgstr "Pitcairn"
 
 msgid "Poland"
-msgstr "Poland"
+msgstr "Ba Lan"
 
 msgid "Portugal"
-msgstr "Portugal"
+msgstr "Bồ Đào Nha"
 
 msgid "Puerto Rico"
 msgstr "Puerto Rico"
 
 msgid "Qatar"
 msgstr "Qatar"
 
 msgid "Romania"
-msgstr "Romania"
+msgstr "România"
 
 msgid "Russia"
-msgstr "Russia"
+msgstr "Nga"
 
 msgid "Russian Federation"
-msgstr "Russian Federation"
+msgstr "Liên bang Nga"
 
 msgid "Rwanda"
 msgstr "Rwanda"
 
 msgid "Réunion"
-msgstr "Réunion"
+msgstr "Đoàn tụ"
 
 msgid "Saint Barthélemy"
-msgstr "Saint Barthélemy"
+msgstr "Thánh Barthélemy"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Saint Helena, Ascension and Tristan da Cunha"
+msgstr "Thánh Helena, Thăng thiên và Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Saint Kitts and Nevis"
+msgstr "Saint Kitts và Nevis"
 
 msgid "Saint Lucia"
-msgstr "Saint Lucia"
+msgstr "Thánh Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Saint Martin (French part)"
+msgstr "Saint Martin (phần tiếng Pháp)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Saint Pierre and Miquelon"
+msgstr "Saint Pierre và Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Saint Vincent and the Grenadines"
+msgstr "Saint Vincent và Grenadines"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
 msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tome and Principe"
+msgstr "Sao Tome và Principe"
 
 msgid "Saudi Arabia"
-msgstr "Saudi Arabia"
+msgstr "Ả Rập Saudi"
 
 msgid "Senegal"
-msgstr "Senegal"
+msgstr "Sénégal"
 
 msgid "Serbia"
 msgstr "Serbia"
 
 msgid "Seychelles"
 msgstr "Seychelles"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
 msgstr "Singapore"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sint Maarten (Dutch part)"
+msgstr "Sint Maarten (phần Hà Lan)"
 
 msgid "Slovakia"
 msgstr "Slovakia"
 
 msgid "Slovenia"
 msgstr "Slovenia"
 
 msgid "Solomon Islands"
-msgstr "Solomon Islands"
+msgstr "Quần đảo Solomon"
 
 msgid "Somalia"
-msgstr "Somalia"
+msgstr "Somali"
 
 msgid "South Africa"
-msgstr "South Africa"
+msgstr "Nam Phi"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "South Georgia and the South Sandwich Islands"
+msgstr "Nam Georgia và Quần đảo Nam Sandwich"
 
 msgid "South Korea"
-msgstr "South Korea"
+msgstr "Hàn Quốc"
 
 msgid "South Sudan"
-msgstr "South Sudan"
+msgstr "Nam Sudan"
 
 msgid "Spain"
-msgstr "Spain"
+msgstr "Tây Ban Nha"
 
 msgid "Sri Lanka"
 msgstr "Sri Lanka"
 
 msgid "Sudan"
 msgstr "Sudan"
 
 msgid "Suriname"
 msgstr "Suriname"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard and Jan Mayen"
+msgstr "Svalbard và Jan Mayen"
 
 msgid "Swaziland"
 msgstr "Swaziland"
 
 msgid "Sweden"
-msgstr "Sweden"
+msgstr "Thụy Điển"
 
 msgid "Switzerland"
-msgstr "Switzerland"
+msgstr "Thụy Sĩ"
 
 msgid "Syria"
 msgstr "Syria"
 
 msgid "Syrian Arab Republic"
-msgstr "Syrian Arab Republic"
+msgstr "Cộng hòa Ả Rập Syria"
 
 msgid "Taiwan"
-msgstr "Taiwan"
+msgstr "Đài Loan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Taiwan (Province of China)"
+msgstr "Đài Loan (Tỉnh Trung Quốc)"
 
 msgid "Tajikistan"
 msgstr "Tajikistan"
 
 msgid "Tanzania"
 msgstr "Tanzania"
 
 msgid "Tanzania, the United Republic of"
-msgstr "Tanzania, the United Republic of"
+msgstr "Tanzania, Cộng hòa Thống nhất"
 
 msgid "Thailand"
-msgstr "Thailand"
+msgstr "Thái Lan"
 
 msgid "Timor-Leste"
 msgstr "Timor-Leste"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
 msgstr "Tonga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinidad and Tobago"
+msgstr "Trinidad và Tobago"
 
 msgid "Tunisia"
 msgstr "Tunisia"
 
 msgid "Turkey"
-msgstr "Turkey"
+msgstr "Thổ Nhĩ Kỳ"
 
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Turks and Caicos Islands"
+msgstr "Quần đảo Thổ Nhĩ Kỳ và Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
-msgstr "Ukraine"
+msgstr "Ukraina"
 
 msgid "United Arab Emirates"
-msgstr "United Arab Emirates"
+msgstr "Các tiểu vương quốc Ả Rập thống nhất"
 
 msgid "United Kingdom"
-msgstr "United Kingdom"
+msgstr "Vương quốc Anh"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "United Kingdom of Great Britain and Northern Ireland"
+msgstr "Vương quốc Liên hiệp Anh và Bắc Ireland"
 
 msgid "United States Minor Outlying Islands"
-msgstr "United States Minor Outlying Islands"
+msgstr "Quần đảo xa xôi nhỏ của Hoa Kỳ"
 
 msgid "United States of America"
-msgstr "United States of America"
+msgstr "Hợp chủng quốc Hoa Kỳ"
 
 msgid "Uruguay"
 msgstr "Uruguay"
 
 msgid "Uzbekistan"
 msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Venezuela (Bolivarian Republic of)"
+msgstr "Venezuela (Cộng hòa Bolivar)"
 
 msgid "Viet Nam"
-msgstr "Viet Nam"
+msgstr "Việt Nam"
 
 msgid "Vietnam"
-msgstr "Vietnam"
+msgstr "Việt Nam"
 
 msgid "Virgin Islands (British)"
-msgstr "Virgin Islands (British)"
+msgstr "Quần đảo Virgin (Anh)"
 
 msgid "Virgin Islands (U.S.)"
-msgstr "Virgin Islands (U.S.)"
+msgstr "Quần đảo Virgin (Mỹ)"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis and Futuna"
+msgstr "Wallis và Futuna"
 
 msgid "Western Sahara"
-msgstr "Western Sahara"
+msgstr "Tây Sahara"
 
 msgid "Yemen"
-msgstr "Yemen"
+msgstr "Yêmen"
 
 msgid "Zambia"
 msgstr "Zambia"
 
 msgid "Zimbabwe"
 msgstr "Zimbabwe"
 
 msgid "Åland Islands"
-msgstr "Åland Islands"
+msgstr "Quần đảo Åland"
```

### Comparing `django-countries-7.6/django_countries/locale/th_TH/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/locale/tr_TR/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Trinidad ve Tobago"
 
 msgid "Tunisia"
 msgstr "Tunus"
 
-msgid "Turkey"
-msgstr "Türkiye"
-
 msgid "Turkmenistan"
 msgstr "Türkmenistan"
 
 msgid "Turks and Caicos Islands"
 msgstr "Turks ve Kaykos Adaları"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Türkiye"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
 msgstr "Ukrayna"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/tr_TR/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 msgstr "Trinidad ve Tobago"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Tunus"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Türkiye"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Türkmenistan"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/uk/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/uk/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -743,26 +743,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "Тринідад і Тобаго"
 
 msgid "Tunisia"
 msgstr "Туніс"
 
-msgid "Turkey"
-msgstr "Туреччина"
-
 msgid "Turkmenistan"
 msgstr "Туркменістан"
 
 msgid "Turks and Caicos Islands"
 msgstr "Теркс і Кайкос острова"
 
 msgid "Tuvalu"
 msgstr "Тувалу"
 
+msgid "Türkiye"
+msgstr "Туреччина"
+
 msgid "Uganda"
 msgstr "Уганда"
 
 msgid "Ukraine"
 msgstr "Україна"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/uk/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
 msgstr "Тринідад і Тобаго"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "Туніс"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "Туреччина"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "Туркменістан"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/vi/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/sl/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,823 +1,812 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2011-06-05 21:30+0000\n"
-"Last-Translator: martin stone, 2024\n"
-"Language-Team: Vietnamese (http://app.transifex.com/smileychris/django-"
-"countries/language/vi/)\n"
+"PO-Revision-Date: 2020-03-26 01:43+0000\n"
+"Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
+"Language-Team: Slovenian (http://www.transifex.com/smileychris/django-"
+"countries/language/sl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: vi\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: sl\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
 msgid "Afghanistan"
-msgstr "Afghanistan"
+msgstr "Afganistan"
 
 msgid "Albania"
-msgstr "Albania"
+msgstr "Albanija"
 
 msgid "Algeria"
-msgstr "Algeria"
+msgstr "Alžirija"
 
 msgid "All"
-msgstr "Tất cả"
+msgstr "Vse"
 
 msgid "American Samoa"
-msgstr "Samoa thuộc Mỹ"
+msgstr "Ameriška Samoa"
 
 msgid "Andorra"
-msgstr "Andorra"
+msgstr "Andora"
 
 msgid "Angola"
-msgstr "Ăng-gô-la"
+msgstr "Angola"
 
 msgid "Anguilla"
-msgstr "Anguilla"
+msgstr "Angvila"
 
 msgid "Antarctica"
-msgstr "Nam Cực"
+msgstr "Antarktika"
 
 msgid "Antigua and Barbuda"
-msgstr "Antigua và Barbuda"
+msgstr "Antigva in Barbuda"
 
 msgid "Argentina"
 msgstr "Argentina"
 
 msgid "Armenia"
-msgstr "Armenia"
+msgstr "Armenija"
 
 msgid "Aruba"
 msgstr "Aruba"
 
 msgid "Australia"
-msgstr "Úc"
+msgstr "Avstralija"
 
 msgid "Austria"
-msgstr "Áo"
+msgstr "Avstrija"
 
 msgid "Azerbaijan"
-msgstr "Azerbaijan"
+msgstr "Azerbajdžan"
 
 msgid "Bahamas"
-msgstr "Bahama"
+msgstr "Bahami"
 
 msgid "Bahrain"
-msgstr "Bahrain"
+msgstr "Bahrajn"
 
 msgid "Bangladesh"
-msgstr "Bangladesh"
+msgstr "Bangladeš"
 
 msgid "Barbados"
 msgstr "Barbados"
 
 msgid "Belarus"
-msgstr "Bêlarut"
+msgstr "Belorusija"
 
 msgid "Belgium"
-msgstr "Bỉ"
+msgstr "Belgija"
 
 msgid "Belize"
 msgstr "Belize"
 
 msgid "Benin"
-msgstr "Bénin"
+msgstr "Benin"
 
 msgid "Bermuda"
-msgstr "Bermuda"
+msgstr "Bermudi"
 
 msgid "Bhutan"
-msgstr "Bhutan"
+msgstr "Butan"
 
 msgid "Bolivia"
-msgstr "Bolivia"
+msgstr "Bolivija"
 
 msgid "Bolivia (Plurinational State of)"
-msgstr "Bolivia (Nhà nước đa quốc gia)"
+msgstr "Bolivija"
 
 msgid "Bonaire, Sint Eustatius and Saba"
-msgstr "Bonaire, Sint Eustatius và Saba"
+msgstr "Bonaire, Sint Eustatius in Saba"
 
 msgid "Bosnia and Herzegovina"
-msgstr "Bosnia và Herzegovina"
+msgstr "Bosna in Hercegovina"
 
 msgid "Botswana"
-msgstr "Botswana"
+msgstr "Bocvana"
 
 msgid "Bouvet Island"
-msgstr "Đảo Bouvet"
+msgstr "Bouvetov otok"
 
 msgid "Brazil"
-msgstr "Brazil"
+msgstr "Brazilija"
 
 msgid "British Indian Ocean Territory"
-msgstr "Lãnh thổ Ấn Độ Dương thuộc Anh"
+msgstr "Britansko ozemlje v Indijskem oceanu"
 
 msgid "Brunei"
-msgstr "Brunei"
+msgstr "Brunej"
 
 msgid "Brunei Darussalam"
-msgstr "Brunei Darussalam"
+msgstr "Brunej"
 
 msgid "Bulgaria"
-msgstr "Bulgaria"
+msgstr "Bolgarija"
 
 msgid "Burkina Faso"
 msgstr "Burkina Faso"
 
 msgid "Burundi"
 msgstr "Burundi"
 
 msgid "Cabo Verde"
-msgstr "Cabo Verde"
+msgstr "Zelenortski otoki"
 
 msgid "Cambodia"
-msgstr "Campuchia"
+msgstr "Kambodža"
 
 msgid "Cameroon"
-msgstr "Cameroon"
+msgstr "Kamerun"
 
 msgid "Canada"
-msgstr "Canada"
+msgstr "Kanada"
 
 msgid "Cayman Islands"
-msgstr "Quần đảo Cayman"
+msgstr "Kajmanski otoki"
 
 msgid "Central African Republic"
-msgstr "Cộng hòa Trung Phi"
+msgstr "Srednjeafriška republika"
 
 msgid "Chad"
-msgstr "Tchad"
+msgstr "Čad"
 
 msgid "Chile"
-msgstr "Chilê"
+msgstr "Čile"
 
 msgid "China"
-msgstr "Trung Quốc"
+msgstr "Kitajska"
 
 msgid "Christmas Island"
-msgstr "Đảo Giáng Sinh"
+msgstr "Velikonočni otok"
 
 msgid "Cocos (Keeling) Islands"
-msgstr "Quần đảo Cocos (Keeling)"
+msgstr "Kokosovi (Keeling) otoki"
 
 msgid "Colombia"
-msgstr "Colombia"
+msgstr "Kolumbija"
 
 msgid "Comoros"
-msgstr "Comoros"
+msgstr "Komori"
 
 msgid "Congo"
-msgstr "Công-gô"
+msgstr "Kongo"
 
 msgid "Congo (the Democratic Republic of the)"
-msgstr "Congo (Cộng hòa Dân chủ)"
+msgstr "Kongo (demokratična republika)"
 
 msgid "Cook Islands"
-msgstr "Quần đảo Cook"
+msgstr "Cookovi otoki"
 
 msgid "Costa Rica"
-msgstr "Costa Rica"
+msgstr "Kostarika"
 
 msgid "Country"
-msgstr "Quốc gia"
+msgstr "Država"
 
 msgid "Croatia"
-msgstr "Croatia"
+msgstr "Hrvaška"
 
 msgid "Cuba"
-msgstr "Cuba"
+msgstr "Kuba"
 
 msgid "Curaçao"
 msgstr "Curaçao"
 
 msgid "Cyprus"
-msgstr "Síp"
+msgstr "Ciper"
 
 msgid "Czech Republic"
-msgstr "Cộng hòa Séc"
+msgstr "Češka"
 
 msgid "Czechia"
-msgstr "Séc"
+msgstr "Češka"
 
 msgid "Côte d'Ivoire"
-msgstr "Côte d'Ivoire"
+msgstr "Slonokoščena obala"
 
 msgid "Denmark"
-msgstr "Đan Mạch"
+msgstr "Danska"
 
 msgid "Djibouti"
-msgstr "Djibouti"
+msgstr "Džibuti"
 
 msgid "Dominica"
-msgstr "Dominica"
+msgstr "Dominika"
 
 msgid "Dominican Republic"
-msgstr "Cộng hòa Dominica"
+msgstr "Dominikanska republika"
 
 msgid "Ecuador"
-msgstr "Ecuador"
+msgstr "Ekvador"
 
 msgid "Egypt"
-msgstr "Ai Cập"
+msgstr "Egipt"
 
 msgid "El Salvador"
-msgstr "El Salvador"
+msgstr "Salvador"
 
 msgid "Equatorial Guinea"
-msgstr "Guinea Xích đạo"
+msgstr "Ekvatorialna Gvineja"
 
 msgid "Eritrea"
-msgstr "Eritrea"
+msgstr "Eritreja"
 
 msgid "Estonia"
-msgstr "Estonia"
-
-msgid "Eswatini"
-msgstr "Tiếng Swaziland"
+msgstr "Estonija"
 
 msgid "Ethiopia"
-msgstr "Ethiopia"
+msgstr "Etiopija"
 
 msgid "Falkland Islands  [Malvinas]"
-msgstr "Quần đảo Falkland [Malvinas]"
-
-msgid "Falkland Islands (Malvinas)"
-msgstr "Quần đảo Falkland (Malvinas)"
+msgstr "Falklandski otoki"
 
 msgid "Faroe Islands"
-msgstr "Quần đảo Faroe"
+msgstr "Ferski otoki"
 
 msgid "Fiji"
-msgstr "Fiji"
+msgstr "Fidži"
 
 msgid "Finland"
-msgstr "Phần Lan"
+msgstr "Finska"
 
 msgid "France"
-msgstr "Pháp"
+msgstr "Francija"
 
 msgid "French Guiana"
-msgstr "Guiana thuộc Pháp"
+msgstr "Francoska Gvajana"
 
 msgid "French Polynesia"
-msgstr "Polynesia thuộc Pháp"
+msgstr "Francoska Polinezija"
 
 msgid "French Southern Territories"
-msgstr "Lãnh thổ phía Nam thuộc Pháp"
+msgstr "Francoska južna ozemlja"
 
 msgid "Gabon"
 msgstr "Gabon"
 
 msgid "Gambia"
-msgstr "Gambia"
+msgstr "Gambija"
 
 msgid "Georgia"
-msgstr "Georgia"
+msgstr "Gruzija"
 
 msgid "Germany"
-msgstr "Đức"
+msgstr "Nemčija"
 
 msgid "Ghana"
-msgstr "Ghana"
+msgstr "Gana"
 
 msgid "Gibraltar"
 msgstr "Gibraltar"
 
 msgid "Greece"
-msgstr "Hy Lạp"
+msgstr "Grčija"
 
 msgid "Greenland"
-msgstr "Greenland"
+msgstr "Grenlandija"
 
 msgid "Grenada"
 msgstr "Grenada"
 
 msgid "Guadeloupe"
-msgstr "Guadeloupe"
+msgstr "Gvadelupe"
 
 msgid "Guam"
 msgstr "Guam"
 
 msgid "Guatemala"
-msgstr "Guatemala"
+msgstr "Gvatemala"
 
 msgid "Guernsey"
 msgstr "Guernsey"
 
 msgid "Guinea"
-msgstr "Guinea"
+msgstr "Gvineja"
 
 msgid "Guinea-Bissau"
-msgstr "Guinea-Bissau"
+msgstr "Gvineja Bissau"
 
 msgid "Guyana"
-msgstr "Guyana"
+msgstr "Gvajana"
 
 msgid "Haiti"
 msgstr "Haiti"
 
 msgid "Heard Island and McDonald Islands"
-msgstr "Đảo Heard và Quần đảo McDonald"
+msgstr "Otok Heard in otočje McDonald"
 
 msgid "Holy See"
-msgstr "Tòa Thánh"
+msgstr "Sveti sedež"
 
 msgid "Honduras"
 msgstr "Honduras"
 
 msgid "Hong Kong"
-msgstr "Hồng Kông"
+msgstr "Hong Kong"
 
 msgid "Hungary"
-msgstr "Hungary"
+msgstr "Madžarska"
 
 msgid "Iceland"
-msgstr "Ai-len"
+msgstr "Islandija"
 
 msgid "India"
-msgstr "Ấn Độ"
+msgstr "Indija"
 
 msgid "Indonesia"
-msgstr "Indonesia"
+msgstr "Indonezija"
 
 msgid "Iran"
 msgstr "Iran"
 
 msgid "Iran (Islamic Republic of)"
-msgstr "Iran (Cộng hòa Hồi giáo)"
+msgstr "Iran"
 
 msgid "Iraq"
-msgstr "Iraq"
+msgstr "Irak"
 
 msgid "Ireland"
-msgstr "Ai-len"
+msgstr "Irska"
 
 msgid "Isle of Man"
-msgstr "Đảo Man"
+msgstr "Otok Man"
 
 msgid "Israel"
-msgstr "Israel"
+msgstr "Izrael"
 
 msgid "Italy"
-msgstr "Ý"
+msgstr "Italija"
 
 msgid "Jamaica"
-msgstr "Jamaica"
+msgstr "Jamajka"
 
 msgid "Japan"
-msgstr "Nhật Bản"
+msgstr "Japonska"
 
 msgid "Jersey"
-msgstr "Áo"
+msgstr "Jersey"
 
 msgid "Jordan"
-msgstr "Jordan"
+msgstr "Jordanija"
 
 msgid "Kazakhstan"
-msgstr "Kazakhstan"
+msgstr "Kazahstan"
 
 msgid "Kenya"
-msgstr "Kenya"
+msgstr "Kenija"
 
 msgid "Kiribati"
 msgstr "Kiribati"
 
 msgid "Korea (the Democratic People's Republic of)"
-msgstr "Hàn Quốc (Cộng hòa Dân chủ Nhân dân)"
+msgstr "Severna Koreja"
 
 msgid "Korea (the Republic of)"
-msgstr "Hàn Quốc (Cộng hòa)"
+msgstr "Južna Koreja"
 
 msgid "Kuwait"
-msgstr "Kuwait"
+msgstr "Kuvajt"
 
 msgid "Kyrgyzstan"
-msgstr "Kyrgyzstan"
+msgstr "Kirgizistan"
 
 msgid "Lao People's Democratic Republic"
-msgstr "Cộng hòa Dân chủ Nhân dân Lào"
+msgstr "Laos"
 
 msgid "Laos"
-msgstr "Lào"
+msgstr "Laos"
 
 msgid "Latvia"
-msgstr "Latvia"
+msgstr "Latvija"
 
 msgid "Lebanon"
-msgstr "Liban"
+msgstr "Libanon"
 
 msgid "Lesotho"
-msgstr "Lesotho"
+msgstr "Lesoto"
 
 msgid "Liberia"
-msgstr "Liberia"
+msgstr "Liberija"
 
 msgid "Libya"
-msgstr "Lybia"
+msgstr "Libija"
 
 msgid "Liechtenstein"
-msgstr "Liechtenstein"
+msgstr "Lihtenštajn"
 
 msgid "Lithuania"
 msgstr "Litva"
 
 msgid "Luxembourg"
-msgstr "Luxembourg"
+msgstr "Luksemburg"
 
 msgid "Macao"
-msgstr "Ma Cao"
+msgstr "Macau"
 
 msgid "Macedonia"
-msgstr "Macedonia"
+msgstr "Severna Makedonija"
 
 msgid "Macedonia (the former Yugoslav Republic of)"
-msgstr "Macedonia (Cộng hòa Nam Tư cũ)"
+msgstr "Severna Makedonija"
 
 msgid "Madagascar"
-msgstr "Madagascar"
+msgstr "Madagaskar"
 
 msgid "Malawi"
-msgstr "Ma-la-uy"
+msgstr "Malavi"
 
 msgid "Malaysia"
-msgstr "Malaysia"
+msgstr "Malezija"
 
 msgid "Maldives"
-msgstr "Maldives"
+msgstr "Maldivi"
 
 msgid "Mali"
 msgstr "Mali"
 
 msgid "Malta"
 msgstr "Malta"
 
 msgid "Marshall Islands"
-msgstr "Quần đảo Marshall"
+msgstr "Maršalovi otoki"
 
 msgid "Martinique"
-msgstr "Martinique"
+msgstr "Martinik"
 
 msgid "Mauritania"
-msgstr "Mauritanie"
+msgstr "Mavretanija"
 
 msgid "Mauritius"
-msgstr "Mauritius"
+msgstr "Mavricij"
 
 msgid "Mayotte"
 msgstr "Mayotte"
 
 msgid "Mexico"
-msgstr "Mexico"
+msgstr "Mehika"
 
 msgid "Micronesia (Federated States of)"
-msgstr "Micronesia (Liên bang)"
+msgstr "Mikronezija"
 
 msgid "Moldova"
-msgstr "Mô-đô-va"
+msgstr "Moldavija"
 
 msgid "Moldova (the Republic of)"
-msgstr "Moldova (Cộng hòa)"
+msgstr "Moldavija"
 
 msgid "Monaco"
-msgstr "Monaco"
+msgstr "Monako"
 
 msgid "Mongolia"
-msgstr "Mông Cổ"
+msgstr "Mongolija"
 
 msgid "Montenegro"
-msgstr "Montenegro"
+msgstr "Črna gora"
 
 msgid "Montserrat"
-msgstr "Montserrat"
+msgstr "Monserat"
 
 msgid "Morocco"
-msgstr "Maroc"
+msgstr "Maroko"
 
 msgid "Mozambique"
-msgstr "Mozambique"
+msgstr "Mozambik"
 
 msgid "Myanmar"
-msgstr "Myanmar"
+msgstr "Mjanmar"
 
 msgid "Namibia"
-msgstr "Namibia"
+msgstr "Namibija"
 
 msgid "Nauru"
 msgstr "Nauru"
 
 msgid "Nepal"
 msgstr "Nepal"
 
 msgid "Netherlands"
-msgstr "Hà Lan"
+msgstr "Nizozemska"
 
 msgid "New Caledonia"
-msgstr "Tân Caledonia"
+msgstr "Nova Kaledonija"
 
 msgid "New Zealand"
-msgstr "New Zealand"
+msgstr "Nova Zelandija"
 
 msgid "Nicaragua"
-msgstr "Nicaragua"
+msgstr "Nikaragva"
 
 msgid "Niger"
-msgstr "Nigeria"
+msgstr "Niger"
 
 msgid "Nigeria"
-msgstr "Nigeria"
+msgstr "Nigerija"
 
 msgid "Niue"
 msgstr "Niue"
 
 msgid "Norfolk Island"
-msgstr "Đảo Norfolk"
+msgstr "Otok Norfolk"
 
 msgid "North Korea"
-msgstr "Bắc Triều Tiên"
-
-msgid "North Macedonia"
-msgstr "Bắc Macedonia"
+msgstr "Severna Koreja"
 
 msgid "Northern Mariana Islands"
-msgstr "Quần đảo Bắc Mariana"
+msgstr "Severni Marianski otoki"
 
 msgid "Norway"
-msgstr "Na Uy"
+msgstr "Norveška"
 
 msgid "Oman"
-msgstr "Ô-man"
+msgstr "Oman"
 
 msgid "Pakistan"
 msgstr "Pakistan"
 
 msgid "Palau"
 msgstr "Palau"
 
 msgid "Palestine, State of"
-msgstr "Palestine, Bang"
+msgstr "Palestina"
 
 msgid "Panama"
 msgstr "Panama"
 
 msgid "Papua New Guinea"
-msgstr "Papua New Guinea"
+msgstr "Papua Nova Gvineja"
 
 msgid "Paraguay"
-msgstr "Paraguay"
+msgstr "Paragvaj"
 
 msgid "Peru"
 msgstr "Peru"
 
 msgid "Philippines"
-msgstr "Philippines"
+msgstr "Filipini"
 
 msgid "Pitcairn"
-msgstr "Pitcairn"
+msgstr "Pitcairnovi otoki"
 
 msgid "Poland"
-msgstr "Ba Lan"
+msgstr "Polska"
 
 msgid "Portugal"
-msgstr "Bồ Đào Nha"
+msgstr "Portugalska"
 
 msgid "Puerto Rico"
-msgstr "Puerto Rico"
+msgstr "Portorika"
 
 msgid "Qatar"
-msgstr "Qatar"
+msgstr "Katar"
 
 msgid "Romania"
-msgstr "România"
+msgstr "Romunija"
 
 msgid "Russia"
-msgstr "Nga"
+msgstr "Rusija"
 
 msgid "Russian Federation"
-msgstr "Liên bang Nga"
+msgstr "Ruska federacija"
 
 msgid "Rwanda"
-msgstr "Rwanda"
+msgstr "Ruanda"
 
 msgid "Réunion"
-msgstr "Đoàn tụ"
+msgstr "Reunion"
 
 msgid "Saint Barthélemy"
-msgstr "Thánh Barthélemy"
+msgstr "Saint Barthélemy"
 
 msgid "Saint Helena, Ascension and Tristan da Cunha"
-msgstr "Thánh Helena, Thăng thiên và Tristan da Cunha"
+msgstr "Saint Helena, Ascension in Tristan da Cunha"
 
 msgid "Saint Kitts and Nevis"
-msgstr "Saint Kitts và Nevis"
+msgstr "Saint Kitts in Nevis"
 
 msgid "Saint Lucia"
-msgstr "Thánh Lucia"
+msgstr "Saint Lucia"
 
 msgid "Saint Martin (French part)"
-msgstr "Saint Martin (phần tiếng Pháp)"
+msgstr "Saint Martin (francoski del)"
 
 msgid "Saint Pierre and Miquelon"
-msgstr "Saint Pierre và Miquelon"
+msgstr "Saint Pierre in Miquelon"
 
 msgid "Saint Vincent and the Grenadines"
-msgstr "Saint Vincent và Grenadines"
+msgstr "Saint Vincent in Grenadine"
 
 msgid "Samoa"
 msgstr "Samoa"
 
 msgid "San Marino"
 msgstr "San Marino"
 
 msgid "Sao Tome and Principe"
-msgstr "Sao Tome và Principe"
+msgstr "Sao Tome in Principe"
 
 msgid "Saudi Arabia"
-msgstr "Ả Rập Saudi"
+msgstr "Saudova Arabija"
 
 msgid "Senegal"
-msgstr "Sénégal"
+msgstr "Senegal"
 
 msgid "Serbia"
-msgstr "Serbia"
+msgstr "Srbija"
 
 msgid "Seychelles"
-msgstr "Seychelles"
+msgstr "Sejšeli"
 
 msgid "Sierra Leone"
 msgstr "Sierra Leone"
 
 msgid "Singapore"
-msgstr "Singapore"
+msgstr "Singapur"
 
 msgid "Sint Maarten (Dutch part)"
-msgstr "Sint Maarten (phần Hà Lan)"
+msgstr "Sint Maarten (nizozemski del)"
 
 msgid "Slovakia"
-msgstr "Slovakia"
+msgstr "Slovaška"
 
 msgid "Slovenia"
-msgstr "Slovenia"
+msgstr "Slovenija"
 
 msgid "Solomon Islands"
-msgstr "Quần đảo Solomon"
+msgstr "Salomonovi otoki"
 
 msgid "Somalia"
-msgstr "Somali"
+msgstr "Somalija"
 
 msgid "South Africa"
-msgstr "Nam Phi"
+msgstr "Južna Afrika"
 
 msgid "South Georgia and the South Sandwich Islands"
-msgstr "Nam Georgia và Quần đảo Nam Sandwich"
+msgstr "Južna Georgia in Južni Sandwichevi otoki"
 
 msgid "South Korea"
-msgstr "Hàn Quốc"
+msgstr "Južna Koreja"
 
 msgid "South Sudan"
-msgstr "Nam Sudan"
+msgstr "Južni Sudan"
 
 msgid "Spain"
-msgstr "Tây Ban Nha"
+msgstr "Španija"
 
 msgid "Sri Lanka"
-msgstr "Sri Lanka"
+msgstr "Šrilanka"
 
 msgid "Sudan"
 msgstr "Sudan"
 
 msgid "Suriname"
-msgstr "Suriname"
+msgstr "Surinam"
 
 msgid "Svalbard and Jan Mayen"
-msgstr "Svalbard và Jan Mayen"
+msgstr "Svalbard in Jan Mayen"
 
 msgid "Swaziland"
-msgstr "Swaziland"
+msgstr "Svazi"
 
 msgid "Sweden"
-msgstr "Thụy Điển"
+msgstr "Švedska"
 
 msgid "Switzerland"
-msgstr "Thụy Sĩ"
+msgstr "Švica"
 
 msgid "Syria"
-msgstr "Syria"
+msgstr "Sirija"
 
 msgid "Syrian Arab Republic"
-msgstr "Cộng hòa Ả Rập Syria"
+msgstr "Sirija"
 
 msgid "Taiwan"
-msgstr "Đài Loan"
+msgstr "Tajvan"
 
 msgid "Taiwan (Province of China)"
-msgstr "Đài Loan (Tỉnh Trung Quốc)"
+msgstr "Tajvan"
 
 msgid "Tajikistan"
-msgstr "Tajikistan"
+msgstr "Tadžikistan"
 
 msgid "Tanzania"
-msgstr "Tanzania"
-
-msgid "Tanzania, the United Republic of"
-msgstr "Tanzania, Cộng hòa Thống nhất"
+msgstr "Tanzanija"
 
 msgid "Thailand"
-msgstr "Thái Lan"
+msgstr "Tajska"
 
 msgid "Timor-Leste"
-msgstr "Timor-Leste"
+msgstr "Timor"
 
 msgid "Togo"
 msgstr "Togo"
 
 msgid "Tokelau"
 msgstr "Tokelau"
 
 msgid "Tonga"
 msgstr "Tonga"
 
 msgid "Trinidad and Tobago"
-msgstr "Trinidad và Tobago"
+msgstr "Trinidad in Tobago"
 
 msgid "Tunisia"
-msgstr "Tunisia"
-
-msgid "Turkey"
-msgstr "Thổ Nhĩ Kỳ"
+msgstr "Tunizija"
 
 msgid "Turkmenistan"
 msgstr "Turkmenistan"
 
 msgid "Turks and Caicos Islands"
-msgstr "Quần đảo Thổ Nhĩ Kỳ và Caicos"
+msgstr "Otoki Turks in Caicos"
 
 msgid "Tuvalu"
 msgstr "Tuvalu"
 
+msgid "Türkiye"
+msgstr "Turčija"
+
 msgid "Uganda"
 msgstr "Uganda"
 
 msgid "Ukraine"
-msgstr "Ukraina"
+msgstr "Ukrajina"
 
 msgid "United Arab Emirates"
-msgstr "Các tiểu vương quốc Ả Rập thống nhất"
+msgstr "Združeni arabski emirati"
 
 msgid "United Kingdom"
-msgstr "Vương quốc Anh"
+msgstr "Združeno kraljestvo"
 
 msgid "United Kingdom of Great Britain and Northern Ireland"
-msgstr "Vương quốc Liên hiệp Anh và Bắc Ireland"
+msgstr "Združeno kraljestvo Velike Britanije in Severne Irske"
 
 msgid "United States Minor Outlying Islands"
-msgstr "Quần đảo xa xôi nhỏ của Hoa Kỳ"
+msgstr "Stranski zunanji otoki Združenih držav"
 
 msgid "United States of America"
-msgstr "Hợp chủng quốc Hoa Kỳ"
+msgstr "Združene države Amerike"
 
 msgid "Uruguay"
-msgstr "Uruguay"
+msgstr "Urugvaj"
 
 msgid "Uzbekistan"
 msgstr "Uzbekistan"
 
 msgid "Vanuatu"
 msgstr "Vanuatu"
 
 msgid "Venezuela"
 msgstr "Venezuela"
 
 msgid "Venezuela (Bolivarian Republic of)"
-msgstr "Venezuela (Cộng hòa Bolivar)"
+msgstr "Venezuela"
 
 msgid "Viet Nam"
-msgstr "Việt Nam"
+msgstr "Vietnam"
 
 msgid "Vietnam"
-msgstr "Việt Nam"
+msgstr "Vietnam"
 
 msgid "Virgin Islands (British)"
-msgstr "Quần đảo Virgin (Anh)"
+msgstr "Britanski Deviški otoki"
 
 msgid "Virgin Islands (U.S.)"
-msgstr "Quần đảo Virgin (Mỹ)"
+msgstr "Deviški otoki"
 
 msgid "Wallis and Futuna"
-msgstr "Wallis và Futuna"
+msgstr "Wallis in Futuna"
 
 msgid "Western Sahara"
-msgstr "Tây Sahara"
+msgstr "Zahodna Sahara"
 
 msgid "Yemen"
-msgstr "Yêmen"
+msgstr "Jemen"
 
 msgid "Zambia"
-msgstr "Zambia"
+msgstr "Zambija"
 
 msgid "Zimbabwe"
-msgstr "Zimbabwe"
+msgstr "Zimbabve"
 
 msgid "Åland Islands"
-msgstr "Quần đảo Åland"
+msgstr "Alandski otoki"
```

### Comparing `django-countries-7.6/django_countries/locale/vi/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/locale/zh_CN/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/smileychris/django-"
-"countries/language/zh_CN/)\n"
+"Language-Team: Chinese Simplified (http://www.transifex.com/smileychris/"
+"django-countries/language/zh-Hans/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
+"Language: zh-Hans\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Afghanistan"
 msgstr "阿富汗"
 
 msgid "Albania"
 msgstr "阿尔巴尼亚"
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "特立尼达和多巴哥共和国"
 
 msgid "Tunisia"
 msgstr "突尼斯"
 
-msgid "Turkey"
-msgstr "土耳其"
-
 msgid "Turkmenistan"
 msgstr "土库曼斯坦"
 
 msgid "Turks and Caicos Islands"
 msgstr "特克斯和凯科斯群岛"
 
 msgid "Tuvalu"
 msgstr "图瓦卢"
 
+msgid "Türkiye"
+msgstr "土耳其"
+
 msgid "Uganda"
 msgstr "乌干达"
 
 msgid "Ukraine"
 msgstr "乌克兰"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/zh_CN/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Carl Dong <accounts@carldong.me>, 2016
-# Chris Beaven <smileychris@gmail.com>, 2016
 # louyihua <supermouselyh@hotmail.com>, 2015
 # Zach Cheung <kuroro.zhang@gmail.com>, 2019
 # 薛文曜 <xuewenyao@hotmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-03-26 14:14+1300\n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/smileychris/django-countries/language/zh_CN/)\n"
+"Language-Team: Chinese Simplified (http://www.transifex.com/smileychris/django-countries/language/zh-Hans/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
+"Language: zh-Hans\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: base.py:11
 msgid "Brunei"
 msgstr "文莱"
 
 #: base.py:12
@@ -1003,15 +1002,15 @@
 msgstr "特立尼达和多巴哥共和国"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "突尼斯"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "土耳其"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "土库曼斯坦"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Chinese Simplified (http://www.transifex.com/smileychris/"
-"django-countries/language/zh-Hans/)\n"
+"Language-Team: Chinese (China) (http://www.transifex.com/smileychris/django-"
+"countries/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh-Hans\n"
+"Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Afghanistan"
 msgstr "阿富汗"
 
 msgid "Albania"
 msgstr "阿尔巴尼亚"
@@ -728,26 +728,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "特立尼达和多巴哥共和国"
 
 msgid "Tunisia"
 msgstr "突尼斯"
 
-msgid "Turkey"
-msgstr "土耳其"
-
 msgid "Turkmenistan"
 msgstr "土库曼斯坦"
 
 msgid "Turks and Caicos Islands"
 msgstr "特克斯和凯科斯群岛"
 
 msgid "Tuvalu"
 msgstr "图瓦卢"
 
+msgid "Türkiye"
+msgstr "土耳其"
+
 msgid "Uganda"
 msgstr "乌干达"
 
 msgid "Ukraine"
 msgstr "乌克兰"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/zh_Hans/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
 # Carl Dong <accounts@carldong.me>, 2016
+# Chris Beaven <smileychris@gmail.com>, 2016
 # louyihua <supermouselyh@hotmail.com>, 2015
 # Zach Cheung <kuroro.zhang@gmail.com>, 2019
 # 薛文曜 <xuewenyao@hotmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: django-countries\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-03-26 14:14+1300\n"
 "PO-Revision-Date: 2020-03-26 01:43+0000\n"
 "Last-Translator: Chris Beaven <smileychris@gmail.com>\n"
-"Language-Team: Chinese Simplified (http://www.transifex.com/smileychris/django-countries/language/zh-Hans/)\n"
+"Language-Team: Chinese (China) (http://www.transifex.com/smileychris/django-countries/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh-Hans\n"
+"Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: base.py:11
 msgid "Brunei"
 msgstr "文莱"
 
 #: base.py:12
@@ -1002,15 +1003,15 @@
 msgstr "特立尼达和多巴哥共和国"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "突尼斯"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "土耳其"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "土库曼斯坦"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/locale/zh_Hant/LC_MESSAGES/django.mo` & `django-countries-7.6.1/django_countries/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -740,26 +740,26 @@
 
 msgid "Trinidad and Tobago"
 msgstr "千里達及托巴哥"
 
 msgid "Tunisia"
 msgstr "突尼西亞"
 
-msgid "Turkey"
-msgstr "土耳其"
-
 msgid "Turkmenistan"
 msgstr "土庫曼"
 
 msgid "Turks and Caicos Islands"
 msgstr "特克斯與凱科斯群島"
 
 msgid "Tuvalu"
 msgstr "吐瓦魯"
 
+msgid "Türkiye"
+msgstr "土耳其"
+
 msgid "Uganda"
 msgstr "烏干達"
 
 msgid "Ukraine"
 msgstr "烏克蘭"
 
 msgid "United Arab Emirates"
```

### Comparing `django-countries-7.6/django_countries/locale/zh_Hant/LC_MESSAGES/django.po` & `django-countries-7.6.1/django_countries/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 msgstr "千里達及托巴哥"
 
 #: data.py:258
 msgid "Tunisia"
 msgstr "突尼西亞"
 
 #: data.py:259
-msgid "Turkey"
+msgid "Türkiye"
 msgstr "土耳其"
 
 #: data.py:260
 msgid "Turkmenistan"
 msgstr "土庫曼"
 
 #: data.py:261
```

### Comparing `django-countries-7.6/django_countries/makesprite.py` & `django-countries-7.6.1/django_countries/makesprite.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/release.py` & `django-countries-7.6.1/django_countries/release.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/serializer_fields.py` & `django-countries-7.6.1/django_countries/serializer_fields.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/serializers.py` & `django-countries-7.6.1/django_countries/serializers.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/bq.gif` & `django-countries-7.6.1/django_countries/static/flags/bq.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/gg.gif` & `django-countries-7.6.1/django_countries/static/flags/gg.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/im.gif` & `django-countries-7.6.1/django_countries/static/flags/im.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/je.gif` & `django-countries-7.6.1/django_countries/static/flags/je.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/mr.gif` & `django-countries-7.6.1/django_countries/static/flags/mr.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/sprite-hq.css` & `django-countries-7.6.1/django_countries/static/flags/sprite-hq.css`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/sprite-hq.png` & `django-countries-7.6.1/django_countries/static/flags/sprite-hq.png`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/sprite.css` & `django-countries-7.6.1/django_countries/static/flags/sprite.css`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/sprite.png` & `django-countries-7.6.1/django_countries/static/flags/sprite.png`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/ss.gif` & `django-countries-7.6.1/django_countries/static/flags/ss.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/sx.gif` & `django-countries-7.6.1/django_countries/static/flags/sx.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/static/flags/xk.gif` & `django-countries-7.6.1/django_countries/static/flags/xk.gif`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/custom_countries.py` & `django-countries-7.6.1/django_countries/tests/custom_countries.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/graphql/schema.py` & `django-countries-7.6.1/django_countries/tests/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/models.py` & `django-countries-7.6.1/django_countries/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/settings.py` & `django-countries-7.6.1/django_countries/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_admin_filters.py` & `django-countries-7.6.1/django_countries/tests/test_admin_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.contrib import admin
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.models import AnonymousUser
 from django.test import TestCase
 from django.test.client import RequestFactory
 
-from django_countries import filters
+from django_countries import countries, filters
 from django_countries.tests import models
 
 test_site = admin.AdminSite(name="test-admin")
 
 
 class PersonAdmin(admin.ModelAdmin):
     list_filter = [("country", filters.CountryFilter)]
@@ -47,17 +47,30 @@
         request.user = AnonymousUser()
         cl = ChangeList(request, **self.get_changelist_kwargs())
         cl.get_results(request)
         self.assertEqual(
             list(cl.result_list), list(models.Person.objects.exclude(country="AU"))
         )
 
-    def test_choices(self):
-        request = RequestFactory().get("/person/", data={"country": "NZ"})
+    def _test_choices(self, selected_country_code="NZ"):
+        request_params = {}
+        selected_country = "All"
+
+        if selected_country_code:
+            request_params["country"] = selected_country_code
+            selected_country = countries.name(selected_country_code)
+
+        request = RequestFactory().get("/person/", data=request_params)
         request.user = AnonymousUser()
         cl = ChangeList(request, **self.get_changelist_kwargs())
         choices = list(cl.filter_specs[0].choices(cl))
         self.assertEqual(
             [c["display"] for c in choices], ["All", "Australia", "New Zealand"]
         )
         for choice in choices:
-            self.assertEqual(choice["selected"], choice["display"] == "New Zealand")
+            self.assertEqual(choice["selected"], choice["display"] == selected_country)
+
+    def test_choices(self):
+        return self._test_choices()
+
+    def test_choices_empty_selection(self):
+        return self._test_choices(selected_country_code=None)
```

### Comparing `django-countries-7.6/django_countries/tests/test_countries.py` & `django-countries-7.6.1/django_countries/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_drf.py` & `django-countries-7.6.1/django_countries/tests/test_drf.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_fields.py` & `django-countries-7.6.1/django_countries/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_settings.py` & `django-countries-7.6.1/django_countries/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_tags.py` & `django-countries-7.6.1/django_countries/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/tests/test_widgets.py` & `django-countries-7.6.1/django_countries/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries/widgets.py` & `django-countries-7.6.1/django_countries/widgets.py`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/django_countries.egg-info/PKG-INFO` & `django-countries-7.6.1/django_countries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-countries
-Version: 7.6
+Version: 7.6.1
 Summary: Provides a country field for Django models.
 Home-page: https://github.com/SmileyChris/django-countries/
 Author: Chris Beaven
 Author-email: smileychris@gmail.com
 License: MIT
 Project-URL: Change Log, https://github.com/SmileyChris/django-countries/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/SmileyChris/django-countries
@@ -628,14 +628,20 @@
 Change Log
 ==========
 
 This log shows interesting changes that happen for each version, latest
 versions first. It can be assumed that translations have been updated each
 release, and any new translations added.
 
+7.6.1 (2 April 2024)
+====================
+
+- Fix a TypeError when no country is selected, introduced in the Django 5 fix.
+
+
 7.6 (27 March 2024)
 ===================
 
 - Replace deprecated ``pkg_resources.iter_entry_points`` with
   ``importlib_metadata``.
 
 - Support Django 5.0.
```

### Comparing `django-countries-7.6/django_countries.egg-info/SOURCES.txt` & `django-countries-7.6.1/django_countries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-countries-7.6/setup.cfg` & `django-countries-7.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-countries
-version = 7.6
+version = 7.6.1
 description = Provides a country field for Django models.
 long_description = file: README.rst, CHANGES.rst
 author = Chris Beaven
 author_email = smileychris@gmail.com
 url = https://github.com/SmileyChris/django-countries/
 keywords = django, countries, flags
 license = MIT
```

