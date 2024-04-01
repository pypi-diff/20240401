# Comparing `tmp/crm1-0.0.4.tar.gz` & `tmp/crm1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.4.tar", max compression
+gzip compressed data, was "crm1-0.0.5.tar", max compression
```

## Comparing `crm1-0.0.4.tar` & `crm1-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      158 2024-04-01 19:41:03.227788 crm1-0.0.4/crm1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.4/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.4/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     6947 2024-04-01 19:42:38.977440 crm1-0.0.4/crm1/helpers/versions.py
--rw-r--r--   0        0        0      182 2024-04-01 19:40:39.007960 crm1-0.0.4/crm1/spec/__init__.py
--rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.4/crm1/spec/dependency.py
--rw-r--r--   0        0        0      938 2024-04-01 17:35:19.065640 crm1-0.0.4/crm1/spec/mod.py
--rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.4/crm1/spec/repository.py
--rw-r--r--   0        0        0     1748 2024-04-01 19:40:39.007960 crm1-0.0.4/crm1/spec/unsafe_modext.py
--rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.4/crm1/types/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-01 19:38:40.277289 crm1-0.0.4/crm1/types/dependency.py
--rw-r--r--   0        0        0     1221 2024-04-01 19:41:25.588271 crm1-0.0.4/crm1/types/mod.py
--rw-r--r--   0        0        0     1933 2024-04-01 19:41:34.284778 crm1-0.0.4/crm1/types/repository.py
--rw-r--r--   0        0        0     2709 2024-04-01 19:42:47.392723 crm1-0.0.4/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      571 2024-04-01 19:41:18.584106 crm1-0.0.4/crm1/utils.py
--rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.4/LICENSE
--rw-r--r--   0        0        0      397 2024-04-01 19:44:43.372035 crm1-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3855 2024-04-01 19:43:56.788453 crm1-0.0.4/README.md
--rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 crm1-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      158 2024-04-01 19:41:03.227788 crm1-0.0.5/crm1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.5/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.5/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     6947 2024-04-01 19:42:38.977440 crm1-0.0.5/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      182 2024-04-01 19:40:39.007960 crm1-0.0.5/crm1/spec/__init__.py
+-rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.5/crm1/spec/dependency.py
+-rw-r--r--   0        0        0      978 2024-04-01 20:26:21.932441 crm1-0.0.5/crm1/spec/mod.py
+-rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.5/crm1/spec/repository.py
+-rw-r--r--   0        0        0     1692 2024-04-01 20:21:17.411767 crm1-0.0.5/crm1/spec/unsafe_modext.py
+-rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.5/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-01 19:38:40.277289 crm1-0.0.5/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1221 2024-04-01 19:41:25.588271 crm1-0.0.5/crm1/types/mod.py
+-rw-r--r--   0        0        0     1933 2024-04-01 19:41:34.284778 crm1-0.0.5/crm1/types/repository.py
+-rw-r--r--   0        0        0     2709 2024-04-01 19:42:47.392723 crm1-0.0.5/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      595 2024-04-01 20:25:30.948258 crm1-0.0.5/crm1/utils.py
+-rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.5/LICENSE
+-rw-r--r--   0        0        0      397 2024-04-01 19:57:15.478309 crm1-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3855 2024-04-01 19:43:56.788453 crm1-0.0.5/README.md
+-rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 crm1-0.0.5/PKG-INFO
```

### Comparing `crm1-0.0.4/crm1/helpers/versions.py` & `crm1-0.0.5/crm1/helpers/versions.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/spec/mod.py` & `crm1-0.0.5/crm1/spec/mod.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 
 from dataclasses_json import LetterCase, dataclass_json
 
 from .dependency import RDependency
+from .unsafe_modext import UnsafeModExt
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class RMod:
     """Raw mod data. This is used for deserialization."""
 
@@ -24,9 +25,9 @@
     """The version of the mod."""
     game_version: str
     """The version of the game that the mod is compatible with."""
     url: str
     """The download URL of the mod's jar."""
     deps: list[RDependency]
     """A list of dependencies of the mod."""
-    ext: dict
-    """A dictionary of optional extra information about the mod."""
+    ext: dict | UnsafeModExt
+    """Some optional additional info of the mod."""
```

### Comparing `crm1-0.0.4/crm1/spec/repository.py` & `crm1-0.0.5/crm1/spec/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/spec/unsafe_modext.py` & `crm1-0.0.5/crm1/spec/unsafe_modext.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,13 @@
     changelog: Optional[str] = None
     """A URL to the releases's changelog."""
     published_at: Optional[int] = None
     """The time the release was published at, in milliseconds since the Unix epoch."""
     alt_download: Optional[list[list[str, str]]] = None
     """A list of alternative download URLs.
     Each element is a list of two strings: the name and the URL."""
+    alt_versions: Optional[list["RMod"]] = None
     suggests: Optional[list[spec.RDependency]] = None
     """A list of suggested mods, that are not required
     but are recommended to be installed with this mod."""
     prerelease: Optional[bool] = None
     """Pre-release status of the mod release. If true, the mod's release is a pre-release."""
-    ext: Optional[dict] = CatchAll
-    """All mod.ext data that is not covered by the above fields."""
```

### Comparing `crm1-0.0.4/crm1/types/dependency.py` & `crm1-0.0.5/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/types/mod.py` & `crm1-0.0.5/crm1/types/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/types/repository.py` & `crm1-0.0.5/crm1/types/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/types/repository_pool.py` & `crm1-0.0.5/crm1/types/repository_pool.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/crm1/utils.py` & `crm1-0.0.5/crm1/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 from . import spec
 
 
 @lru_cache(maxsize=128)
 def get_request(address: str) -> dict:
     """Performs a GET request to the given address and returns the HJSON response."""
     response = requests.get(address, timeout=5)
-    return hjson.loads(response.text)
+    return hjson.loads(response.text, object_pairs_hook=dict)
 
 
 def fetch_repository(address: str) -> spec.RRepository:
     """Fetches a repository from the given address."""
     data = get_request(address)
     return spec.RRepository.from_dict(data)
```

### Comparing `crm1-0.0.4/LICENSE` & `crm1-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/README.md` & `crm1-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.0.4/PKG-INFO` & `crm1-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CRM-1 repository exploration package
 License: MIT
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

