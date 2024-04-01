# Comparing `tmp/ckanext-or_facet-0.2.0.tar.gz` & `tmp/ckanext-or_facet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-or_facet-0.2.0.tar", last modified: Sun Mar 31 04:44:50 2024, max compression
+gzip compressed data, was "ckanext-or_facet-0.3.0.tar", last modified: Mon Apr  1 13:22:08 2024, max compression
```

## Comparing `ckanext-or_facet-0.2.0.tar` & `ckanext-or_facet-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34499 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1348 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      716 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext/or_facet/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/ckanext/or_facet/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3775 2024-03-31 04:41:20.000000 ckanext-or_facet-0.2.0/ckanext/or_facet/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext/or_facet/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext/or_facet/templates/or_facet/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      454 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/ckanext/or_facet/templates/or_facet/facet_switcher.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext/or_facet/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/ckanext/or_facet/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7333 2024-03-31 04:25:19.000000 ckanext-or_facet-0.2.0/ckanext/or_facet/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1348 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      576 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      121 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-03-31 04:44:50.000000 ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4118 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.2.0/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      565 2024-03-31 04:44:50.132572 ckanext-or_facet-0.2.0/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3813 2024-03-31 04:43:06.000000 ckanext-or_facet-0.2.0/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-04-01 13:16:42.000000 ckanext-or_facet-0.3.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      132 2024-04-01 13:16:42.000000 ckanext-or_facet-0.3.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1757 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      848 2024-04-01 13:05:26.000000 ckanext-or_facet-0.3.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2024-04-01 13:13:41.000000 ckanext-or_facet-0.3.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext/or_facet/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.3.0/ckanext/or_facet/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3168 2024-04-01 13:18:36.000000 ckanext-or_facet-0.3.0/ckanext/or_facet/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext/or_facet/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext/or_facet/templates/or_facet/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      454 2024-03-30 13:06:34.000000 ckanext-or_facet-0.3.0/ckanext/or_facet/templates/or_facet/facet_switcher.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext/or_facet/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.3.0/ckanext/or_facet/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7432 2024-04-01 13:15:52.000000 ckanext-or_facet-0.3.0/ckanext/or_facet/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 13:22:08.984140 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1757 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      576 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      121 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       57 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-01 13:22:08.000000 ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4100 2024-04-01 13:16:20.000000 ckanext-or_facet-0.3.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-30 13:06:34.000000 ckanext-or_facet-0.3.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1605 2024-04-01 13:22:08.987474 ckanext-or_facet-0.3.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2024-04-01 13:13:42.000000 ckanext-or_facet-0.3.0/setup.py
```

### Comparing `ckanext-or_facet-0.2.0/LICENSE` & `ckanext-or_facet-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -654,8 +654,8 @@
 of the code.  There are many ways you could offer source, and different
 solutions will be better for different programs; see section 13 for the
 specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
-<http://www.gnu.org/licenses/>.
+<http://www.gnu.org/licenses/>.
```

### Comparing `ckanext-or_facet-0.2.0/PKG-INFO` & `ckanext-or_facet-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: ckanext-or_facet
-Version: 0.2.0
+Version: 0.3.0
 Summary: Combine search facets using OR operator
 Home-page: https://github.com/DataShades/ckanext-or_facet
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
-Keywords: CKAN extension facet
+Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ckantoolkit
-Requires-Dist: six
+Requires-Dist: typing_extensions
+Provides-Extra: test
+Requires-Dist: pytest-ckan; extra == "test"
+Provides-Extra: dev
+Requires-Dist: pytest-ckan; extra == "dev"
 
 [![Tests](https://github.com/DataShades/ckanext-or_facet/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/DataShades/ckanext-or_facet/actions)
 
 
 # ckanext-or_facet
 
 
@@ -28,19 +35,26 @@
 
 ## Installation
 
 
 To install ckanext-or-facet:
 
 1. Install the ckanext-or_facet Python package:
+   ```sh
+   pip install ckanext-or-facet
+   ```
 
-		pip install ckanext-or-facet
 
-1. Add ``or_facet`` to the ``ckan.plugins`` setting in your CKAN config file
+1. Add ``or_facet`` to the ``ckan.plugins`` setting in CKAN config file
+
+1. **Starting from CKAN v2.10.4**: Add ``ckan.search.solr_allowed_query_parsers =
+   edismax bool`` to CKAN config file
 
 
 
-## Config Settings
 
-    # List of facets that are using OR when applied.
-    # (optional, default: empty list).
-    ckanext.or_facet.optional = tags res_format
+## Config Settings
+```ini
+# List of facets that are using OR when applied.
+# (optional, default: empty list).
+ckanext.or_facet.optional = tags res_format
+```
```

### Comparing `ckanext-or_facet-0.2.0/README.md` & `ckanext-or_facet-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,26 @@
 
 ## Installation
 
 
 To install ckanext-or-facet:
 
 1. Install the ckanext-or_facet Python package:
+   ```sh
+   pip install ckanext-or-facet
+   ```
 
-		pip install ckanext-or-facet
 
-1. Add ``or_facet`` to the ``ckan.plugins`` setting in your CKAN config file
+1. Add ``or_facet`` to the ``ckan.plugins`` setting in CKAN config file
+
+1. **Starting from CKAN v2.10.4**: Add ``ckan.search.solr_allowed_query_parsers =
+   edismax bool`` to CKAN config file
 
 
 
-## Config Settings
 
-    # List of facets that are using OR when applied.
-    # (optional, default: empty list).
-    ckanext.or_facet.optional = tags res_format
+## Config Settings
+```ini
+# List of facets that are using OR when applied.
+# (optional, default: empty list).
+ckanext.or_facet.optional = tags res_format
+```
```

### Comparing `ckanext-or_facet-0.2.0/ckanext/or_facet/tests/test_plugin.py` & `ckanext-or_facet-0.3.0/ckanext/or_facet/tests/test_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Tests for plugin.py."""
 import pytest
 import ckan.tests.helpers as helpers
 import ckan.tests.factories as factories
 import ckanext.or_facet.plugin as plugin
 
 
-def _orPrefix(field):
-    return "{!edismax q.op=OR tag=orFq%s}" % field
+def _prepare_ors(field, fqs):
+    return "{{!bool tag=orFq{} {}}}".format(
+        field,
+        " ".join(f"should='{fq}'" for fq in fqs),
+    )
 
 
-class TestConfig(object):
+class TestConfig:
     def test_missing_config_parsed(self):
         assert plugin._get_default_ors() == []
 
     @pytest.mark.ckan_config("or_facet.or_facets", None)
     def test_empty_config_parsed(self):
         assert plugin._get_default_ors() == []
 
@@ -22,68 +25,68 @@
         assert plugin._get_default_ors() == ["tags"]
 
     @pytest.mark.ckan_config("or_facet.or_facets", "tags res_format")
     def test_multiple_config_parsed(self):
         assert plugin._get_default_ors() == ["tags", "res_format"]
 
 
-class TestExtraOrs(object):
+class TestExtraOrs:
     def test_base_case(self):
         extras = {
             "ext_a": 1,
             plugin._extra_or_prefix + "tags": "on",
             plugin._extra_or_prefix + "groups": "off",
         }
         assert plugin._get_extra_ors_state(extras) == {"tags": True, "groups": False}
 
 
-class TestSplit(object):
+class TestSplit:
     @pytest.mark.parametrize(
-        "fq, field, expected",
+        ("fq", "field", "expected"),
         [
             (
                 'tags:"Structural Framework"',
                 "tags",
-                ('{!edismax q.op=OR tag=orFqtags}tags:"Structural Framework"', ""),
+                ("{!bool tag=orFqtags should='tags:\"Structural Framework\"'}", ""),
             ),
             ("organization:123", "tags", (None, "organization:123")),
             ("", "tags", (None, "")),
-            ("x:1", "x", (_orPrefix("x") + "x:1", "")),
-            ("x:hello x:world", "x", (_orPrefix("x") + "x:hello x:world", "")),
-            ("x:a y:b", "y", (_orPrefix("y") + "y:b", "x:a")),
-            ('x:"a" y:"b"', "y", (_orPrefix("y") + 'y:"b"', 'x:"a"')),
+            ("x:1", "x", (_prepare_ors("x", ["x:1"]), "")),
+            ("x:hello x:world", "x", (_prepare_ors("x", ["x:hello", "x:world"]), "")),
+            ("x:a y:b", "y", (_prepare_ors("y", ["y:b"]), "x:a")),
+            ('x:"a" y:"b"', "y", (_prepare_ors("y", ['y:"b"']), 'x:"a"')),
             (
                 "z:1 x:a z:2 x:\"b\" z:3 x:'c'",
                 "x",
-                (_orPrefix("x") + "x:a x:\"b\" x:'c'", "z:1  z:2  z:3"),
+                (_prepare_ors("x", ["x:a", 'x:"b"', r"x:\'c\'"]), "z:1  z:2  z:3"),
             ),
             (
                 "x-x:a-a y-y:b-b z-z:c-c",
                 "x-x",
-                (_orPrefix("x-x") + "x-x:a-a", "y-y:b-b z-z:c-c"),
+                (_prepare_ors("x-x", ["x-x:a-a"]), "y-y:b-b z-z:c-c"),
             ),
             (
                 "x-x:a-a y-y:b-b z-z:c-c",
                 "y-y",
-                (_orPrefix("y-y") + "y-y:b-b", "x-x:a-a  z-z:c-c"),
+                (_prepare_ors("y-y", ["y-y:b-b"]), "x-x:a-a  z-z:c-c"),
             ),
             (
                 "x-x:a-a y-y:b-b z-z:c-c",
                 "z-z",
-                (_orPrefix("z-z") + "z-z:c-c", "x-x:a-a y-y:b-b"),
+                (_prepare_ors("z-z", ["z-z:c-c"]), "x-x:a-a y-y:b-b"),
             ),
         ],
     )
     def test_split(self, fq, field, expected):
         assert plugin._split_fq(fq, field) == expected
 
 
 @pytest.mark.usefixtures("with_plugins", "clean_db", "clean_index")
-@pytest.mark.ckan_config("ckan.search.solr_allowed_query_parsers", "edismax")
-class TestPlugin(object):
+@pytest.mark.ckan_config("ckan.search.solr_allowed_query_parsers", "edismax bool")
+class TestPlugin:
     @pytest.mark.ckan_config("or_facet.or_facets", "tags res_format")
     def test_search_with_two_ors(self, organization):
         expected_tags = {"bye": 1, "hello": 1, "world": 2}
         expected_formats = {"JSON": 1, "HTML": 1, "CSV": 2}
 
         d1 = factories.Dataset(tags=[{"name": "hello"}, {"name": "world"}])
         d2 = factories.Dataset(tags=[{"name": "bye"}, {"name": "world"}])
@@ -93,25 +96,25 @@
         factories.Resource(package_id=d2["id"], format="CSV")
         factories.Resource(package_id=d2["id"], format="HTML")
 
         for tag, count in expected_tags.items():
             result = helpers.call_action(
                 "package_search",
                 fl="id,tags",
-                fq="tags:{}".format(tag),
-                **{"facet.field": '["tags"]'}
+                fq=f"tags:{tag}",
+                **{"facet.field": '["tags"]'},
             )
             assert result["count"] == count
             assert result["facets"]["tags"] == expected_tags
 
         for fmt, count in expected_formats.items():
             result = helpers.call_action(
                 "package_search",
-                fq="res_format:{}".format(fmt),
-                **{"facet.field": '["res_format"]'}
+                fq=f"res_format:{fmt}",
+                **{"facet.field": '["res_format"]'},
             )
             assert result["count"] == count
             assert result["facets"]["res_format"] == expected_formats
 
     @pytest.mark.ckan_config("or_facet.or_facets", "tags")
     def test_search_with_one_or_and_one_extra_or(self):
         expected_tags = {"bye": 1, "hello": 1, "world": 2}
@@ -125,71 +128,74 @@
         factories.Resource(package_id=d2["id"], format="CSV")
         factories.Resource(package_id=d2["id"], format="HTML")
 
         for tag, count in expected_tags.items():
             result = helpers.call_action(
                 "package_search",
                 fl="id,tags",
-                fq="tags:{}".format(tag),
+                fq=f"tags:{tag}",
                 **{
                     "facet.field": '["tags"]',
                     plugin._extra_or_prefix + "res_format": "on",
-                }
+                },
             )
             assert result["count"] == count
             assert result["facets"]["tags"] == expected_tags
 
         for fmt, count in expected_formats.items():
             result = helpers.call_action(
                 "package_search",
-                fq="res_format:{}".format(fmt),
+                fq=f"res_format:{fmt}",
                 **{
                     "facet.field": '["res_format"]',
                     plugin._extra_or_prefix + "res_format": "on",
-                }
+                },
             )
             assert result["count"] == count
             assert result["facets"]["res_format"] == expected_formats
 
     @pytest.mark.ckan_config("or_facet.or_facets", "tags")
     def test_search_with_one_or(self):
         expected_tags = {"bye": 1, "hello": 1, "world": 2}
         factories.Dataset(tags=[{"name": "hello"}, {"name": "world"}])
         factories.Dataset(tags=[{"name": "bye"}, {"name": "world"}])
 
         for tag, count in expected_tags.items():
             result = helpers.call_action(
                 "package_search",
                 fl="id,tags",
-                fq="tags:{}".format(tag),
-                **{"facet.field": '["tags"]'}
+                fq=f"tags:{tag}",
+                **{"facet.field": '["tags"]'},
             )
             assert result["count"] == count
             assert result["facets"]["tags"] == expected_tags
 
     def test_search_without_ors(self):
         factories.Dataset(tags=[{"name": "hello"}, {"name": "world"}])
         factories.Dataset(tags=[{"name": "bye"}, {"name": "world"}])
 
         result = helpers.call_action(
             "package_search",
             fl="id,tags",
             fq="tags:hello",
-            **{"facet.field": '["tags"]'}
+            **{"facet.field": '["tags"]'},
         )
         assert result["count"] == 1
         assert result["facets"]["tags"] == {"hello": 1, "world": 1}
 
         result = helpers.call_action(
-            "package_search", fl="id,tags", fq="tags:bye", **{"facet.field": '["tags"]'}
+            "package_search",
+            fl="id,tags",
+            fq="tags:bye",
+            **{"facet.field": '["tags"]'},
         )
         assert result["count"] == 1
         assert result["facets"]["tags"] == {"bye": 1, "world": 1}
 
         result = helpers.call_action(
             "package_search",
             fl="id,tags",
             fq="tags:world",
-            **{"facet.field": '["tags"]'}
+            **{"facet.field": '["tags"]'},
         )
         assert result["count"] == 2
         assert result["facets"]["tags"] == {"bye": 1, "hello": 1, "world": 2}
```

### Comparing `ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/PKG-INFO` & `ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: ckanext-or_facet
-Version: 0.2.0
+Version: 0.3.0
 Summary: Combine search facets using OR operator
 Home-page: https://github.com/DataShades/ckanext-or_facet
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
-Keywords: CKAN extension facet
+Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ckantoolkit
-Requires-Dist: six
+Requires-Dist: typing_extensions
+Provides-Extra: test
+Requires-Dist: pytest-ckan; extra == "test"
+Provides-Extra: dev
+Requires-Dist: pytest-ckan; extra == "dev"
 
 [![Tests](https://github.com/DataShades/ckanext-or_facet/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/DataShades/ckanext-or_facet/actions)
 
 
 # ckanext-or_facet
 
 
@@ -28,19 +35,26 @@
 
 ## Installation
 
 
 To install ckanext-or-facet:
 
 1. Install the ckanext-or_facet Python package:
+   ```sh
+   pip install ckanext-or-facet
+   ```
 
-		pip install ckanext-or-facet
 
-1. Add ``or_facet`` to the ``ckan.plugins`` setting in your CKAN config file
+1. Add ``or_facet`` to the ``ckan.plugins`` setting in CKAN config file
+
+1. **Starting from CKAN v2.10.4**: Add ``ckan.search.solr_allowed_query_parsers =
+   edismax bool`` to CKAN config file
 
 
 
-## Config Settings
 
-    # List of facets that are using OR when applied.
-    # (optional, default: empty list).
-    ckanext.or_facet.optional = tags res_format
+## Config Settings
+```ini
+# List of facets that are using OR when applied.
+# (optional, default: empty list).
+ckanext.or_facet.optional = tags res_format
+```
```

### Comparing `ckanext-or_facet-0.2.0/ckanext_or_facet.egg-info/SOURCES.txt` & `ckanext-or_facet-0.3.0/ckanext_or_facet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-or_facet-0.2.0/pyproject.toml` & `ckanext-or_facet-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 [tool.black]
 # line-length = 88
 # preview = true
 
 [tool.ruff]
+
 target-version = "py38"
+
+[tool.ruff.lint]
 select = [
-       # "B",  # likely bugs and design problems
-       # "BLE",  # do not catch blind exception
-       # "C40",  # better list/set/dict comprehensions
-       # "C90",  # check McCabe complexity
-       # "COM",  # trailing commas
+       "B",  # likely bugs and design problems
+       "BLE",  # do not catch blind exception
+       "C40",  # better list/set/dict comprehensions
+       "C90",  # check McCabe complexity
+       "COM",  # trailing commas
        "E",  # pycodestyle error
-       # "W",  # pycodestyle warning
+       "W",  # pycodestyle warning
        "F",  # pyflakes
-       # "G",  # format strings for logging statements
-       # "N",  # naming conventions
-       # "PL",  # pylint
-       # "PT",  # pytest style
-       # "PIE",  # misc lints
-       # "Q",  # preferred quoting style
-       # "RET",  # improvements for return statements
-       # "RSE",  # improvements for rise statements
-       # "S",  # security testing
-       # "SIM",  # simplify code
-       # "T10",  # debugging statements
-       # "T20",  # print statements
-       # "TID",  # tidier imports
-       # "TRY",  # better exceptions
-       # "UP",  # upgrade syntax for newer versions of the language
+       "G",  # format strings for logging statements
+       "N",  # naming conventions
+       "PL",  # pylint
+       "PT",  # pytest style
+       "PIE",  # misc lints
+       "Q",  # preferred quoting style
+       "RET",  # improvements for return statements
+       "RSE",  # improvements for rise statements
+       "S",  # security testing
+       "SIM",  # simplify code
+       "T10",  # debugging statements
+       "T20",  # print statements
+       "TID",  # tidier imports
+       "TRY",  # better exceptions
+       "UP",  # upgrade syntax for newer versions of the language
 ]
 ignore = [
        "E712", # comparison to bool: violated by SQLAlchemy filters
        "PT004", # fixture does not return anything, add leading underscore: violated by clean_db
        "PLC1901", # simplify comparison to empty string: violated by SQLAlchemy filters
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "ckanext/or_facet/tests*" = ["S", "PL"]
 
 [tool.isort]
 known_ckan = "ckan"
 known_ckanext = "ckanext"
 known_self = "ckanext.or_facet"
 sections = "FUTURE,STDLIB,FIRSTPARTY,THIRDPARTY,CKAN,CKANEXT,SELF,LOCALFOLDER"
```

