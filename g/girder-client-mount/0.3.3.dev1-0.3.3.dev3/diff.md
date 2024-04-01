# Comparing `tmp/girder_client_mount-0.3.3.dev1.tar.gz` & `tmp/girder_client_mount-0.3.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder_client_mount-0.3.3.dev1.tar", last modified: Thu Mar 14 13:54:44 2024, max compression
+gzip compressed data, was "girder_client_mount-0.3.3.dev3.tar", last modified: Mon Apr  1 14:32:43 2024, max compression
```

## Comparing `girder_client_mount-0.3.3.dev1.tar` & `girder_client_mount-0.3.3.dev3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:54:44.784951 girder_client_mount-0.3.3.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:54:44.780951 girder_client_mount-0.3.3.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:54:44.780951 girder_client_mount-0.3.3.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-14 13:54:44.784951 girder_client_mount-0.3.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:54:44.780951 girder_client_mount-0.3.3.dev1/girder_client_mount/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/girder_client_mount/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30021 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/girder_client_mount/girder_client_mount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:54:44.784951 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:54:32.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-14 13:54:44.000000 girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:54:44.784951 girder_client_mount-0.3.3.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-14 13:54:17.000000 girder_client_mount-0.3.3.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:43.274882 girder_client_mount-0.3.3.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:43.270882 girder_client_mount-0.3.3.dev3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:43.270882 girder_client_mount-0.3.3.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-01 14:32:43.274882 girder_client_mount-0.3.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:43.270882 girder_client_mount-0.3.3.dev3/girder_client_mount/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/girder_client_mount/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31988 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/girder_client_mount/girder_client_mount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:43.274882 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:32:31.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 14:32:43.000000 girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:32:43.274882 girder_client_mount-0.3.3.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 14:32:15.000000 girder_client_mount-0.3.3.dev3/tox.ini
```

### Comparing `girder_client_mount-0.3.3.dev1/.github/workflows/main.yml` & `girder_client_mount-0.3.3.dev3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/.gitignore` & `girder_client_mount-0.3.3.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/.pre-commit-config.yaml` & `girder_client_mount-0.3.3.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/LICENSE` & `girder_client_mount-0.3.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/PKG-INFO` & `girder_client_mount-0.3.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder_client_mount
-Version: 0.3.3.dev1
+Version: 0.3.3.dev3
 Summary: Mount a girder server via fuse
 Home-page: https://github.com/DigitalSlideArchive/girder-client-mount
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder,fuse,girder-client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder_client_mount-0.3.3.dev1/README.rst` & `girder_client_mount-0.3.3.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/girder_client_mount/girder_client_mount.py` & `girder_client_mount-0.3.3.dev3/girder_client_mount/girder_client_mount.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+
 import argparse
 import errno
 import functools
 import hashlib
 import logging
 import os
 import pathlib
@@ -28,14 +29,18 @@
 
 logger = logging.getLogger(__name__)
 
 # See http://docs.python.org/3.3/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
+def hashkey_first(funcname, *args, **kwargs):
+    return (funcname, args[1])
+
+
 class ClientFuse(fuse.Operations):
     """
     Handle FUSE operations that are non-default.
 
     It exposes the Girder resources via the resource path in a read-only
     manner.
     """
@@ -78,14 +83,22 @@
         self.nextFH = 1
         self.openFiles = {}
         self.openFilesLock = threading.Lock()
         options = options or {}
         self._allow_other = 'allow_other' in options
         self.cache = cachetools.TTLCache(maxsize=10000, ttl=int(options.pop('stat_cache_ttl', 1)))
         self.diskcache = None
+        self._mount_stats = {
+            'open': 0,
+            'read': 0,
+            'release': 0,
+            'dir': 0,
+            'bytesread': 0,
+            'pathlookups': 0,
+        }
         self._configure_disk_cache(options)
 
     def _configure_disk_cache(self, cacheopts):
         """
         Configure the disk cache.
 
         :param cacheopts: An optional dictionary of options.  Any option that
@@ -120,15 +133,18 @@
                     options[key] = value
                 elif not value:
                     use = False
         if use:
             chunk = int(options.pop('chunk', 128 * 1024))
             self.diskcache = {
                 'chunk': chunk,
-                'cache': diskcache.Cache(**options)
+                'cache': diskcache.Cache(**options),
+                'hits': 0,
+                'miss': 0,
+                'bytesread': 0,
             }
 
     def __call__(self, op, path, *args, **kwargs):
         """
         Generically allow logging and error handling for any operation.
 
         :param op: operation to perform.
@@ -150,22 +166,23 @@
         finally:
             if op != 'read':
                 logger.debug('<- %s %s', op, repr(ret))
             else:
                 logger.debug('<- %s (length %d) %r', op, len(ret), ret[:16])
 
     @cachetools.cachedmethod(lambda self: self.cache, key=functools.partial(
-        cachetools.keys.hashkey, '_get_path'))
+        hashkey_first, '_get_path'))
     def _get_path(self, path):
         """
         Given a fuse path, return the associated resource.
 
         :param path: path within the fuse.
         :returns: a Girder resource dictionary.
         """
+        self._mount_stats['pathlookups'] += 1
         if path.endswith('/*'):
             path = path[:-1]
         # If asked about a file in top level directory or the top directory,
         # return that it doesn't exist.  Other methods should handle '',
         # 'user', and 'collection' before calling this method.
         if '/' not in path.rstrip('/')[1:]:
             raise fuse.FuseOSError(errno.ENOENT)
@@ -257,14 +274,28 @@
             logger.debug('listFile %r', doc['_id'])
             for file in self.gc.listFile(doc['_id']):
                 entries.append(self._name(file, 'file'))
         # we can't reach items with slashes in their names, so don't list them
         entries = [entry for entry in entries if '/' not in entry]
         return entries
 
+    def _mount_stats_repr(self):
+        import json
+
+        curstats = self._mount_stats.copy()
+        curstats['openfiles'] = {}
+        for fh in self.openFiles:
+            try:
+                curstats['openfiles'][fh] = self.openFiles[fh]['path']
+            except Exception:
+                pass
+        if self.diskcache:
+            curstats['diskcache'] = {k: v for k, v in self.diskcache.items() if k != 'cache'}
+        return (json.dumps(curstats, indent=2) + '\n').encode()
+
     # We don't handle extended attributes or ioctl.
     getxattr = None
     listxattr = None
     ioctl = None
 
     def access(self, path, mode):
         """
@@ -298,28 +329,35 @@
         We may want to disallow flush, since this is a read-only system:
             raise fuse.FuseOSError(errno.EACCES)
         For now, always succeed.
         """
         return 0
 
     @cachetools.cachedmethod(lambda self: self.cache, key=functools.partial(
-        cachetools.keys.hashkey, 'getattr'))
+        hashkey_first, 'getattr'))
     def getattr(self, path, fh=None):
         """
         Get the attributes dictionary of a path.
 
         :param path: path within the fuse.
         :param fh: an open file handle.  Ignored, since path is always
             specified.
         :returns: an attribute dictionary.
         """
         if path.rstrip('/') in ('', '/user', '/collection'):
             attr = self._defaultStat.copy()
             attr['st_mode'] = (0o555 if self._allow_other else 0o500) | stat.S_IFDIR
             attr['st_size'] = 0
+        elif path.rstrip('/') == '/stats':
+            attr = self._defaultStat.copy()
+            attr['st_ino'] = -1
+            attr['st_nlink'] = 1
+            attr['st_ctime'] = attr['st_mtime'] = int(time.time() * 1e9)
+            attr['st_mode'] = 0o400 | stat.S_IFREG
+            attr['st_size'] = len(self._mount_stats_repr())
         else:
             resource = self._get_path(path)
             attr = self._stat(resource['document'], resource['model'])
         if self._blockSize and attr.get('st_size'):
             attr['st_blocks'] = int(
                 (attr['st_size'] + self._blockSize - 1) / self._blockSize)
         return attr
@@ -332,69 +370,80 @@
             must be valid.
         :param size: maximum number of bytes to read.  There may be less if
             this is near the end of the file.
         :param offset: the offset within the file to read.
         :param fh: an open file handle.
         :returns: a block of up to <size> bytes.
         """
+        if path.rstrip('/') == '/stats':
+            data = self._mount_stats_repr()
+            return data[offset:offset + size]
         with self.openFilesLock:
             if fh not in self.openFiles:
                 raise fuse.FuseOSError(errno.EBADF)
             info = self.openFiles[fh]
+        self._mount_stats['read'] += 1
         if self.diskcache:
             result = b''
             for idx in range(
                     offset // self.diskcache['chunk'],
                     (offset + size + self.diskcache['chunk'] - 1) // self.diskcache['chunk']):
                 idxoffset = idx * self.diskcache['chunk']
                 idxlen = min(self.diskcache['chunk'], info['size'] - idxoffset)
                 key = '%s-%d-%d' % (info['hash'], idxoffset, idxlen)
                 try:
                     data = self.diskcache['cache'].get(key, None, read=True)
+                    if data is not None:
+                        self.diskcache['hits'] += 1
                 except Exception:
                     logger.exception('diskcache threw an exception in get')
                     data = None
                 if data is None:
                     with info['lock']:
                         if 'handle' not in info:
                             info['handle'] = httpio.open(info['url'], allow_redirects=True)
                         handle = info['handle']
                         handle.seek(idxoffset)
                         data = handle.read(idxlen)
+                        self.diskcache['miss'] += 1
+                        self.diskcache['bytesread'] += len(data)
                     try:
                         self.diskcache['cache'][key] = data
                     except Exception:
                         logger.exception('diskcache threw an exception in set')
                 if isinstance(data, bytes):
                     result += data[max(0, offset - idxoffset):
                                    min(len(data), offset + size - idxoffset)]
                 else:
                     data.seek(max(0, offset - idxoffset))
                     result += data.read(size - len(result))
+            self._mount_stats['bytesread'] += len(result)
             return result
         with info['lock']:
             if 'handle' not in info:
                 info['handle'] = httpio.open(info['url'], allow_redirects=True)
             handle = info['handle']
             handle.seek(offset)
+            self._mount_stats['bytesread'] += size
             return handle.read(size)
 
     def readdir(self, path, fh):
         """
         Get a list of names within a directory.
 
         :param path: path within the fuse.
         :param fh: an open file handle.  Ignored, since path is always
             specified.
         :returns: a list of names.  This always includes . and ..
         """
+        self._mount_stats['dir'] += 1
         path = path.rstrip('/')
         result = ['.', '..']
         if path == '':
-            result.extend(['collection', 'user'])
+            result.extend(['collection', 'user', 'stats'])
         elif path in ('/user', '/collection'):
             try:
                 if path == '/user':
                     logger.debug('listUser')
                     for doc in self.gc.listUser():
                         result.append(self._name(doc, 'user'))
                 else:
@@ -413,14 +462,18 @@
         Open a path and return a descriptor.
 
         :param path: path within the fuse.
         :param flags: a combination of O_* flags.  This will fail if it is not
             read only.
         :returns: a file descriptor.
         """
+        if path.rstrip('/') == '/stats':
+            fh = self.nextFH
+            self.nextFH += 1
+            return fh
         resource = self._get_path(path)
         if resource['model'] == 'item' and self.flatten:
             files = list(self.gc.listFile(resource['document']['_id'], limit=2))
             if len(files) == 1 and files[0]['name'] == resource['document']['name']:
                 resource = {'document': files[0], 'model': files[0]['_modelType']}
         if resource['model'] != 'file':
             return super().open(path, flags)
@@ -447,14 +500,15 @@
             with httpio.open(info['url']) as f:
                 f.seek(0, os.SEEK_END)
                 info['size'] = f.tell()
         with self.openFilesLock:
             fh = self.nextFH
             self.nextFH += 1
             self.openFiles[fh] = info
+            self._mount_stats['open'] += 1
         return fh
 
     def release(self, path, fh):
         """
         Release an open file handle.
 
         :param path: path within the fuse.
@@ -464,14 +518,15 @@
         with self.openFilesLock:
             if fh in self.openFiles:
                 with self.openFiles[fh]['lock']:
                     if 'handle' in self.openFiles[fh]:
                         self.openFiles[fh]['handle'].close()
                         del self.openFiles[fh]['handle']
                     del self.openFiles[fh]
+                    self._mount_stats['release'] += 1
             else:
                 return super().release(path, fh)
         return 0
 
     def destroy(self, path):
         """
         Handle shutdown of the FUSE.
```

### Comparing `girder_client_mount-0.3.3.dev1/girder_client_mount.egg-info/PKG-INFO` & `girder_client_mount-0.3.3.dev3/girder_client_mount.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder_client_mount
-Version: 0.3.3.dev1
+Version: 0.3.3.dev3
 Summary: Mount a girder server via fuse
 Home-page: https://github.com/DigitalSlideArchive/girder-client-mount
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder,fuse,girder-client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `girder_client_mount-0.3.3.dev1/setup.py` & `girder_client_mount-0.3.3.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `girder_client_mount-0.3.3.dev1/tox.ini` & `girder_client_mount-0.3.3.dev3/tox.ini`

 * *Files identical despite different names*

