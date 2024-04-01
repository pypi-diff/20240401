# Comparing `tmp/scoutbook_parser-0.9.0.tar.gz` & `tmp/scoutbook_parser-0.9.1.tar.gz`

## Comparing `scoutbook_parser-0.9.0.tar` & `scoutbook_parser-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/.git
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/__init__.py
--rw-r--r--   0        0        0  1373832 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/advancement.csv
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/advancement_types.txt
--rw-r--r--   0        0        0    21290 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/personal_data.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/requirements.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/scoutbook_parser/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/scoutbook_parser/__main__.py
--rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/scoutbook_parser/main.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/.gitignore
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/README.md
+-rw-r--r--   0        0        0  1806075 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/output.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/requirements.txt
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/scoutbook_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/scoutbook_parser/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/scoutbook_parser/__main__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/scoutbook_parser/cli.py
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/scoutbook_parser/parser.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/.gitignore
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 scoutbook_parser-0.9.1/PKG-INFO
```

### Comparing `scoutbook_parser-0.9.0/scoutbook_parser/__main__.py` & `scoutbook_parser-0.9.1/scoutbook_parser/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import click
-
-from scoutbook_parser.main import Parser
+from scoutbook_parser.parser import Parser
 
 
 @click.command()
 @click.option(
     "-t",
     "--output-type",
     default="yaml",
@@ -21,27 +20,22 @@
     "--input_personal",
     type=click.Path(exists=True, dir_okay=False),
     help="input filename for personal data (optional)",
 )
 @click.argument(
     "input_advancement",
     type=click.Path(exists=True, dir_okay=False),
-    default="advancement.csv",
 )
 def main(output_type=None, outfile=None, input_personal=None, input_advancement=None):
-    if not outfile:
+    if output_type:
+        pass
+    elif not outfile:
         output_type = "yaml"
-    else:
-        match outfile:
-            case [file, "json"]:
-                output_type = "json"
-            case [file, "yaml"]:
-                output_type = "yaml"
-            case [file, "toml"]:
-                output_type = "toml"
+    elif outfile[-4:].lower() in ('json', 'yaml', 'toml'):
+        output_type = outfile[-4:].lower()
     parser = Parser(
         input_personal=input_personal,
         input_advancement=input_advancement,
         outfile=outfile,
         file_format=output_type,
     )
```

### Comparing `scoutbook_parser-0.9.0/scoutbook_parser/main.py` & `scoutbook_parser-0.9.1/scoutbook_parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import csv
 from itertools import pairwise
-from datetime import datetime
+from datetime import datetime, date
 from pprint import pprint
 import yaml
+import json
+
+class DateTimeEncoder(json.JSONEncoder):
+    """ allows json encoder to write datetime or date items as isoformat """
+
+    def default(self, o):
+        if isinstance(o, (datetime, date)):
+            return o.isoformat()
+
+        return json.JSONEncoder.default(self, )
 
 
 def check_duplicate(iterable):
     return not len(set(iterable)) == len(iterable)
 
 
 def find_min_date(line):
@@ -53,16 +63,15 @@
 
 
 def read_personal_scout(line):
     return {
         line["BSA Member ID"]: {
             "User ID": line["UserID"],
             "BSA ID": line["BSA Member ID"],
-            "First Name": line["First Name"],
-            "Suffix": line["Suffix"],
+            "First Name": line["First Name"], "Suffix": line["Suffix"],
             "Last Name": line["Last Name"],
             "Nickname": line["Nickname"],
             "Address 1": line["Address 1"],
             "Address 2": line["Address 2"],
             "City": line["City"],
             "State": line["State"],
             "Zip": line["Zip"],
@@ -299,30 +308,31 @@
 
                 with open(self.outfile, "w") as f:
                     toml.dump(self.scouts, f)
             case "json":
                 import json
 
                 with open(self.outfile, "w") as f:
-                    json.dump(self.scouts, f)
+                    json.dump(self.scouts, f, cls=DateTimeEncoder)
 
     def dumps(self):
         match self.file_format:
             case "yaml":
                 import yaml
 
                 output_func = yaml.safe_dump
             case "toml":
                 import toml
 
                 output_func = toml.dumps
             case "json":
                 import json
 
-                output_func = json.dumps
+                return json.dumps(self.scouts, cls=DateTimeEncoder)
+
         return output_func(self.scouts)
 
 
 if __name__ == "__main__":
     parser = Parser(
         input_personal="Output_personal_data.csv",
         input_advancement="Output_advancement_data.csv",
```

### Comparing `scoutbook_parser-0.9.0/pyproject.toml` & `scoutbook_parser-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scoutbook_parser"
-version = "0.9.0"
 dependencies = [
 	"click~=8.1",
 	"pyyaml~=6.0",
 	"toml~=0.10",
 	]
+
+
+dynamic = ['version']
 	
 
 requires-python = ">3.9"
 authors = [
 	{name = "Michael Perkins", email="perkinsms@gmail.com"},
 	]
 maintainers = [
@@ -33,11 +35,13 @@
 	]
 
 
 [project.urls]
 Repository = "https://gitlab.com/troopmanager/scoutbook_parser"
 
 [project.scripts]
-sbparse-cli = "scoutbook_parser:main"
+sbparse = "scoutbook_parser:__main__.main"
 
 
 
+[tool.hatch.version]
+path = "VERSION"
```

### Comparing `scoutbook_parser-0.9.0/PKG-INFO` & `scoutbook_parser-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoutbook_parser
-Version: 0.9.0
+Version: 0.9.1
 Summary: Parse BSA Scoutbook export files into TOML, YAML, or JSON
 Project-URL: Repository, https://gitlab.com/troopmanager/scoutbook_parser
 Author-email: Michael Perkins <perkinsms@gmail.com>
 Maintainer-email: Michael Perkins <perkinsms@gmail.com>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

