# Comparing `tmp/torrentp-0.1.7.tar.gz` & `tmp/torrentp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentp-0.1.7.tar", last modified: Sun Feb 25 14:41:46 2024, max compression
+gzip compressed data, was "torrentp-0.1.9.tar", last modified: Mon Apr  1 11:42:31 2024, max compression
```

## Comparing `torrentp-0.1.7.tar` & `torrentp-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:41:46.091280 torrentp-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-02-25 14:41:38.000000 torrentp-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-02-25 14:41:46.091280 torrentp-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-25 14:41:38.000000 torrentp-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 14:41:46.091280 torrentp-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-25 14:41:38.000000 torrentp-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:41:46.091280 torrentp-0.1.7/torrentp/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-25 14:41:38.000000 torrentp-0.1.7/torrentp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-25 14:41:38.000000 torrentp-0.1.7/torrentp/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-25 14:41:38.000000 torrentp-0.1.7/torrentp/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-25 14:41:38.000000 torrentp-0.1.7/torrentp/torrent_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-25 14:41:38.000000 torrentp-0.1.7/torrentp/torrent_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 14:41:46.091280 torrentp-0.1.7/torrentp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-02-25 14:41:46.000000 torrentp-0.1.7/torrentp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 14:41:46.000000 torrentp-0.1.7/torrentp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 14:41:46.000000 torrentp-0.1.7/torrentp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-25 14:41:46.000000 torrentp-0.1.7/torrentp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-25 14:41:46.000000 torrentp-0.1.7/torrentp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:42:31.953215 torrentp-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-04-01 11:42:28.000000 torrentp-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-01 11:42:31.953215 torrentp-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-01 11:42:28.000000 torrentp-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:42:31.953215 torrentp-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-01 11:42:28.000000 torrentp-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:42:31.953215 torrentp-0.1.9/torrentp/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/torrent_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 11:42:28.000000 torrentp-0.1.9/torrentp/torrent_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:42:31.953215 torrentp-0.1.9/torrentp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 11:42:31.000000 torrentp-0.1.9/torrentp.egg-info/top_level.txt
```

### Comparing `torrentp-0.1.7/LICENSE` & `torrentp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentp-0.1.7/setup.py` & `torrentp-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     long_description=README,
     long_description_content_type="text/markdown",
     url=get_property('__url__'),
     author=get_property('__author__'),
     author_email=get_property('__author_email__'),
     license=get_property('__license__'),
     packages=['torrentp'],
-    install_requires=['libtorrent>=2.0.7', ],
+    entry_points={
+        'console_scripts': ['torrentp=torrentp.cli:run_cli']
+    },
+    install_requires=['libtorrent>=2.0.7', 'asyncclick>=8.1.7.2', ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 2.7',
```

### Comparing `torrentp-0.1.7/torrentp/__init__.py` & `torrentp-0.1.9/torrentp/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "0.1.7"
+__version__ = "0.1.9"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `torrentp-0.1.7/torrentp/session.py` & `torrentp-0.1.9/torrentp/session.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.1.7/torrentp/torrent_downloader.py` & `torrentp-0.1.9/torrentp/torrent_downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,25 @@
         self._add_torrent_params = None
         self._session = Session(self._lt)
 
     async def start_download(self, download_speed=0, upload_speed=0):
         if self._file_path.startswith('magnet:'):
             self._add_torrent_params = self._lt.parse_magnet_uri(self._file_path)
             self._add_torrent_params.save_path = self._save_path
-            self._downloader = Downloader(session=self._session(), torrent_info=self._add_torrent_params,
-                                          save_path=self._save_path, libtorrent=lt, is_magnet=True)
+            self._downloader = Downloader(
+                session=self._session(), torrent_info=self._add_torrent_params, 
+                save_path=self._save_path, libtorrent=lt, is_magnet=True
+            )
 
         else:
             self._torrent_info = TorrentInfo(self._file_path, self._lt)
-            self._downloader = Downloader(session=self._session(), torrent_info=self._torrent_info(),
-                                          save_path=self._save_path, libtorrent=None, is_magnet=False)
+            self._downloader = Downloader(
+                session=self._session(), torrent_info=self._torrent_info(), 
+                save_path=self._save_path, libtorrent=None, is_magnet=False
+            )
 
         self._session.set_download_limit(download_speed)
         self._session.set_upload_limit(upload_speed)
 
         self._file = self._downloader
         await self._file.download()
```

