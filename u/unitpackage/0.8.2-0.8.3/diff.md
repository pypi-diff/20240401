# Comparing `tmp/unitpackage-0.8.2.tar.gz` & `tmp/unitpackage-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitpackage-0.8.2.tar", last modified: Tue Mar 26 22:07:18 2024, max compression
+gzip compressed data, was "unitpackage-0.8.3.tar", last modified: Mon Apr  1 20:13:35 2024, max compression
```

## Comparing `unitpackage-0.8.2.tar` & `unitpackage-0.8.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 22:07:18.228455 unitpackage-0.8.2/
--rw-rw-rw-   0        0        0    35823 2024-02-21 18:31:20.000000 unitpackage-0.8.2/LICENSE
--rw-rw-rw-   0        0        0     5090 2024-03-26 22:07:18.227457 unitpackage-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     4606 2024-03-26 22:07:08.000000 unitpackage-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 22:07:18.229499 unitpackage-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1708 2024-03-26 22:07:08.000000 unitpackage-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 22:07:18.173078 unitpackage-0.8.2/unitpackage/
--rw-rw-rw-   0        0        0        0 2024-03-22 17:22:40.000000 unitpackage-0.8.2/unitpackage/__init__.py
--rw-rw-rw-   0        0        0     9972 2024-03-22 20:20:16.000000 unitpackage-0.8.2/unitpackage/collection.py
-drwxrwxrwx   0        0        0        0 2024-03-26 22:07:18.224283 unitpackage-0.8.2/unitpackage/cv/
--rw-rw-rw-   0        0        0        0 2024-02-21 18:31:20.000000 unitpackage-0.8.2/unitpackage/cv/__init__.py
--rw-rw-rw-   0        0        0     3676 2024-03-26 17:33:40.000000 unitpackage-0.8.2/unitpackage/cv/cv_collection.py
--rw-rw-rw-   0        0        0     9401 2024-03-22 20:20:16.000000 unitpackage-0.8.2/unitpackage/cv/cv_entry.py
--rw-rw-rw-   0        0        0     7546 2024-03-22 20:20:16.000000 unitpackage-0.8.2/unitpackage/descriptor.py
--rw-rw-rw-   0        0        0    24707 2024-03-26 22:05:55.000000 unitpackage-0.8.2/unitpackage/entry.py
--rw-rw-rw-   0        0        0     7647 2024-03-26 22:05:55.000000 unitpackage-0.8.2/unitpackage/local.py
--rw-rw-rw-   0        0        0     2953 2024-03-22 20:20:16.000000 unitpackage-0.8.2/unitpackage/remote.py
-drwxrwxrwx   0        0        0        0 2024-03-26 22:07:18.226302 unitpackage-0.8.2/unitpackage.egg-info/
--rw-rw-rw-   0        0        0     5090 2024-03-26 22:07:17.000000 unitpackage-0.8.2/unitpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-03-26 22:07:17.000000 unitpackage-0.8.2/unitpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 22:07:17.000000 unitpackage-0.8.2/unitpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-03-26 22:07:17.000000 unitpackage-0.8.2/unitpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-26 22:07:17.000000 unitpackage-0.8.2/unitpackage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:13:35.725324 unitpackage-0.8.3/
+-rw-rw-rw-   0        0        0    35823 2024-02-21 18:31:20.000000 unitpackage-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0     5090 2024-04-01 20:13:35.723943 unitpackage-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4606 2024-04-01 20:13:26.000000 unitpackage-0.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:13:35.725937 unitpackage-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2024-04-01 20:13:25.000000 unitpackage-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:13:35.632109 unitpackage-0.8.3/unitpackage/
+-rw-rw-rw-   0        0        0        0 2024-03-22 17:22:40.000000 unitpackage-0.8.3/unitpackage/__init__.py
+-rw-rw-rw-   0        0        0     9972 2024-03-22 20:20:16.000000 unitpackage-0.8.3/unitpackage/collection.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:13:35.720951 unitpackage-0.8.3/unitpackage/cv/
+-rw-rw-rw-   0        0        0        0 2024-02-21 18:31:20.000000 unitpackage-0.8.3/unitpackage/cv/__init__.py
+-rw-rw-rw-   0        0        0     3676 2024-03-26 17:33:40.000000 unitpackage-0.8.3/unitpackage/cv/cv_collection.py
+-rw-rw-rw-   0        0        0     9401 2024-03-22 20:20:16.000000 unitpackage-0.8.3/unitpackage/cv/cv_entry.py
+-rw-rw-rw-   0        0        0     7546 2024-03-22 20:20:16.000000 unitpackage-0.8.3/unitpackage/descriptor.py
+-rw-rw-rw-   0        0        0    25561 2024-04-01 20:12:32.000000 unitpackage-0.8.3/unitpackage/entry.py
+-rw-rw-rw-   0        0        0     8690 2024-04-01 20:12:32.000000 unitpackage-0.8.3/unitpackage/local.py
+-rw-rw-rw-   0        0        0     2953 2024-03-22 20:20:16.000000 unitpackage-0.8.3/unitpackage/remote.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:13:35.721948 unitpackage-0.8.3/unitpackage.egg-info/
+-rw-rw-rw-   0        0        0     5090 2024-04-01 20:13:35.000000 unitpackage-0.8.3/unitpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-01 20:13:35.000000 unitpackage-0.8.3/unitpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:13:35.000000 unitpackage-0.8.3/unitpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-04-01 20:13:35.000000 unitpackage-0.8.3/unitpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 20:13:35.000000 unitpackage-0.8.3/unitpackage.egg-info/top_level.txt
```

### Comparing `unitpackage-0.8.2/LICENSE` & `unitpackage-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/PKG-INFO` & `unitpackage-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: unitpackage
-Version: 0.8.2
+Version: 0.8.3
 Summary: a Python library to interact with a collection of frictionless datapackages
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy<6,>=5
 Requires-Dist: filelock<4,>=3
 Requires-Dist: frictionless<6,>=5.10.1
 Requires-Dist: matplotlib<4,>=3.5.0
 Requires-Dist: pandas<3,>=2
 Requires-Dist: plotly<6,>=5
 Requires-Dist: pybtex<0.25,>=0.24
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.8.2?labpath=tree%2Fdoc%2Findex.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.8.3?labpath=tree%2Fdoc%2Findex.md)
 [![DOI](https://zenodo.org/badge/637997870.svg)](https://zenodo.org/badge/latestdoi/637997870)
 
 This module provides a Python library to interact with a collection of
 [frictionless datapackages](https://frictionlessdata.io/). Such datapackages consist of a CSV (data) file which is annotated with a JSON file.
 This allows storing additional information such as units used in the columns of a CSV or store metadata describing the underlying data.
 Example datapackages can be found [here](https://github.com/echemdb/unitpackage/tree/main/doc/files/) and a JSON could be structured as follows
```

### Comparing `unitpackage-0.8.2/README.md` & `unitpackage-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
 00000010: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
 00000020: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
 00000030: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
 00000040: 722e 6f72 672f 7632 2f67 682f 6563 6865  r.org/v2/gh/eche
 00000050: 6d64 622f 756e 6974 7061 636b 6167 652f  mdb/unitpackage/
-00000060: 302e 382e 323f 6c61 6270 6174 683d 7472  0.8.2?labpath=tr
+00000060: 302e 382e 333f 6c61 6270 6174 683d 7472  0.8.3?labpath=tr
 00000070: 6565 2532 4664 6f63 2532 4669 6e64 6578  ee%2Fdoc%2Findex
 00000080: 2e6d 6429 0d0a 5b21 5b44 4f49 5d28 6874  .md)..[![DOI](ht
 00000090: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
 000000a0: 2f62 6164 6765 2f36 3337 3939 3738 3730  /badge/637997870
 000000b0: 2e73 7667 295d 2868 7474 7073 3a2f 2f7a  .svg)](https://z
 000000c0: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
 000000d0: 6c61 7465 7374 646f 692f 3633 3739 3937  latestdoi/637997
```

### Comparing `unitpackage-0.8.2/setup.py` & `unitpackage-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  along with unitpackage. If not, see <https://www.gnu.org/licenses/>.
 # ********************************************************************
 
 from distutils.core import setup
 
 setup(
     name='unitpackage',
-    version="0.8.2",
+    version="0.8.3",
     packages=['unitpackage', 'unitpackage.cv'],
     license='GPL 3.0+',
     description="a Python library to interact with a collection of frictionless datapackages",
     long_description=open('README.md', encoding="UTF-8").read(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
```

### Comparing `unitpackage-0.8.2/unitpackage/collection.py` & `unitpackage-0.8.3/unitpackage/collection.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/unitpackage/cv/cv_collection.py` & `unitpackage-0.8.3/unitpackage/cv/cv_collection.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/unitpackage/cv/cv_entry.py` & `unitpackage-0.8.3/unitpackage/cv/cv_entry.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/unitpackage/descriptor.py` & `unitpackage-0.8.3/unitpackage/descriptor.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/unitpackage/entry.py` & `unitpackage-0.8.3/unitpackage/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -658,24 +658,40 @@
             >>> entry.save(outdir='./test/generated')
             >>> basename = entry.identifier
             >>> os.path.exists(f'test/generated/{basename}.json') and os.path.exists(f'test/generated/{basename}.csv')
             True
 
         When a ``basename`` is set, the files are named ``basename.csv`` and ``basename.json``.
         Note that for a valid frictionless package this base name
-        'MUST be lower-case and contain only alphanumeric
+        MUST be lower-case and contain only alphanumeric
         characters along with ".", "_" or "-" characters'::
 
             >>> import os
             >>> entry = Entry.create_examples()[0]
             >>> basename = 'save_basename'
             >>> entry.save(basename=basename, outdir='./test/generated')
             >>> os.path.exists(f'test/generated/{basename}.json') and os.path.exists(f'test/generated/{basename}.csv')
             True
 
+        TESTS:
+
+        Save entry with metadata containing datetime format,
+        which is not natively supported by JSON.
+
+            >>> import os
+            >>> from datetime import datetime
+            >>> import pandas as pd
+            >>> from unitpackage.entry import Entry
+            >>> df = pd.DataFrame({'x':[1,2,3], 'y':[2,3,4]})
+            >>> basename = 'save_datetime'
+            >>> entry = Entry.from_df(df=df, basename=basename, metadata={'current time':datetime.now()})
+            >>> entry.save(outdir='./test/generated')
+            >>> os.path.exists(f'test/generated/{basename}.json') and os.path.exists(f'test/generated/{basename}.csv')
+            True
+
         """
         if not os.path.isdir(outdir):
             os.makedirs(outdir)
 
         basename = basename or self.identifier
         csv_name = os.path.join(outdir, basename + ".csv")
         json_name = os.path.join(outdir, basename + ".json")
@@ -690,8 +706,12 @@
 
         # update the identifier and filepath of the resource
         if basename:
             metadata.get_resource(self.identifier).path = basename + ".csv"
             metadata.get_resource(self.identifier).name = basename
 
         self.df.to_csv(csv_name, index=False)
-        metadata.to_json(json_name)
+
+        with open(json_name, mode="w", encoding="utf-8") as json:
+            from unitpackage.local import write_metadata
+
+            write_metadata(json, self.package.to_dict())
```

### Comparing `unitpackage-0.8.2/unitpackage/local.py` & `unitpackage-0.8.3/unitpackage/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,7 +213,36 @@
             logger.warning(
                 f"Fields with names {unused_provided_fields} was provided but does not appear in the field names of tabular resource {package_schema.field_names}."
             )
 
         resource.schema = Schema.from_descriptor({"fields": new_fields})
 
     return package
+
+
+def write_metadata(out, metadata):
+    r"""
+    Write `metadata` to the `out` stream in JSON format.
+
+    """
+
+    def defaultconverter(item):
+        r"""
+        Return `item` that Python's json package does not know how to serialize
+        in a format that Python's json package does know how to serialize.
+        """
+        from datetime import date, datetime
+
+        # The YAML standard knows about dates and times, so we might see these
+        # in the metadata. However, standard JSON does not know about these so
+        # we need to serialize them as strings explicitly.
+        if isinstance(item, (datetime, date)):
+            return str(item)
+
+        raise TypeError(f"Cannot serialize ${item} of type ${type(item)} to JSON.")
+
+    import json
+
+    json.dump(metadata, out, default=defaultconverter, ensure_ascii=False, indent=4)
+    # json.dump does not save files with a newline, which compromises the tests
+    # where the output files are compared to an expected json.
+    out.write("\n")
```

### Comparing `unitpackage-0.8.2/unitpackage/remote.py` & `unitpackage-0.8.3/unitpackage/remote.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.8.2/unitpackage.egg-info/PKG-INFO` & `unitpackage-0.8.3/unitpackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: unitpackage
-Version: 0.8.2
+Version: 0.8.3
 Summary: a Python library to interact with a collection of frictionless datapackages
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy<6,>=5
 Requires-Dist: filelock<4,>=3
 Requires-Dist: frictionless<6,>=5.10.1
 Requires-Dist: matplotlib<4,>=3.5.0
 Requires-Dist: pandas<3,>=2
 Requires-Dist: plotly<6,>=5
 Requires-Dist: pybtex<0.25,>=0.24
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.8.2?labpath=tree%2Fdoc%2Findex.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.8.3?labpath=tree%2Fdoc%2Findex.md)
 [![DOI](https://zenodo.org/badge/637997870.svg)](https://zenodo.org/badge/latestdoi/637997870)
 
 This module provides a Python library to interact with a collection of
 [frictionless datapackages](https://frictionlessdata.io/). Such datapackages consist of a CSV (data) file which is annotated with a JSON file.
 This allows storing additional information such as units used in the columns of a CSV or store metadata describing the underlying data.
 Example datapackages can be found [here](https://github.com/echemdb/unitpackage/tree/main/doc/files/) and a JSON could be structured as follows
```

