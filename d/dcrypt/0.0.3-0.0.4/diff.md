# Comparing `tmp/dcrypt-0.0.3.tar.gz` & `tmp/dcrypt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrypt-0.0.3.tar", last modified: Mon Mar 25 17:04:54 2024, max compression
+gzip compressed data, was "dcrypt-0.0.4.tar", last modified: Mon Apr  1 19:12:50 2024, max compression
```

## Comparing `dcrypt-0.0.3.tar` & `dcrypt-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 17:04:54.085119 dcrypt-0.0.3/
--rw-rw-rw-   0        0        0     1104 2024-03-25 17:01:41.000000 dcrypt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    11520 2024-03-25 17:04:54.085119 dcrypt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10317 2024-01-01 18:33:14.000000 dcrypt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 17:04:53.888298 dcrypt-0.0.3/dcrypt/
--rw-rw-rw-   0        0        0      587 2024-03-25 16:51:25.000000 dcrypt-0.0.3/dcrypt/__init__.py
--rw-rw-rw-   0        0        0     1227 2024-03-25 16:46:41.000000 dcrypt-0.0.3/dcrypt/base.py
--rw-rw-rw-   0        0        0     8554 2024-03-25 16:50:08.000000 dcrypt-0.0.3/dcrypt/cryptkey.py
--rw-rw-rw-   0        0        0      247 2023-12-28 20:16:41.000000 dcrypt-0.0.3/dcrypt/exceptions.py
--rw-rw-rw-   0        0        0     1493 2024-01-10 18:27:14.000000 dcrypt-0.0.3/dcrypt/json.py
--rw-rw-rw-   0        0        0     9741 2024-01-01 17:48:11.000000 dcrypt-0.0.3/dcrypt/object.py
--rw-rw-rw-   0        0        0     5818 2024-03-25 16:24:51.000000 dcrypt-0.0.3/dcrypt/signature.py
--rw-rw-rw-   0        0        0     1774 2023-12-31 13:34:08.000000 dcrypt-0.0.3/dcrypt/text.py
-drwxrwxrwx   0        0        0        0 2024-03-25 17:04:54.085119 dcrypt-0.0.3/dcrypt.egg-info/
--rw-rw-rw-   0        0        0    11520 2024-03-25 17:04:53.000000 dcrypt-0.0.3/dcrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2024-03-25 17:04:53.000000 dcrypt-0.0.3/dcrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 17:04:53.000000 dcrypt-0.0.3/dcrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-03-25 17:04:53.000000 dcrypt-0.0.3/dcrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-25 17:04:53.000000 dcrypt-0.0.3/dcrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1443 2024-03-25 17:03:47.000000 dcrypt-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-25 17:04:54.085119 dcrypt-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-25 17:04:54.069502 dcrypt-0.0.3/tests/
--rw-rw-rw-   0        0        0     1218 2024-01-10 18:32:54.000000 dcrypt-0.0.3/tests/test_common_signature.py
--rw-rw-rw-   0        0        0     1320 2024-01-10 18:33:41.000000 dcrypt-0.0.3/tests/test_cryptkey.py
--rw-rw-rw-   0        0        0     1196 2024-01-10 18:33:47.000000 dcrypt-0.0.3/tests/test_json_crypt.py
--rw-rw-rw-   0        0        0     3951 2024-01-10 18:33:53.000000 dcrypt-0.0.3/tests/test_object_crypt.py
--rw-rw-rw-   0        0        0     1214 2024-01-10 18:33:59.000000 dcrypt-0.0.3/tests/test_signature.py
--rw-rw-rw-   0        0        0     2055 2024-01-10 18:34:12.000000 dcrypt-0.0.3/tests/test_text_crypt.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:12:50.570185 dcrypt-0.0.4/
+-rw-rw-rw-   0        0        0     1104 2024-03-25 17:01:41.000000 dcrypt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    11520 2024-04-01 19:12:50.570185 dcrypt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10317 2024-01-01 18:33:14.000000 dcrypt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 19:12:50.394275 dcrypt-0.0.4/dcrypt/
+-rw-rw-rw-   0        0        0      587 2024-04-01 19:05:41.000000 dcrypt-0.0.4/dcrypt/__init__.py
+-rw-rw-rw-   0        0        0     1227 2024-03-25 16:46:41.000000 dcrypt-0.0.4/dcrypt/base.py
+-rw-rw-rw-   0        0        0     8554 2024-03-25 16:50:08.000000 dcrypt-0.0.4/dcrypt/cryptkey.py
+-rw-rw-rw-   0        0        0      247 2023-12-28 20:16:41.000000 dcrypt-0.0.4/dcrypt/exceptions.py
+-rw-rw-rw-   0        0        0     1493 2024-01-10 18:27:14.000000 dcrypt-0.0.4/dcrypt/json.py
+-rw-rw-rw-   0        0        0     9741 2024-01-01 17:48:11.000000 dcrypt-0.0.4/dcrypt/object.py
+-rw-rw-rw-   0        0        0     5818 2024-03-25 16:24:51.000000 dcrypt-0.0.4/dcrypt/signature.py
+-rw-rw-rw-   0        0        0     1774 2023-12-31 13:34:08.000000 dcrypt-0.0.4/dcrypt/text.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:12:50.567670 dcrypt-0.0.4/dcrypt.egg-info/
+-rw-rw-rw-   0        0        0    11520 2024-04-01 19:12:50.000000 dcrypt-0.0.4/dcrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2024-04-01 19:12:50.000000 dcrypt-0.0.4/dcrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:12:50.000000 dcrypt-0.0.4/dcrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-01 19:12:50.000000 dcrypt-0.0.4/dcrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 19:12:50.000000 dcrypt-0.0.4/dcrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1443 2024-04-01 19:04:39.000000 dcrypt-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:12:50.578223 dcrypt-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 19:12:50.563801 dcrypt-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1218 2024-01-10 18:32:54.000000 dcrypt-0.0.4/tests/test_common_signature.py
+-rw-rw-rw-   0        0        0     1320 2024-01-10 18:33:41.000000 dcrypt-0.0.4/tests/test_cryptkey.py
+-rw-rw-rw-   0        0        0     1196 2024-01-10 18:33:47.000000 dcrypt-0.0.4/tests/test_json_crypt.py
+-rw-rw-rw-   0        0        0     3951 2024-01-10 18:33:53.000000 dcrypt-0.0.4/tests/test_object_crypt.py
+-rw-rw-rw-   0        0        0     1214 2024-01-10 18:33:59.000000 dcrypt-0.0.4/tests/test_signature.py
+-rw-rw-rw-   0        0        0     2055 2024-01-10 18:34:12.000000 dcrypt-0.0.4/tests/test_text_crypt.py
```

### Comparing `dcrypt-0.0.3/LICENSE` & `dcrypt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/PKG-INFO` & `dcrypt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encrypt text and Python objects using RSA + Fernet encryption.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/dcrypt
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/dcrypt/issues
 Project-URL: Repository, https://github.com/ti-oluwa/dcrypt
 Keywords: encryption,decryption,rsa,fernet,encrypt,decrypt,encryptor,decryptor,encrypter,decrypter,encrypting,decrypting,encryptors,decryptors,encrypters,decrypters,cryptography
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==41.0.4
-Requires-Dist: rsa==4.9
+Requires-Dist: cryptography>=41.0.4
+Requires-Dist: rsa>=4.9
 Requires-Dist: simple_file_handler>=0.0.1
 
 ## dcrypt
 
 Use RSA + Fernet encryption to encrypt and decrypt text and Python objects.
 
 ## Installation
```

### Comparing `dcrypt-0.0.3/README.md` & `dcrypt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/__init__.py` & `dcrypt-0.0.4/dcrypt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 from .cryptkey import CryptKey
 from .text import TextCrypt
 from .object import ObjectCrypt
 from .json import JSONCrypt
 from .exceptions import EncryptionError, DecryptionError
 
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __all__ = [
     'Signature', 'CommonSignature', 
     'CryptKey', 'TextCrypt', 'ObjectCrypt', 
     'JSONCrypt', 'EncryptionError', 'DecryptionError'
 ]
 __author__ = "Daniel T. Afolayan"
```

### Comparing `dcrypt-0.0.3/dcrypt/base.py` & `dcrypt-0.0.4/dcrypt/base.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/cryptkey.py` & `dcrypt-0.0.4/dcrypt/cryptkey.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/json.py` & `dcrypt-0.0.4/dcrypt/json.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/object.py` & `dcrypt-0.0.4/dcrypt/object.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/signature.py` & `dcrypt-0.0.4/dcrypt/signature.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt/text.py` & `dcrypt-0.0.4/dcrypt/text.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/dcrypt.egg-info/PKG-INFO` & `dcrypt-0.0.4/dcrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encrypt text and Python objects using RSA + Fernet encryption.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/dcrypt
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/dcrypt/issues
 Project-URL: Repository, https://github.com/ti-oluwa/dcrypt
 Keywords: encryption,decryption,rsa,fernet,encrypt,decrypt,encryptor,decryptor,encrypter,decrypter,encrypting,decrypting,encryptors,decryptors,encrypters,decrypters,cryptography
@@ -16,16 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==41.0.4
-Requires-Dist: rsa==4.9
+Requires-Dist: cryptography>=41.0.4
+Requires-Dist: rsa>=4.9
 Requires-Dist: simple_file_handler>=0.0.1
 
 ## dcrypt
 
 Use RSA + Fernet encryption to encrypt and decrypt text and Python objects.
 
 ## Installation
```

### Comparing `dcrypt-0.0.3/pyproject.toml` & `dcrypt-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Natural Language :: English",
     "Typing :: Typed",
 ]
 dependencies = [
-  "cryptography==41.0.4",
-  "rsa==4.9",
+  "cryptography>=41.0.4",
+  "rsa>=4.9",
   "simple_file_handler>=0.0.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ti-oluwa/dcrypt"
 "Bug Tracker" = "https://github.com/ti-oluwa/dcrypt/issues"
 "Repository" = "https://github.com/ti-oluwa/dcrypt"
```

### Comparing `dcrypt-0.0.3/tests/test_common_signature.py` & `dcrypt-0.0.4/tests/test_common_signature.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/tests/test_cryptkey.py` & `dcrypt-0.0.4/tests/test_cryptkey.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/tests/test_json_crypt.py` & `dcrypt-0.0.4/tests/test_json_crypt.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/tests/test_object_crypt.py` & `dcrypt-0.0.4/tests/test_object_crypt.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/tests/test_signature.py` & `dcrypt-0.0.4/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `dcrypt-0.0.3/tests/test_text_crypt.py` & `dcrypt-0.0.4/tests/test_text_crypt.py`

 * *Files identical despite different names*

