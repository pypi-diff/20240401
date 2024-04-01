# Comparing `tmp/django-quizblock-1.2.8.tar.gz` & `tmp/django-quizblock-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-quizblock-1.2.8.tar", last modified: Sat Apr  9 00:42:08 2022, max compression
+gzip compressed data, was "django-quizblock-1.3.0.tar", last modified: Thu Mar 28 20:10:01 2024, max compression
```

## Comparing `django-quizblock-1.2.8.tar` & `django-quizblock-1.3.0.tar`

### file list

```diff
@@ -1,86 +1,82 @@
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.174061 django-quizblock-1.2.8/
--rw-r--r--   0 sdreher    (501) staff       (20)       33 2014-06-27 19:20:52.000000 django-quizblock-1.2.8/MANIFEST.in
--rw-r--r--   0 sdreher    (501) staff       (20)      297 2022-04-09 00:42:08.174306 django-quizblock-1.2.8/PKG-INFO
--rw-r--r--   0 sdreher    (501) staff       (20)      322 2022-04-08 15:39:43.000000 django-quizblock-1.2.8/README.md
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.127965 django-quizblock-1.2.8/django_quizblock.egg-info/
--rw-r--r--   0 sdreher    (501) staff       (20)      297 2022-04-09 00:42:07.000000 django-quizblock-1.2.8/django_quizblock.egg-info/PKG-INFO
--rw-r--r--   0 sdreher    (501) staff       (20)     3040 2022-04-09 00:42:08.000000 django-quizblock-1.2.8/django_quizblock.egg-info/SOURCES.txt
--rw-r--r--   0 sdreher    (501) staff       (20)        1 2022-04-09 00:42:07.000000 django-quizblock-1.2.8/django_quizblock.egg-info/dependency_links.txt
--rw-r--r--   0 sdreher    (501) staff       (20)        1 2015-03-04 18:39:58.000000 django-quizblock-1.2.8/django_quizblock.egg-info/not-zip-safe
--rw-r--r--   0 sdreher    (501) staff       (20)       23 2022-04-09 00:42:07.000000 django-quizblock-1.2.8/django_quizblock.egg-info/requires.txt
--rw-r--r--   0 sdreher    (501) staff       (20)       10 2022-04-09 00:42:08.000000 django-quizblock-1.2.8/django_quizblock.egg-info/top_level.txt
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.132821 django-quizblock-1.2.8/quizblock/
--rw-r--r--   0 sdreher    (501) staff       (20)     6148 2022-01-22 01:46:44.000000 django-quizblock-1.2.8/quizblock/.DS_Store
--rw-r--r--   0 sdreher    (501) staff       (20)       54 2016-06-16 12:56:25.000000 django-quizblock-1.2.8/quizblock/__init__.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.135720 django-quizblock-1.2.8/quizblock/__pycache__/
--rw-r--r--   0 sdreher    (501) staff       (20)      207 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      693 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/__pycache__/apps.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)    17700 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     1192 2022-04-08 15:47:15.000000 django-quizblock-1.2.8/quizblock/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     5885 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      187 2018-05-21 12:58:49.000000 django-quizblock-1.2.8/quizblock/admin.py
--rw-r--r--   0 sdreher    (501) staff       (20)      305 2016-06-16 12:56:34.000000 django-quizblock-1.2.8/quizblock/apps.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.141659 django-quizblock-1.2.8/quizblock/migrations/
--rw-r--r--   0 sdreher    (501) staff       (20)     4310 2019-06-17 19:17:13.000000 django-quizblock-1.2.8/quizblock/migrations/0001_initial.py
--rw-r--r--   0 sdreher    (501) staff       (20)      443 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/migrations/0002_auto_20150202_1707.py
--rw-r--r--   0 sdreher    (501) staff       (20)      714 2016-06-16 12:56:34.000000 django-quizblock-1.2.8/quizblock/migrations/0003_auto_20150209_1601.py
--rw-r--r--   0 sdreher    (501) staff       (20)      515 2016-06-16 12:56:34.000000 django-quizblock-1.2.8/quizblock/migrations/0004_question_css_extra.py
--rw-r--r--   0 sdreher    (501) staff       (20)      445 2020-08-18 18:04:14.000000 django-quizblock-1.2.8/quizblock/migrations/0006_auto_20160613_1001.py
--rw-r--r--   0 sdreher    (501) staff       (20)      459 2016-06-16 12:56:32.000000 django-quizblock-1.2.8/quizblock/migrations/0006_auto_20160613_1001.py~
--rw-r--r--   0 sdreher    (501) staff       (20)        0 2014-01-18 16:15:47.000000 django-quizblock-1.2.8/quizblock/migrations/__init__.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.144747 django-quizblock-1.2.8/quizblock/migrations/__pycache__/
--rw-r--r--   0 sdreher    (501) staff       (20)     2307 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      677 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/0002_auto_20150202_1707.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      838 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/0003_auto_20150209_1601.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      734 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/0004_question_css_extra.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      612 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/0006_auto_20160613_1001.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)      165 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)    18012 2022-04-08 15:39:43.000000 django-quizblock-1.2.8/quizblock/models.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.120959 django-quizblock-1.2.8/quizblock/static/
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.121060 django-quizblock-1.2.8/quizblock/static/quizblock/
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.146046 django-quizblock-1.2.8/quizblock/static/quizblock/js/
--rw-r--r--   0 sdreher    (501) staff       (20)     1467 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/static/quizblock/js/quizblock-admin.js
--rw-r--r--   0 sdreher    (501) staff       (20)     2180 2015-07-07 14:21:38.000000 django-quizblock-1.2.8/quizblock/static/quizblock/js/quizshow.js
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.121319 django-quizblock-1.2.8/quizblock/templates/
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.161743 django-quizblock-1.2.8/quizblock/templates/quizblock/
--rw-r--r--   0 sdreher    (501) staff       (20)      214 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/answer_confirm_delete.html
--rw-r--r--   0 sdreher    (501) staff       (20)      782 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/edit_answer.html
--rw-r--r--   0 sdreher    (501) staff       (20)     2832 2022-04-08 16:54:01.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/edit_question.html
--rw-r--r--   0 sdreher    (501) staff       (20)      507 2016-06-16 12:56:25.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/include_jquery.html
--rw-r--r--   0 sdreher    (501) staff       (20)      440 2015-03-05 16:31:42.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/long_answer_show_answer.html
--rw-r--r--   0 sdreher    (501) staff       (20)      544 2015-03-05 16:31:42.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/long_text.html
--rw-r--r--   0 sdreher    (501) staff       (20)     2438 2015-07-07 14:21:38.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/multiple_choice.html
--rw-r--r--   0 sdreher    (501) staff       (20)     1071 2015-07-07 14:21:38.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/multiple_choice_show_answer.html
--rw-r--r--   0 sdreher    (501) staff       (20)     1312 2015-10-14 16:16:12.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/question.html
--rw-r--r--   0 sdreher    (501) staff       (20)      214 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/question_confirm_delete.html
--rw-r--r--   0 sdreher    (501) staff       (20)     2457 2022-04-08 16:54:01.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/quiz_detail.html
--rw-r--r--   0 sdreher    (501) staff       (20)      426 2022-04-08 16:54:01.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/quizblock.html
--rw-r--r--   0 sdreher    (501) staff       (20)      414 2015-03-05 16:31:42.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/short_text.html
--rw-r--r--   0 sdreher    (501) staff       (20)      358 2014-01-18 16:15:47.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/show_answer.html
--rw-r--r--   0 sdreher    (501) staff       (20)     2080 2015-07-07 14:21:38.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice.html
--rw-r--r--   0 sdreher    (501) staff       (20)      608 2015-02-24 14:30:34.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice_dropdown.html
--rw-r--r--   0 sdreher    (501) staff       (20)      688 2016-07-07 14:44:48.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice_show_answer.html
--rw-r--r--   0 sdreher    (501) staff       (20)      688 2015-03-05 16:31:42.000000 django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice_show_answer.html~
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.163728 django-quizblock-1.2.8/quizblock/templatetags/
--rw-r--r--   0 sdreher    (501) staff       (20)        0 2014-01-18 16:15:47.000000 django-quizblock-1.2.8/quizblock/templatetags/__init__.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.165284 django-quizblock-1.2.8/quizblock/templatetags/__pycache__/
--rw-r--r--   0 sdreher    (501) staff       (20)      167 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     2482 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/templatetags/__pycache__/getresponse.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     2084 2014-01-26 14:41:00.000000 django-quizblock-1.2.8/quizblock/templatetags/getresponse.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.170666 django-quizblock-1.2.8/quizblock/tests/
--rw-r--r--   0 sdreher    (501) staff       (20)        0 2016-06-16 12:56:25.000000 django-quizblock-1.2.8/quizblock/tests/__init__.py
-drwxr-xr-x   0 sdreher    (501) staff       (20)        0 2022-04-09 00:42:08.173546 django-quizblock-1.2.8/quizblock/tests/__pycache__/
--rw-r--r--   0 sdreher    (501) staff       (20)      160 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)    17399 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/tests/__pycache__/test_models.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     5984 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/tests/__pycache__/test_reports.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     4314 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/tests/__pycache__/test_templatetags.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)     6602 2022-04-08 15:47:12.000000 django-quizblock-1.2.8/quizblock/tests/__pycache__/test_views.cpython-39.pyc
--rw-r--r--   0 sdreher    (501) staff       (20)    19718 2018-05-21 12:58:49.000000 django-quizblock-1.2.8/quizblock/tests/test_models.py
--rw-r--r--   0 sdreher    (501) staff       (20)    19370 2015-03-05 17:16:47.000000 django-quizblock-1.2.8/quizblock/tests/test_models.py~
--rw-r--r--   0 sdreher    (501) staff       (20)     8748 2016-06-16 12:56:34.000000 django-quizblock-1.2.8/quizblock/tests/test_reports.py
--rw-r--r--   0 sdreher    (501) staff       (20)     4595 2016-06-16 12:56:25.000000 django-quizblock-1.2.8/quizblock/tests/test_templatetags.py
--rw-r--r--   0 sdreher    (501) staff       (20)     8111 2016-06-16 12:56:25.000000 django-quizblock-1.2.8/quizblock/tests/test_views.py
--rw-r--r--   0 sdreher    (501) staff       (20)     1244 2016-06-16 12:56:34.000000 django-quizblock-1.2.8/quizblock/urls.py
--rw-r--r--   0 sdreher    (501) staff       (20)     4521 2019-06-17 19:17:13.000000 django-quizblock-1.2.8/quizblock/views.py
--rw-r--r--   0 sdreher    (501) staff       (20)       67 2022-04-09 00:42:08.175081 django-quizblock-1.2.8/setup.cfg
--rw-r--r--   0 sdreher    (501) staff       (20)     2154 2022-04-09 00:36:11.000000 django-quizblock-1.2.8/setup.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.185834 django-quizblock-1.3.0/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       33 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/MANIFEST.in
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      349 2024-03-28 20:10:01.185778 django-quizblock-1.3.0/PKG-INFO
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      322 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/README.md
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.185542 django-quizblock-1.3.0/django_quizblock.egg-info/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      349 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/PKG-INFO
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2895 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/SOURCES.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        1 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/dependency_links.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)        1 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/not-zip-safe
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       23 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/requires.txt
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       10 2024-03-28 20:10:01.000000 django-quizblock-1.3.0/django_quizblock.egg-info/top_level.txt
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.173865 django-quizblock-1.3.0/quizblock/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       54 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/quizblock/__init__.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.175675 django-quizblock-1.3.0/quizblock/__pycache__/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      226 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      954 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    31834 2024-03-28 20:06:22.000000 django-quizblock-1.3.0/quizblock/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1973 2024-03-28 19:45:36.000000 django-quizblock-1.3.0/quizblock/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    10196 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      187 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/quizblock/admin.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      305 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/quizblock/apps.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.176890 django-quizblock-1.3.0/quizblock/migrations/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4310 2024-03-28 19:29:48.000000 django-quizblock-1.3.0/quizblock/migrations/0001_initial.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      443 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/migrations/0002_auto_20150202_1707.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      714 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/migrations/0003_auto_20150209_1601.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      515 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/migrations/0004_question_css_extra.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      445 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/migrations/0006_auto_20160613_1001.py
+-rw-------   0 evanpetersen   (502) staff       (20)        0 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/migrations/__init__.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.178149 django-quizblock-1.3.0/quizblock/migrations/__pycache__/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4393 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      912 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/0002_auto_20150202_1707.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1167 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/0003_auto_20150209_1601.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      978 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/0004_question_css_extra.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      846 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/0006_auto_20160613_1001.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      182 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    18122 2024-03-28 20:06:14.000000 django-quizblock-1.3.0/quizblock/models.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.170575 django-quizblock-1.3.0/quizblock/static/
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.170646 django-quizblock-1.3.0/quizblock/static/quizblock/
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.178625 django-quizblock-1.3.0/quizblock/static/quizblock/js/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1467 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/static/quizblock/js/quizblock-admin.js
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2180 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/static/quizblock/js/quizshow.js
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.170802 django-quizblock-1.3.0/quizblock/templates/
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.181885 django-quizblock-1.3.0/quizblock/templates/quizblock/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      214 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/answer_confirm_delete.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      782 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/edit_answer.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2832 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/edit_question.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      507 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/include_jquery.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      440 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/long_answer_show_answer.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      544 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/long_text.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2438 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/multiple_choice.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1071 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/multiple_choice_show_answer.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1312 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/question.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      214 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/question_confirm_delete.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2457 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/quiz_detail.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      426 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/quizblock.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      414 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/short_text.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      358 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/show_answer.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2080 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      608 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice_dropdown.html
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      688 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice_show_answer.html
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.182170 django-quizblock-1.3.0/quizblock/templatetags/
+-rw-------   0 evanpetersen   (502) staff       (20)        0 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templatetags/__init__.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.182471 django-quizblock-1.3.0/quizblock/templatetags/__pycache__/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      184 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4465 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/templatetags/__pycache__/getresponse.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2084 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/templatetags/getresponse.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.183504 django-quizblock-1.3.0/quizblock/tests/
+-rw-------   0 evanpetersen   (502) staff       (20)        0 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/tests/__init__.py
+drwxr-xr-x   0 evanpetersen   (502) staff       (20)        0 2024-03-28 20:10:01.185097 django-quizblock-1.3.0/quizblock/tests/__pycache__/
+-rw-r--r--   0 evanpetersen   (502) staff       (20)      177 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    39220 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/tests/__pycache__/test_models.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    14491 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/tests/__pycache__/test_reports.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     8592 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/tests/__pycache__/test_templatetags.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    14757 2024-03-28 19:41:33.000000 django-quizblock-1.3.0/quizblock/tests/__pycache__/test_views.cpython-311.pyc
+-rw-r--r--   0 evanpetersen   (502) staff       (20)    19712 2024-03-28 19:30:36.000000 django-quizblock-1.3.0/quizblock/tests/test_models.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     8748 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/tests/test_reports.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4595 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/tests/test_templatetags.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     8111 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/tests/test_views.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     1323 2024-03-28 19:41:12.000000 django-quizblock-1.3.0/quizblock/urls.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     4521 2024-03-28 19:29:49.000000 django-quizblock-1.3.0/quizblock/views.py
+-rw-r--r--   0 evanpetersen   (502) staff       (20)       67 2024-03-28 20:10:01.186035 django-quizblock-1.3.0/setup.cfg
+-rw-r--r--   0 evanpetersen   (502) staff       (20)     2169 2024-03-28 19:37:03.000000 django-quizblock-1.3.0/setup.py
```

### Comparing `django-quizblock-1.2.8/django_quizblock.egg-info/SOURCES.txt` & `django-quizblock-1.3.0/django_quizblock.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,39 +4,37 @@
 setup.py
 django_quizblock.egg-info/PKG-INFO
 django_quizblock.egg-info/SOURCES.txt
 django_quizblock.egg-info/dependency_links.txt
 django_quizblock.egg-info/not-zip-safe
 django_quizblock.egg-info/requires.txt
 django_quizblock.egg-info/top_level.txt
-quizblock/.DS_Store
 quizblock/__init__.py
 quizblock/admin.py
 quizblock/apps.py
 quizblock/models.py
 quizblock/urls.py
 quizblock/views.py
-quizblock/__pycache__/__init__.cpython-39.pyc
-quizblock/__pycache__/apps.cpython-39.pyc
-quizblock/__pycache__/models.cpython-39.pyc
-quizblock/__pycache__/urls.cpython-39.pyc
-quizblock/__pycache__/views.cpython-39.pyc
+quizblock/__pycache__/__init__.cpython-311.pyc
+quizblock/__pycache__/apps.cpython-311.pyc
+quizblock/__pycache__/models.cpython-311.pyc
+quizblock/__pycache__/urls.cpython-311.pyc
+quizblock/__pycache__/views.cpython-311.pyc
 quizblock/migrations/0001_initial.py
 quizblock/migrations/0002_auto_20150202_1707.py
 quizblock/migrations/0003_auto_20150209_1601.py
 quizblock/migrations/0004_question_css_extra.py
 quizblock/migrations/0006_auto_20160613_1001.py
-quizblock/migrations/0006_auto_20160613_1001.py~
 quizblock/migrations/__init__.py
-quizblock/migrations/__pycache__/0001_initial.cpython-39.pyc
-quizblock/migrations/__pycache__/0002_auto_20150202_1707.cpython-39.pyc
-quizblock/migrations/__pycache__/0003_auto_20150209_1601.cpython-39.pyc
-quizblock/migrations/__pycache__/0004_question_css_extra.cpython-39.pyc
-quizblock/migrations/__pycache__/0006_auto_20160613_1001.cpython-39.pyc
-quizblock/migrations/__pycache__/__init__.cpython-39.pyc
+quizblock/migrations/__pycache__/0001_initial.cpython-311.pyc
+quizblock/migrations/__pycache__/0002_auto_20150202_1707.cpython-311.pyc
+quizblock/migrations/__pycache__/0003_auto_20150209_1601.cpython-311.pyc
+quizblock/migrations/__pycache__/0004_question_css_extra.cpython-311.pyc
+quizblock/migrations/__pycache__/0006_auto_20160613_1001.cpython-311.pyc
+quizblock/migrations/__pycache__/__init__.cpython-311.pyc
 quizblock/static/quizblock/js/quizblock-admin.js
 quizblock/static/quizblock/js/quizshow.js
 quizblock/templates/quizblock/answer_confirm_delete.html
 quizblock/templates/quizblock/edit_answer.html
 quizblock/templates/quizblock/edit_question.html
 quizblock/templates/quizblock/include_jquery.html
 quizblock/templates/quizblock/long_answer_show_answer.html
@@ -48,23 +46,21 @@
 quizblock/templates/quizblock/quiz_detail.html
 quizblock/templates/quizblock/quizblock.html
 quizblock/templates/quizblock/short_text.html
 quizblock/templates/quizblock/show_answer.html
 quizblock/templates/quizblock/single_choice.html
 quizblock/templates/quizblock/single_choice_dropdown.html
 quizblock/templates/quizblock/single_choice_show_answer.html
-quizblock/templates/quizblock/single_choice_show_answer.html~
 quizblock/templatetags/__init__.py
 quizblock/templatetags/getresponse.py
-quizblock/templatetags/__pycache__/__init__.cpython-39.pyc
-quizblock/templatetags/__pycache__/getresponse.cpython-39.pyc
+quizblock/templatetags/__pycache__/__init__.cpython-311.pyc
+quizblock/templatetags/__pycache__/getresponse.cpython-311.pyc
 quizblock/tests/__init__.py
 quizblock/tests/test_models.py
-quizblock/tests/test_models.py~
 quizblock/tests/test_reports.py
 quizblock/tests/test_templatetags.py
 quizblock/tests/test_views.py
-quizblock/tests/__pycache__/__init__.cpython-39.pyc
-quizblock/tests/__pycache__/test_models.cpython-39.pyc
-quizblock/tests/__pycache__/test_reports.cpython-39.pyc
-quizblock/tests/__pycache__/test_templatetags.cpython-39.pyc
-quizblock/tests/__pycache__/test_views.cpython-39.pyc
+quizblock/tests/__pycache__/__init__.cpython-311.pyc
+quizblock/tests/__pycache__/test_models.cpython-311.pyc
+quizblock/tests/__pycache__/test_reports.cpython-311.pyc
+quizblock/tests/__pycache__/test_templatetags.cpython-311.pyc
+quizblock/tests/__pycache__/test_views.cpython-311.pyc
```

### Comparing `django-quizblock-1.2.8/quizblock/__pycache__/apps.cpython-39.pyc` & `django-quizblock-1.3.0/quizblock/__pycache__/apps.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 16 12:56:34 2016 UTC, .py size: 305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-00000000: 610d 0d0a 0000 0000 02a2 6257 3101 0000  a.........bW1...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000050: 6503 8303 5a04 6405 5300 2906 e900 0000  e...Z.d.S.).....
-00000060: 0029 01da 1075 6e69 636f 6465 5f6c 6974  .)...unicode_lit
-00000070: 6572 616c 7329 01da 0941 7070 436f 6e66  erals)...AppConf
-00000080: 6967 6300 0000 0000 0000 0000 0000 0000  igc.............
-00000090: 0000 0002 0000 0040 0000 0073 1c00 0000  .......@...s....
-000000a0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-000000b0: 6403 6404 8400 5a05 6405 5300 2906 da0f  d.d...Z.d.S.)...
-000000c0: 5175 697a 426c 6f63 6b43 6f6e 6669 67da  QuizBlockConfig.
-000000d0: 0971 7569 7a62 6c6f 636b 5a09 5175 697a  .quizblockZ.Quiz
-000000e0: 626c 6f63 6b63 0100 0000 0000 0000 0000  blockc..........
-000000f0: 0000 0200 0000 0500 0000 4300 0000 7320  ..........C...s 
-00000100: 0000 0064 0164 026c 006d 017d 0101 007c  ...d.d.l.m.}...|
-00000110: 01a0 027c 00a0 0364 03a1 01a1 0101 0064  ...|...d.......d
-00000120: 0053 0029 044e 7201 0000 0029 01da 1352  .S.).Nr....)...R
-00000130: 6570 6f72 7461 626c 6549 6e74 6572 6661  eportableInterfa
-00000140: 6365 5a04 5175 697a 2904 5a10 7061 6765  ceZ.Quiz).Z.page
-00000150: 7472 6565 2e72 6570 6f72 7473 7206 0000  tree.reportsr...
-00000160: 00da 0872 6567 6973 7465 72da 0967 6574  ...register..get
-00000170: 5f6d 6f64 656c 2902 da04 7365 6c66 7206  _model)...selfr.
-00000180: 0000 00a9 0072 0a00 0000 fa3b 2f55 7365  .....r.....;/Use
-00000190: 7273 2f73 6472 6568 6572 2f77 6f72 6b73  rs/sdreher/works
-000001a0: 7061 6365 2f64 6a61 6e67 6f2d 7175 697a  pace/django-quiz
-000001b0: 626c 6f63 6b2f 7175 697a 626c 6f63 6b2f  block/quizblock/
-000001c0: 6170 7073 2e70 79da 0572 6561 6479 0a00  apps.py..ready..
-000001d0: 0000 7304 0000 0000 010c 017a 1551 7569  ..s........z.Qui
-000001e0: 7a42 6c6f 636b 436f 6e66 6967 2e72 6561  zBlockConfig.rea
-000001f0: 6479 4e29 06da 085f 5f6e 616d 655f 5fda  dyN)...__name__.
-00000200: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000210: 7561 6c6e 616d 655f 5fda 046e 616d 65da  ualname__..name.
-00000220: 0c76 6572 626f 7365 5f6e 616d 6572 0c00  .verbose_namer..
-00000230: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000240: 0072 0b00 0000 7204 0000 0006 0000 0073  .r....r........s
-00000250: 0600 0000 0801 0401 0402 7204 0000 004e  ..........r....N
-00000260: 2905 5a0a 5f5f 6675 7475 7265 5f5f 7202  ).Z.__future__r.
-00000270: 0000 00da 0b64 6a61 6e67 6f2e 6170 7073  .....django.apps
-00000280: 7203 0000 0072 0400 0000 720a 0000 0072  r....r....r....r
-00000290: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-000002a0: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-000002b0: 000c 020c 03                             .....
+00000000: a70d 0d0a 0000 0000 2cc5 0566 3101 0000  ........,..f1...
+00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
+00000020: 0000 0000 00f3 3a00 0000 9700 6400 6401  ......:.....d.d.
+00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
+00000040: 5a03 0100 0200 4700 6403 8400 6404 6503  Z.....G.d...d.e.
+00000050: a603 0000 ab03 0000 0000 0000 0000 5a04  ..............Z.
+00000060: 6405 5300 2906 e900 0000 0029 01da 1075  d.S.)......)...u
+00000070: 6e69 636f 6465 5f6c 6974 6572 616c 7329  nicode_literals)
+00000080: 01da 0941 7070 436f 6e66 6967 6300 0000  ...AppConfigc...
+00000090: 0000 0000 0000 0000 0001 0000 0000 0000  ................
+000000a0: 00f3 1c00 0000 9700 6500 5a01 6400 5a02  ........e.Z.d.Z.
+000000b0: 6401 5a03 6402 5a04 6403 8400 5a05 6404  d.Z.d.Z.d...Z.d.
+000000c0: 5300 2905 da0f 5175 697a 426c 6f63 6b43  S.)...QuizBlockC
+000000d0: 6f6e 6669 67da 0971 7569 7a62 6c6f 636b  onfig..quizblock
+000000e0: da09 5175 697a 626c 6f63 6b63 0100 0000  ..Quizblockc....
+000000f0: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000100: f362 0000 0097 0064 0164 026c 006d 017d  .b.....d.d.l.m.}
+00000110: 0101 007c 01a0 0200 0000 0000 0000 0000  ...|............
+00000120: 0000 0000 0000 0000 0000 007c 00a0 0300  ...........|....
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0064 03a6 0100 00ab 0100 0000 0000  ...d............
+00000150: 0000 00a6 0100 00ab 0100 0000 0000 0000  ................
+00000160: 0001 0064 0053 0029 044e 7202 0000 0029  ...d.S.).Nr....)
+00000170: 01da 1352 6570 6f72 7461 626c 6549 6e74  ...ReportableInt
+00000180: 6572 6661 6365 da04 5175 697a 2904 da10  erface..Quiz)...
+00000190: 7061 6765 7472 6565 2e72 6570 6f72 7473  pagetree.reports
+000001a0: 720a 0000 00da 0872 6567 6973 7465 72da  r......register.
+000001b0: 0967 6574 5f6d 6f64 656c 2902 da04 7365  .get_model)...se
+000001c0: 6c66 720a 0000 0073 0200 0000 2020 fa3a  lfr....s....  .:
+000001d0: 2f55 7365 7273 2f65 7661 6e70 6574 6572  /Users/evanpeter
+000001e0: 7365 6e2f 6374 6c2f 646a 616e 676f 2d71  sen/ctl/django-q
+000001f0: 7569 7a62 6c6f 636b 2f71 7569 7a62 6c6f  uizblock/quizblo
+00000200: 636b 2f61 7070 732e 7079 da05 7265 6164  ck/apps.py..read
+00000210: 797a 1551 7569 7a42 6c6f 636b 436f 6e66  yz.QuizBlockConf
+00000220: 6967 2e72 6561 6479 0a00 0000 733a 0000  ig.ready....s:..
+00000230: 0080 00d8 0838 d008 38d0 0838 d008 38d0  .....8..8..8..8.
+00000240: 0838 d008 38d8 081b d708 24d2 0824 a054  .8..8.....$..$.T
+00000250: a75e a25e b046 d125 3bd4 253b d108 3cd4  .^.^.F.%;.%;..<.
+00000260: 083c d008 3cd0 083c d008 3cf3 0000 0000  .<..<..<..<.....
+00000270: 4e29 06da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000280: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000290: 6c6e 616d 655f 5fda 046e 616d 65da 0c76  lname__..name..v
+000002a0: 6572 626f 7365 5f6e 616d 6572 1100 0000  erbose_namer....
+000002b0: a900 7212 0000 0072 1000 0000 7206 0000  ..r....r....r...
+000002c0: 0072 0600 0000 0600 0000 732d 0000 0080  .r........s-....
+000002d0: 0080 0080 0080 0080 00d8 0b16 8044 d813  .............D..
+000002e0: 1e80 4cf0 0402 053d f000 0205 3df0 0002  ..L....=....=...
+000002f0: 053d f000 0205 3df0 0002 053d 7212 0000  .=....=....=r...
+00000300: 0072 0600 0000 4e29 05da 0a5f 5f66 7574  .r....N)...__fut
+00000310: 7572 655f 5f72 0300 0000 da0b 646a 616e  ure__r......djan
+00000320: 676f 2e61 7070 7372 0400 0000 7206 0000  go.appsr....r...
+00000330: 0072 1800 0000 7212 0000 0072 1000 0000  .r....r....r....
+00000340: fa08 3c6d 6f64 756c 653e 721b 0000 0001  ..<module>r.....
+00000350: 0000 0073 5d00 0000 f003 0101 01d8 0027  ...s]..........'
+00000360: d000 27d0 0027 d000 27d0 0027 d000 27e0  ..'..'..'..'..'.
+00000370: 0021 d000 21d0 0021 d000 21d0 0021 d000  .!..!..!..!..!..
+00000380: 21f0 0606 013d f000 0601 3df0 0006 013d  !....=....=....=
+00000390: f000 0601 3df0 0006 013d 9069 f100 0601  ....=....=.i....
+000003a0: 3df4 0006 013d f000 0601 3df0 0006 013d  =....=....=....=
+000003b0: f000 0601 3d72 1200 0000                 ....=r....
```

### Comparing `django-quizblock-1.2.8/quizblock/migrations/0001_initial.py` & `django-quizblock-1.3.0/quizblock/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/migrations/0003_auto_20150209_1601.py` & `django-quizblock-1.3.0/quizblock/migrations/0003_auto_20150209_1601.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/migrations/0004_question_css_extra.py` & `django-quizblock-1.3.0/quizblock/migrations/0004_question_css_extra.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/migrations/__pycache__/0004_question_css_extra.cpython-39.pyc` & `django-quizblock-1.3.0/quizblock/migrations/__pycache__/0004_question_css_extra.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 16 12:56:34 2016 UTC, .py size: 515 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-00000000: 610d 0d0a 0000 0000 02a2 6257 0302 0000  a.........bW....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
-00000050: 8400 6404 6504 6a05 8303 5a05 6405 5300  ..d.e.j...Z.d.S.
-00000060: 2906 e900 0000 0029 01da 1075 6e69 636f  )......)...unico
-00000070: 6465 5f6c 6974 6572 616c 7329 02da 066d  de_literals)...m
-00000080: 6f64 656c 73da 0a6d 6967 7261 7469 6f6e  odels..migration
-00000090: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-000000a0: 0000 0800 0000 4000 0000 7332 0000 0065  ......@...s2...e
-000000b0: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000c0: 0564 0264 0365 066a 0764 0464 0564 0564  .d.d.e.j.d.d.d.d
-000000d0: 068d 0364 0564 078d 0467 015a 0864 0853  ...d.d...g.Z.d.S
-000000e0: 0029 09da 094d 6967 7261 7469 6f6e 2902  .)...Migration).
-000000f0: da09 7175 697a 626c 6f63 6bda 1730 3030  ..quizblock..000
-00000100: 335f 6175 746f 5f32 3031 3530 3230 395f  3_auto_20150209_
-00000110: 3136 3031 da08 7175 6573 7469 6f6e da09  1601..question..
-00000120: 6373 735f 6578 7472 6173 2300 0000 6578  css_extras#...ex
-00000130: 7472 6120 4353 5320 636c 6173 7365 7320  tra CSS classes 
-00000140: 2873 7061 6365 2073 6570 6172 6174 6564  (space separated
-00000150: 2954 2903 da09 6865 6c70 5f74 6578 74da  )T)...help_text.
-00000160: 046e 756c 6cda 0562 6c61 6e6b 2904 da0a  .null..blank)...
-00000170: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
-00000180: da05 6669 656c 64da 1070 7265 7365 7276  ..field..preserv
-00000190: 655f 6465 6661 756c 744e 2909 da08 5f5f  e_defaultN)...__
-000001a0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000001b0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000001c0: da0c 6465 7065 6e64 656e 6369 6573 7204  ..dependenciesr.
-000001d0: 0000 00da 0841 6464 4669 656c 6472 0300  .....AddFieldr..
-000001e0: 0000 da09 5465 7874 4669 656c 64da 0a6f  ....TextField..o
-000001f0: 7065 7261 7469 6f6e 73a9 0072 1800 0000  perations..r....
-00000200: 7218 0000 00fa 592f 5573 6572 732f 7364  r.....Y/Users/sd
-00000210: 7265 6865 722f 776f 726b 7370 6163 652f  reher/workspace/
-00000220: 646a 616e 676f 2d71 7569 7a62 6c6f 636b  django-quizblock
-00000230: 2f71 7569 7a62 6c6f 636b 2f6d 6967 7261  /quizblock/migra
-00000240: 7469 6f6e 732f 3030 3034 5f71 7565 7374  tions/0004_quest
-00000250: 696f 6e5f 6373 735f 6578 7472 612e 7079  ion_css_extra.py
-00000260: 7205 0000 0008 0000 0073 1200 0000 0803  r........s......
-00000270: 02ff 0405 0401 0201 0201 0e01 02fc 04ff  ................
-00000280: 7205 0000 004e 2906 da0a 5f5f 6675 7475  r....N)...__futu
-00000290: 7265 5f5f 7202 0000 00da 0964 6a61 6e67  re__r......djang
-000002a0: 6f2e 6462 7203 0000 0072 0400 0000 7205  o.dbr....r....r.
-000002b0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-000002c0: 0000 7219 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002d0: 3e03 0000 0073 0400 0000 0c02 1003       >....s........
+00000000: a70d 0d0a 0000 0000 2dc5 0566 0302 0000  ........-..f....
+00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
+00000020: 0000 0000 00f3 4800 0000 9700 6400 6401  ......H.....d.d.
+00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
+00000040: 5a03 6d04 5a04 0100 0200 4700 6403 8400  Z.m.Z.....G.d...
+00000050: 6404 6504 6a05 0000 0000 0000 0000 a603  d.e.j...........
+00000060: 0000 ab03 0000 0000 0000 0000 5a05 6405  ............Z.d.
+00000070: 5300 2906 e900 0000 0029 01da 1075 6e69  S.)......)...uni
+00000080: 636f 6465 5f6c 6974 6572 616c 7329 02da  code_literals)..
+00000090: 066d 6f64 656c 73da 0a6d 6967 7261 7469  .models..migrati
+000000a0: 6f6e 7363 0000 0000 0000 0000 0000 0000  onsc............
+000000b0: 0900 0000 0000 0000 f360 0000 0097 0065  .........`.....e
+000000c0: 005a 0164 005a 0264 0167 015a 0302 0065  .Z.d.Z.d.g.Z...e
+000000d0: 046a 0500 0000 0000 0000 0064 0264 0302  .j.........d.d..
+000000e0: 0065 066a 0700 0000 0000 0000 0064 0464  .e.j.........d.d
+000000f0: 0564 05ac 06a6 0300 00ab 0300 0000 0000  .d..............
+00000100: 0000 0064 05ac 07a6 0400 00ab 0400 0000  ...d............
+00000110: 0000 0000 0067 015a 0864 0853 0029 09da  .....g.Z.d.S.)..
+00000120: 094d 6967 7261 7469 6f6e 2902 da09 7175  .Migration)...qu
+00000130: 697a 626c 6f63 6bda 1730 3030 335f 6175  izblock..0003_au
+00000140: 746f 5f32 3031 3530 3230 395f 3136 3031  to_20150209_1601
+00000150: da08 7175 6573 7469 6f6e da09 6373 735f  ..question..css_
+00000160: 6578 7472 6173 2300 0000 6578 7472 6120  extras#...extra 
+00000170: 4353 5320 636c 6173 7365 7320 2873 7061  CSS classes (spa
+00000180: 6365 2073 6570 6172 6174 6564 2954 2903  ce separated)T).
+00000190: da09 6865 6c70 5f74 6578 74da 046e 756c  ..help_text..nul
+000001a0: 6cda 0562 6c61 6e6b 2904 da0a 6d6f 6465  l..blank)...mode
+000001b0: 6c5f 6e61 6d65 da04 6e61 6d65 da05 6669  l_name..name..fi
+000001c0: 656c 64da 1070 7265 7365 7276 655f 6465  eld..preserve_de
+000001d0: 6661 756c 744e 2909 da08 5f5f 6e61 6d65  faultN)...__name
+000001e0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000001f0: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
+00000200: 7065 6e64 656e 6369 6573 7205 0000 00da  pendenciesr.....
+00000210: 0841 6464 4669 656c 6472 0400 0000 da09  .AddFieldr......
+00000220: 5465 7874 4669 656c 64da 0a6f 7065 7261  TextField..opera
+00000230: 7469 6f6e 73a9 00f3 0000 0000 fa58 2f55  tions........X/U
+00000240: 7365 7273 2f65 7661 6e70 6574 6572 7365  sers/evanpeterse
+00000250: 6e2f 6374 6c2f 646a 616e 676f 2d71 7569  n/ctl/django-qui
+00000260: 7a62 6c6f 636b 2f71 7569 7a62 6c6f 636b  zblock/quizblock
+00000270: 2f6d 6967 7261 7469 6f6e 732f 3030 3034  /migrations/0004
+00000280: 5f71 7565 7374 696f 6e5f 6373 735f 6578  _question_css_ex
+00000290: 7472 612e 7079 7207 0000 0072 0700 0000  tra.pyr....r....
+000002a0: 0800 0000 735d 0000 0080 0080 0080 0080  ....s]..........
+000002b0: 0080 00f0 0600 0931 f003 0214 0680 4cf0  .......1......L.
+000002c0: 0a00 091c 880a d408 1bd8 1721 d811 1cd8  ...........!....
+000002d0: 1222 9026 d412 22d0 2d53 d05a 5ed0 666a  .".&..".-S.Z^.fj
+000002e0: d012 6bd1 126b d412 6bd8 1d21 f009 0509  ..k..k..k..!....
+000002f0: 0af1 0005 090a f400 0509 0af0 0307 1206  ................
+00000300: 804a 804a 804a 721b 0000 0072 0700 0000  .J.J.Jr....r....
+00000310: 4e29 06da 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
+00000320: 0300 0000 da09 646a 616e 676f 2e64 6272  ......django.dbr
+00000330: 0400 0000 7205 0000 0072 0700 0000 721a  ....r....r....r.
+00000340: 0000 0072 1b00 0000 721c 0000 00fa 083c  ...r....r......<
+00000350: 6d6f 6475 6c65 3e72 1f00 0000 0100 0000  module>r........
+00000360: 7368 0000 00f0 0301 0101 f006 0001 28d0  sh............(.
+00000370: 0027 d000 27d0 0027 d000 27d0 0027 e000  .'..'..'..'..'..
+00000380: 28d0 0028 d000 28d0 0028 d000 28d0 0028  (..(..(..(..(..(
+00000390: d000 28d0 0028 f006 0d01 06f0 000d 0106  ..(..(..........
+000003a0: f000 0d01 06f0 000d 0106 f000 0d01 0690  ................
+000003b0: 0ad4 1024 f100 0d01 06f4 000d 0106 f000  ...$............
+000003c0: 0d01 06f0 000d 0106 f000 0d01 0672 1b00  .............r..
+000003d0: 0000                                     ..
```

### Comparing `django-quizblock-1.2.8/quizblock/models.py` & `django-quizblock-1.3.0/quizblock/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.contrib.auth.models import User
 try:
     from django.urls import reverse
 except ImportError:
     from django.core.urlresolvers import reverse
 from django.db import models
 from django.db.models import Q
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 from pagetree.models import PageBlock
 from pagetree.reports import ReportColumnInterface
 
 from django.contrib.contenttypes.fields import GenericRelation
 
 
 class Quiz(models.Model):
@@ -27,15 +27,15 @@
     exportable = True
     importable = True
 
     def pageblock(self):
         return self.pageblocks.first()
 
     def __str__(self):
-        return smart_text(self.pageblock())
+        return smart_str(self.pageblock())
 
     def needs_submit(self):
         return not self.rhetorical
 
     def submit(self, user, data):
         """ a big open question here is whether we should
         be validating submitted answers here, on submission,
@@ -130,15 +130,18 @@
         Submission.objects.filter(user=user, quiz=self).delete()
 
     def as_dict(self):
         d = dict(description=self.description,
                  rhetorical=self.rhetorical,
                  allow_redo=self.allow_redo,
                  show_submit_state=self.show_submit_state)
-        d['questions'] = [q.as_dict() for q in self.question_set.all()]
+        if self.pk is not None and self.question_set.count() > 0:
+            d['questions'] = [q.as_dict() for q in self.question_set.all()]
+        else:
+            d['questions'] = []
         return d
 
     def import_from_dict(self, d):
         self.description = d.get('description', '')
         self.rhetorical = d.get('rhetorical', False)
         self.allow_redo = d.get('allow_redo', True)
         self.show_submit_state = d.get('show_submit_state', True)
@@ -366,29 +369,29 @@
 class Submission(models.Model):
     quiz = models.ForeignKey(Quiz, on_delete=models.CASCADE)
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     submitted = models.DateTimeField(auto_now_add=True, editable=False)
 
     def __str__(self):
         return "quiz %d submission by %s at %s" % (self.quiz.id,
-                                                   smart_text(self.user),
+                                                   smart_str(self.user),
                                                    self.submitted)
 
 
 class Response(models.Model):
     question = models.ForeignKey(Question, on_delete=models.CASCADE)
     submission = models.ForeignKey(Submission, on_delete=models.CASCADE)
     value = models.TextField(blank=True)
 
     class Meta:
         ordering = ('question',)
 
     def __str__(self):
-        return "response to %s [%s]" % (smart_text(self.question),
-                                        smart_text(self.submission))
+        return "response to %s [%s]" % (smart_str(self.question),
+                                        smart_str(self.submission))
 
     def is_correct(self):
         return self.value in self.question.correct_answer_values()
 
     def answer(self):
         """Returns the Answer associated with this Response.
 
@@ -499,9 +502,9 @@
                     # did the user select the specified answer?
                     values = responses.values_list('value', flat=True)
                     if self.answer.value in values:
                         value = self.answer.id
                 else:  # short or long text
                     value = responses.first().value
 
-            value = smart_text(value)
+            value = smart_str(value)
         return value
```

### Comparing `django-quizblock-1.2.8/quizblock/static/quizblock/js/quizblock-admin.js` & `django-quizblock-1.3.0/quizblock/static/quizblock/js/quizblock-admin.js`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/static/quizblock/js/quizshow.js` & `django-quizblock-1.3.0/quizblock/static/quizblock/js/quizshow.js`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/edit_answer.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/edit_answer.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/edit_question.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/edit_question.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/long_text.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/long_text.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/multiple_choice.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/multiple_choice.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/multiple_choice_show_answer.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/multiple_choice_show_answer.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/question.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/question.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/quiz_detail.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/quiz_detail.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice_dropdown.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice_dropdown.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templates/quizblock/single_choice_show_answer.html` & `django-quizblock-1.3.0/quizblock/templates/quizblock/single_choice_show_answer.html`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/templatetags/getresponse.py` & `django-quizblock-1.3.0/quizblock/templatetags/getresponse.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/tests/test_models.py` & `django-quizblock-1.3.0/quizblock/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import unicode_literals
 
 from django.test import TestCase
 from quizblock.models import Quiz, Question, Answer, Submission
 from quizblock.models import Response
 from django.contrib.auth.models import User
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 
 
 class FakeReq(object):
     def __init__(self):
         self.POST = dict()
 
 
@@ -114,15 +114,15 @@
         self.assertEqual(q.submission_set.count(), 0)
         self.assertEqual(q.question_set.count(), 1)
         self.assertEqual(q.question_set.first().intro_text, '')
 
     def test_summary_render(self):
         q = Quiz(description="short")
         self.assertEqual(q.summary_render(), "short")
-        q.description = ''.join(smart_text(x) for x in range(75))
+        q.description = ''.join(smart_str(x) for x in range(75))
         expected = ('012345678910111213141516171819202122'
                     '2324252627282930313233343...')
         self.assertEqual(q.summary_render(), expected)
 
     def test_edit(self):
         q = Quiz()
         q.edit(dict(description='foo', rhetorical='on',
@@ -176,15 +176,15 @@
 
 
 class QuestionTest(TestCase):
     def test_str(self):
         quiz = Quiz.objects.create()
         question = Question.objects.create(
             quiz=quiz, text="foo", question_type="long text")
-        self.assertEqual(smart_text(question), "foo")
+        self.assertEqual(smart_str(question), "foo")
 
     def test_display_number(self):
         quiz = Quiz.objects.create()
         question = Question.objects.create(
             quiz=quiz, text="foo", question_type="long text")
         self.assertEqual(question.display_number(), 1)
 
@@ -411,15 +411,15 @@
 
 class AnswerTest(TestCase):
     def test_str(self):
         quiz = Quiz.objects.create()
         question = Question.objects.create(
             quiz=quiz, text="foo", question_type="single choice")
         answer = Answer.objects.create(question=question, label="an answer")
-        self.assertEqual(smart_text(answer), "an answer")
+        self.assertEqual(smart_str(answer), "an answer")
 
     def test_edit_form(self):
         quiz = Quiz.objects.create()
         question = Question.objects.create(
             quiz=quiz, text="foo", question_type="single choice")
         answer = Answer.objects.create(question=question, label="an answer")
         f = answer.edit_form()
@@ -468,15 +468,15 @@
 
 class SubmissionTest(TestCase):
     def test_str(self):
         quiz = Quiz.objects.create()
         user = User.objects.create(username="testuser")
         s = Submission.objects.create(quiz=quiz, user=user)
         self.assertTrue(
-            smart_text(s).startswith(
+            smart_str(s).startswith(
                 "quiz %d submission by testuser" % quiz.id))
 
 
 class ResponseTest(TestCase):
     def setUp(self):
         self.quiz = Quiz.objects.create()
         self.question = Question.objects.create(
@@ -489,15 +489,15 @@
             quiz=self.quiz, user=self.user)
 
     def test_str(self):
         response = Response.objects.create(
             question=self.question,
             submission=self.submission,
             value=self.answer.label)
-        self.assertTrue(smart_text(response).startswith("response to "))
+        self.assertTrue(smart_str(response).startswith("response to "))
 
     def test_is_correct(self):
         response = Response.objects.create(
             question=self.question,
             submission=self.submission,
             value=self.answer.label)
         self.assertFalse(response.is_correct())
```

### Comparing `django-quizblock-1.2.8/quizblock/tests/test_reports.py` & `django-quizblock-1.3.0/quizblock/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/tests/test_templatetags.py` & `django-quizblock-1.3.0/quizblock/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/tests/test_views.py` & `django-quizblock-1.3.0/quizblock/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/quizblock/urls.py` & `django-quizblock-1.3.0/quizblock/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import unicode_literals
 
-from django.conf.urls import url
+from django.urls import re_path
 from .views import (
     EditQuizView, DeleteQuestionView, DeleteAnswerView,
     ReorderAnswersView, ReorderQuestionsView,
     AddQuestionToQuizView, EditQuestionView,
     AddAnswerToQuestionView, EditAnswerView,
 )
 
 urlpatterns = [
-    url(r'^edit_quiz/(?P<pk>\d+)/$', EditQuizView.as_view(), {}, 'edit-quiz'),
-    url(r'^edit_quiz/(?P<pk>\d+)/add_question/$',
-        AddQuestionToQuizView.as_view(), {}, 'add-question-to-quiz'),
-    url(r'^edit_question/(?P<pk>\d+)/$', EditQuestionView.as_view(), {},
-        'edit-question'),
-    url(r'^edit_question/(?P<pk>\d+)/add_answer/$',
-        AddAnswerToQuestionView.as_view(), {}, 'add-answer-to-question'),
-    url(r'^delete_question/(?P<pk>\d+)/$', DeleteQuestionView.as_view(), {},
-        'delete-question'),
-    url(r'^reorder_answers/(?P<pk>\d+)/$', ReorderAnswersView.as_view(), {},
-        'reorder-answer'),
-    url(r'^reorder_questions/(?P<pk>\d+)/$', ReorderQuestionsView.as_view(),
-        {}, 'reorder-questions'),
-    url(r'^delete_answer/(?P<pk>\d+)/$', DeleteAnswerView.as_view(),
-        {}, 'delete-answer'),
-    url(r'^edit_answer/(?P<pk>\d+)/$', EditAnswerView.as_view(),
-        {}, 'edit-answer'),
+    re_path(r'^edit_quiz/(?P<pk>\d+)/$', EditQuizView.as_view(), {},
+            'edit-quiz'),
+    re_path(r'^edit_quiz/(?P<pk>\d+)/add_question/$',
+            AddQuestionToQuizView.as_view(), {}, 'add-question-to-quiz'),
+    re_path(r'^edit_question/(?P<pk>\d+)/$', EditQuestionView.as_view(), {},
+            'edit-question'),
+    re_path(r'^edit_question/(?P<pk>\d+)/add_answer/$',
+            AddAnswerToQuestionView.as_view(), {}, 'add-answer-to-question'),
+    re_path(r'^delete_question/(?P<pk>\d+)/$', DeleteQuestionView.as_view(),
+            {}, 'delete-question'),
+    re_path(r'^reorder_answers/(?P<pk>\d+)/$', ReorderAnswersView.as_view(),
+            {}, 'reorder-answer'),
+    re_path(r'^reorder_questions/(?P<pk>\d+)/$',
+            ReorderQuestionsView.as_view(), {}, 'reorder-questions'),
+    re_path(r'^delete_answer/(?P<pk>\d+)/$', DeleteAnswerView.as_view(),
+            {}, 'delete-answer'),
+    re_path(r'^edit_answer/(?P<pk>\d+)/$', EditAnswerView.as_view(),
+            {}, 'edit-answer'),
 ]
```

### Comparing `django-quizblock-1.2.8/quizblock/views.py` & `django-quizblock-1.3.0/quizblock/views.py`

 * *Files identical despite different names*

### Comparing `django-quizblock-1.2.8/setup.py` & `django-quizblock-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from setuptools import setup, find_packages
 
 setup(
     name="django-quizblock",
-    version="1.2.8",
-    author="Anders Pearson",
+    version="1.3.0",
+    author="Anders Pearson, Evan Petersen",
     author_email="ctl-dev@columbia.edu",
     url="https://github.com/ccnmtl/django-quizblock",
     description="Basic Quiz PageBlock",
     long_description="Basic Quiz PageBlocks (see django-pagetree and django-pageblocks)",
     install_requires = ['django-pagetree >= 1.1.2'],
     scripts = [],
     license = "BSD",
```

