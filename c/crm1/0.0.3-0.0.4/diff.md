# Comparing `tmp/crm1-0.0.3.tar.gz` & `tmp/crm1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.3.tar", max compression
+gzip compressed data, was "crm1-0.0.4.tar", max compression
```

## Comparing `crm1-0.0.3.tar` & `crm1-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      169 2024-04-01 17:34:54.072808 crm1-0.0.3/crm1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.3/crm1/autorepotools.py
--rw-r--r--   0        0        0      116 2024-04-01 17:28:25.816110 crm1-0.0.3/crm1/data/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-01 17:35:12.466081 crm1-0.0.3/crm1/data/known_modext.py
--rw-r--r--   0        0        0      141 2024-04-01 17:35:24.455160 crm1-0.0.3/crm1/data/responses/__init__.py
--rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.3/crm1/data/responses/dependency.py
--rw-r--r--   0        0        0      938 2024-04-01 17:35:19.065640 crm1-0.0.3/crm1/data/responses/mod.py
--rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.3/crm1/data/responses/repository.py
--rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.3/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     5669 2024-04-01 19:21:07.202554 crm1-0.0.3/crm1/helpers/versions.py
--rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.3/crm1/types/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-01 17:35:06.616656 crm1-0.0.3/crm1/types/dependency.py
--rw-r--r--   0        0        0     1268 2024-04-01 17:33:24.402313 crm1-0.0.3/crm1/types/mod.py
--rw-r--r--   0        0        0     1975 2024-04-01 18:12:09.042145 crm1-0.0.3/crm1/types/repository.py
--rw-r--r--   0        0        0     2736 2024-04-01 18:12:11.019815 crm1-0.0.3/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      598 2024-04-01 18:12:31.642977 crm1-0.0.3/crm1/utils.py
--rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.3/LICENSE
--rw-r--r--   0        0        0      397 2024-04-01 19:26:35.740855 crm1-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3869 2024-04-01 19:25:44.514186 crm1-0.0.3/README.md
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 crm1-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      158 2024-04-01 19:41:03.227788 crm1-0.0.4/crm1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.4/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.4/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     6947 2024-04-01 19:42:38.977440 crm1-0.0.4/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      182 2024-04-01 19:40:39.007960 crm1-0.0.4/crm1/spec/__init__.py
+-rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.4/crm1/spec/dependency.py
+-rw-r--r--   0        0        0      938 2024-04-01 17:35:19.065640 crm1-0.0.4/crm1/spec/mod.py
+-rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.4/crm1/spec/repository.py
+-rw-r--r--   0        0        0     1748 2024-04-01 19:40:39.007960 crm1-0.0.4/crm1/spec/unsafe_modext.py
+-rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.4/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-01 19:38:40.277289 crm1-0.0.4/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1221 2024-04-01 19:41:25.588271 crm1-0.0.4/crm1/types/mod.py
+-rw-r--r--   0        0        0     1933 2024-04-01 19:41:34.284778 crm1-0.0.4/crm1/types/repository.py
+-rw-r--r--   0        0        0     2709 2024-04-01 19:42:47.392723 crm1-0.0.4/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      571 2024-04-01 19:41:18.584106 crm1-0.0.4/crm1/utils.py
+-rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.4/LICENSE
+-rw-r--r--   0        0        0      397 2024-04-01 19:44:43.372035 crm1-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3855 2024-04-01 19:43:56.788453 crm1-0.0.4/README.md
+-rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 crm1-0.0.4/PKG-INFO
```

### Comparing `crm1-0.0.3/crm1/data/known_modext.py` & `crm1-0.0.4/crm1/spec/unsafe_modext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 from typing import Optional
 
 from dataclasses_json import CatchAll, LetterCase, dataclass_json
 
-from .. import data as datacls
+from .. import spec
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
-class KnownModExt:
+class UnsafeModExt:
     """Some known mod.ext data."""
 
     icon: Optional[str] = None
     """A URL to the mod's icon."""
     modid: Optional[str] = None
     """The mod's ID. This is similar to mod.id, but does not include the group. Eg. `examplemod`."""
     loader: Optional[str] = None
@@ -30,14 +30,14 @@
     changelog: Optional[str] = None
     """A URL to the releases's changelog."""
     published_at: Optional[int] = None
     """The time the release was published at, in milliseconds since the Unix epoch."""
     alt_download: Optional[list[list[str, str]]] = None
     """A list of alternative download URLs.
     Each element is a list of two strings: the name and the URL."""
-    suggests: Optional[list[datacls.resp.RDependency]] = None
+    suggests: Optional[list[spec.RDependency]] = None
     """A list of suggested mods, that are not required
     but are recommended to be installed with this mod."""
     prerelease: Optional[bool] = None
     """Pre-release status of the mod release. If true, the mod's release is a pre-release."""
     ext: Optional[dict] = CatchAll
     """All mod.ext data that is not covered by the above fields."""
```

### Comparing `crm1-0.0.3/crm1/data/responses/mod.py` & `crm1-0.0.4/crm1/spec/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.3/crm1/data/responses/repository.py` & `crm1-0.0.4/crm1/spec/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.3/crm1/helpers/versions.py` & `crm1-0.0.4/crm1/helpers/versions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,52 @@
+"""A module for handling versions."""
+
 from dataclasses import dataclass
-from typing import Optional
 from enum import Enum
+from typing import Optional
 
 
 class VersionEndMode(Enum):
+    """The mode of the end of a version range. This can be inclusive or exclusive."""
+
     INCLUSIVE = "inclusive"
     EXCLUSIVE = "exclusive"
 
 
 DONTCARE = VersionEndMode.EXCLUSIVE
+"""This is used to represent the end of a version range which's version is not specified."""
 
 
 @dataclass
 class Version:
+    """A version."""
+
     major: int
+    """The major version."""
     minor: int
+    """The minor version."""
     patch: int
+    """The patch version."""
 
     @staticmethod
     def from_string(version: str) -> "Version":
+        """Create a Version object from a string.
+        The string should be in the format of `major.minor.patch`."""
         parts = version.split(".")
         if len(parts) < 2:
             raise ValueError("Invalid version string")
         if len(parts) > 3:
             raise ValueError("Invalid version string")
         major = int(parts[0])
         minor = int(parts[1])
         patch = int(parts[2]) if len(parts) == 3 else 0
         return Version(major, minor, patch)
 
     def to_string(self) -> str:
+        """Convert the version to a string in the format of `major.minor.patch`."""
         return f"{self.major}.{self.minor}" + (
             f".{self.patch}" if self.patch is not None else ""
         )
 
     def __eq__(self, other: "Version") -> bool:
         return (
             self.major == other.major
@@ -74,25 +87,37 @@
 
     def __str__(self) -> str:
         return self.to_string()
 
 
 @dataclass
 class VersionRange:
+    """A range of versions."""
+
     lower: Optional[Version]
+    """The lower bound of the range."""
     lower_mode: VersionEndMode
+    """The mode of the lower bound of the range."""
     upper: Optional[Version]
+    """The upper bound of the range."""
     upper_mode: VersionEndMode
-    
+    """The mode of the upper bound of the range."""
+
     def __post_init__(self):
-        if self.lower is not None and self.upper is not None and self.lower > self.upper:
+        if (
+            self.lower is not None
+            and self.upper is not None
+            and self.lower > self.upper
+        ):
             raise ValueError("Invalid range")
 
     @staticmethod
     def from_string(range_: str) -> "VersionRange":
+        """Create a VersionRange object from a string.
+        The string should be in the format of `[lower,upper]`. Examples: `[1.0,2.0.1)`, `(1.0,]`."""
         if range_.startswith("["):
             lower_mode = VersionEndMode.INCLUSIVE
         elif range_.startswith("("):
             lower_mode = VersionEndMode.EXCLUSIVE
         else:
             raise ValueError("Invalid range string")
         if range_.endswith("]"):
@@ -106,25 +131,32 @@
         if len(parts) != 2:
             raise ValueError("Invalid range string")
         lower = Version.from_string(parts[0]) if parts[0] else None
         upper = Version.from_string(parts[1]) if parts[1] else None
         return VersionRange(lower, lower_mode, upper, upper_mode)
 
     def to_string(self) -> str:
-        if self.lower is not None and self.upper is not None and self.lower == self.upper:
+        """Convert the version range to a string in the format of `[lower,upper]`.
+        Examples: `[1.0,2.0.1)`, `(1.0,]`."""
+        if (
+            self.lower is not None
+            and self.upper is not None
+            and self.lower == self.upper
+        ):
             return self.lower.to_string()
         return (
             ("[" if self.lower_mode == VersionEndMode.INCLUSIVE else "(")
             + (self.lower.to_string() if self.lower else "")
             + ","
             + (self.upper.to_string() if self.upper else "")
             + ("]" if self.upper_mode == VersionEndMode.INCLUSIVE else ")")
         )
 
     def contains(self, version: Version) -> bool:
+        """Check if the version is in the range."""
         if self.lower is not None:
             if self.lower_mode == VersionEndMode.INCLUSIVE:
                 if version < self.lower:
                     return False
             else:
                 if version <= self.lower:
                     return False
@@ -141,14 +173,15 @@
         return self.contains(version)
 
     def __str__(self) -> str:
         return self.to_string()
 
 
 def range_from_maven_string(version: str):
+    """Create a VersionRange object from a Maven version string."""
     if version.startswith(">="):
         lower_mode = VersionEndMode.INCLUSIVE
         lower = Version.from_string(version[2:])
         upper = None
         upper_mode = DONTCARE
     elif version.startswith(">"):
         lower_mode = VersionEndMode.EXCLUSIVE
```

### Comparing `crm1-0.0.3/crm1/types/dependency.py` & `crm1-0.0.4/crm1/types/dependency.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Don't import this module directly."""
 
 from typing import TYPE_CHECKING, Optional, overload
 
-from .. import data as datacls
+from .. import spec
 
 if TYPE_CHECKING:
     from .mod import Mod
     from .repository import Repository
     from .repository_pool import RepositoryPool
 
 
@@ -17,15 +17,15 @@
     """The ID of the mod."""
     version: str
     """The version of the mod."""
     source: Optional[str]
     """The repository rootId of the mod."""
     mod: Optional["Mod"] = None
 
-    def __init__(self, meta: datacls.resp.RDependency):
+    def __init__(self, meta: spec.RDependency):
         self.id = meta.id
         self.version = meta.version
         self.source = meta.source
         self.mod = None
 
     @overload
     def resolve(self, pool: "RepositoryPool") -> "Mod":
```

### Comparing `crm1-0.0.3/crm1/types/repository.py` & `crm1-0.0.4/crm1/types/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Don't import this module directly."""
 
 from typing import Optional, overload
 
-from .. import data as datacls
 from .. import utils
 from .mod import Mod
+from .. import spec
 
 
 class Repository:
     """A repository."""
 
     address: Optional[str]
     """The address of the repository."""
-    data: datacls.resp.RRepository
+    data: spec.RRepository
     """The raw data of the repository."""
 
     @overload
-    def __init__(self, address: Optional[str], data: datacls.resp.RRepository):
+    def __init__(self, address: Optional[str], data: spec.RRepository):
         """Initializes a repository with an address and data."""
 
     @overload
     def __init__(self, address: str):
         """Initializes a repository with an address. The data will be fetched."""
 
     @overload
     def __init__(self, address: Optional[str], data: dict):
-        """Initializes a repository with an address and data. The data will be converted to a datacls.resp.RRepository."""
+        """Initializes a repository with an address and data.
+        The data will be converted to a spec.RRepository."""
 
     def __init__(self, address, data=None):
         if isinstance(data, dict):
-            data = datacls.resp.RRepository.from_dict(address)
+            data = spec.RRepository.from_dict(address)
         self.address = address
         self.data = data
         if data is None:
             self.update()
-        if not isinstance(self.data, datacls.resp.RRepository):
+        if not isinstance(self.data, spec.RRepository):
             raise ValueError("Invalid data type")
         if self.data.spec_version != 1:
             raise ValueError("Unsupported spec version", self.data.spec_version)
 
     def get_mod(self, id_: str) -> Optional[Mod]:
         """Gets a mod by its ID."""
         for mod in self.data.mods:
```

### Comparing `crm1-0.0.3/crm1/types/repository_pool.py` & `crm1-0.0.4/crm1/types/repository_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Don't import this module directly."""
 
 from typing import Optional, overload
 
-from .. import data as datacls
+from .. import spec
 from .mod import Mod
 from .repository import Repository
 
 
 class RepositoryPool:
     """A pool of repositories."""
 
@@ -17,26 +17,26 @@
         self.repositories = {}
 
     @overload
     def add_repository(self, address: str):
         """Adds a repository to the pool by providing the address."""
 
     @overload
-    def add_repository(self, repo: datacls.resp.RRepository):
+    def add_repository(self, repo: spec.RRepository):
         """Adds a repository to the pool that has already been fetched."""
 
     @overload
     def add_repository(self, repo: Repository):
         """Adds a repository to the pool."""
 
     def add_repository(self, repo):
         """Above"""
         if isinstance(repo, str):
             repo = Repository(repo)
-        if isinstance(repo, datacls.resp.RRepository):
+        if isinstance(repo, spec.RRepository):
             repo = Repository(None, repo)
         self.repositories[repo.root_id] = repo
 
     def get_repository(self, root_id: str) -> Repository:
         """Gets a repository by its root ID."""
         return self.repositories[root_id]
```

### Comparing `crm1-0.0.3/crm1/utils.py` & `crm1-0.0.4/crm1/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Don't import this module directly."""
 
 from functools import lru_cache
 
 import hjson
 import requests
 
-from . import data as datacls
+from . import spec
 
 
 @lru_cache(maxsize=128)
 def get_request(address: str) -> dict:
     """Performs a GET request to the given address and returns the HJSON response."""
     response = requests.get(address, timeout=5)
     return hjson.loads(response.text)
 
 
-def fetch_repository(address: str) -> datacls.resp.RRepository:
+def fetch_repository(address: str) -> spec.RRepository:
     """Fetches a repository from the given address."""
     data = get_request(address)
-    return datacls.resp.RRepository.from_dict(data)
+    return spec.RRepository.from_dict(data)
```

### Comparing `crm1-0.0.3/LICENSE` & `crm1-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.3/README.md` & `crm1-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ```
 
 Everything is typed and documented, so you can use your IDE's autocomplete and documentation features to explore the functionality of the package.
 
 ## Helpers
 
-### ```helpers.versions```
+### Versions
 
 The ```helpers.versions``` module provides classes to work with versions and version ranges.
 
 ```python
 from crm1.helpers.versions import Version, VersionRange, range_from_maven_string
```

### Comparing `crm1-0.0.3/PKG-INFO` & `crm1-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.3
+Version: 0.0.4
 Summary: A CRM-1 repository exploration package
 License: MIT
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -74,15 +74,15 @@
 
 ```
 
 Everything is typed and documented, so you can use your IDE's autocomplete and documentation features to explore the functionality of the package.
 
 ## Helpers
 
-### ```helpers.versions```
+### Versions
 
 The ```helpers.versions``` module provides classes to work with versions and version ranges.
 
 ```python
 from crm1.helpers.versions import Version, VersionRange, range_from_maven_string
```

