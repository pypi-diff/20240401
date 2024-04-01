# Comparing `tmp/unihan_db-0.8.0.tar.gz` & `tmp/unihan_db-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unihan_db-0.8.0.tar", max compression
+gzip compressed data, was "unihan_db-0.9.0.tar", max compression
```

## Comparing `unihan_db-0.8.0.tar` & `unihan_db-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1094 2023-05-29 17:46:49.608802 unihan_db-0.8.0/LICENSE
--rw-r--r--   0        0        0     3337 2023-05-29 17:46:49.608802 unihan_db-0.8.0/README.md
--rw-r--r--   0        0        0     3045 2023-05-29 17:46:49.608802 unihan_db-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      496 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/__about__.py
--rw-r--r--   0        0        0      219 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/__init__.py
--rw-r--r--   0        0        0     6394 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/bootstrap.py
--rw-r--r--   0        0        0     8418 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/importer.py
--rw-r--r--   0        0        0    13498 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/tables.py
--rw-r--r--   0        0        0     1752 2023-05-29 17:46:49.608802 unihan_db-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0    13881 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryIndices.txt
--rw-r--r--   0        0        0    11472 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryLikeData.txt
--rw-r--r--   0        0        0    13661 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_IRGSources.txt
--rw-r--r--   0        0        0     2419 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_NumericValues.txt
--rw-r--r--   0        0        0     9456 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_OtherMappings.txt
--rw-r--r--   0        0        0    17767 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt
--rw-r--r--   0        0        0    21631 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_Readings.txt
--rw-r--r--   0        0        0    19028 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_Variants.txt
--rw-r--r--   0        0        0      820 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/test_bootstrap.py
--rw-r--r--   0        0        0     4916 1970-01-01 00:00:00.000000 unihan_db-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-10 11:45:01.838666 unihan_db-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3374 2023-06-10 11:45:01.838666 unihan_db-0.9.0/README.md
+-rw-r--r--   0        0        0     2959 2023-06-10 11:45:01.838666 unihan_db-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2023-06-10 11:45:01.838666 unihan_db-0.9.0/src/unihan_db/__about__.py
+-rw-r--r--   0        0        0      219 2023-06-10 11:45:01.838666 unihan_db-0.9.0/src/unihan_db/__init__.py
+-rw-r--r--   0        0        0     7290 2023-06-10 11:45:01.838666 unihan_db-0.9.0/src/unihan_db/bootstrap.py
+-rw-r--r--   0        0        0    11894 2023-06-10 11:45:01.838666 unihan_db-0.9.0/src/unihan_db/importer.py
+-rw-r--r--   0        0        0    13472 2023-06-10 11:45:01.838666 unihan_db-0.9.0/src/unihan_db/tables.py
+-rw-r--r--   0        0        0     2185 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    13881 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/fixtures/Unihan_DictionaryIndices.txt
+-rw-r--r--   0        0        0    11472 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/fixtures/Unihan_DictionaryLikeData.txt
+-rw-r--r--   0        0        0    13661 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/fixtures/Unihan_IRGSources.txt
+-rw-r--r--   0        0        0     2419 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/fixtures/Unihan_NumericValues.txt
+-rw-r--r--   0        0        0     9456 2023-06-10 11:45:01.838666 unihan_db-0.9.0/tests/fixtures/Unihan_OtherMappings.txt
+-rw-r--r--   0        0        0    17767 2023-06-10 11:45:01.842666 unihan_db-0.9.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt
+-rw-r--r--   0        0        0    21631 2023-06-10 11:45:01.842666 unihan_db-0.9.0/tests/fixtures/Unihan_Readings.txt
+-rw-r--r--   0        0        0    19028 2023-06-10 11:45:01.842666 unihan_db-0.9.0/tests/fixtures/Unihan_Variants.txt
+-rw-r--r--   0        0        0     1194 2023-06-10 11:45:01.842666 unihan_db-0.9.0/tests/test_bootstrap.py
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 unihan_db-0.9.0/PKG-INFO
```

### Comparing `unihan_db-0.8.0/LICENSE` & `unihan_db-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/README.md` & `unihan_db-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,15 @@
 $ cd unihan-etl
 ```
 
 [Bootstrap your environment and learn more about contributing](https://cihai.git-pull.com/contributing/). We use the same conventions / tools across all cihai projects: `pytest`, `sphinx`, `flake8`, `mypy`, `black`, `isort`, `tmuxp`, and file watcher helpers (e.g. `entr(1)`).
 
 ## Python versions
 
-- 0.8.0: Last Python 3.7 release
+- 0.8.0: 
+  - Last Python 3.7 release
+  - Last SQLAlchemy 1.3 release
 
 ## More information
 
 [![Docs](https://github.com/cihai/unihan-db/workflows/docs/badge.svg)](https://unihan-db.git-pull.com/)
 [![Build Status](https://github.com/cihai/unihan-db/workflows/tests/badge.svg)](https://github.com/cihai/unihan-db/actions?query=workflow%3A%22tests%22)
```

### Comparing `unihan_db-0.8.0/pyproject.toml` & `unihan_db-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "unihan_db"
-version = "0.8.0"
+version = "0.9.0"
 description = "SQLAlchemy models for UNIHAN CJK database"
 license = "MIT"
 authors = ["Tony Narlock <tony@git-pull.com>"]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 2 - Pre-Alpha",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Database",
   "Topic :: Software Development :: Internationalization",
   "Topic :: Software Development :: Localization",
   "Topic :: Utilities",
 ]
 keywords = [
@@ -44,27 +44,27 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cihai/unihan-db/issues"
 Documentation = "https://unihan-db.git-pull.com"
 Repository = "https://github.com/cihai/unihan-db"
 "Release notes" = "https://github.com/cihai/unihan-db/blob/master/CHANGES"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 appdirs = "*"
-SQLAlchemy = "<2"
+SQLAlchemy = ">=2"
 unihan-etl = "~=0.19.1"
 
 [tool.poetry.group.dev.dependencies]
 ### Docs ###
 sphinx = "*"
 furo = "*"
 gp-libs = "*"
 sphinx-autobuild = "*"
 sphinx-autodoc-typehints = "*"
-sphinx-inline-tabs = "<2023.4.21"  # For Python 3.7 support
+sphinx-inline-tabs = "*"
 sphinxext-opengraph = "<0.8"  # https://github.com/wpilibsuite/sphinxext-opengraph/issues/100
 sphinx-copybutton = "*"
 sphinxext-rediraffe = "*"
 myst_parser = ">=0.18.1"
 docutils = "*"
 
 ### Testing ###
@@ -77,15 +77,14 @@
 coverage = "*"
 pytest-cov = "*"
 
 ### Lint ###
 black = "*"
 ruff = "*"
 mypy = "*"
-sqlalchemy-stubs = "*"
 types-appdirs = "*"
 
 [tool.poetry.extras]
 docs = [
   "docutils",
   "sphinx",
   "sphinx-autodoc-typehints",
@@ -100,22 +99,19 @@
 ]
 test = ["pytest", "pytest-rerunfailures", "pytest-watcher"]
 coverage = ["codecov", "coverage", "pytest-cov"]
 lint = [
   "black",
   "ruff",
   "mypy",
-  "sqlalchemy-stubs",
   "types-appdirs",
 ]
 
 [tool.mypy]
-plugins = [
-  "sqlmypy",
-]
+strict = true
 files = [
   "src/",
   "tests/",
 ]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `unihan_db-0.8.0/src/unihan_db/bootstrap.py` & `unihan_db-0.9.0/src/unihan_db/bootstrap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import logging
 import sys
 from datetime import datetime
-
+import typing as t
 from sqlalchemy import create_engine, event
-from sqlalchemy.orm import class_mapper, mapper, scoped_session, sessionmaker
-
+import sqlalchemy
+from sqlalchemy.orm import Session, class_mapper, scoped_session, sessionmaker
+from sqlalchemy.orm.decl_api import registry
+from sqlalchemy.orm.scoping import ScopedSession
 from unihan_etl import process as unihan
+from unihan_etl.types import UntypedUnihanData
 from unihan_etl.util import merge_dict
 
 from . import dirs, importer
 from .tables import Base, Unhn
 
 log = logging.getLogger(__name__)
 
+mapper_reg = registry()
+
+if t.TYPE_CHECKING:
+    from unihan_etl.types import (
+        UntypedNormalizedData,
+    )
 
-def setup_logger(logger=None, level="INFO"):
+
+def setup_logger(
+    logger: t.Optional[logging.Logger] = None,
+    level: t.Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = "INFO",
+) -> None:
     """
     Setup logging for CLI use.
 
     Parameters
     ----------
     logger : :py:class:`logging.Logger`
         instance of logger
@@ -115,53 +128,60 @@
 
 TABLE_NAME = "Unihan"
 
 
 DEFAULT_FIELDS = ["ucn", "char"]
 
 
-def is_bootstrapped(metadata):
+def is_bootstrapped(metadata: sqlalchemy.MetaData) -> bool:
     """Return True if cihai is correctly bootstrapped."""
     fields = UNIHAN_FIELDS + DEFAULT_FIELDS
     if TABLE_NAME in metadata.tables.keys():
         table = metadata.tables[TABLE_NAME]
 
         if set(fields) == {c.name for c in table.columns}:
             return True
         else:
             return False
     else:
         return False
 
 
-def bootstrap_data(options=None):
+def bootstrap_data(
+    options: t.Union[UntypedUnihanData, None] = None,
+) -> t.Optional["UntypedNormalizedData"]:
     if options is None:
         options = {}
+    _options = options
 
-    options = merge_dict(UNIHAN_ETL_DEFAULT_OPTIONS.copy(), options)
+    _options = merge_dict(UNIHAN_ETL_DEFAULT_OPTIONS.copy(), _options)
 
-    p = unihan.Packager(options)
+    p = unihan.Packager(_options)
     p.download()
     return p.export()
 
 
-def bootstrap_unihan(session, options=None):
-    if options is None:
-        options = {}
+def bootstrap_unihan(
+    session: t.Union[Session, ScopedSession[t.Any]],
+    options: t.Optional[UntypedUnihanData] = None,
+) -> None:
+    _options = options if options is not None else {}
 
     """Download, extract and import unihan to database."""
     if session.query(Unhn).count() == 0:
-        data = bootstrap_data(options)
+        data = bootstrap_data(_options)
+        assert data is not None
         log.info("bootstrap Unhn table")
         log.info("bootstrap Unhn table finished")
         count = 0
         total_count = len(data)
         items = []
 
         for char in data:
+            assert isinstance(char, dict)
             c = Unhn(char=char["char"], ucn=char["ucn"])
             importer.import_char(c, char)
             items.append(c)
 
             if log.isEnabledFor(logging.INFO):
                 count += 1
                 sys.stdout.write(
@@ -173,15 +193,15 @@
         session.add_all(items)
         # This takes a bit of time and doesn't provide progress, but it's by
         # far the fastest way to insert as of SQLAlchemy 1.11.
         session.commit()
         log.info("Done adding rows.")
 
 
-def to_dict(obj, found=None):
+def to_dict(obj: t.Any, found: t.Optional[t.Set[t.Any]] = None) -> t.Dict[str, object]:
     """
     Return dictionary of an SQLAlchemy Query result.
 
     Supports recursive relationships.
 
     Parameters
     ----------
@@ -192,52 +212,59 @@
 
     Returns
     -------
     dict :
         dictionary representation of a SQLAlchemy query
     """
 
-    def _get_key_value(c):
+    def _get_key_value(c: str) -> t.Any:
         if isinstance(getattr(obj, c), datetime):
             return (c, getattr(obj, c).isoformat())
         else:
             return (c, getattr(obj, c))
 
+    _found: t.Set[t.Any]
+
     if found is None:
-        found = set()
-    mapper = class_mapper(obj.__class__)
-    columns = [column.key for column in mapper.columns]
+        _found = set()
+    else:
+        _found = found
+
+    _mapper = class_mapper(obj.__class__)
+    columns = [column.key for column in _mapper.columns]
 
     result = dict(map(_get_key_value, columns))
-    for name, relation in mapper.relationships.items():
-        if relation not in found:
-            found.add(relation)
+    for name, relation in _mapper.relationships.items():
+        if relation not in _found:
+            _found.add(relation)
             related_obj = getattr(obj, name)
             if related_obj is not None:
                 if relation.uselist:
                     result[name] = [to_dict(child, found) for child in related_obj]
                 else:
                     result[name] = to_dict(related_obj, found)
     return result
 
 
-def add_to_dict(b):
+def add_to_dict(b: t.Any) -> t.Any:
     """
     Add :func:`.to_dict` method to SQLAlchemy Base object.
 
     Parameters
     ----------
     b : :func:`~sqlalchemy:sqlalchemy.ext.declarative.declarative_base`
         SQLAlchemy Base class
     """
     b.to_dict = to_dict
     return b
 
 
-def get_session(engine_url="sqlite:///{user_data_dir}/unihan_db.db"):
+def get_session(
+    engine_url: str = "sqlite:///{user_data_dir}/unihan_db.db",
+) -> "ScopedSession[t.Any]":
     """
     Return new SQLAlchemy session object from engine string.
 
     *engine_url* accepts a string template variable for ``{user_data_dir}``,
     which is replaced to the XDG data directory for the user running the script
     process. This variable is only useful for SQLite, where file paths are
     used for the engine_url.
@@ -247,14 +274,13 @@
     engine_url : str
         SQLAlchemy engine string
     """
 
     engine_url = engine_url.format(**{"user_data_dir": dirs.user_data_dir})
     engine = create_engine(engine_url)
 
-    event.listen(mapper, "after_configured", add_to_dict(Base))
-    Base.metadata.bind = engine
-    Base.metadata.create_all()
+    event.listen(mapper_reg, "after_configured", add_to_dict(Base))
+    Base.metadata.create_all(bind=engine)
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
 
     return session
```

### Comparing `unihan_db-0.8.0/src/unihan_db/tables.py` & `unihan_db-0.9.0/src/unihan_db/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 values branched off into field-specialized tables through `polymorphic
 joins`_.
 
 .. _polymorphic joins: https://en.wikipedia.org/wiki/Polymorphic_association
 
 """
 from sqlalchemy import Boolean, Column, ForeignKey, Integer, String
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import DeclarativeBase, relationship
 
-Base = declarative_base()
+
+class Base(DeclarativeBase):
+    pass
 
 
 class Unhn(Base):
     __tablename__ = "Unhn"
     char = Column(String(1), primary_key=True, index=True, unique=True)
     ucn = Column(String(8), index=True, unique=True)
```

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryIndices.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_DictionaryIndices.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryLikeData.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_DictionaryLikeData.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_IRGSources.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_IRGSources.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_NumericValues.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_NumericValues.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_OtherMappings.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_OtherMappings.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_Readings.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_Readings.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/tests/fixtures/Unihan_Variants.txt` & `unihan_db-0.9.0/tests/fixtures/Unihan_Variants.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.8.0/PKG-INFO` & `unihan_db-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: unihan-db
-Version: 0.8.0
+Version: 0.9.0
 Summary: SQLAlchemy models for UNIHAN CJK database
 Home-page: https://unihan-db.git-pull.com
 License: MIT
 Keywords: unihan,sqlalchemy,cjk,chinese,japanese,sql,database
 Author: Tony Narlock
 Author-email: tony@git-pull.com
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Utilities
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
-Requires-Dist: SQLAlchemy (<2)
+Requires-Dist: SQLAlchemy (>=2)
 Requires-Dist: appdirs
 Requires-Dist: unihan-etl (>=0.19.1,<0.20.0)
 Project-URL: Bug Tracker, https://github.com/cihai/unihan-db/issues
 Project-URL: Documentation, https://unihan-db.git-pull.com
 Project-URL: Repository, https://github.com/cihai/unihan-db
 Project-URL: Release notes, https://github.com/cihai/unihan-db/blob/master/CHANGES
 Description-Content-Type: text/markdown
@@ -120,14 +119,16 @@
 $ cd unihan-etl
 ```
 
 [Bootstrap your environment and learn more about contributing](https://cihai.git-pull.com/contributing/). We use the same conventions / tools across all cihai projects: `pytest`, `sphinx`, `flake8`, `mypy`, `black`, `isort`, `tmuxp`, and file watcher helpers (e.g. `entr(1)`).
 
 ## Python versions
 
-- 0.8.0: Last Python 3.7 release
+- 0.8.0: 
+  - Last Python 3.7 release
+  - Last SQLAlchemy 1.3 release
 
 ## More information
 
 [![Docs](https://github.com/cihai/unihan-db/workflows/docs/badge.svg)](https://unihan-db.git-pull.com/)
 [![Build Status](https://github.com/cihai/unihan-db/workflows/tests/badge.svg)](https://github.com/cihai/unihan-db/actions?query=workflow%3A%22tests%22)
```

