# Comparing `tmp/sentinelc-appfeed-3.0.1.tar.gz` & `tmp/sentinelc-appfeed-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinelc-appfeed-3.0.1.tar", last modified: Thu Mar 28 20:48:41 2024, max compression
+gzip compressed data, was "sentinelc-appfeed-3.0.2.tar", last modified: Mon Apr  1 21:35:49 2024, max compression
```

## Comparing `sentinelc-appfeed-3.0.1.tar` & `sentinelc-appfeed-3.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 20:48:41.146476 sentinelc-appfeed-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17558 2024-03-28 20:48:41.145475 sentinelc-appfeed-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17176 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 20:48:41.141476 sentinelc-appfeed-3.0.1/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/scripts/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 20:48:41.141476 sentinelc-appfeed-3.0.1/sentinelc_appfeed/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 20:48:41.145475 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/ArgparseCustomTypes.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/jinja.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     2418 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/safe_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    16406 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 20:48:41.145475 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17558 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      676 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-28 20:48:41.000000 sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 20:48:41.146476 sentinelc-appfeed-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-03-28 20:48:31.000000 sentinelc-appfeed-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:49.863069 sentinelc-appfeed-3.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      612 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-01 21:35:49.863069 sentinelc-appfeed-3.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17176 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:49.859069 sentinelc-appfeed-3.0.2/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/scripts/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:49.859069 sentinelc-appfeed-3.0.2/sentinelc_appfeed/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:49.862069 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/ArgparseCustomTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/jinja.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/safe_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16578 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:35:49.862069 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-01 21:35:49.000000 sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 21:35:49.863069 sentinelc-appfeed-3.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-01 21:35:40.000000 sentinelc-appfeed-3.0.2/setup.py
```

### Comparing `sentinelc-appfeed-3.0.1/LICENSE.txt` & `sentinelc-appfeed-3.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/PKG-INFO` & `sentinelc-appfeed-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinelc-appfeed
-Version: 3.0.1
+Version: 3.0.2
 Summary: Tools used to validate, create and publish an app libary feed for the SentinelC platform.
 Home-page: https://gitlab.com/sentinelc/app-library-builder
 Maintainer: SentinelC
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: PyYAML
 Requires-Dist: humanfriendly
```

### Comparing `sentinelc-appfeed-3.0.1/README.md` & `sentinelc-appfeed-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/scripts/upload.py` & `sentinelc-appfeed-3.0.2/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed/builder.py` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed/builder.py`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/safe_yaml.py` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/safe_yaml.py`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed/utils/utils.py` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed/validator.py` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,31 +66,34 @@
     "textarea",
 }
 
 accepted_archs = ["amd64", "arm64"]
 
 requirement_defaults = {"storage": None, "memory": None}
 
-version_regexp = r"([a-z0-9\.\-]+?)(-r([0-9]+))?$"
+app_name_regexp = r"^[a-z0-9]+(?:-[a-z0-9]+)*$"
+
+version_regexp = r"(^[a-z0-9\.\-]+?)(-r([0-9]+))?$"
 
 logo_formats = dict(jpg="image/jpeg", webp="image/webp", png="image/png")
 
 expose_port_regexp = r"^([\d]+)/(tcp|udp)$"
 
 
 def is_valid_port_number(port_number):
     return type(port_number) is int and port_number > 0 and port_number <= 65535
 
 
 def validate_version(version_string):
-    if not re.search(version_regexp, version_string):
-        raise ValidationError(
-            "Version name is invalid. It must be alphanumeric, and can include dashes and dots."
-        )
-    return True
+    return re.search(version_regexp, version_string)
+
+
+def validate_app_name(app_name):
+    # lowercase a-z, 0-9 and dashes allowed. Cannot start or end with a dash.
+    return re.search(app_name_regexp, app_name)
 
 
 def get_last_commit_timestamp(filename):
     timestamp = os.popen(f"git log --format=%ct {filename}").read()
     timestamp = timestamp[:-1]
     return timestamp_to_json_string(timestamp.split("\n")[-1])
 
@@ -164,16 +167,15 @@
     bail_on_shallow_git_repos()
     path = f"{manifest_path}/{app_name}"
 
     # Validate App Name
     # app_name = path.split("/")[-1]
     eprint(f"- Validating {app_name}")
 
-    match = re.search(r"(^[a-z0-9\-]+$)", app_name)
-    if not match:
+    if not validate_app_name(app_name):
         raise ValidationError(f"Invalid app name: {app_name}")
 
     # Get App Infos
     app_files = get_localized_objects_yaml(path, app_name, "description file")
 
     if app_files["en"] is None:
         raise ValidationError(
@@ -217,15 +219,18 @@
                 eprint(f"  - Mandatory field '{field}' is missing")
 
     # Return object if valid
     if not has_mandatory_fields:
         raise ValidationError("Missing mandatory field(s)")
 
     # validate version
-    validate_version(app["version"])
+    if not validate_version(app["version"]):
+        raise ValidationError(
+            "Version name is invalid. It must be alphanumeric, and can include dashes and dots."
+        )
 
     # Optional fields - will be filled with nulls
     for field in description_defaults:
         if field not in app:
             app[field] = description_defaults[field]
 
     # variables translations
```

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/PKG-INFO` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinelc-appfeed
-Version: 3.0.1
+Version: 3.0.2
 Summary: Tools used to validate, create and publish an app libary feed for the SentinelC platform.
 Home-page: https://gitlab.com/sentinelc/app-library-builder
 Maintainer: SentinelC
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: PyYAML
 Requires-Dist: humanfriendly
```

### Comparing `sentinelc-appfeed-3.0.1/sentinelc_appfeed.egg-info/SOURCES.txt` & `sentinelc-appfeed-3.0.2/sentinelc_appfeed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentinelc-appfeed-3.0.1/setup.py` & `sentinelc-appfeed-3.0.2/setup.py`

 * *Files identical despite different names*

