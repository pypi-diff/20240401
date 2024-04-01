# Comparing `tmp/dfindexeddb-20240331a0.tar.gz` & `tmp/dfindexeddb-20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfindexeddb-20240331a0.tar", last modified: Sat Mar 30 13:51:39 2024, max compression
+gzip compressed data, was "dfindexeddb-20240402.tar", last modified: Mon Apr  1 20:21:05 2024, max compression
```

## Comparing `dfindexeddb-20240331a0.tar` & `dfindexeddb-20240402.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.491468 dfindexeddb-20240331a0/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-03-30 13:51:39.491468 dfindexeddb-20240331a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.483468 dfindexeddb-20240331a0/dfindexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb/indexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/blink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    44731 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/v8.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb/indexeddb/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/firefox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb/indexeddb/safari/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/safari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/indexeddb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb/leveldb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/ldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/leveldb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/dfindexeddb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 13:51:39.487468 dfindexeddb-20240331a0/dfindexeddb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 13:51:39.000000 dfindexeddb-20240331a0/dfindexeddb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 13:51:39.491468 dfindexeddb-20240331a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-30 13:51:34.000000 dfindexeddb-20240331a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 20:21:00.000000 dfindexeddb-20240402/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 20:21:00.000000 dfindexeddb-20240402/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-04-01 20:21:05.455962 dfindexeddb-20240402/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-01 20:21:00.000000 dfindexeddb-20240402/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.447962 dfindexeddb-20240402/dfindexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44731 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/v8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.451962 dfindexeddb-20240402/dfindexeddb/indexeddb/safari/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/safari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/indexeddb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/dfindexeddb/leveldb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/ldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-01 20:21:00.000000 dfindexeddb-20240402/dfindexeddb/leveldb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-01 20:21:01.000000 dfindexeddb-20240402/dfindexeddb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-01 20:21:01.000000 dfindexeddb-20240402/dfindexeddb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:21:05.455962 dfindexeddb-20240402/dfindexeddb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 20:21:05.000000 dfindexeddb-20240402/dfindexeddb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-01 20:21:01.000000 dfindexeddb-20240402/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:21:05.455962 dfindexeddb-20240402/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 20:21:01.000000 dfindexeddb-20240402/setup.py
```

### Comparing `dfindexeddb-20240331a0/LICENSE` & `dfindexeddb-20240402/LICENSE`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/PKG-INFO` & `dfindexeddb-20240402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240331a0
+Version: 20240402
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dfindexeddb-20240331a0/README.md` & `dfindexeddb-20240402/README.md`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/__init__.py` & `dfindexeddb-20240402/dfindexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/errors.py` & `dfindexeddb-20240402/dfindexeddb/errors.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/__init__.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/__init__.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/blink.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/blink.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/definitions.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/record.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/record.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/chromium/v8.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/chromium/v8.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/cli.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/cli.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/firefox/__init__.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/indexeddb/safari/__init__.py` & `dfindexeddb-20240402/dfindexeddb/indexeddb/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/__init__.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/cli.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
+  parser_db.set_defaults(func=DbCommand)
 
   parser_log = subparsers.add_parser(
       'log', help='Parse a leveldb log file.')
   parser_log.add_argument(
       '-s', '--source',
       required=True,
       type=pathlib.Path,
```

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/definitions.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/descriptor.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -361,22 +361,28 @@
       LevelDBVersion
     """
     active_files = defaultdict(dict)
     deleted_files = defaultdict(set)
     current_log = None
 
     for version_edit in self.GetVersionEdits():
-      current_log = f'{version_edit.log_number:06d}.log'
+      if version_edit.log_number:
+        current_log = f'{version_edit.log_number:06d}.log'
 
       for new_file in version_edit.new_files:
         active_files[new_file.level][f'{new_file.number:06d}.ldb'] = new_file
 
       for deleted_file in version_edit.deleted_files:
         active_files[deleted_file.level].pop(f'{deleted_file.number:06d}.ldb')
         deleted_files[deleted_file.level].add(f'{deleted_file.number:06d}.ldb')
 
       yield LevelDBVersion(
           current_log=current_log,
           active_files=dict(active_files),
           deleted_files=dict(deleted_files),
           version_edit_offset=version_edit.offset,
           last_sequence=version_edit.last_sequence)
+
+  def GetLatestVersion(self) -> LevelDBVersion:
+    """Returns the latest LevelDBVersion instance."""
+    *_, latest = self.GetVersions()
+    return latest
```

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/ldb.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/ldb.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/log.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/log.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/record.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/record.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/leveldb/utils.py` & `dfindexeddb-20240402/dfindexeddb/leveldb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/utils.py` & `dfindexeddb-20240402/dfindexeddb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/dfindexeddb/version.py` & `dfindexeddb-20240402/dfindexeddb/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for dfIndexeddb."""
 
-__version__ = "20240331a"
+
+__version__ = "20240402"
 
 
 def GetVersion():
   """Returns the version information."""
   return __version__
```

### Comparing `dfindexeddb-20240331a0/dfindexeddb.egg-info/PKG-INFO` & `dfindexeddb-20240402/dfindexeddb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240331a0
+Version: 20240402
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dfindexeddb-20240331a0/dfindexeddb.egg-info/SOURCES.txt` & `dfindexeddb-20240402/dfindexeddb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240331a0/pyproject.toml` & `dfindexeddb-20240402/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfindexeddb"
-version = "20240331a"
+version = "20240402"
 requires-python = ">=3.8"
 description = "dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files."
 license = {file = "LICENSE"}
 authors = [{name = "Syd Pleno", email = "sydp@google.com"}]
 maintainers = [
   {name = "dfIndexeddb Developers", email = "dfindexeddb-dev@googlegroups.com"},
 ]
```

### Comparing `dfindexeddb-20240331a0/setup.py` & `dfindexeddb-20240402/setup.py`

 * *Files identical despite different names*

