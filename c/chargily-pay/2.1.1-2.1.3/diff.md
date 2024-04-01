# Comparing `tmp/chargily_pay-2.1.1.tar.gz` & `tmp/chargily_pay-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chargily_pay-2.1.1.tar", last modified: Mon Mar 11 19:05:33 2024, max compression
+gzip compressed data, was "chargily_pay-2.1.3.tar", last modified: Sat Mar 30 21:26:13 2024, max compression
```

## Comparing `chargily_pay-2.1.1.tar` & `chargily_pay-2.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.977256 chargily_pay-2.1.1/.github/
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/.github/workflows/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      624 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/.github/workflows/django.yml
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     1144 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/.github/workflows/python-publish.yml
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       77 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/.gitignore
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/.vscode/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      265 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/.vscode/settings.json
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     1061 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/LICENSE
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       34 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/MANIFEST.in
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      138 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/Makefile
--rw-r--r--   0 tarek     (1000) tarek     (1000)     6301 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/PKG-INFO
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     5908 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/README.md
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      592 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/dev_requirements.txt
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/docs/
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/docs/examples/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     5980 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/docs/examples/django.md
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/docs/reference/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     7881 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/docs/reference/api.md
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     2394 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/docs/reference/entity.md
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     8288 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/docs/usage.md
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      682 2024-03-11 19:05:20.000000 chargily_pay-2.1.1/pyproject.toml
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      188 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/requirements.txt
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       38 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/setup.cfg
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.981256 chargily_pay-2.1.1/src/
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/src/chargily_pay/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       31 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/src/chargily_pay/__init__.py
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     9921 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/src/chargily_pay/api.py
--rw-rw-r--   0 tarek     (1000) tarek     (1000)     1845 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/src/chargily_pay/entity.py
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      112 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/src/chargily_pay/settings.py
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/src/chargily_pay.egg-info/
--rw-r--r--   0 tarek     (1000) tarek     (1000)     6301 2024-03-11 19:05:33.000000 chargily_pay-2.1.1/src/chargily_pay.egg-info/PKG-INFO
--rw-rw-r--   0 tarek     (1000) tarek     (1000)      601 2024-03-11 19:05:33.000000 chargily_pay-2.1.1/src/chargily_pay.egg-info/SOURCES.txt
--rw-rw-r--   0 tarek     (1000) tarek     (1000)        1 2024-03-11 19:05:33.000000 chargily_pay-2.1.1/src/chargily_pay.egg-info/dependency_links.txt
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       15 2024-03-11 19:05:33.000000 chargily_pay-2.1.1/src/chargily_pay.egg-info/requires.txt
--rw-rw-r--   0 tarek     (1000) tarek     (1000)       13 2024-03-11 19:05:33.000000 chargily_pay-2.1.1/src/chargily_pay.egg-info/top_level.txt
-drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-11 19:05:33.985255 chargily_pay-2.1.1/tests/
--rw-rw-r--   0 tarek     (1000) tarek     (1000)    18098 2024-03-11 18:49:11.000000 chargily_pay-2.1.1/tests/test_api.py
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.596697 chargily_pay-2.1.3/
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.584696 chargily_pay-2.1.3/.github/
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.588697 chargily_pay-2.1.3/.github/workflows/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      624 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/.github/workflows/django.yml
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     1144 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/.github/workflows/python-publish.yml
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       77 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/.gitignore
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.588697 chargily_pay-2.1.3/.vscode/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      265 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/.vscode/settings.json
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     1061 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/LICENSE
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       34 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/MANIFEST.in
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      138 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/Makefile
+-rw-r--r--   0 tarek     (1000) tarek     (1000)     6367 2024-03-30 21:26:13.596697 chargily_pay-2.1.3/PKG-INFO
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     5974 2024-03-30 19:27:47.000000 chargily_pay-2.1.3/README.md
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      592 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/dev_requirements.txt
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.588697 chargily_pay-2.1.3/docs/
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.588697 chargily_pay-2.1.3/docs/examples/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     5980 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/docs/examples/django.md
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.592697 chargily_pay-2.1.3/docs/reference/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     7881 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/docs/reference/api.md
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     2394 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/docs/reference/entity.md
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     8288 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/docs/usage.md
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      682 2024-03-30 19:27:40.000000 chargily_pay-2.1.3/pyproject.toml
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      188 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/requirements.txt
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       38 2024-03-30 21:26:13.596697 chargily_pay-2.1.3/setup.cfg
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.584696 chargily_pay-2.1.3/src/
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.592697 chargily_pay-2.1.3/src/chargily_pay/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       31 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/src/chargily_pay/__init__.py
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     9945 2024-03-30 19:17:10.000000 chargily_pay-2.1.3/src/chargily_pay/api.py
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)     1851 2024-03-30 17:42:10.000000 chargily_pay-2.1.3/src/chargily_pay/entity.py
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      112 2024-03-11 18:49:11.000000 chargily_pay-2.1.3/src/chargily_pay/settings.py
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.592697 chargily_pay-2.1.3/src/chargily_pay.egg-info/
+-rw-r--r--   0 tarek     (1000) tarek     (1000)     6367 2024-03-30 21:26:13.000000 chargily_pay-2.1.3/src/chargily_pay.egg-info/PKG-INFO
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)      601 2024-03-30 21:26:13.000000 chargily_pay-2.1.3/src/chargily_pay.egg-info/SOURCES.txt
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)        1 2024-03-30 21:26:13.000000 chargily_pay-2.1.3/src/chargily_pay.egg-info/dependency_links.txt
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       15 2024-03-30 21:26:13.000000 chargily_pay-2.1.3/src/chargily_pay.egg-info/requires.txt
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)       13 2024-03-30 21:26:13.000000 chargily_pay-2.1.3/src/chargily_pay.egg-info/top_level.txt
+drwxrwxr-x   0 tarek     (1000) tarek     (1000)        0 2024-03-30 21:26:13.592697 chargily_pay-2.1.3/tests/
+-rw-rw-r--   0 tarek     (1000) tarek     (1000)    17919 2024-03-30 19:00:50.000000 chargily_pay-2.1.3/tests/test_api.py
```

### Comparing `chargily_pay-2.1.1/.github/workflows/django.yml` & `chargily_pay-2.1.3/.github/workflows/django.yml`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/.github/workflows/python-publish.yml` & `chargily_pay-2.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/LICENSE` & `chargily_pay-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/PKG-INFO` & `chargily_pay-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: chargily_pay
-Version: 2.1.1
+Version: 2.1.3
 Summary: This Plugin is to integrate ePayment gateway with Chargily V2 easily.
 Author-email: Berkane Tarek <tarekg320@gmail.com>
 License: MIT
 Keywords: chargily,api,payment
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31
 
 # Welcome to Python Package Repository
 # for [Chargily Pay](https://chargily.com/business/pay "Chargily Pay")™ Gateway - V2.
 
 Thank you for your interest in Python Package of Chargily Pay™, an open source project by Chargily, a leading fintech company in Algeria specializing in payment solutions and  e-commerce facilitating, this Package is providing the easiest and free way to integrate e-payment API through widespread payment methods in Algeria such as EDAHABIA (Algerie Post) and CIB (SATIM) into your Python/Django projects.
 
 This package is developed by **Tarek Berkane ([tarek-berkane](https://github.com/tarek-berkane))** and is open to contributions from developers like you.
 
+## Requirements
+Chargily-Pay v2 requires `Python 3.8` and above.
+
 ## Installation
 ```bash
 pip install chargily-pay
 ```
 
 ## Usage
 ```python
```

### Comparing `chargily_pay-2.1.1/README.md` & `chargily_pay-2.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Welcome to Python Package Repository
 # for [Chargily Pay](https://chargily.com/business/pay "Chargily Pay")™ Gateway - V2.
 
 Thank you for your interest in Python Package of Chargily Pay™, an open source project by Chargily, a leading fintech company in Algeria specializing in payment solutions and  e-commerce facilitating, this Package is providing the easiest and free way to integrate e-payment API through widespread payment methods in Algeria such as EDAHABIA (Algerie Post) and CIB (SATIM) into your Python/Django projects.
 
 This package is developed by **Tarek Berkane ([tarek-berkane](https://github.com/tarek-berkane))** and is open to contributions from developers like you.
 
+## Requirements
+Chargily-Pay v2 requires `Python 3.8` and above.
+
 ## Installation
 ```bash
 pip install chargily-pay
 ```
 
 ## Usage
 ```python
```

### Comparing `chargily_pay-2.1.1/dev_requirements.txt` & `chargily_pay-2.1.3/dev_requirements.txt`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/docs/examples/django.md` & `chargily_pay-2.1.3/docs/examples/django.md`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/docs/reference/api.md` & `chargily_pay-2.1.3/docs/reference/api.md`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/docs/reference/entity.md` & `chargily_pay-2.1.3/docs/reference/entity.md`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/docs/usage.md` & `chargily_pay-2.1.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/pyproject.toml` & `chargily_pay-2.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chargily_pay"
-version = "2.1.1"
+version = "2.1.3"
 authors = [{ name = "Berkane Tarek", email = "tarekg320@gmail.com" }]
 description = "This Plugin is to integrate ePayment gateway with Chargily V2 easily."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["chargily", "api", "payment"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["requests==2.31"]
 
 [tool.setuptools.packages.find]
 where = ["src"]                                             # ["."] by default
```

### Comparing `chargily_pay-2.1.1/src/chargily_pay/api.py` & `chargily_pay-2.1.3/src/chargily_pay/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hmac
 import hashlib
 from dataclasses import asdict
+from typing import List
 
 import requests
 from requests.compat import urljoin
 
 from .entity import Checkout, Customer, PaymentLink, Price, Product
 from .settings import CHARGILIY_URL
 
@@ -184,15 +185,15 @@
             headers=self.headers,
             json=price_dict,
         )
 
         return response
 
     @response_or_exception
-    def update_price(self, id, metadata: list[dict]):
+    def update_price(self, id, metadata: List[dict]):
         """Update a price"""
 
         response = requests.post(
             urljoin(self.url, f"prices/{id}"),
             headers=self.headers,
             json={"metadata": metadata},
         )
```

### Comparing `chargily_pay-2.1.1/src/chargily_pay/entity.py` & `chargily_pay-2.1.3/src/chargily_pay/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Optional, List
 
 
 @dataclass
 class Address:
     country: Optional[str] = ""
     state: Optional[str] = ""
     address: Optional[str] = ""
@@ -11,31 +11,31 @@
 
 @dataclass
 class Customer:
     name: str
     email: str
     phone: Optional[str] = None
     address: Address = None
-    metadata: list = field(default_factory=list)
+    metadata: List = field(default_factory=list)
 
 
 @dataclass
 class Product:
     name: str
     description: Optional[str] = None
-    images: list[str] = None
-    metadata: list[dict] = field(default_factory=list)
+    images: List[str] = None
+    metadata: List[dict] = field(default_factory=list)
 
 
 @dataclass
 class Price:
     amount: int
     currency: str
     product_id: str
-    metadata: list[dict] = field(default_factory=list)
+    metadata: List[dict] = field(default_factory=list)
 
 
 @dataclass
 class CheckoutItem:
     price: str
     quantity: int
 
@@ -49,15 +49,15 @@
     failure_url: str = None
     customer_id: str = None
     description: str = None
     locale: str = None
     payment_method: str = None
     webhook_endpoint: str = None
     pass_fees_to_customer: bool = None
-    metadata: list[dict] = field(default_factory=list)
+    metadata: List[dict] = field(default_factory=list)
 
     def __post_init__(self):
         if not self.items and not self.amount:
             raise Exception("Either items or amount must be provided")
 
         if self.amount:
             if self.amount <= 10:
@@ -72,12 +72,12 @@
     quantity: int
     adjustable_quantity: bool = None
 
 
 @dataclass
 class PaymentLink:
     name: str
-    items: list[PaymentItem]
+    items: List[PaymentItem]
     after_completion_message: str = None
     locale: str = None
     pass_fees_to_customer: bool = None
-    metadata: list[dict] = None
+    metadata: List[dict] = None
```

### Comparing `chargily_pay-2.1.1/src/chargily_pay.egg-info/PKG-INFO` & `chargily_pay-2.1.3/src/chargily_pay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: chargily_pay
-Version: 2.1.1
+Version: 2.1.3
 Summary: This Plugin is to integrate ePayment gateway with Chargily V2 easily.
 Author-email: Berkane Tarek <tarekg320@gmail.com>
 License: MIT
 Keywords: chargily,api,payment
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31
 
 # Welcome to Python Package Repository
 # for [Chargily Pay](https://chargily.com/business/pay "Chargily Pay")™ Gateway - V2.
 
 Thank you for your interest in Python Package of Chargily Pay™, an open source project by Chargily, a leading fintech company in Algeria specializing in payment solutions and  e-commerce facilitating, this Package is providing the easiest and free way to integrate e-payment API through widespread payment methods in Algeria such as EDAHABIA (Algerie Post) and CIB (SATIM) into your Python/Django projects.
 
 This package is developed by **Tarek Berkane ([tarek-berkane](https://github.com/tarek-berkane))** and is open to contributions from developers like you.
 
+## Requirements
+Chargily-Pay v2 requires `Python 3.8` and above.
+
 ## Installation
 ```bash
 pip install chargily-pay
 ```
 
 ## Usage
 ```python
```

### Comparing `chargily_pay-2.1.1/src/chargily_pay.egg-info/SOURCES.txt` & `chargily_pay-2.1.3/src/chargily_pay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chargily_pay-2.1.1/tests/test_api.py` & `chargily_pay-2.1.3/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,21 +463,19 @@
                     quantity=1,
                 )
             ],
         )
         response = self.chargily.create_payment_link(payment_link)
         payment_link_id = response["id"]
         self.assertEqual(response["name"], "Payment link name")
-        try:
-            payment_link.name = "Payment link name 2"
-            response = self.chargily.update_payment_link(payment_link_id, payment_link)
-            self.assertEqual(response["name"], "Payment link name 2")
-            raise Exception("Should fail")
-        except requests.exceptions.HTTPError as err:
-            self.assertEqual(err.response.status_code, 422)
+
+        payment_link.name = "Payment link name 2"
+        response = self.chargily.update_payment_link(payment_link_id, payment_link)
+        self.assertEqual(response["name"], "Payment link name 2")
+
 
     def test_retrieve_payment_link(self):
         product = Product(
             name="Product name",
             description="Product description",
         )
         response = self.chargily.create_product(product)
```

