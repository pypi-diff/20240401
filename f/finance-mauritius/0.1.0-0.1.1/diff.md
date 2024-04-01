# Comparing `tmp/finance_mauritius-0.1.0.tar.gz` & `tmp/finance_mauritius-0.1.1.tar.gz`

## Comparing `finance_mauritius-0.1.0.tar` & `finance_mauritius-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/.python-version
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/mcb copy.CSV
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/mcb.CSV
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/requirements.lock
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/test.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/src/finance_mauritius/__init__.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/src/finance_mauritius/mcb.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/.gitignore
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 finance_mauritius-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/.python-version
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/src/finance_mauritius/__init__.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/src/finance_mauritius/mcb.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/.gitignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/README.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 finance_mauritius-0.1.1/PKG-INFO
```

### Comparing `finance_mauritius-0.1.0/src/finance_mauritius/mcb.py` & `finance_mauritius-0.1.1/src/finance_mauritius/mcb.py`

 * *Files identical despite different names*

### Comparing `finance_mauritius-0.1.0/.gitignore` & `finance_mauritius-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `finance_mauritius-0.1.0/README.md` & `finance_mauritius-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # finance-mauritius
 
+```
+pip install finance-mauritius
+```
+
 Export your data in Excel format
 
 ```python
 from finance_mauritius.mcb import MCB
 
 >>> MCB.process_csv('mcb.CSV')
 {
```

