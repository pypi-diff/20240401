# Comparing `tmp/bhbotlist-3.0.4.tar.gz` & `tmp/bhbotlist-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhbotlist-3.0.4.tar", last modified: Tue Mar 21 18:50:04 2023, max compression
+gzip compressed data, was "bhbotlist-3.0.5.tar", last modified: Mon Apr  1 15:49:00 2024, max compression
```

## Comparing `bhbotlist-3.0.4.tar` & `bhbotlist-3.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2023-03-21 18:50:04.130769 bhbotlist-3.0.4/
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)     1088 2023-03-21 18:47:33.000000 bhbotlist-3.0.4/LICENSE
--rw-r--r--   0 anshtyagi   (501) staff       (20)     1213 2023-03-21 18:50:04.130571 bhbotlist-3.0.4/PKG-INFO
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      898 2023-03-21 18:47:06.000000 bhbotlist-3.0.4/README.md
--rw-r--r--   0 anshtyagi   (501) staff       (20)       38 2023-03-21 18:50:04.130846 bhbotlist-3.0.4/setup.cfg
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      652 2023-03-21 18:46:47.000000 bhbotlist-3.0.4/setup.py
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2023-03-21 18:50:04.128126 bhbotlist-3.0.4/src/
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2023-03-21 18:50:04.129057 bhbotlist-3.0.4/src/bhbotlist/
--rw-rw-rw-   0 anshtyagi   (501) staff       (20)      935 2023-03-21 18:47:58.000000 bhbotlist-3.0.4/src/bhbotlist/__init__.py
-drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2023-03-21 18:50:04.130286 bhbotlist-3.0.4/src/bhbotlist.egg-info/
--rw-r--r--   0 anshtyagi   (501) staff       (20)     1213 2023-03-21 18:50:03.000000 bhbotlist-3.0.4/src/bhbotlist.egg-info/PKG-INFO
--rw-r--r--   0 anshtyagi   (501) staff       (20)      236 2023-03-21 18:50:03.000000 bhbotlist-3.0.4/src/bhbotlist.egg-info/SOURCES.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)        1 2023-03-21 18:50:03.000000 bhbotlist-3.0.4/src/bhbotlist.egg-info/dependency_links.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)        8 2023-03-21 18:50:03.000000 bhbotlist-3.0.4/src/bhbotlist.egg-info/requires.txt
--rw-r--r--   0 anshtyagi   (501) staff       (20)       10 2023-03-21 18:50:03.000000 bhbotlist-3.0.4/src/bhbotlist.egg-info/top_level.txt
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.514546 bhbotlist-3.0.5/
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)     1088 2023-03-21 18:47:33.000000 bhbotlist-3.0.5/LICENSE
+-rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-01 15:49:00.514462 bhbotlist-3.0.5/PKG-INFO
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)      898 2023-03-21 18:47:06.000000 bhbotlist-3.0.5/README.md
+-rw-r--r--   0 anshtyagi   (501) staff       (20)       38 2024-04-01 15:49:00.514760 bhbotlist-3.0.5/setup.cfg
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)      652 2024-04-01 15:48:58.000000 bhbotlist-3.0.5/setup.py
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.512190 bhbotlist-3.0.5/src/
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.513068 bhbotlist-3.0.5/src/bhbotlist/
+-rw-rw-rw-   0 anshtyagi   (501) staff       (20)      935 2024-04-01 15:41:56.000000 bhbotlist-3.0.5/src/bhbotlist/__init__.py
+drwxr-xr-x   0 anshtyagi   (501) staff       (20)        0 2024-04-01 15:49:00.514187 bhbotlist-3.0.5/src/bhbotlist.egg-info/
+-rw-r--r--   0 anshtyagi   (501) staff       (20)     1199 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/PKG-INFO
+-rw-r--r--   0 anshtyagi   (501) staff       (20)      246 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/SOURCES.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)        1 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/dependency_links.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)        8 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/requires.txt
+-rw-r--r--   0 anshtyagi   (501) staff       (20)       10 2024-04-01 15:49:00.000000 bhbotlist-3.0.5/src/bhbotlist.egg-info/top_level.txt
```

### Comparing `bhbotlist-3.0.4/LICENSE` & `bhbotlist-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bhbotlist-3.0.4/PKG-INFO` & `bhbotlist-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bhbotlist
-Version: 3.0.4
+Version: 3.0.5
 Summary: API for bhlist.co.in
 Author: BHBL
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 # bhbotlist 
 useful library for [bhlist.co.in](https://bhlist.co.in)
 
 # API DOCS
 Link to api docs: [API DOCS](https://docs.bhlist.co.in)
 
@@ -58,9 +57,7 @@
 3: hasVoted()
 ```
 
 
 **JOIN OUR DISCORD SERVER FOR SUPPORT**\
 [DISCORD LINK](https://bhlist.co.in/dc)
 
-
-
```

### Comparing `bhbotlist-3.0.4/README.md` & `bhbotlist-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bhbotlist-3.0.4/setup.py` & `bhbotlist-3.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bhbotlist",
-    version="3.0.4",
+    version="3.0.5",
     author="BHBL",
     description="API for bhlist.co.in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `bhbotlist-3.0.4/src/bhbotlist/__init__.py` & `bhbotlist-3.0.5/src/bhbotlist/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 class bhbotlist():
   def __init__(self,client,token):
     self.client = client
     self.token = token
   
   async def serverCountPost(self):
     async with aiohttp.ClientSession() as session:
-        res = await session.post(url="https://api.bhlist.co.in/bots/stats",headers={'serverCount': str(len(self.client.guilds)),'Content-Type': 'application/json', 'Authorization': str(self.token)})
+        res = await session.post(url="https://api.bhlist.co.in/post/stats",headers={'serverCount': str(len(self.client.guilds)),'Content-Type': 'application/json', 'Authorization': str(self.token)})
         await print("Server count posted.")
         return await res.json()
   
   async def hasVoted(self,id):
     async with aiohttp.ClientSession(headers={"Authorization": self.token}) as session:
-      async with session.get(f"https://api.bhlist.co.in/bots/check/{id}") as res:
+      async with session.get(f"https://api.bhlist.co.in/vote/check/{id}") as res:
         return await res.json()
   
   async def search(self,id):
     async with aiohttp.ClientSession() as session:
         async with session.get(f"https://api.bhlist.co.in/bots/{id}") as res:
           return await res.json()
```

### Comparing `bhbotlist-3.0.4/src/bhbotlist.egg-info/PKG-INFO` & `bhbotlist-3.0.5/src/bhbotlist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bhbotlist
-Version: 3.0.4
+Version: 3.0.5
 Summary: API for bhlist.co.in
 Author: BHBL
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 # bhbotlist 
 useful library for [bhlist.co.in](https://bhlist.co.in)
 
 # API DOCS
 Link to api docs: [API DOCS](https://docs.bhlist.co.in)
 
@@ -58,9 +57,7 @@
 3: hasVoted()
 ```
 
 
 **JOIN OUR DISCORD SERVER FOR SUPPORT**\
 [DISCORD LINK](https://bhlist.co.in/dc)
 
-
-
```

