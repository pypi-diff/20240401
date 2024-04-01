# Comparing `tmp/recommender-xblock-2.1.1.tar.gz` & `tmp/recommender-xblock-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommender-xblock-2.1.1.tar", last modified: Mon Jan 22 14:08:09 2024, max compression
+gzip compressed data, was "recommender-xblock-2.2.0.tar", last modified: Mon Apr  1 14:51:36 2024, max compression
```

## Comparing `recommender-xblock-2.1.1.tar` & `recommender-xblock-2.2.0.tar`

### file list

```diff
@@ -1,66 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50994 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/recommender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9606 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/css/introjs.css
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/css/recommender.css
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/css/recommenderstudio.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     9534 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/css/tooltipster.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/js/src/cats.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    16944 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/js/src/jquery.tooltipster.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    57653 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/js/src/recommender.js
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/js/src/recommenderstudio.js
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/static/js/src/underscore-min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    16614 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/templates/recommender.html
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/templates/recommenderstudio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.903369 recommender-xblock-2.1.1/recommender/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/ru/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.907369 recommender-xblock-2.1.1/recommender/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/recommender/translations/zh_CN/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/recommender_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-01-22 14:08:09.000000 recommender-xblock-2.1.1/recommender_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-22 14:08:09.000000 recommender-xblock-2.1.1/recommender_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:08:09.000000 recommender-xblock-2.1.1/recommender_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-22 14:08:09.000000 recommender-xblock-2.1.1/recommender_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-22 14:08:09.000000 recommender-xblock-2.1.1/recommender_xblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 14:08:09.911369 recommender-xblock-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-01-22 14:08:01.000000 recommender-xblock-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.532064 recommender-xblock-2.2.0/recommender/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50640 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/recommender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.532064 recommender-xblock-2.2.0/recommender/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/recommender/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9606 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/css/introjs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/css/recommender.css
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/css/recommenderstudio.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9534 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/css/tooltipster.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.532064 recommender-xblock-2.2.0/recommender/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/recommender/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/js/src/cats.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16944 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/js/src/jquery.tooltipster.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    57653 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/js/src/recommender.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/js/src/recommenderstudio.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/static/js/src/underscore-min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/recommender/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    16614 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/templates/recommender.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/templates/recommenderstudio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/recommender/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/recommender/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/recommender_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 14:51:36.000000 recommender-xblock-2.2.0/recommender_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-01 14:51:36.000000 recommender-xblock-2.2.0/recommender_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:51:36.000000 recommender-xblock-2.2.0/recommender_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 14:51:36.000000 recommender-xblock-2.2.0/recommender_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 14:51:36.000000 recommender-xblock-2.2.0/recommender_xblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:51:36.536064 recommender-xblock-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 14:51:31.000000 recommender-xblock-2.2.0/setup.py
```

### Comparing `recommender-xblock-2.1.1/LICENSE` & `recommender-xblock-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/PKG-INFO` & `recommender-xblock-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: recommender-xblock
-Version: 2.1.1
+Version: 2.2.0
 Summary: recommender XBlock
 Home-page: https://github.com/openedx/RecommenderXBlock
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx recommender
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 RecommenderXBlock
 =================
 
 This XBlock shows students a list of recommended resources for a given
 problem. The resources are recommended, edited, and voted by students.
```

### Comparing `recommender-xblock-2.1.1/README.rst` & `recommender-xblock-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/recommender.py` & `recommender-xblock-2.2.0/recommender/recommender.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from copy import deepcopy
 
 import six
 from six.moves.urllib.parse import unquote_plus, urlparse, urlunparse
 
 import bleach
 from webob.response import Response
-from django.utils import translation
 
 from xblock.core import XBlock
 from xblock.exceptions import JsonHandlerError
 from xblock.fields import Scope, List, Dict, Boolean, String, JSONField
 from web_fragments.fragment import Fragment
 from xblock.reference.plugins import Filesystem
 from xblockutils.resources import ResourceLoader
@@ -274,14 +273,16 @@
     )
 
     # the dictionary keys for storing the content of a recommendation
     resource_content_fields = [
         'url', 'title', 'description', 'descriptionText'
     ]
 
+    i18n_js_namespace = 'RecommenderXBlockI18N'
+
     def _get_onetime_url(self, filename):
         """
         Return one time url for uploaded screenshot
 
         We benchmarked this as less than 8ms on a sandbox machine.
         """
         if filename.startswith('fs://'):
@@ -944,27 +945,21 @@
             result['reason'] = self.flagged_reasons[self.flagged_ids.index(resource['id'])]
         else:
             result['flag_mode'] = ''
             result['reason'] = ''
 
         return result
 
-    @staticmethod
-    def _get_statici18n_js_url():  # pragma: no cover
-        """
-        Returns the Javascript translation file for the currently selected language, if any found by `pkg_resources`
-        """
-        lang_code = translation.get_language()
-        if not lang_code:
-            return None
-        text_js = 'public/js/translations/{lang_code}/text.js'
-        country_code = lang_code.split('-')[0]
-        for code in (translation.to_locale(lang_code), lang_code, country_code):
-            if pkg_resources.resource_exists(resource_loader.module_name, text_js.format(lang_code=code)):
-                return text_js.format(lang_code=code)
+    def _get_statici18n_js_url(self):
+        """Return the JavaScript translation file provided by the XBlockI18NService."""
+        if i18n_service := self.runtime.service(self, 'i18n'):
+            if url_getter_func := getattr(i18n_service, 'get_javascript_i18n_catalog_url', None):
+                if javascript_url := url_getter_func(self):
+                    return javascript_url
+
         return None
 
     def student_view(self, _context=None):  # pylint: disable=unused-argument
         """
         The primary view of the RecommenderXBlock, shown to students
         when viewing courses.
         """
@@ -1005,17 +1000,16 @@
         frag.add_javascript_url("//ajax.googleapis.com/ajax/libs/jqueryui/1.10.4/jquery-ui.min.js")
         frag.add_javascript_url('//cdnjs.cloudflare.com/ajax/libs/mustache.js/0.8.1/mustache.min.js')
         frag.add_javascript_url('//cdnjs.cloudflare.com/ajax/libs/intro.js/0.5.0/intro.min.js')
         frag.add_css(self.resource_string("static/css/tooltipster.css"))
         frag.add_css(self.resource_string("static/css/recommender.css"))
         frag.add_css(self.resource_string("static/css/introjs.css"))
         frag.add_javascript(self.resource_string("static/js/src/jquery.tooltipster.min.js"))
-        statici18n_js_url = self._get_statici18n_js_url()
-        if statici18n_js_url:
-            frag.add_javascript(self.resource_string(statici18n_js_url))
+        if statici18n_js_url := self._get_statici18n_js_url():
+            frag.add_javascript(statici18n_js_url)
         frag.add_javascript(self.resource_string("static/js/src/cats.js"))
         frag.add_javascript(self.resource_string("static/js/src/recommender.js"))
         frag.initialize_js('RecommenderXBlock', self.get_client_configuration())
         return frag
 
     def studio_view(self, _context=None):  # pylint: disable=unused-argument
         """
@@ -1025,17 +1019,16 @@
         frag = Fragment()
         frag.add_content(resource_loader.render_django_template(
             "templates/recommenderstudio.html",
             i18n_service=self.runtime.service(self, "i18n")
         ))
         frag.add_css(load("static/css/recommenderstudio.css"))
         frag.add_javascript_url("//ajax.googleapis.com/ajax/libs/jqueryui/1.10.4/jquery-ui.min.js")
-        statici18n_js_url = self._get_statici18n_js_url()
-        if statici18n_js_url:
-            frag.add_javascript(self.resource_string(statici18n_js_url))
+        if statici18n_js_url := self._get_statici18n_js_url():
+            frag.add_javascript(statici18n_js_url)
         frag.add_javascript(load("static/js/src/recommenderstudio.js"))
         frag.initialize_js('RecommenderXBlock')
         return frag
 
     def add_xml_to_node(self, node):
         """
         Serialize the XBlock to XML for exporting.
```

### Comparing `recommender-xblock-2.1.1/recommender/static/css/introjs.css` & `recommender-xblock-2.2.0/recommender/static/css/introjs.css`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/css/recommender.css` & `recommender-xblock-2.2.0/recommender/static/css/recommender.css`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/css/recommenderstudio.css` & `recommender-xblock-2.2.0/recommender/static/css/recommenderstudio.css`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/css/tooltipster.css` & `recommender-xblock-2.2.0/recommender/static/css/tooltipster.css`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/js/src/cats.js` & `recommender-xblock-2.2.0/recommender/static/js/src/cats.js`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/js/src/jquery.tooltipster.min.js` & `recommender-xblock-2.2.0/recommender/static/js/src/jquery.tooltipster.min.js`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/js/src/recommender.js` & `recommender-xblock-2.2.0/recommender/static/js/src/recommender.js`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/js/src/recommenderstudio.js` & `recommender-xblock-2.2.0/recommender/static/js/src/recommenderstudio.js`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/static/js/src/underscore-min.js` & `recommender-xblock-2.2.0/recommender/static/js/src/underscore-min.js`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/templates/recommender.html` & `recommender-xblock-2.2.0/recommender/templates/recommender.html`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender/templates/recommenderstudio.html` & `recommender-xblock-2.2.0/recommender/templates/recommenderstudio.html`

 * *Files identical despite different names*

### Comparing `recommender-xblock-2.1.1/recommender_xblock.egg-info/PKG-INFO` & `recommender-xblock-2.2.0/recommender_xblock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: recommender-xblock
-Version: 2.1.1
+Version: 2.2.0
 Summary: recommender XBlock
 Home-page: https://github.com/openedx/RecommenderXBlock
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx recommender
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 RecommenderXBlock
 =================
 
 This XBlock shows students a list of recommended resources for a given
 problem. The resources are recommended, edited, and voted by students.
```

### Comparing `recommender-xblock-2.1.1/setup.py` & `recommender-xblock-2.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 for fname in files:
                     if os.path.splitext(fname)[1] == '.po':
                         po_path = os.path.join(dirname, fname)
                         mo_path = os.path.splitext(po_path)[0] + '.mo'
                         self.announce('Compiling translation at %s' % po_path)
                         subprocess.check_call(['msgfmt', po_path, '-o', mo_path], cwd=self.install_lib)
         except Exception as ex:
-            self.announce('Translations compilation failed: %s' % ex.message)
+            self.announce('Translations compilation failed: %s' % getattr(ex, 'message', str(ex)))
 
 
 def package_data(pkg, root_list):
     """Generic function to find package_data for `pkg` under `root`."""
     data = []
     for root in root_list:
         for dirname, _, files in os.walk(os.path.join(pkg, root)):
@@ -89,9 +89,10 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

