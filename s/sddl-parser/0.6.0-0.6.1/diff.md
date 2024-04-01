# Comparing `tmp/sddl_parser-0.6.0.tar.gz` & `tmp/sddl_parser-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddl_parser-0.6.0.tar", max compression
+gzip compressed data, was "sddl_parser-0.6.1.tar", max compression
```

## Comparing `sddl_parser-0.6.0.tar` & `sddl_parser-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7059 2024-02-21 12:59:47.666639 sddl_parser-0.6.0/README.md
--rw-r--r--   0        0        0      434 2024-02-21 13:02:14.852078 sddl_parser-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1450 2024-02-20 13:03:32.286757 sddl_parser-0.6.0/sddl_parser/__init__.py
--rw-r--r--   0        0        0    51462 2024-02-20 13:03:32.141401 sddl_parser-0.6.0/sddl_parser/ace_rights_enums.py
--rw-r--r--   0        0        0     1537 2024-02-20 13:03:32.156940 sddl_parser-0.6.0/sddl_parser/api.py
--rw-r--r--   0        0        0     1290 2024-02-20 13:03:32.176439 sddl_parser-0.6.0/sddl_parser/enums.py
--rw-r--r--   0        0        0     5014 2024-02-21 12:36:49.363880 sddl_parser-0.6.0/sddl_parser/parser.py
--rw-r--r--   0        0        0     6138 2024-02-21 12:36:49.377003 sddl_parser-0.6.0/sddl_parser/parser_conditional_ace.py
--rw-r--r--   0        0        0     1109 2024-02-21 10:17:35.226996 sddl_parser-0.6.0/sddl_parser/parser_sid.py
--rw-r--r--   0        0        0     2836 2024-02-20 13:03:32.220896 sddl_parser-0.6.0/sddl_parser/sid_enum.py
--rw-r--r--   0        0        0     3450 2024-02-21 11:16:04.150395 sddl_parser-0.6.0/sddl_parser/types.py
--rw-r--r--   0        0        0     5344 2024-02-20 13:03:32.269158 sddl_parser-0.6.0/sddl_parser/well_known_dictionary.py
--rw-r--r--   0        0        0     7494 1970-01-01 00:00:00.000000 sddl_parser-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7059 2024-04-01 20:21:44.092809 sddl_parser-0.6.1/README.md
+-rw-r--r--   0        0        0      434 2024-04-01 20:21:44.092809 sddl_parser-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1450 2024-04-01 20:21:44.092809 sddl_parser-0.6.1/sddl_parser/__init__.py
+-rw-r--r--   0        0        0    51462 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/ace_rights_enums.py
+-rw-r--r--   0        0        0     1537 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/api.py
+-rw-r--r--   0        0        0     1290 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/enums.py
+-rw-r--r--   0        0        0     5014 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/parser.py
+-rw-r--r--   0        0        0     6138 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/parser_conditional_ace.py
+-rw-r--r--   0        0        0     1109 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/parser_sid.py
+-rw-r--r--   0        0        0     2836 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/sid_enum.py
+-rw-r--r--   0        0        0     3821 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/types.py
+-rw-r--r--   0        0        0     5344 2024-04-01 20:21:44.096809 sddl_parser-0.6.1/sddl_parser/well_known_dictionary.py
+-rw-r--r--   0        0        0     7494 1970-01-01 00:00:00.000000 sddl_parser-0.6.1/PKG-INFO
```

### Comparing `sddl_parser-0.6.0/README.md` & `sddl_parser-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/__init__.py` & `sddl_parser-0.6.1/sddl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/ace_rights_enums.py` & `sddl_parser-0.6.1/sddl_parser/ace_rights_enums.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/api.py` & `sddl_parser-0.6.1/sddl_parser/api.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/enums.py` & `sddl_parser-0.6.1/sddl_parser/enums.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/parser.py` & `sddl_parser-0.6.1/sddl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/parser_conditional_ace.py` & `sddl_parser-0.6.1/sddl_parser/parser_conditional_ace.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/parser_sid.py` & `sddl_parser-0.6.1/sddl_parser/parser_sid.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/sid_enum.py` & `sddl_parser-0.6.1/sddl_parser/sid_enum.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/sddl_parser/types.py` & `sddl_parser-0.6.1/sddl_parser/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,25 +35,32 @@
         self.rights = rights_to_type(self.rights_int, access_mask)
         return self
 
     def pformat(self, indent: int = 0) -> str:
         flags = "|".join([f.name for f in self.flags])
         rights = "|".join([r.name for r in self.rights])
         sid = self.sid.name if isinstance(self.sid, SIDEnum) else self.sid
-        return f"{' '*indent}{self.type.name} {flags} {rights} {sid}"
+        entry = f"{' '*indent}{self.type.name} {flags} {rights} {sid}"
+        if self.conditional_ace_string:
+            entry += f"\n{' '*indent}Condition: {self.conditional_ace_string}"
+        return entry
 
     def asdict(self) -> dict:
         return {
             "type": self.type.name,
             "flags": [f.name for f in self.flags],
             "rights": [r.name for r in self.rights],
             "sid": self.sid.name if isinstance(self.sid, SIDEnum) else self.sid,
+            "conditional_ace": self.conditional_ace,
+            "conditional_ace_string": self.conditional_ace_string,
         }
 
 
+'O:SYG:SYD:AI(XA;ID;0x1200a9;;;BU;(WIN://SYSAPPID Contains "Microsoft.MicrosoftEdge.Stable_8wekyb3d8bbwe"))'
+
 @dataclass
 class ACL:
     flags: Set[SDDLFlags]
     aces: List[ACE]
 
     def pformat(self, indent: int = 0) -> str:
         return (
```

### Comparing `sddl_parser-0.6.0/sddl_parser/well_known_dictionary.py` & `sddl_parser-0.6.1/sddl_parser/well_known_dictionary.py`

 * *Files identical despite different names*

### Comparing `sddl_parser-0.6.0/PKG-INFO` & `sddl_parser-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sddl-parser
-Version: 0.6.0
+Version: 0.6.1
 Summary: Parse SDDL strings
 Author: Max Harley
 Author-email: maxh@maxh.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

