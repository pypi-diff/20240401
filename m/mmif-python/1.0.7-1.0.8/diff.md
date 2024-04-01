# Comparing `tmp/mmif-python-1.0.7.tar.gz` & `tmp/mmif-python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.7.tar", last modified: Thu Jul 20 02:53:17 2023, max compression
+gzip compressed data, was "mmif-python-1.0.8.tar", last modified: Mon Jul 24 02:27:54 2023, max compression
```

## Comparing `mmif-python-1.0.7.tar` & `mmif-python-1.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-20 02:52:48.000000 mmif-python-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 02:52:48.000000 mmif-python-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 02:53:17.784157 mmif-python-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 02:52:48.000000 mmif-python-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 02:52:48.000000 mmif-python-1.0.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-20 02:52:48.000000 mmif-python-1.0.7/mmif/utils/video_document_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:53:17.784157 mmif-python-1.0.7/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 02:53:17.000000 mmif-python-1.0.7/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 02:52:48.000000 mmif-python-1.0.7/requirements.cv
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 02:52:48.000000 mmif-python-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 02:53:17.784157 mmif-python-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-20 02:52:48.000000 mmif-python-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-24 02:27:16.000000 mmif-python-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 02:27:16.000000 mmif-python-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-24 02:27:54.356726 mmif-python-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 02:27:16.000000 mmif-python-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 02:27:17.000000 mmif-python-1.0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:53.000000 mmif-python-1.0.8/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 02:27:53.000000 mmif-python-1.0.8/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-24 02:27:53.000000 mmif-python-1.0.8/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27494 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-24 02:27:16.000000 mmif-python-1.0.8/mmif/utils/video_document_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 02:27:53.000000 mmif-python-1.0.8/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 02:27:53.000000 mmif-python-1.0.8/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:27:54.356726 mmif-python-1.0.8/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 02:27:54.000000 mmif-python-1.0.8/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 02:27:16.000000 mmif-python-1.0.8/requirements.cv
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 02:27:16.000000 mmif-python-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:27:54.356726 mmif-python-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-24 02:27:16.000000 mmif-python-1.0.8/setup.py
```

### Comparing `mmif-python-1.0.7/LICENSE` & `mmif-python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/PKG-INFO` & `mmif-python-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.7/mmif/__init__.py` & `mmif-python-1.0.8/mmif/__init__.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.8/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/res/mmif.json` & `mmif-python-1.0.8/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/serialize/annotation.py` & `mmif-python-1.0.8/mmif/serialize/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     MmifObject that represents an annotation in a MMIF view.
     """
 
     def __init__(self, anno_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         self._type: ThingTypesBase = ThingTypesBase('')
         # to store the parent view ID
         self._parent_view_id = ''
-        self.reserved_names.add('_parent_view_id')
+        self._props_ephemeral: AnnotationProperties = AnnotationProperties()
+        self.reserved_names.update(('_parent_view_id', '_props_ephemeral'))
         if not hasattr(self, 'properties'):  # don't overwrite DocumentProperties on super() call
             self.properties: AnnotationProperties = AnnotationProperties()
             self._attribute_classes = {'properties': AnnotationProperties}
         self.disallow_additional_properties()
         self._required_attributes = ["_type", "properties"]
         super().__init__(anno_obj)
     
@@ -116,22 +117,26 @@
                              "either string, number, boolean, None, or a list of them."
                              f"(\"{name}\": \"{str(value)}\"")
 
     def get(self, prop_name: str) -> Union['AnnotationProperties', JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES], List[List[JSON_PRMTV_TYPES]]]:
         """
         A special getter for Annotation properties. This is to allow for
         directly accessing properties without having to go through the
-        properties object.
+        properties object, or view-level annotation properties encoded in the 
+        ``view.metadata.contains`` dict. Note that the regular props will take 
+        the priority over the ephemeral props when there are conflicts.
         """
         if prop_name in {'at_type', '@type'}:
             return str(self._type)
         elif prop_name == 'properties':
             return self.properties
         elif prop_name in self.properties:
             return self.properties[prop_name]
+        elif prop_name in self._props_ephemeral:
+            return self._props_ephemeral[prop_name]
         else:
             raise KeyError(f"Property {prop_name} does not exist in this annotation.")
 
     get_property = get
 
     def __getitem__(self, prop_name: str):
         return self.get(prop_name)
@@ -159,31 +164,25 @@
     If ``document_obj`` is not provided, an empty Document will be generated.
 
     :param document_obj: the JSON data that defines the document
     """
     def __init__(self, doc_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         # see https://github.com/clamsproject/mmif-python/issues/226 for discussion
         # around the use of these three dictionaries
+        # (names changed since, `existing` >> `ephemeral` and `temporary` >> `pending`)
         self._props_original: DocumentProperties = DocumentProperties()
-        self._props_existing: AnnotationProperties = AnnotationProperties()
-        self._props_temporary: AnnotationProperties = AnnotationProperties()
-        self.reserved_names.update(('_props_original', '_props_existing', '_props_temporary'))
+        self._props_pending: AnnotationProperties = AnnotationProperties()
+        self.reserved_names.update(('_props_original', '_props_pending'))
         
         self._type: Union[ThingTypesBase, DocumentTypesBase] = ThingTypesBase('')
         self.properties = self._props_original
         self.disallow_additional_properties()
         self._attribute_classes = {'properties': DocumentProperties}
         super().__init__(doc_obj)
     
-    def _add_property_from_annotation(self, annotation: Annotation):
-        if annotation.at_type != AnnotationTypes.Annotation:
-            raise ValueError("Only `Annotation` type can be added as a property to a `Document` object.")
-        for prop_name, prop_value in annotation.properties.items():
-            self._props_existing[prop_name] = prop_value
-
     def add_property(self, name: str,
                      value: Union[JSON_PRMTV_TYPES, List[JSON_PRMTV_TYPES]]
                      ) -> None:
         """
         Adds a property to the document's properties.
         
         Unlike the parent :class:`Annotation` class, added properties of a 
@@ -213,36 +212,40 @@
             self.properties.text = Text(value)
         elif name == "mime":
             self.properties.mime = str(value)
         elif name == "location":
             self.location = value
         elif name not in self._props_original:
             if self.check_prop_value_is_simple_enough(value):
-                self._props_temporary[name] = value
+                self._props_pending[name] = value
             else:
                 super().add_property(name, value)
 
     def get(self, prop_name):
         """
-        A special getter for Document properties. This is to allow for reading 
-        the three properties in a specific order so that the latest value is 
-        returned, in case there are multiple values for the same key.
+        A special getter for Document properties. The major difference from
+        the super class's :py:meth:`Annotation.get` method is that Document 
+        class has one more set of *"pending"* properties, that are added after 
+        the Document object is created and will be serialized as a separate 
+        :py:class:`Annotation` object of which ``@type = Annotation``. The 
+        pending properties will take the priority over the regular properties 
+        when there are conflicts.
         """
         if prop_name == 'id':
             # because all three dicts have `id` key as required field, we need
             # this special case to return the correct value from the correct dict
             return self.id
         elif prop_name == 'location':
             # because location is internally stored in self.location_,
             # it doesn't work with regular __getitem__ method
             return self.location
-        elif prop_name in self._props_temporary:
-            return self._props_temporary[prop_name]
-        elif prop_name in self._props_existing:
-            return self._props_existing[prop_name]
+        elif prop_name in self._props_pending:
+            return self._props_pending[prop_name]
+        elif prop_name in self._props_ephemeral:
+            return self._props_ephemeral[prop_name]
         else:
             return super().get(prop_name)
 
     get_property = get
     
     @property
     def text_language(self) -> str:
@@ -305,22 +308,24 @@
     def location_address(self) -> Optional[str]:
         """
         Retrieves the full address from the document location URI.
         Returns None when no location is set.
         """
         return self.properties.location_address()
 
-    def location_path(self) -> Optional[str]:
+    def location_path(self, nonexist_ok=True) -> Optional[str]:
         """
         Retrieves a path that's resolved to a pathname in the local file system.
         To obtain the original value of the "path" part in the location string
         (before resolving), use ``properties.location_path_literal`` method.
         Returns None when no location is set.
+        
+        :param nonexist_ok: if False, raise FileNotFoundError when the resolved path doesn't exist
         """
-        return self.properties.location_path_resolved()
+        return self.properties.location_path_resolved(nonexist_ok=nonexist_ok)
 
 
 class AnnotationProperties(MmifObject, MutableMapping[str, T]):
     """
     AnnotationProperties object that represents the
     ``properties`` object within a MMIF annotation.
```

### Comparing `mmif-python-1.0.7/mmif/serialize/mmif.py` & `mmif-python-1.0.8/mmif/serialize/mmif.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,32 +89,48 @@
         if sanitize:
             self.sanitize()
         return super().serialize(pretty)
 
     def _deserialize(self, input_dict: dict) -> None:
         """
         Deserializes the MMIF JSON string into a Mmif object.
-        This will read in existing ``Annotation`` typed annotations and 
+        After *regular* deserialization, this method will perform the following 
+        *special* handling of Annotation.properties that allows apps to access 
+        Annotation/Document properties that are not encoded in the objects 
+        themselves. This is to allow apps to access in a more intuitive way, 
+        without having too much hassle to iterate views and manually collect the properties.
+        
+        1. This will read in existing *view*-scoped properties from *contains*
+        metadata and attach them to the corresponding ``Annotation`` objects.
+
+        1. This will read in existing ``Annotation`` typed annotations and 
         attach the document-level properties to the ``Document`` objects, 
-        using a volatile property dict. This will allow apps to access the
-        document-level properties without having too much hassle to iterate
-        views and manually collect the properties.
+        using an ephemeral property dict. 
+        
         """
         super()._deserialize(input_dict)
         for view in self.views:
-            doc_id = None
-            if AnnotationTypes.Annotation in view.metadata.contains:
-                if 'document' in view.metadata.contains[AnnotationTypes.Annotation]:
-                    doc_id = view.metadata.contains[AnnotationTypes.Annotation]['document']
+            # this dict will be populated with properties 
+            # that are not encoded in individual annotations objects themselves
+            extrinsic_props = defaultdict(dict)
+            for at_type, type_lv_props in view.metadata.contains.items():
+                for prop_key, prop_value in type_lv_props.items():
+                    extrinsic_props[at_type][prop_key] = prop_value
+            for ann in view.get_annotations():
+                # first add all extrinsic properties to the Annotation objects
+                # as "ephemeral" properties
+                for prop_key, prop_value in extrinsic_props[ann.at_type].items():
+                    ann._props_ephemeral[prop_key] = prop_value
+                # then, do the same to associated Document objects. Note that, 
                 # in a view, it is guaranteed that all Annotation objects are not duplicates
-                for ann in view.get_annotations(AnnotationTypes.Annotation):
-                    if doc_id is None:
-                        doc_id = ann.get_property('document')
+                if ann.at_type == AnnotationTypes.Annotation:
                     try:
-                        self.get_document_by_id(doc_id)._add_property_from_annotation(ann)
+                        doc_id = ann.get_property('document')
+                        for prop_key, prop_value in ann.properties.items():
+                            self.get_document_by_id(doc_id)._props_ephemeral[prop_key] = prop_value
                     except KeyError:
                         warnings.warn(f"Annotation {ann.id} has a document ID {doc_id} that does not exist in the MMIF object. Skipping.", RuntimeWarning)
 
     def generate_capital_annotations(self):
         """
         Automatically convert any "pending" temporary properties from 
         `Document` objects to `Annotation` objects . The generated `Annotation` 
@@ -139,17 +155,17 @@
                     if 'document' in view.metadata.contains[AnnotationTypes.Annotation]:
                         doc_id = view.metadata.contains[AnnotationTypes.Annotation]['document']
                     for ann in view.get_annotations(AnnotationTypes.Annotation):
                         if doc_id is None:
                             doc_id = ann.get_property('document')
                         existing_anns[doc_id].update(ann.properties)
                 for doc in view.get_documents():
-                    anns_to_write[doc.id].update(doc._props_temporary)
+                    anns_to_write[doc.id].update(doc._props_pending)
             for doc in self.documents:
-                anns_to_write[doc.id].update(doc._props_temporary)
+                anns_to_write[doc.id].update(doc._props_pending)
             # additional iteration of views, to find a proper view to add the 
             # generated annotations. If none found, use the last view as the kitchen sink
             last_view_for_docs = defaultdict(lambda: last_view)
             doc_ids = set(anns_to_write.keys())
             for doc_id in doc_ids:
                 for view in reversed(self.views):
                     # first try to find out if this view "contains" any annotation to the doc
```

### Comparing `mmif-python-1.0.7/mmif/serialize/model.py` & `mmif-python-1.0.8/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/serialize/view.py` & `mmif-python-1.0.8/mmif/serialize/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         :return: the generated :class:`mmif.serialize.annotation.Annotation`
         """
         new_annotation = Annotation()
         new_annotation.at_type = at_type
         self._set_id(new_annotation, aid)
         for propk, propv in properties.items():
             new_annotation.add_property(propk, propv)
+        for propk, propv in self.metadata.contains.get(at_type, {}).items():
+            new_annotation._props_ephemeral[propk] = propv
         return self.add_annotation(new_annotation, overwrite)
 
     def add_annotation(self, annotation: 'Annotation', overwrite=False) -> 'Annotation':
         """
         Adds an annotation to the current view.
 
         Fails if there is already an annotation with the same ID
```

### Comparing `mmif-python-1.0.7/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.8/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/vocabulary/base_types.py` & `mmif-python-1.0.8/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif/vocabulary/document_types.py` & `mmif-python-1.0.8/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.8/mmif_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.7/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.8/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.7/setup.py` & `mmif-python-1.0.8/setup.py`

 * *Files identical despite different names*

