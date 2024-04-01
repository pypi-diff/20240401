# Comparing `tmp/aioice2-0.9.0.post0.tar.gz` & `tmp/aioice2-0.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aioice2/aioice2/dist/.tmp-y6mbihw6/aioice2-0.9.0.post0.tar", last modified: Mon Apr  1 06:40:00 2024, max compression
+gzip compressed data, was "/home/runner/work/aioice2/aioice2/dist/.tmp-1l9hxln5/aioice2-0.9.0.post1.tar", last modified: Mon Apr  1 10:48:12 2024, max compression
```

## Comparing `aioice2-0.9.0.post0.tar` & `aioice2-0.9.0.post1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/examples/ice-client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/examples/signaling-server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)    40514 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/stun.py
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/turn.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/src/aioice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/src/aioice2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:40:00.000000 aioice2-0.9.0.post0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/data/binding_request.bin
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/data/binding_request_ice_controlled.bin
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/data/binding_request_ice_controlling.bin
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/data/binding_response.bin
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/echoserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43726 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_ice_trickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_stun.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/test_turn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/turnserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 06:39:56.000000 aioice2-0.9.0.post0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/examples/ice-client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/examples/signaling-server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40633 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/stun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/turn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/src/aioice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/src/aioice2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:48:12.000000 aioice2-0.9.0.post1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/data/binding_request.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/data/binding_request_ice_controlled.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/data/binding_request_ice_controlling.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/data/binding_response.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/echoserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43726 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_ice_trickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_stun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/test_turn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/turnserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 10:48:08.000000 aioice2-0.9.0.post1/tests/utils.py
```

### Comparing `aioice2-0.9.0.post0/LICENSE` & `aioice2-0.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/PKG-INFO` & `aioice2-0.9.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioice2
-Version: 0.9.0.post0
+Version: 0.9.0.post1
 Summary: An implementation of Interactive Connectivity Establishment (RFC 5245)
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/CoLearn-Dev/aioice2
 Project-URL: documentation, https://aioice.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `aioice2-0.9.0.post0/README.rst` & `aioice2-0.9.0.post1/README.rst`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/docs/Makefile` & `aioice2-0.9.0.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/docs/api.rst` & `aioice2-0.9.0.post1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/docs/changelog.rst` & `aioice2-0.9.0.post1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/docs/conf.py` & `aioice2-0.9.0.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/docs/index.rst` & `aioice2-0.9.0.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/examples/ice-client.py` & `aioice2-0.9.0.post1/examples/ice-client.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/examples/signaling-server.py` & `aioice2-0.9.0.post1/examples/signaling-server.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/pyproject.toml` & `aioice2-0.9.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/src/aioice/candidate.py` & `aioice2-0.9.0.post1/src/aioice/candidate.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/src/aioice/ice.py` & `aioice2-0.9.0.post1/src/aioice/ice.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,15 +664,17 @@
         return request
 
     def check_complete(self, pair: CandidatePair) -> None:
         pair.task = None
 
         if pair.state == CandidatePair.State.SUCCEEDED:
             if pair.nominated:
-                self._nominated[pair.component] = pair
+                # Always choose the one with minimum RTT
+                if pair.component not in self._nominated:
+                    self._nominated[pair.component] = pair
 
                 # 8.1.2.  Updating States
                 #
                 # The agent MUST remove all Waiting and Frozen pairs in the check
                 # list and triggered check queue for the same component as the
                 # nominated pairs for that media stream.
                 for p in self._check_list:
```

### Comparing `aioice2-0.9.0.post0/src/aioice/mdns.py` & `aioice2-0.9.0.post1/src/aioice/mdns.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/src/aioice/stun.py` & `aioice2-0.9.0.post1/src/aioice/stun.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/src/aioice/turn.py` & `aioice2-0.9.0.post1/src/aioice/turn.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/src/aioice2.egg-info/PKG-INFO` & `aioice2-0.9.0.post1/src/aioice2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioice2
-Version: 0.9.0.post0
+Version: 0.9.0.post1
 Summary: An implementation of Interactive Connectivity Establishment (RFC 5245)
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/CoLearn-Dev/aioice2
 Project-URL: documentation, https://aioice.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `aioice2-0.9.0.post0/src/aioice2.egg-info/SOURCES.txt` & `aioice2-0.9.0.post1/src/aioice2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/echoserver.py` & `aioice2-0.9.0.post1/tests/echoserver.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_candidate.py` & `aioice2-0.9.0.post1/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_exceptions.py` & `aioice2-0.9.0.post1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_ice.py` & `aioice2-0.9.0.post1/tests/test_ice.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_ice_trickle.py` & `aioice2-0.9.0.post1/tests/test_ice_trickle.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_mdns.py` & `aioice2-0.9.0.post1/tests/test_mdns.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_stun.py` & `aioice2-0.9.0.post1/tests/test_stun.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/test_turn.py` & `aioice2-0.9.0.post1/tests/test_turn.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/turnserver.py` & `aioice2-0.9.0.post1/tests/turnserver.py`

 * *Files identical despite different names*

### Comparing `aioice2-0.9.0.post0/tests/utils.py` & `aioice2-0.9.0.post1/tests/utils.py`

 * *Files identical despite different names*

