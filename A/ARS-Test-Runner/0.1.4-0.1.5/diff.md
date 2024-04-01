# Comparing `tmp/ARS_Test_Runner-0.1.4.tar.gz` & `tmp/ARS_Test_Runner-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARS_Test_Runner-0.1.4.tar", last modified: Thu Mar 28 18:50:48 2024, max compression
+gzip compressed data, was "ARS_Test_Runner-0.1.5.tar", last modified: Mon Apr  1 14:22:09 2024, max compression
```

## Comparing `ARS_Test_Runner-0.1.4.tar` & `ARS_Test_Runner-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-03-28 18:50:48.457638 ARS_Test_Runner-0.1.4/
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-03-28 18:50:48.452107 ARS_Test_Runner-0.1.4/ARS_Test_Runner/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/__init__.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/cli.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22011 2024-03-28 18:49:06.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/semantic_test.py
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-03-28 18:50:48.456338 ARS_Test_Runner-0.1.4/ARS_Test_Runner/templates/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/templates/affects_creative.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/templates/treats.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner/templates/treats_creative.json
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-03-28 18:50:48.456982 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/SOURCES.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/dependency_links.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/entry_points.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/requires.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-03-28 18:50:47.000000 ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/top_level.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.4/LICENSE.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-03-28 18:50:48.457434 ARS_Test_Runner-0.1.4/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.4/README.md
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-03-28 18:50:48.458129 ARS_Test_Runner-0.1.4/setup.cfg
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-03-28 18:49:58.000000 ARS_Test_Runner-0.1.4/setup.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 14:22:09.488538 ARS_Test_Runner-0.1.5/
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 14:22:09.481298 ARS_Test_Runner-0.1.5/ARS_Test_Runner/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/__init__.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/cli.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22254 2024-04-01 14:16:02.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/semantic_test.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 14:22:09.486768 ARS_Test_Runner-0.1.5/ARS_Test_Runner/templates/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/templates/affects_creative.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/templates/treats.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner/templates/treats_creative.json
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-01 14:22:09.487640 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-01 14:22:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-01 14:22:09.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/SOURCES.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-01 14:22:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/dependency_links.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-01 14:22:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/entry_points.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-01 14:22:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/requires.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-01 14:22:08.000000 ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/top_level.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.5/LICENSE.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-01 14:22:09.488242 ARS_Test_Runner-0.1.5/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.5/README.md
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-01 14:22:09.489598 ARS_Test_Runner-0.1.5/setup.cfg
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-01 14:21:20.000000 ARS_Test_Runner-0.1.5/setup.py
```

### Comparing `ARS_Test_Runner-0.1.4/ARS_Test_Runner/cli.py` & `ARS_Test_Runner-0.1.5/ARS_Test_Runner/cli.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.4/ARS_Test_Runner/semantic_test.py` & `ARS_Test_Runner-0.1.5/ARS_Test_Runner/semantic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,18 +121,23 @@
 
     if 'error' in message.keys():
         report_card={}
         report_card['pk']={}
         report_card['results']=message
     else:
         children, parent_pk = await get_children(message, ARS_URL, output_curie)
-        if 'error' in children.keys():
-            report_card = {}
-            report_card['pk']={}
-            report_card['results']=children['error']
+        if len(children) == 1:
+            response = children[0]
+            agent = response[0]
+            mesg = response[1]
+            parent_pk = response[2]
+            if 'error' in mesg.keys():
+                report_card = {}
+                report_card['parent_pk'] = parent_pk
+                report_card['results']=mesg['error']
         else:
             report_card = await ARS_semantic_analysis(children, parent_pk, output_curie, expected_output)
 
     return report_card
 
 async def ARS_semantic_analysis(children: List[List], pk: str, output_curie: List[str], expected_output: str):
     """" function to perform pass fail analysis on individual ARA's results """
@@ -324,16 +329,16 @@
             logging.error(r.text)
 
         if data["status"]=="Done":
             #print(f"finished processing message at: {(datetime.datetime.now()).strftime('%H:%M:%S')}")
             break
     else:
         logging.debug(f"Parent pk: {parent_pk} is still 'Running' even after 8 min, please check the timeout operation")
-        data = None
-        return {"error": "ARS still Running"}, None
+        children.append(['ars-default-agent', {"error": "ARS still Running"} , parent_pk])
+        return children, parent_pk
 
     if data is not None:
         for child in data["children"]:
             agent = child["actor"]["agent"]
             childPk = child["message"]
             logging.debug("---Checking child for " + agent + ", pk=" + parent_pk)
             childData = await get_child(childPk, ARS_URL, output_curie)
```

### Comparing `ARS_Test_Runner-0.1.4/ARS_Test_Runner/templates/affects_creative.json` & `ARS_Test_Runner-0.1.5/ARS_Test_Runner/templates/affects_creative.json`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.4/ARS_Test_Runner.egg-info/PKG-INFO` & `ARS_Test_Runner-0.1.5/ARS_Test_Runner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS-Test-Runner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.4/LICENSE.txt` & `ARS_Test_Runner-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.4/PKG-INFO` & `ARS_Test_Runner-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS_Test_Runner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.4/README.md` & `ARS_Test_Runner-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.4/setup.py` & `ARS_Test_Runner-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from semantic_release import setup_hook
     setup_hook(sys.argv)
 except ImportError:
     pass
 
-__version__='0.1.4'
+__version__='0.1.5'
 setup(
     name="ARS_Test_Runner",
     version= __version__,
     description="Python package for ARS pass/fail test",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Shervin Abdollahi, Mark Williams",
```

