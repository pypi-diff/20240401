# Comparing `tmp/eflips_ingest-1.0.0.tar.gz` & `tmp/eflips_ingest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_ingest-1.0.0.tar", max compression
+gzip compressed data, was "eflips_ingest-1.0.1.tar", max compression
```

## Comparing `eflips_ingest-1.0.0.tar` & `eflips_ingest-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    34143 2024-03-27 14:26:26.430593 eflips_ingest-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     7014 2024-03-27 14:26:26.430593 eflips_ingest-1.0.0/README.md
--rw-r--r--   0        0        0      207 2024-03-27 14:26:26.430593 eflips_ingest-1.0.0/eflips/ingest/__init__.py
--rw-r--r--   0        0        0     5811 2024-03-27 14:26:26.430593 eflips_ingest-1.0.0/eflips/ingest/base.py
--rw-r--r--   0        0        0    63440 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/bvgxml.py
--rw-r--r--   0        0        0    15422 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/dummy.py
--rw-r--r--   0        0        0     2994 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/util.py
--rw-r--r--   0        0        0      383 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/xmldata/README.md
--rw-r--r--   0        0        0     1058 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/xmldata/__init__.py
--rw-r--r--   0        0        0    47033 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/eflips/ingest/xmldata/bvg_xml.py
--rw-r--r--   0        0        0     1120 2024-03-27 14:26:26.434593 eflips_ingest-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     7014 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/README.md
+-rw-r--r--   0        0        0      207 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/__init__.py
+-rw-r--r--   0        0        0     5811 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/base.py
+-rw-r--r--   0        0        0    15422 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/dummy.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/__init__.py
+-rw-r--r--   0        0        0    63454 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/bvgxml.py
+-rw-r--r--   0        0        0      383 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/README.md
+-rw-r--r--   0        0        0     1065 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/__init__.py
+-rw-r--r--   0        0        0    47033 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/bvg_xml.py
+-rw-r--r--   0        0        0     3049 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/eflips/ingest/util.py
+-rw-r--r--   0        0        0     1120 2024-04-01 14:16:30.047527 eflips_ingest-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.0.1/PKG-INFO
```

### Comparing `eflips_ingest-1.0.0/LICENSE.md` & `eflips_ingest-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.0/README.md` & `eflips_ingest-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.0/eflips/ingest/base.py` & `eflips_ingest-1.0.1/eflips/ingest/base.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.0/eflips/ingest/bvgxml.py` & `eflips_ingest-1.0.1/eflips/ingest/legacy/bvgxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 from lxml import etree
 from sqlalchemy import create_engine, func
 from sqlalchemy.orm import Session
 from tqdm.auto import tqdm
 from xsdata.formats.dataclass.parsers import XmlParser
 
 import eflips.ingest.util
-from eflips.ingest.util import soldner_to_pointz
-from eflips.ingest.xmldata import (
+from eflips.ingest.legacy.xmldata import (
     Linienfahrplan,
     NetzpunktNetzpunkttyp,
 )
+from eflips.ingest.util import soldner_to_pointz
 
 
 def load_and_validate_xml(filename: Path) -> Linienfahrplan:
     """
     Loads the xml string into a Linienfahrplan object and validates it against the schema
     - also removes the 'ns2' strings from the first and last lines
 
@@ -53,15 +53,15 @@
 
     # We want to remove the occurrences of 'ns2: and ':ns2' in the first and last line. Only then does our schema
     # and the 'xmldata' package work. For some reason, with the ns2 it generates two differnet python files, and
     # then it doesn't work.
     xml_string = xml_string.replace("ns2:", "")
     xml_string = xml_string.replace(":ns2", "")
 
-    xsd_path = Path(__file__).parent.parent.parent / "data" / "bvg_xml.xsd"
+    xsd_path = Path(__file__).parent.parent.parent.parent / "data" / "bvg_xml.xsd"
     xmlschema_doc = etree.parse(xsd_path)
     xmlschema = etree.XMLSchema(xmlschema_doc)
 
     xml_doc = etree.fromstring(xml_string)
 
     if not xmlschema.validate(xml_doc):
         raise ValueError(f"XML file {filename} is not valid.")
```

### Comparing `eflips_ingest-1.0.0/eflips/ingest/dummy.py` & `eflips_ingest-1.0.1/eflips/ingest/dummy.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.0/eflips/ingest/util.py` & `eflips_ingest-1.0.1/eflips/ingest/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from typing import Tuple
 
 import requests
 from pyproj import Transformer
 
 import eflips.ingest
 
+"""
+Some utility functions for the ingest module.
+"""
+
 # The transformer is initialized here, so that it is only initialized once
 transformer = Transformer.from_crs("EPSG:3068", "EPSG:4326")
 
 
 @lru_cache(maxsize=4096)
 def get_altitude_openelevation(latlon: Tuple[Number, Number]) -> float:
     """
```

### Comparing `eflips_ingest-1.0.0/eflips/ingest/xmldata/__init__.py` & `eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This file was generated by xsdata, v24.1, on 2024-01-25 17:07:33
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
-from eflips.ingest.xmldata.bvg_xml import (
+from eflips.ingest.legacy.xmldata.bvg_xml import (
     ErgebnisReturnCode,
     FahrtFahrgastrelevant,
     Linienfahrplan,
     MeldungMeldungskategorie,
     MeldungMeldungsnummer,
     MeldungMeldungstext,
     NetzpunktNetzpunkttyp,
```

### Comparing `eflips_ingest-1.0.0/eflips/ingest/xmldata/bvg_xml.py` & `eflips_ingest-1.0.1/eflips/ingest/legacy/xmldata/bvg_xml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.0/pyproject.toml` & `eflips_ingest-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-ingest"
-version = "1.0.0"
+version = "1.0.1"
 description = "A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format."
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/mpm-tu-berlin/eflips-import"
```

### Comparing `eflips_ingest-1.0.0/PKG-INFO` & `eflips_ingest-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-ingest
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format.
 Home-page: https://github.com/mpm-tu-berlin/eflips-import
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

