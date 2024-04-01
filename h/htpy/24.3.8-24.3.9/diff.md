# Comparing `tmp/htpy-24.3.8.tar.gz` & `tmp/htpy-24.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htpy-24.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "htpy-24.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `htpy-24.3.8.tar` & `htpy-24.3.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       57 2024-03-03 13:00:59.192983 htpy-24.3.8/.envrc
--rw-r--r--   0        0        0       46 2024-03-09 13:39:41.722930 htpy-24.3.8/.gitignore
--rw-r--r--   0        0        0     1057 2023-10-29 21:51:04.877884 htpy-24.3.8/LICENSE
--rw-r--r--   0        0        0      322 2024-03-09 20:27:19.833957 htpy-24.3.8/README.md
--rw-r--r--   0        0        0       50 2024-03-10 12:35:36.989725 htpy-24.3.8/allowlist
--rw-r--r--   0        0        0      249 2024-03-03 13:33:34.150382 htpy-24.3.8/conftest.py
--rw-r--r--   0        0        0        9 2024-03-02 19:38:17.864052 htpy-24.3.8/docs/CNAME
--rw-r--r--   0        0        0    17486 2024-03-05 20:59:52.115770 htpy-24.3.8/docs/assets/htpy.webp
--rw-r--r--   0        0        0     3264 2024-03-09 19:38:20.478207 htpy-24.3.8/docs/common-patterns.md
--rw-r--r--   0        0        0     2557 2024-03-09 11:27:32.254799 htpy-24.3.8/docs/django.md
--rw-r--r--   0        0        0     2482 2024-03-09 19:46:12.386823 htpy-24.3.8/docs/faq.md
--rw-r--r--   0        0        0     3100 2024-03-09 20:23:00.454609 htpy-24.3.8/docs/index.md
--rw-r--r--   0        0        0     1767 2024-03-09 19:48:03.051069 htpy-24.3.8/docs/references.md
--rw-r--r--   0        0        0     7101 2024-03-09 14:23:14.104720 htpy-24.3.8/docs/usage.md
--rw-r--r--   0        0        0        0 2024-03-08 20:09:37.710488 htpy-24.3.8/examples/djangoproject/exampleproject/__init__.py
--rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153857 htpy-24.3.8/examples/djangoproject/exampleproject/asgi.py
--rw-r--r--   0        0        0     3215 2024-03-08 21:16:49.814277 htpy-24.3.8/examples/djangoproject/exampleproject/settings.py
--rw-r--r--   0        0        0      952 2024-03-08 21:10:49.153824 htpy-24.3.8/examples/djangoproject/exampleproject/urls.py
--rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153702 htpy-24.3.8/examples/djangoproject/exampleproject/wsgi.py
--rw-r--r--   0        0        0        0 2024-03-08 20:15:31.191691 htpy-24.3.8/examples/djangoproject/form/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415543 htpy-24.3.8/examples/djangoproject/form/admin.py
--rw-r--r--   0        0        0      140 2024-03-08 20:55:19.065671 htpy-24.3.8/examples/djangoproject/form/apps.py
--rw-r--r--   0        0        0      551 2024-03-08 21:09:54.963068 htpy-24.3.8/examples/djangoproject/form/components.py
--rw-r--r--   0        0        0       95 2024-03-08 20:31:59.157434 htpy-24.3.8/examples/djangoproject/form/forms.py
--rw-r--r--   0        0        0        0 2024-03-08 20:15:31.193856 htpy-24.3.8/examples/djangoproject/form/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415774 htpy-24.3.8/examples/djangoproject/form/models.py
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415536 htpy-24.3.8/examples/djangoproject/form/tests.py
--rw-r--r--   0        0        0      295 2024-03-08 20:30:30.923484 htpy-24.3.8/examples/djangoproject/form/views.py
--rw-r--r--   0        0        0        0 2024-03-08 20:10:21.327962 htpy-24.3.8/examples/djangoproject/index/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415912 htpy-24.3.8/examples/djangoproject/index/admin.py
--rw-r--r--   0        0        0      142 2024-03-08 20:15:01.419100 htpy-24.3.8/examples/djangoproject/index/apps.py
--rw-r--r--   0        0        0        0 2024-03-08 20:10:21.330107 htpy-24.3.8/examples/djangoproject/index/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415529 htpy-24.3.8/examples/djangoproject/index/models.py
--rw-r--r--   0        0        0      107 2024-03-08 20:12:51.957222 htpy-24.3.8/examples/djangoproject/index/templates/base.html
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415746 htpy-24.3.8/examples/djangoproject/index/tests.py
--rw-r--r--   0        0        0      159 2024-03-08 21:57:51.272614 htpy-24.3.8/examples/djangoproject/index/views.py
--rwxr-xr-x   0        0        0      671 2024-03-08 21:10:49.133835 htpy-24.3.8/examples/djangoproject/manage.py
--rw-r--r--   0        0        0        0 2024-03-08 20:38:21.778715 htpy-24.3.8/examples/djangoproject/widget/__init__.py
--rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415902 htpy-24.3.8/examples/djangoproject/widget/admin.py
--rw-r--r--   0        0        0      144 2024-03-08 20:55:19.065101 htpy-24.3.8/examples/djangoproject/widget/apps.py
--rw-r--r--   0        0        0        0 2024-03-08 20:38:21.780794 htpy-24.3.8/examples/djangoproject/widget/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415928 htpy-24.3.8/examples/djangoproject/widget/models.py
--rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415824 htpy-24.3.8/examples/djangoproject/widget/tests.py
--rw-r--r--   0        0        0      773 2024-03-08 21:14:26.968101 htpy-24.3.8/examples/djangoproject/widget/views.py
--rw-r--r--   0        0        0      348 2024-03-08 21:07:31.025272 htpy-24.3.8/examples/djangoproject/widget/widgets.py
--rw-r--r--   0        0        0     1042 2023-12-11 20:24:46.525531 htpy-24.3.8/examples/htmx_flask.py
--rw-r--r--   0        0        0      177 2024-03-09 20:19:16.408517 htpy-24.3.8/examples/index_example.py
--rw-r--r--   0        0        0     1217 2024-03-09 19:38:31.365824 htpy-24.3.8/examples/structure/boostrap_modal.py
--rw-r--r--   0        0        0      726 2024-03-08 22:27:23.834011 htpy-24.3.8/examples/structure/extends_base.py
--rw-r--r--   0        0        0     1023 2024-03-08 22:36:51.254744 htpy-24.3.8/examples/structure/extends_class.py
--rw-r--r--   0        0        0      384 2024-03-03 13:43:15.955057 htpy-24.3.8/htpy.code-workspace
--rw-r--r--   0        0        0     4195 2024-03-10 18:34:30.055035 htpy-24.3.8/htpy/__init__.py
--rw-r--r--   0        0        0     3463 2024-03-10 12:35:44.632718 htpy-24.3.8/htpy/__init__.pyi
--rw-r--r--   0        0        0     1735 2024-03-07 10:26:38.499381 htpy-24.3.8/htpy/_attrs.py
--rw-r--r--   0        0        0        0 2023-10-29 15:28:12.549039 htpy-24.3.8/htpy/py.typed
--rw-r--r--   0        0        0      543 2024-03-09 20:29:26.894374 htpy-24.3.8/mkdocs.yml
--rw-r--r--   0        0        0     1600 2024-03-09 14:43:49.883001 htpy-24.3.8/pyproject.toml
--rw-r--r--   0        0        0     1256 2024-03-09 13:37:51.172194 htpy-24.3.8/scripts/benchmark_big_table.py
--rwxr-xr-x   0        0        0       65 2024-03-02 18:11:27.585869 htpy-24.3.8/scripts/fix
--rwxr-xr-x   0        0        0       59 2024-03-10 18:34:51.540054 htpy-24.3.8/scripts/release
--rwxr-xr-x   0        0        0      286 2024-03-03 13:37:46.454442 htpy-24.3.8/scripts/test
--rw-r--r--   0        0        0     4187 2024-03-10 12:30:32.366729 htpy-24.3.8/tests/test_attributes.py
--rw-r--r--   0        0        0     2520 2024-03-10 12:31:53.604177 htpy-24.3.8/tests/test_children.py
--rw-r--r--   0        0        0      935 2024-03-10 12:32:49.438483 htpy-24.3.8/tests/test_django.py
--rw-r--r--   0        0        0      351 2024-03-10 18:36:07.188647 htpy-24.3.8/tests/test_element.py
--rw-r--r--   0        0        0      818 2024-03-03 18:10:59.058546 htpy-24.3.8/tests/test_escaping.py
--rw-r--r--   0        0        0      461 2023-11-01 19:49:28.962824 htpy-24.3.8/tests/test_iter.py
--rw-r--r--   0        0        0      371 2024-03-04 12:51:33.461811 htpy-24.3.8/tests/test_jinja2.py
--rw-r--r--   0        0        0      103 2023-11-01 20:01:02.686135 htpy-24.3.8/tests/test_repr.py
--rw-r--r--   0        0        0      357 2023-11-06 13:17:37.888178 htpy-24.3.8/tests/test_types.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 htpy-24.3.8/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-03-03 13:00:59.192983 htpy-24.3.9/.envrc
+-rw-r--r--   0        0        0       46 2024-03-09 13:39:41.722930 htpy-24.3.9/.gitignore
+-rw-r--r--   0        0        0     1057 2023-10-29 21:51:04.877884 htpy-24.3.9/LICENSE
+-rw-r--r--   0        0        0      322 2024-03-09 20:27:19.833957 htpy-24.3.9/README.md
+-rw-r--r--   0        0        0       46 2024-03-10 21:34:04.445438 htpy-24.3.9/allowlist
+-rw-r--r--   0        0        0      249 2024-03-03 13:33:34.150382 htpy-24.3.9/conftest.py
+-rw-r--r--   0        0        0        9 2024-03-02 19:38:17.864052 htpy-24.3.9/docs/CNAME
+-rw-r--r--   0        0        0    17486 2024-03-05 20:59:52.115770 htpy-24.3.9/docs/assets/htpy.webp
+-rw-r--r--   0        0        0     3264 2024-03-09 19:38:20.478207 htpy-24.3.9/docs/common-patterns.md
+-rw-r--r--   0        0        0     2557 2024-03-09 11:27:32.254799 htpy-24.3.9/docs/django.md
+-rw-r--r--   0        0        0     2482 2024-03-09 19:46:12.386823 htpy-24.3.9/docs/faq.md
+-rw-r--r--   0        0        0     3100 2024-03-09 20:23:00.454609 htpy-24.3.9/docs/index.md
+-rw-r--r--   0        0        0     1767 2024-03-09 19:48:03.051069 htpy-24.3.9/docs/references.md
+-rw-r--r--   0        0        0     7101 2024-03-09 14:23:14.104720 htpy-24.3.9/docs/usage.md
+-rw-r--r--   0        0        0        0 2024-03-08 20:09:37.710488 htpy-24.3.9/examples/djangoproject/exampleproject/__init__.py
+-rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153857 htpy-24.3.9/examples/djangoproject/exampleproject/asgi.py
+-rw-r--r--   0        0        0     3215 2024-03-08 21:16:49.814277 htpy-24.3.9/examples/djangoproject/exampleproject/settings.py
+-rw-r--r--   0        0        0      952 2024-03-08 21:10:49.153824 htpy-24.3.9/examples/djangoproject/exampleproject/urls.py
+-rw-r--r--   0        0        0      405 2024-03-08 21:10:49.153702 htpy-24.3.9/examples/djangoproject/exampleproject/wsgi.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:15:31.191691 htpy-24.3.9/examples/djangoproject/form/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415543 htpy-24.3.9/examples/djangoproject/form/admin.py
+-rw-r--r--   0        0        0      140 2024-03-08 20:55:19.065671 htpy-24.3.9/examples/djangoproject/form/apps.py
+-rw-r--r--   0        0        0      551 2024-03-08 21:09:54.963068 htpy-24.3.9/examples/djangoproject/form/components.py
+-rw-r--r--   0        0        0       95 2024-03-08 20:31:59.157434 htpy-24.3.9/examples/djangoproject/form/forms.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:15:31.193856 htpy-24.3.9/examples/djangoproject/form/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415774 htpy-24.3.9/examples/djangoproject/form/models.py
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415536 htpy-24.3.9/examples/djangoproject/form/tests.py
+-rw-r--r--   0        0        0      295 2024-03-08 20:30:30.923484 htpy-24.3.9/examples/djangoproject/form/views.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:10:21.327962 htpy-24.3.9/examples/djangoproject/index/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415912 htpy-24.3.9/examples/djangoproject/index/admin.py
+-rw-r--r--   0        0        0      142 2024-03-08 20:15:01.419100 htpy-24.3.9/examples/djangoproject/index/apps.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:10:21.330107 htpy-24.3.9/examples/djangoproject/index/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415529 htpy-24.3.9/examples/djangoproject/index/models.py
+-rw-r--r--   0        0        0      107 2024-03-08 20:12:51.957222 htpy-24.3.9/examples/djangoproject/index/templates/base.html
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415746 htpy-24.3.9/examples/djangoproject/index/tests.py
+-rw-r--r--   0        0        0      159 2024-03-08 21:57:51.272614 htpy-24.3.9/examples/djangoproject/index/views.py
+-rwxr-xr-x   0        0        0      671 2024-03-08 21:10:49.133835 htpy-24.3.9/examples/djangoproject/manage.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:38:21.778715 htpy-24.3.9/examples/djangoproject/widget/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-08 20:55:24.415902 htpy-24.3.9/examples/djangoproject/widget/admin.py
+-rw-r--r--   0        0        0      144 2024-03-08 20:55:19.065101 htpy-24.3.9/examples/djangoproject/widget/apps.py
+-rw-r--r--   0        0        0        0 2024-03-08 20:38:21.780794 htpy-24.3.9/examples/djangoproject/widget/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-08 20:55:24.415928 htpy-24.3.9/examples/djangoproject/widget/models.py
+-rw-r--r--   0        0        0       26 2024-03-08 20:55:24.415824 htpy-24.3.9/examples/djangoproject/widget/tests.py
+-rw-r--r--   0        0        0      773 2024-03-08 21:14:26.968101 htpy-24.3.9/examples/djangoproject/widget/views.py
+-rw-r--r--   0        0        0      348 2024-03-08 21:07:31.025272 htpy-24.3.9/examples/djangoproject/widget/widgets.py
+-rw-r--r--   0        0        0     1042 2023-12-11 20:24:46.525531 htpy-24.3.9/examples/htmx_flask.py
+-rw-r--r--   0        0        0      177 2024-03-09 20:19:16.408517 htpy-24.3.9/examples/index_example.py
+-rw-r--r--   0        0        0     1217 2024-03-09 19:38:31.365824 htpy-24.3.9/examples/structure/boostrap_modal.py
+-rw-r--r--   0        0        0      726 2024-03-08 22:27:23.834011 htpy-24.3.9/examples/structure/extends_base.py
+-rw-r--r--   0        0        0     1023 2024-03-08 22:36:51.254744 htpy-24.3.9/examples/structure/extends_class.py
+-rw-r--r--   0        0        0      384 2024-03-03 13:43:15.955057 htpy-24.3.9/htpy.code-workspace
+-rw-r--r--   0        0        0     4195 2024-03-10 21:34:11.537898 htpy-24.3.9/htpy/__init__.py
+-rw-r--r--   0        0        0     3443 2024-03-10 21:34:04.445818 htpy-24.3.9/htpy/__init__.pyi
+-rw-r--r--   0        0        0     1735 2024-03-07 10:26:38.499381 htpy-24.3.9/htpy/_attrs.py
+-rw-r--r--   0        0        0        0 2023-10-29 15:28:12.549039 htpy-24.3.9/htpy/py.typed
+-rw-r--r--   0        0        0      543 2024-03-09 20:29:26.894374 htpy-24.3.9/mkdocs.yml
+-rw-r--r--   0        0        0     1600 2024-03-09 14:43:49.883001 htpy-24.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1256 2024-03-09 13:37:51.172194 htpy-24.3.9/scripts/benchmark_big_table.py
+-rwxr-xr-x   0        0        0       65 2024-03-02 18:11:27.585869 htpy-24.3.9/scripts/fix
+-rwxr-xr-x   0        0        0       59 2024-03-10 18:34:51.540054 htpy-24.3.9/scripts/release
+-rwxr-xr-x   0        0        0      286 2024-03-03 13:37:46.454442 htpy-24.3.9/scripts/test
+-rw-r--r--   0        0        0     4187 2024-03-10 12:30:32.366729 htpy-24.3.9/tests/test_attributes.py
+-rw-r--r--   0        0        0     2520 2024-03-10 12:31:53.604177 htpy-24.3.9/tests/test_children.py
+-rw-r--r--   0        0        0      935 2024-03-10 12:32:49.438483 htpy-24.3.9/tests/test_django.py
+-rw-r--r--   0        0        0      351 2024-03-10 18:36:07.188647 htpy-24.3.9/tests/test_element.py
+-rw-r--r--   0        0        0      818 2024-03-03 18:10:59.058546 htpy-24.3.9/tests/test_escaping.py
+-rw-r--r--   0        0        0      461 2023-11-01 19:49:28.962824 htpy-24.3.9/tests/test_iter.py
+-rw-r--r--   0        0        0      371 2024-03-04 12:51:33.461811 htpy-24.3.9/tests/test_jinja2.py
+-rw-r--r--   0        0        0      103 2023-11-01 20:01:02.686135 htpy-24.3.9/tests/test_repr.py
+-rw-r--r--   0        0        0      592 2024-03-10 21:34:04.446097 htpy-24.3.9/tests/test_types.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 htpy-24.3.9/PKG-INFO
```

### Comparing `htpy-24.3.8/LICENSE` & `htpy-24.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/assets/htpy.webp` & `htpy-24.3.9/docs/assets/htpy.webp`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/common-patterns.md` & `htpy-24.3.9/docs/common-patterns.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/django.md` & `htpy-24.3.9/docs/django.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/faq.md` & `htpy-24.3.9/docs/faq.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/index.md` & `htpy-24.3.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/references.md` & `htpy-24.3.9/docs/references.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/docs/usage.md` & `htpy-24.3.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/djangoproject/exampleproject/settings.py` & `htpy-24.3.9/examples/djangoproject/exampleproject/settings.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/djangoproject/exampleproject/urls.py` & `htpy-24.3.9/examples/djangoproject/exampleproject/urls.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/djangoproject/form/components.py` & `htpy-24.3.9/examples/djangoproject/form/components.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/djangoproject/manage.py` & `htpy-24.3.9/examples/djangoproject/manage.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/djangoproject/widget/views.py` & `htpy-24.3.9/examples/djangoproject/widget/views.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/htmx_flask.py` & `htpy-24.3.9/examples/htmx_flask.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/structure/boostrap_modal.py` & `htpy-24.3.9/examples/structure/boostrap_modal.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/structure/extends_base.py` & `htpy-24.3.9/examples/structure/extends_base.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/examples/structure/extends_class.py` & `htpy-24.3.9/examples/structure/extends_class.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/htpy/__init__.py` & `htpy-24.3.9/htpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "24.3.8"
+__version__ = "24.3.9"
 
 import functools
 import types
 
 from markupsafe import Markup as _Markup
 from markupsafe import escape as _escape
```

### Comparing `htpy-24.3.8/htpy/__init__.pyi` & `htpy-24.3.9/htpy/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from collections.abc import Generator, Iterator
+from collections.abc import Generator, Iterator, Sequence
 from typing import Protocol, TypeAlias, overload
 
 class _HasHtml(Protocol):
     def __html__(self) -> str: ...
 
 _ClassNamesDict: TypeAlias = dict[str, bool | None]
 _ClassNames: TypeAlias = list[str | None | bool | _ClassNamesDict] | _ClassNamesDict
-Children: TypeAlias = (
+Node: TypeAlias = (
     None
     | bool
     | str
     | BaseElement
     | _HasHtml
-    | list["Children"]
-    | tuple["Children", ...]
-    | Generator["Children", None, None]
+    | Sequence["Node"]
+    | tuple["Node", ...]
+    | Generator["Node", None, None]
 )
 
 Attribute: TypeAlias = None | bool | str | _ClassNames
 
 class BaseElement:
-    def __init__(self, name: str, attrs: dict[str, Attribute], children: list[Children]): ...
+    def __init__(self, name: str, attrs: dict[str, Attribute], children: Node): ...
     @overload
     def __call__(
         self, id_class: str, attrs: dict[str, Attribute], **kwargs: Attribute
     ) -> Element: ...
     @overload
     def __call__(self, id_class: str = "", **kwargs: Attribute) -> Element: ...
     @overload
     def __call__(self, attrs: dict[str, Attribute], **kwargs: Attribute) -> Element: ...
     @overload
     def __call__(self, **kwargs: Attribute) -> Element: ...
     def __iter__(self) -> Iterator[str]: ...
 
 class Element(BaseElement):
-    def __getitem__(self, children: Children) -> Element: ...
+    def __getitem__(self, children: Node) -> Element: ...
 
 class VoidElement(BaseElement): ...
 
 class ElementWithDoctype(Element):
     def __init__(
-        self, name: str, attrs: dict[str, Attribute], children: list[Children], *, doctype: str
+        self, name: str, attrs: dict[str, Attribute], children: list[Node], *, doctype: str
     ): ...
 
 def __getattr__(name: str) -> Element: ...
 
 # This list should contain all non-deprecated HTML elements
 html: ElementWithDoctype
```

### Comparing `htpy-24.3.8/htpy/_attrs.py` & `htpy-24.3.9/htpy/_attrs.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/mkdocs.yml` & `htpy-24.3.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/pyproject.toml` & `htpy-24.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/scripts/benchmark_big_table.py` & `htpy-24.3.9/scripts/benchmark_big_table.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/tests/test_attributes.py` & `htpy-24.3.9/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/tests/test_children.py` & `htpy-24.3.9/tests/test_children.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/tests/test_django.py` & `htpy-24.3.9/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/tests/test_escaping.py` & `htpy-24.3.9/tests/test_escaping.py`

 * *Files identical despite different names*

### Comparing `htpy-24.3.8/PKG-INFO` & `htpy-24.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htpy
-Version: 24.3.8
+Version: 24.3.9
 Summary: HTML in Python
 Author-email: Andreas Pelme <andreas@pelme.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

