# Comparing `tmp/surge_api-1.5.1-py3-none-any.whl.zip` & `tmp/surge_api-1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18201 bytes, number of entries: 16
--rw-r--r--  2.0 unx      288 b- defN 24-Feb-25 03:28 surge/__init__.py
+Zip file size: 18180 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      260 b- defN 24-Apr-01 21:14 surge/__init__.py
 -rw-r--r--  2.0 unx     3066 b- defN 24-Mar-29 01:22 surge/api_resource.py
 -rw-r--r--  2.0 unx      949 b- defN 23-Nov-30 19:24 surge/carousel.py
 -rw-r--r--  2.0 unx     1606 b- defN 23-Jun-19 05:11 surge/errors.py
 -rw-r--r--  2.0 unx    13792 b- defN 24-Mar-29 01:22 surge/projects.py
 -rw-r--r--  2.0 unx    27971 b- defN 24-Mar-29 01:22 surge/questions.py
 -rw-r--r--  2.0 unx     5481 b- defN 24-Mar-29 01:22 surge/reports.py
 -rw-r--r--  2.0 unx      939 b- defN 23-Jun-19 05:11 surge/responses.py
 -rw-r--r--  2.0 unx     6053 b- defN 24-Mar-29 01:22 surge/tasks.py
 -rw-r--r--  2.0 unx     4373 b- defN 24-Mar-29 01:22 surge/teams.py
 -rw-r--r--  2.0 unx      442 b- defN 23-Jun-19 05:11 surge/utils.py
--rw-r--r--  2.0 unx     1062 b- defN 24-Mar-29 01:23 surge_api-1.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4402 b- defN 24-Mar-29 01:23 surge_api-1.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 01:23 surge_api-1.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-29 01:23 surge_api-1.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 24-Mar-29 01:23 surge_api-1.5.1.dist-info/RECORD
-16 files, 71723 bytes uncompressed, 16263 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx     1062 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4402 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-01 21:16 surge_api-1.5.2.dist-info/RECORD
+16 files, 71695 bytes uncompressed, 16242 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: surge/teams.py
 Comment: 
 
 Filename: surge/utils.py
 Comment: 
 
-Filename: surge_api-1.5.1.dist-info/LICENSE
+Filename: surge_api-1.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: surge_api-1.5.1.dist-info/METADATA
+Filename: surge_api-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: surge_api-1.5.1.dist-info/WHEEL
+Filename: surge_api-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: surge_api-1.5.1.dist-info/top_level.txt
+Filename: surge_api-1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: surge_api-1.5.1.dist-info/RECORD
+Filename: surge_api-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## surge/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 from surge.projects import Project
 from surge.tasks import Task
 from surge.teams import Team
 from surge.reports import Report
 
 api_key = os.environ.get("SURGE_API_KEY", None)
-base_url = "http://localhost:3000/api"#os.environ.get("SURGE_BASE_URL", "https://app.surgehq.ai/api")
+base_url = os.environ.get("SURGE_BASE_URL", "https://app.surgehq.ai/api")
```

## Comparing `surge_api-1.5.1.dist-info/LICENSE` & `surge_api-1.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `surge_api-1.5.1.dist-info/METADATA` & `surge_api-1.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surge-api
-Version: 1.5.1
+Version: 1.5.2
 Summary: Surge Python SDK
 Home-page: https://github.com/surge-ai/surge-python
 Author: Surge
 Author-email: team@surgehq.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `surge_api-1.5.1.dist-info/RECORD` & `surge_api-1.5.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-surge/__init__.py,sha256=mi1cNvhaeasPZjGDBXfnKOFLpR0URXAF1sK94anaLQM,288
+surge/__init__.py,sha256=EbBXghvhL6SxEURWh2-92f0oM9vsw0sG3C82fHCI_ko,260
 surge/api_resource.py,sha256=CWoRluTsaBfjP4LakN4Au0wiq7MkEJQd33MMRZXaeFY,3066
 surge/carousel.py,sha256=ZCYGVsgd8G2u-goTB49RuzbknV-s3v7hYgr9jQVYtv8,949
 surge/errors.py,sha256=N83WpLlqrRi_Y03-q8JUXlutgCUpUrMeL47TvbOv11c,1606
 surge/projects.py,sha256=X2iD67DRkaViGe6Mv5p169Rl5dQL_UyP7Bp8k5POzdA,13792
 surge/questions.py,sha256=0xNhWUIMJ3eJGLHrbL-tM3q2P37fydjxL0pTh1Umq98,27971
 surge/reports.py,sha256=BgbbcCEXF7haGBgZkdws2tRxnq8bwl1IJtdGAFgjwj4,5481
 surge/responses.py,sha256=uQIQj55KS2H334OBXIe59FFEerOnDuqk0MhTTUye-D4,939
 surge/tasks.py,sha256=Tpk5azp4qMwICc9RkUX-Cvdnljv1JmL7DHZxPlJGvP8,6053
 surge/teams.py,sha256=kH4_za61bwsJxwrM-N7kBd7bojiazuDOt-Auk3e3aYU,4373
 surge/utils.py,sha256=4SO3vQVwOOgn-mrDFmUH0HipfRJwcU8v5eTXp4uoZag,442
-surge_api-1.5.1.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
-surge_api-1.5.1.dist-info/METADATA,sha256=KLmvx7OGI3EAtHSQfjlOlMNHV3XiX9jIXmkLppghHew,4402
-surge_api-1.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-surge_api-1.5.1.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
-surge_api-1.5.1.dist-info/RECORD,,
+surge_api-1.5.2.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
+surge_api-1.5.2.dist-info/METADATA,sha256=-Cr5jvqLlshkKAcaAz0S8ETwWnvVUt7xjnsHl9NRoJ0,4402
+surge_api-1.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+surge_api-1.5.2.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
+surge_api-1.5.2.dist-info/RECORD,,
```

