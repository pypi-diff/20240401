# Comparing `tmp/taskcluster-7.0.0.tar.gz` & `tmp/taskcluster-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taskcluster-7.0.0.tar", last modified: Fri Mar  8 19:37:49 2019, max compression
+gzip compressed data, was "dist/taskcluster-7.0.1.tar", last modified: Thu Mar 21 22:43:38 2019, max compression
```

## Comparing `taskcluster-7.0.0.tar` & `taskcluster-7.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-08 19:37:49.000000 taskcluster-7.0.0/
--rw-r--r--   0 asasaki    (501) staff       (20)      415 2019-03-08 19:37:49.000000 taskcluster-7.0.0/PKG-INFO
--rw-r--r--   0 asasaki    (501) staff       (20)   146309 2019-03-08 19:34:03.000000 taskcluster-7.0.0/README.md
--rw-r--r--   0 asasaki    (501) staff       (20)       85 2019-03-08 19:37:49.000000 taskcluster-7.0.0/setup.cfg
--rw-r--r--   0 asasaki    (501) staff       (20)     2599 2019-03-08 19:36:43.000000 taskcluster-7.0.0/setup.py
-drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster/
--rw-r--r--   0 asasaki    (501) staff       (20)      557 2017-10-17 18:31:42.000000 taskcluster-7.0.0/taskcluster/__init__.py
--rw-r--r--   0 asasaki    (501) staff       (20)      660 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/_client_importer.py
-drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster/aio/
--rw-r--r--   0 asasaki    (501) staff       (20)      468 2018-07-16 18:46:09.000000 taskcluster-7.0.0/taskcluster/aio/__init__.py
--rw-r--r--   0 asasaki    (501) staff       (20)      660 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/_client_importer.py
--rw-r--r--   0 asasaki    (501) staff       (20)    11685 2019-03-08 19:09:49.000000 taskcluster-7.0.0/taskcluster/aio/asyncclient.py
--rw-r--r--   0 asasaki    (501) staff       (20)     4340 2018-12-11 01:12:14.000000 taskcluster-7.0.0/taskcluster/aio/asyncutils.py
--rw-r--r--   0 asasaki    (501) staff       (20)    32143 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/auth.py
--rw-r--r--   0 asasaki    (501) staff       (20)     5994 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/authevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    18561 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/awsprovisioner.py
--rw-r--r--   0 asasaki    (501) staff       (20)     5221 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/awsprovisionerevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    14438 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/ec2manager.py
--rw-r--r--   0 asasaki    (501) staff       (20)     6404 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/github.py
--rw-r--r--   0 asasaki    (501) staff       (20)     8433 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/githubevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    11565 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/hooks.py
--rw-r--r--   0 asasaki    (501) staff       (20)    10514 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/index.py
--rw-r--r--   0 asasaki    (501) staff       (20)     2995 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/login.py
--rw-r--r--   0 asasaki    (501) staff       (20)     6545 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/notify.py
--rw-r--r--   0 asasaki    (501) staff       (20)     4004 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/purgecache.py
--rw-r--r--   0 asasaki    (501) staff       (20)    47546 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/queue.py
--rw-r--r--   0 asasaki    (501) staff       (20)    27575 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/queueevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)     4595 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/secrets.py
--rw-r--r--   0 asasaki    (501) staff       (20)     2344 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/aio/treeherderevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    31736 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/auth.py
--rw-r--r--   0 asasaki    (501) staff       (20)     5959 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/authevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    18346 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/awsprovisioner.py
--rw-r--r--   0 asasaki    (501) staff       (20)     5186 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/awsprovisionerevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    27072 2019-03-08 19:09:49.000000 taskcluster-7.0.0/taskcluster/client.py
--rw-r--r--   0 asasaki    (501) staff       (20)    14139 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/ec2manager.py
--rw-r--r--   0 asasaki    (501) staff       (20)     1105 2017-04-06 01:12:13.000000 taskcluster-7.0.0/taskcluster/exceptions.py
--rw-r--r--   0 asasaki    (501) staff       (20)     6273 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/github.py
--rw-r--r--   0 asasaki    (501) staff       (20)     8398 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/githubevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    11374 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/hooks.py
--rw-r--r--   0 asasaki    (501) staff       (20)    10407 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/index.py
--rw-r--r--   0 asasaki    (501) staff       (20)     2936 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/login.py
--rw-r--r--   0 asasaki    (501) staff       (20)     6426 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/notify.py
--rw-r--r--   0 asasaki    (501) staff       (20)     3921 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/purgecache.py
--rw-r--r--   0 asasaki    (501) staff       (20)    47115 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/queue.py
--rw-r--r--   0 asasaki    (501) staff       (20)    27540 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/queueevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)     4500 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/secrets.py
--rw-r--r--   0 asasaki    (501) staff       (20)     2309 2019-03-08 19:36:19.000000 taskcluster-7.0.0/taskcluster/treeherderevents.py
--rw-r--r--   0 asasaki    (501) staff       (20)    10861 2018-12-11 01:12:14.000000 taskcluster-7.0.0/taskcluster/utils.py
-drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/
--rw-r--r--   0 asasaki    (501) staff       (20)      415 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/PKG-INFO
--rw-r--r--   0 asasaki    (501) staff       (20)     1412 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/SOURCES.txt
--rw-r--r--   0 asasaki    (501) staff       (20)        1 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/dependency_links.txt
--rw-r--r--   0 asasaki    (501) staff       (20)        1 2019-03-08 19:33:45.000000 taskcluster-7.0.0/taskcluster.egg-info/not-zip-safe
--rw-r--r--   0 asasaki    (501) staff       (20)      137 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/requires.txt
--rw-r--r--   0 asasaki    (501) staff       (20)       12 2019-03-08 19:37:49.000000 taskcluster-7.0.0/taskcluster.egg-info/top_level.txt
-drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-08 19:37:49.000000 taskcluster-7.0.0/test/
--rw-r--r--   0 asasaki    (501) staff       (20)     2301 2018-10-09 22:03:08.000000 taskcluster-7.0.0/test/test_async.py
--rw-r--r--   0 asasaki    (501) staff       (20)    37409 2018-10-09 22:03:08.000000 taskcluster-7.0.0/test/test_client.py
--rw-r--r--   0 asasaki    (501) staff       (20)    15840 2019-03-08 19:09:49.000000 taskcluster-7.0.0/test/test_utils.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-21 22:43:38.000000 taskcluster-7.0.1/
+-rw-r--r--   0 asasaki    (501) staff       (20)      507 2019-03-21 22:43:38.000000 taskcluster-7.0.1/PKG-INFO
+-rw-r--r--   0 asasaki    (501) staff       (20)   146957 2019-03-21 22:41:20.000000 taskcluster-7.0.1/README.md
+-rw-r--r--   0 asasaki    (501) staff       (20)       85 2019-03-21 22:43:38.000000 taskcluster-7.0.1/setup.cfg
+-rw-r--r--   0 asasaki    (501) staff       (20)     2590 2019-03-21 22:43:30.000000 taskcluster-7.0.1/setup.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster/
+-rw-r--r--   0 asasaki    (501) staff       (20)      557 2017-10-17 18:31:42.000000 taskcluster-7.0.1/taskcluster/__init__.py
+-rw-r--r--   0 asasaki    (501) staff       (20)      660 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/_client_importer.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster/aio/
+-rw-r--r--   0 asasaki    (501) staff       (20)      468 2018-07-16 18:46:09.000000 taskcluster-7.0.1/taskcluster/aio/__init__.py
+-rw-r--r--   0 asasaki    (501) staff       (20)      660 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/_client_importer.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    11696 2019-03-21 19:31:01.000000 taskcluster-7.0.1/taskcluster/aio/asyncclient.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     4340 2018-12-11 01:12:14.000000 taskcluster-7.0.1/taskcluster/aio/asyncutils.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    32616 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/auth.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     5994 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/authevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    18561 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/awsprovisioner.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     5221 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/awsprovisionerevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    14438 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/ec2manager.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     6404 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/github.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     8433 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/githubevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    11565 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/hooks.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    10514 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/index.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2995 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/login.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     6545 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/notify.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     4004 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/purgecache.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    47546 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/queue.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    27575 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/queueevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     4595 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/secrets.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2344 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/aio/treeherderevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    32209 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/auth.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     5959 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/authevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    18346 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/awsprovisioner.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     5186 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/awsprovisionerevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    27092 2019-03-21 19:31:01.000000 taskcluster-7.0.1/taskcluster/client.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    14139 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/ec2manager.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     1105 2017-04-06 01:12:13.000000 taskcluster-7.0.1/taskcluster/exceptions.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     6273 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/github.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     8398 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/githubevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    11374 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/hooks.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    10407 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/index.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2936 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/login.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     6426 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/notify.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     3921 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/purgecache.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    47115 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/queue.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    27540 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/queueevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     4500 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/secrets.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2309 2019-03-21 22:43:16.000000 taskcluster-7.0.1/taskcluster/treeherderevents.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    10860 2019-03-21 19:31:01.000000 taskcluster-7.0.1/taskcluster/utils.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/
+-rw-r--r--   0 asasaki    (501) staff       (20)      507 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/PKG-INFO
+-rw-r--r--   0 asasaki    (501) staff       (20)     1412 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)        1 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)        1 2019-03-21 22:40:45.000000 taskcluster-7.0.1/taskcluster.egg-info/not-zip-safe
+-rw-r--r--   0 asasaki    (501) staff       (20)      113 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/requires.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)       12 2019-03-21 22:43:38.000000 taskcluster-7.0.1/taskcluster.egg-info/top_level.txt
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2019-03-21 22:43:38.000000 taskcluster-7.0.1/test/
+-rw-r--r--   0 asasaki    (501) staff       (20)     2301 2018-10-09 22:03:08.000000 taskcluster-7.0.1/test/test_async.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    37409 2018-10-09 22:03:08.000000 taskcluster-7.0.1/test/test_client.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    15850 2019-03-21 19:31:01.000000 taskcluster-7.0.1/test/test_utils.py
```

### Comparing `taskcluster-7.0.0/README.md` & `taskcluster-7.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -643,15 +643,15 @@
 await asyncAuth.createRole(payload, roleId='value') # -> result
 ```
 
 #### Update Role
 Update an existing role.
 
 The caller's scopes must satisfy all of the new scopes being added, but
-need not satisfy all of the client's existing scopes.
+need not satisfy all of the role's existing scopes.
 
 An update of a role that will generate an infinite expansion will result
 in an error response.
 
 
 
 Takes the following arguments:
@@ -977,26 +977,42 @@
 auth.statsumToken(project) # -> result`
 auth.statsumToken(project='value') # -> result
 # Async call
 await asyncAuth.statsumToken(project) # -> result
 await asyncAuth.statsumToken(project='value') # -> result
 ```
 
-#### Get Token for Websocktunnel Proxy
-Get temporary `token` and `id` for connecting to websocktunnel
-The token is valid for 96 hours, clients should refresh after expiration.
+#### Get a client token for the Websocktunnel service
+Get a temporary token suitable for use connecting to a
+[websocktunnel](https://github.com/taskcluster/websocktunnel) server.
+
+The resulting token will only be accepted by servers with a matching audience
+value.  Reaching such a server is the callers responsibility.  In general,
+a server URL or set of URLs should be provided to the caller as configuration
+along with the audience value.
 
+The token is valid for a limited time (on the scale of hours). Callers should
+refresh it before expiration.
+
+
+
+Takes the following arguments:
+
+  * `wstAudience`
+  * `wstClient`
 
 Required [output schema](v1/websocktunnel-token-response.json#)
 
 ```python
 # Sync calls
-auth.websocktunnelToken() # -> result`
+auth.websocktunnelToken(wstAudience, wstClient) # -> result`
+auth.websocktunnelToken(wstAudience='value', wstClient='value') # -> result
 # Async call
-await asyncAuth.websocktunnelToken() # -> result
+await asyncAuth.websocktunnelToken(wstAudience, wstClient) # -> result
+await asyncAuth.websocktunnelToken(wstAudience='value', wstClient='value') # -> result
 ```
 
 #### Authenticate Hawk Request
 Validate the request signature given on input and return list of scopes
 that the authenticating client has.
 
 This method is used by other services that wish rely on Taskcluster
```

### Comparing `taskcluster-7.0.0/setup.py` & `taskcluster-7.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import sys
 
 # The VERSION variable is automagically changed
 # by release.sh.  Make sure you understand how
 # that script works if you want to change this
-VERSION = '7.0.0'
+VERSION = '7.0.1'
 
 tests_require = [
-    'nose==1.3.7',
-    'nose-exclude==0.5.0',
-    'httmock==1.2.6',
-    'rednose==1.2.1',
-    'mock==1.0.1',
-    'setuptools-lint==0.3',
-    'flake8==2.5.0',
-    'psutil==2.1.3',
-    'hypothesis==3.6.1',
-    'tox==2.3.2',
-    'coverage==4.1b2',
-    'python-dateutil==2.6.0',
+    'nose',
+    'nose-exclude',
+    'httmock',
+    'rednose',
+    'mock',
+    'setuptools-lint',
+    'flake8',
+    'psutil',
+    'hypothesis',
+    'tox',
+    'coverage',
+    'python-dateutil',
 ]
 
 # requests has a policy of not breaking apis between major versions
 # http://docs.python-requests.org/en/latest/community/release-process/
 install_requires = [
-    'requests>=2.4.3,<3',
-    'mohawk>=0.3.4,<2.0',
-    'slugid>=2,<3',
-    'taskcluster-urls>=10.1.0,<12',
-    'six>=1.10.0,<2',
+    'requests>=2.4.3',
+    'mohawk>=0.3.4',
+    'slugid>=2',
+    'taskcluster-urls>=10.1.0',
+    'six>=1.10.0',
 ]
 
 # from http://testrun.org/tox/latest/example/basic.html
 class Tox(TestCommand):
     user_options = [('tox-args=', 'a', "Arguments to pass to tox")]
 
     def initialize_options(self):
@@ -55,35 +55,36 @@
         if args:
             args = shlex.split(self.tox_args)
         errno = tox.cmdline(args=args)
         sys.exit(errno)
 
 if sys.version_info.major == 2:
     tests_require.extend([
-        'subprocess32==3.2.6',
+        'subprocess32',
     ])
 elif sys.version_info[:2] < (3, 5):
     raise Exception('This library does not support Python 3 versions below 3.5')
 elif sys.version_info[:2] >= (3, 5):
     install_requires.extend([
-        'aiohttp>=2.0.0,<4',
-        'async_timeout>=2.0.0,<4',
+        'aiohttp>=2.0.0',
+        'async_timeout>=2.0.0',
     ])
 
 if __name__ == '__main__':
     setup(
         name='taskcluster',
         version=VERSION,
         description='Python client for Taskcluster',
-        author='John Ford',
-        author_email='jhford@mozilla.com',
+        author='Mozilla Taskcluster and Release Engineering',
+        author_email='release+python@mozilla.com',
         url='https://github.com/taskcluster/taskcluster-client.py',
         packages=['taskcluster', 'taskcluster.aio'],
         install_requires=install_requires,
         test_suite="nose.collector",
         tests_require=tests_require,
         cmdclass={'test': Tox},
         zip_safe=False,
         classifiers=['Programming Language :: Python :: 2.7',
                      'Programming Language :: Python :: 3.5',
-                     'Programming Language :: Python :: 3.6'],
+                     'Programming Language :: Python :: 3.6',
+                     'Programming Language :: Python :: 3.7'],
     )
```

### Comparing `taskcluster-7.0.0/taskcluster/__init__.py` & `taskcluster-7.0.1/taskcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/_client_importer.py` & `taskcluster-7.0.1/taskcluster/_client_importer.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/_client_importer.py` & `taskcluster-7.0.1/taskcluster/aio/_client_importer.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/asyncclient.py` & `taskcluster-7.0.1/taskcluster/aio/asyncclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
             # Throw errors for non-retryable errors
             if status < 200 or status >= 300:
                 # Parse messages from errors
                 data = {}
                 try:
                     data = await response.json()
-                except:
+                except Exception:
                     pass  # Ignore JSON errors in error messages
                 # Find error message
                 message = "Unknown Server Error"
                 if isinstance(data, dict):
                     message = data.get('message')
                 else:
                     if status == 401:
@@ -308,13 +308,14 @@
 
         # Add whichever function we created
         f.__name__ = str(entry['name'])
         attributes[entry['name']] = f
 
     return type(utils.toStr(name), (BaseClient,), attributes)
 
+
 __all__ = [
     'createTemporaryCredentials',
     'config',
     'BaseClient',
     'createApiClient',
 ]
```

### Comparing `taskcluster-7.0.0/taskcluster/aio/asyncutils.py` & `taskcluster-7.0.1/taskcluster/aio/asyncutils.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/auth.py` & `taskcluster-7.0.1/taskcluster/aio/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     async def updateRole(self, *args, **kwargs):
         """
         Update Role
 
         Update an existing role.
 
         The caller's scopes must satisfy all of the new scopes being added, but
-        need not satisfy all of the client's existing scopes.
+        need not satisfy all of the role's existing scopes.
 
         An update of a role that will generate an infinite expansion will result
         in an error response.
 
         This method takes input: ``v1/create-role-request.json#``
 
         This method gives output: ``v1/get-role-response.json#``
@@ -561,18 +561,26 @@
         This method is ``stable``
         """
 
         return await self._makeApiCall(self.funcinfo["statsumToken"], *args, **kwargs)
 
     async def websocktunnelToken(self, *args, **kwargs):
         """
-        Get Token for Websocktunnel Proxy
+        Get a client token for the Websocktunnel service
 
-        Get temporary `token` and `id` for connecting to websocktunnel
-        The token is valid for 96 hours, clients should refresh after expiration.
+        Get a temporary token suitable for use connecting to a
+        [websocktunnel](https://github.com/taskcluster/websocktunnel) server.
+
+        The resulting token will only be accepted by servers with a matching audience
+        value.  Reaching such a server is the callers responsibility.  In general,
+        a server URL or set of URLs should be provided to the caller as configuration
+        along with the audience value.
+
+        The token is valid for a limited time (on the scale of hours). Callers should
+        refresh it before expiration.
 
         This method gives output: ``v1/websocktunnel-token-response.json#``
 
         This method is ``stable``
         """
 
         return await self._makeApiCall(self.funcinfo["websocktunnelToken"], *args, **kwargs)
@@ -898,18 +906,18 @@
             'method': 'post',
             'name': 'updateRole',
             'output': 'v1/get-role-response.json#',
             'route': '/roles/<roleId>',
             'stability': 'stable',
         },
         "websocktunnelToken": {
-            'args': [],
+            'args': ['wstAudience', 'wstClient'],
             'method': 'get',
             'name': 'websocktunnelToken',
             'output': 'v1/websocktunnel-token-response.json#',
-            'route': '/websocktunnel',
+            'route': '/websocktunnel/<wstAudience>/<wstClient>',
             'stability': 'stable',
         },
     }
 
 
 __all__ = ['createTemporaryCredentials', 'config', '_defaultConfig', 'createApiClient', 'createSession', 'Auth']
```

### Comparing `taskcluster-7.0.0/taskcluster/aio/authevents.py` & `taskcluster-7.0.1/taskcluster/aio/authevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/awsprovisioner.py` & `taskcluster-7.0.1/taskcluster/aio/awsprovisioner.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/awsprovisionerevents.py` & `taskcluster-7.0.1/taskcluster/aio/awsprovisionerevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/ec2manager.py` & `taskcluster-7.0.1/taskcluster/aio/ec2manager.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/github.py` & `taskcluster-7.0.1/taskcluster/aio/github.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/githubevents.py` & `taskcluster-7.0.1/taskcluster/aio/githubevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/hooks.py` & `taskcluster-7.0.1/taskcluster/aio/hooks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/index.py` & `taskcluster-7.0.1/taskcluster/aio/index.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/login.py` & `taskcluster-7.0.1/taskcluster/aio/login.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/notify.py` & `taskcluster-7.0.1/taskcluster/aio/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/purgecache.py` & `taskcluster-7.0.1/taskcluster/aio/purgecache.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/queue.py` & `taskcluster-7.0.1/taskcluster/aio/queue.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/queueevents.py` & `taskcluster-7.0.1/taskcluster/aio/queueevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/secrets.py` & `taskcluster-7.0.1/taskcluster/aio/secrets.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/aio/treeherderevents.py` & `taskcluster-7.0.1/taskcluster/aio/treeherderevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/auth.py` & `taskcluster-7.0.1/taskcluster/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     def updateRole(self, *args, **kwargs):
         """
         Update Role
 
         Update an existing role.
 
         The caller's scopes must satisfy all of the new scopes being added, but
-        need not satisfy all of the client's existing scopes.
+        need not satisfy all of the role's existing scopes.
 
         An update of a role that will generate an infinite expansion will result
         in an error response.
 
         This method takes input: ``v1/create-role-request.json#``
 
         This method gives output: ``v1/get-role-response.json#``
@@ -561,18 +561,26 @@
         This method is ``stable``
         """
 
         return self._makeApiCall(self.funcinfo["statsumToken"], *args, **kwargs)
 
     def websocktunnelToken(self, *args, **kwargs):
         """
-        Get Token for Websocktunnel Proxy
+        Get a client token for the Websocktunnel service
 
-        Get temporary `token` and `id` for connecting to websocktunnel
-        The token is valid for 96 hours, clients should refresh after expiration.
+        Get a temporary token suitable for use connecting to a
+        [websocktunnel](https://github.com/taskcluster/websocktunnel) server.
+
+        The resulting token will only be accepted by servers with a matching audience
+        value.  Reaching such a server is the callers responsibility.  In general,
+        a server URL or set of URLs should be provided to the caller as configuration
+        along with the audience value.
+
+        The token is valid for a limited time (on the scale of hours). Callers should
+        refresh it before expiration.
 
         This method gives output: ``v1/websocktunnel-token-response.json#``
 
         This method is ``stable``
         """
 
         return self._makeApiCall(self.funcinfo["websocktunnelToken"], *args, **kwargs)
@@ -898,18 +906,18 @@
             'method': 'post',
             'name': 'updateRole',
             'output': 'v1/get-role-response.json#',
             'route': '/roles/<roleId>',
             'stability': 'stable',
         },
         "websocktunnelToken": {
-            'args': [],
+            'args': ['wstAudience', 'wstClient'],
             'method': 'get',
             'name': 'websocktunnelToken',
             'output': 'v1/websocktunnel-token-response.json#',
-            'route': '/websocktunnel',
+            'route': '/websocktunnel/<wstAudience>/<wstClient>',
             'stability': 'stable',
         },
     }
 
 
 __all__ = ['createTemporaryCredentials', 'config', '_defaultConfig', 'createApiClient', 'createSession', 'Auth']
```

### Comparing `taskcluster-7.0.0/taskcluster/authevents.py` & `taskcluster-7.0.1/taskcluster/authevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/awsprovisioner.py` & `taskcluster-7.0.1/taskcluster/awsprovisioner.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/awsprovisionerevents.py` & `taskcluster-7.0.1/taskcluster/awsprovisionerevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/client.py` & `taskcluster-7.0.1/taskcluster/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         credentials = o.get('credentials')
         if credentials:
             for x in ('accessToken', 'clientId', 'certificate'):
                 value = credentials.get(x)
                 if value and not isinstance(value, six.binary_type):
                     try:
                         credentials[x] = credentials[x].encode('ascii')
-                    except:
+                    except Exception:
                         s = '%s (%s) must be unicode encodable' % (x, credentials[x])
                         raise exceptions.TaskclusterAuthFailure(s)
 
         self.options = o
         if 'credentials' in o:
             log.debug('credentials key scrubbed from logging output')
         log.debug(dict((k, v) for k, v in o.items() if k != 'credentials'))
@@ -512,15 +512,15 @@
                 continue
 
             # Throw errors for non-retryable errors
             if status < 200 or status >= 300:
                 data = {}
                 try:
                     data = response.json()
-                except:
+                except Exception:
                     pass  # Ignore JSON errors in error messages
                 # Find error message
                 message = "Unknown Server Error"
                 if isinstance(data, dict):
                     message = data.get('message')
                 else:
                     if status == 401:
```

### Comparing `taskcluster-7.0.0/taskcluster/ec2manager.py` & `taskcluster-7.0.1/taskcluster/ec2manager.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/exceptions.py` & `taskcluster-7.0.1/taskcluster/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/github.py` & `taskcluster-7.0.1/taskcluster/github.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/githubevents.py` & `taskcluster-7.0.1/taskcluster/githubevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/hooks.py` & `taskcluster-7.0.1/taskcluster/hooks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/index.py` & `taskcluster-7.0.1/taskcluster/index.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/login.py` & `taskcluster-7.0.1/taskcluster/login.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/notify.py` & `taskcluster-7.0.1/taskcluster/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/purgecache.py` & `taskcluster-7.0.1/taskcluster/purgecache.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/queue.py` & `taskcluster-7.0.1/taskcluster/queue.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/queueevents.py` & `taskcluster-7.0.1/taskcluster/queueevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/secrets.py` & `taskcluster-7.0.1/taskcluster/secrets.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/treeherderevents.py` & `taskcluster-7.0.1/taskcluster/treeherderevents.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/taskcluster/utils.py` & `taskcluster-7.0.1/taskcluster/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 
 log = logging.getLogger(__name__)
 
 # Regular expression matching: X days Y hours Z minutes
 # todo: support hr, wk, yr
 r = re.compile(''.join([
-   '^(\s*(?P<years>\d+)\s*y(ears?)?)?',
-   '(\s*(?P<months>\d+)\s*mo(nths?)?)?',
-   '(\s*(?P<weeks>\d+)\s*w(eeks?)?)?',
-   '(\s*(?P<days>\d+)\s*d(ays?)?)?',
-   '(\s*(?P<hours>\d+)\s*h(ours?)?)?',
-   '(\s*(?P<minutes>\d+)\s*m(in(utes?)?)?)?\s*',
-   '(\s*(?P<seconds>\d+)\s*s(ec(onds?)?)?)?\s*$',
+   r'^(\s*(?P<years>\d+)\s*y(ears?)?)?',
+   r'(\s*(?P<months>\d+)\s*mo(nths?)?)?',
+   r'(\s*(?P<weeks>\d+)\s*w(eeks?)?)?',
+   r'(\s*(?P<days>\d+)\s*d(ays?)?)?',
+   r'(\s*(?P<hours>\d+)\s*h(ours?)?)?',
+   r'(\s*(?P<minutes>\d+)\s*m(in(utes?)?)?)?\s*',
+   r'(\s*(?P<seconds>\d+)\s*s(ec(onds?)?)?)?\s*$',
 ]))
 
 
 def calculateSleepTime(attempt):
     """ From the go client
     https://github.com/taskcluster/go-got/blob/031f55c/backoff.go#L24-L29
     """
@@ -262,15 +262,15 @@
                 log.warn('Retrying because of: %s' % rerr)
                 continue
             # raise a connection exception
             raise rerr
         # Handle non 2xx status code and retry if possible
         try:
             response.raise_for_status()
-        except requests.exceptions.RequestException as rerr:
+        except requests.exceptions.RequestException:
             pass
         status = response.status_code
         if 500 <= status and status < 600 and retry < retries:
             if retry < retries:
                 log.warn('Retrying because of: %d status' % status)
                 continue
             else:
```

### Comparing `taskcluster-7.0.0/taskcluster.egg-info/SOURCES.txt` & `taskcluster-7.0.1/taskcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/test/test_async.py` & `taskcluster-7.0.1/test/test_async.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/test/test_client.py` & `taskcluster-7.0.1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `taskcluster-7.0.0/test/test_utils.py` & `taskcluster-7.0.1/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 
 class TestScopeMatch(TestCase):
     def assertScopeMatch(self, assumed, requiredScopeSets, expected):
         try:
             result = subject.scopeMatch(assumed, requiredScopeSets)
             self.assertEqual(result, expected)
-        except:
+        except Exception:
             if expected != 'exception':
                 raise
 
     def test_single_exact_match_string_except_1(self):
         self.assertScopeMatch(["foo:bar"], "foo:bar", "exception")
 
     def test_single_exact_match_string_except_2(self):
```

