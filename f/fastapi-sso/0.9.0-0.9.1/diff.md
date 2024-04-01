# Comparing `tmp/fastapi_sso-0.9.0.tar.gz` & `tmp/fastapi_sso-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sso-0.9.0.tar", max compression
+gzip compressed data, was "fastapi_sso-0.9.1.tar", max compression
```

## Comparing `fastapi_sso-0.9.0.tar` & `fastapi_sso-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1093 2023-11-24 18:46:58.765601 fastapi_sso-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     3305 2023-11-24 18:46:58.765601 fastapi_sso-0.9.0/README.md
--rw-r--r--   0        0        0      552 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/py.typed
--rw-r--r--   0        0        0        0 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/__init__.py
--rw-r--r--   0        0        0    14018 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/base.py
--rw-r--r--   0        0        0     1327 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/facebook.py
--rw-r--r--   0        0        0     1258 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/fitbit.py
--rw-r--r--   0        0        0     2625 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/generic.py
--rw-r--r--   0        0        0     1693 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/github.py
--rw-r--r--   0        0        0     1032 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/gitlab.py
--rw-r--r--   0        0        0     1380 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/google.py
--rw-r--r--   0        0        0      864 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/kakao.py
--rw-r--r--   0        0        0     1914 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/microsoft.py
--rw-r--r--   0        0        0      901 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/naver.py
--rw-r--r--   0        0        0     1250 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/fastapi_sso/sso/spotify.py
--rw-r--r--   0        0        0     2092 2023-11-24 18:46:58.769601 fastapi_sso-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 fastapi_sso-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-12-04 22:24:53.860932 fastapi_sso-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0     3311 2023-12-04 22:24:53.860932 fastapi_sso-0.9.1/README.md
+-rw-r--r--   0        0        0      552 2023-12-04 22:24:53.860932 fastapi_sso-0.9.1/fastapi_sso/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-04 22:24:53.860932 fastapi_sso-0.9.1/fastapi_sso/py.typed
+-rw-r--r--   0        0        0        0 2023-12-04 22:24:53.860932 fastapi_sso-0.9.1/fastapi_sso/sso/__init__.py
+-rw-r--r--   0        0        0    14032 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/base.py
+-rw-r--r--   0        0        0     1327 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/facebook.py
+-rw-r--r--   0        0        0     1258 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/fitbit.py
+-rw-r--r--   0        0        0     2625 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/generic.py
+-rw-r--r--   0        0        0     1693 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/github.py
+-rw-r--r--   0        0        0     1032 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/gitlab.py
+-rw-r--r--   0        0        0     1380 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/google.py
+-rw-r--r--   0        0        0      864 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/kakao.py
+-rw-r--r--   0        0        0     1918 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/microsoft.py
+-rw-r--r--   0        0        0      901 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/naver.py
+-rw-r--r--   0        0        0     1250 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/fastapi_sso/sso/spotify.py
+-rw-r--r--   0        0        0     2136 2023-12-04 22:24:53.864932 fastapi_sso-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 fastapi_sso-0.9.1/PKG-INFO
```

### Comparing `fastapi_sso-0.9.0/LICENSE.md` & `fastapi_sso-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/README.md` & `fastapi_sso-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 - Google
 - Microsoft
 - Facebook
 - Spotify
 - Fitbit
 - Github (credits to [Brandl](https://github.com/Brandl) for hint using `accept` header)
-- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/generic.html))
+- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/reference/sso.generic/))
 
 ### Contributed
 
 - Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor))
 - Naver (by 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92)
 - Gitlab (by Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84)
```

#### html2text {}

```diff
@@ -25,16 +25,16 @@
 preferred way of using the SSO instances is to use `with` statement, which will
 ensure the state is cleared. See example below. ## Support this project If
 you'd like to support this project, consider [buying me a coffee â](https://
 www.buymeacoffee.com/tomas.votava). I tend to process Pull Requests faster when
 properly caffeinated ð. _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]## Supported login providers ###
 Official - Google - Microsoft - Facebook - Spotify - Fitbit - Github (credits
 to [Brandl](https://github.com/Brandl) for hint using `accept` header) -
-generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/
-generic.html)) ### Contributed - Kakao (by Jae-Baek Song - [thdwoqor](https://
+generic (see [docs](https://tomasvotava.github.io/fastapi-sso/reference/
+sso.generic/)) ### Contributed - Kakao (by Jae-Baek Song - [thdwoqor](https://
 github.com/thdwoqor)) - Naver (by 1tang2bang92) - [1tang2bang92](https://
 github.com/1tang2bang92) - Gitlab (by Alessandro Pischedda) - [Cereal84](https:
 //github.com/Cereal84) See [Contributing](#contributing) for a guide on how to
 contribute your own login provider. ## Installation ### Install using `pip`
 ```console pip install fastapi-sso ``` ### Install using `poetry` ```console
 poetry add fastapi-sso ``` ## Contributing If you'd like to contribute and add
 your specific login provider, please see [Contributing](https://
```

### Comparing `fastapi_sso-0.9.0/fastapi_sso/__init__.py` & `fastapi_sso-0.9.1/fastapi_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/base.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
 
 
 class OpenID(pydantic.BaseModel):  # pylint: disable=no-member
     """Class (schema) to represent information got from sso provider in a common form."""
 
     id: Optional[str] = None
-    email: Optional[str] = None
+    email: Optional[pydantic.EmailStr] = None
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     display_name: Optional[str] = None
     picture: Optional[str] = None
     provider: Optional[str] = None
```

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/facebook.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/fitbit.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/fitbit.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/generic.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/generic.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/github.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/github.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/gitlab.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/gitlab.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/google.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/google.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/kakao.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/kakao.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/microsoft.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/microsoft.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,13 +44,13 @@
             "token_endpoint": f"https://login.microsoftonline.com/{self.tenant}/oauth2/v2.0/token",
             "userinfo_endpoint": f"https://graph.microsoft.com/{self.version}/me",
         }
 
     async def openid_from_response(self, response: dict, session: Optional["httpx.AsyncClient"] = None) -> OpenID:
         return OpenID(
             email=response.get("mail"),
-            display_name=response["displayName"],
+            display_name=response.get("displayName"),
             provider=self.provider,
             id=response.get("id"),
             first_name=response.get("givenName"),
             last_name=response.get("surname"),
         )
```

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/naver.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/naver.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/fastapi_sso/sso/spotify.py` & `fastapi_sso-0.9.1/fastapi_sso/sso/spotify.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.9.0/pyproject.toml` & `fastapi_sso-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 [tool.poetry]
 name = "fastapi-sso"
-version = "0.9.0"
+version = "0.9.1"
 description = "FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)"
 authors = ["Tomas Votava <info@tomasvotava.eu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/tomasvotava/fastapi-sso"
 homepage = "https://tomasvotava.github.io/fastapi-sso/"
 documentation = "https://tomasvotava.github.io/fastapi-sso/"
 keywords = ["fastapi", "sso", "oauth", "google", "facebook", "spotify"]
 include = ["fastapi_sso/py.typed"]
 
+
 [tool.pytest.ini_options]
 testpaths = ["tests/"]
 asyncio_mode = "auto"
 addopts = [
     "-v",
     "--cov=fastapi_sso",
     "--cov-report=xml:coverage.xml",
     "--cov-report=json:coverage.json",
     "--cov-report=term-missing",
     "-n",
     "auto",
 ]
 
+
+[tool.black]
+line_length = 120
+
+
 [tool.poe.tasks]
 pylint = "pylint --disable fixme --rcfile .pylintrc fastapi_sso"
 todos = "pylint --disable all --enable fixme --rcfile .pylintrc fastapi_sso"
 black = "black fastapi_sso"
 isort = "isort --settings-path .isort.cfg fastapi_sso"
 mypy = "mypy --config-file mypy.ini fastapi_sso"
 black-check = "black --check fastapi_sso"
@@ -40,35 +46,32 @@
 test = "pytest"
 coverage = "coverage report"
 
 docs = "mkdocs build --clean"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7.0"
-pylint = ">=2,<4"
-uvicorn = ">=0.23.1"
+isort = "^5"
+markdown-include = "^0.8.1"
+mkdocs-material = { extras = ["imaging"], version = "^9.3.2" }
+mkdocstrings = { extras = ["python"], version = ">=0.23,<0.25" }
 mypy = "^1"
+poethepoet = ">=0.21.1,<0.25.0"
+pre-commit = "^3"
+pylint = ">=2,<4"
 pytest = "^7"
+pytest-asyncio = ">=0.21.1,<0.24.0"
 pytest-cov = "^4"
-tox = "^4"
-poethepoet = ">=0.21.1,<0.25.0"
-isort = "^5"
-pytest-asyncio = "^0.21.1"
 pytest-xdist = "^3"
-pre-commit = "^3"
-mkdocs-material = { extras = ["imaging"], version = "^9.3.2" }
-mkdocstrings = { extras = ["python"], version = ">=0.23,<0.25" }
-markdown-include = "^0.8.1"
-
-[tool.black]
-line_length = 120
+tox = "^4"
+uvicorn = ">=0.23.1"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
 fastapi = ">=0.80"
-oauthlib = ">=3.1.0"
-pydantic = ">=1.8.0"
 httpx = ">=0.23.0"
+oauthlib = ">=3.1.0"
+pydantic = { extras=["email"], version = ">=1.8.0" }
+python = ">=3.8,<4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_sso-0.9.0/PKG-INFO` & `fastapi_sso-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sso
-Version: 0.9.0
+Version: 0.9.1
 Summary: FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)
 Home-page: https://tomasvotava.github.io/fastapi-sso/
 License: MIT
 Keywords: fastapi,sso,oauth,google,facebook,spotify
 Author: Tomas Votava
 Author-email: info@tomasvotava.eu
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.80)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: oauthlib (>=3.1.0)
-Requires-Dist: pydantic (>=1.8.0)
+Requires-Dist: pydantic[email] (>=1.8.0)
 Project-URL: Documentation, https://tomasvotava.github.io/fastapi-sso/
 Project-URL: Repository, https://github.com/tomasvotava/fastapi-sso
 Description-Content-Type: text/markdown
 
 # FastAPI SSO
 
 ![Supported Python Versions](https://img.shields.io/pypi/pyversions/fastapi-sso)
@@ -70,15 +70,15 @@
 
 - Google
 - Microsoft
 - Facebook
 - Spotify
 - Fitbit
 - Github (credits to [Brandl](https://github.com/Brandl) for hint using `accept` header)
-- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/sso/generic.html))
+- generic (see [docs](https://tomasvotava.github.io/fastapi-sso/reference/sso.generic/))
 
 ### Contributed
 
 - Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor))
 - Naver (by 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92)
 - Gitlab (by Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84)
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: fastapi-sso Version: 0.9.0 Summary: FastAPI plugin
+Metadata-Version: 2.1 Name: fastapi-sso Version: 0.9.1 Summary: FastAPI plugin
 to enable SSO to most common providers (such as Facebook login, Google login
 and login via Microsoft Office 365 Account) Home-page: https://
 tomasvotava.github.io/fastapi-sso/ License: MIT Keywords:
 fastapi,sso,oauth,google,facebook,spotify Author: Tomas Votava Author-email:
 info@tomasvotava.eu Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: fastapi (>=0.80) Requires-Dist: httpx
-(>=0.23.0) Requires-Dist: oauthlib (>=3.1.0) Requires-Dist: pydantic (>=1.8.0)
-Project-URL: Documentation, https://tomasvotava.github.io/fastapi-sso/ Project-
-URL: Repository, https://github.com/tomasvotava/fastapi-sso Description-
-Content-Type: text/markdown # FastAPI SSO ![Supported Python Versions](https://
-img.shields.io/pypi/pyversions/fastapi-sso) [![Test coverage](https://
-codecov.io/gh/tomasvotava/fastapi-sso/graph/badge.svg?token=SIFCTVSSOS)](https:
-//codecov.io/gh/tomasvotava/fastapi-sso) ![Tests Workflow Status](https://
-img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/
-test.yml?label=tests) ![Pylint Workflow Status](https://img.shields.io/github/
-actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=pylint) ![Mypy
+(>=0.23.0) Requires-Dist: oauthlib (>=3.1.0) Requires-Dist: pydantic[email]
+(>=1.8.0) Project-URL: Documentation, https://tomasvotava.github.io/fastapi-
+sso/ Project-URL: Repository, https://github.com/tomasvotava/fastapi-sso
+Description-Content-Type: text/markdown # FastAPI SSO ![Supported Python
+Versions](https://img.shields.io/pypi/pyversions/fastapi-sso) [![Test coverage]
+(https://codecov.io/gh/tomasvotava/fastapi-sso/graph/
+badge.svg?token=SIFCTVSSOS)](https://codecov.io/gh/tomasvotava/fastapi-sso) !
+[Tests Workflow Status](https://img.shields.io/github/actions/workflow/status/
+tomasvotava/fastapi-sso/test.yml?label=tests) ![Pylint Workflow Status](https:/
+/img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/
+lint.yml?label=pylint) ![Mypy Workflow Status](https://img.shields.io/github/
+actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=mypy) ![Black
 Workflow Status](https://img.shields.io/github/actions/workflow/status/
-tomasvotava/fastapi-sso/lint.yml?label=mypy) ![Black Workflow Status](https://
-img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/
-lint.yml?label=black) ![CodeQL Workflow Status](https://img.shields.io/github/
-actions/workflow/status/tomasvotava/fastapi-sso/codeql-
+tomasvotava/fastapi-sso/lint.yml?label=black) ![CodeQL Workflow Status](https:/
+/img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/codeql-
 analysis.yml?label=CodeQL) ![PyPi weekly downloads](https://img.shields.io/
 pypi/dw/fastapi-sso) ![Project License](https://img.shields.io/github/license/
 tomasvotava/fastapi-sso) ![PyPi Version](https://img.shields.io/pypi/v/fastapi-
 sso) FastAPI plugin to enable SSO to most common providers (such as Facebook
 login, Google login and login via Microsoft Office 365 account). This allows
 you to implement the famous `Login with Google/Facebook/Microsoft` buttons
 functionality on your backend very easily. **Documentation**: [https://
@@ -40,16 +40,16 @@
 instances is to use `with` statement, which will ensure the state is cleared.
 See example below. ## Support this project If you'd like to support this
 project, consider [buying me a coffee â](https://www.buymeacoffee.com/
 tomas.votava). I tend to process Pull Requests faster when properly caffeinated
 ð. _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]## Supported login providers ### Official - Google -
 Microsoft - Facebook - Spotify - Fitbit - Github (credits to [Brandl](https://
 github.com/Brandl) for hint using `accept` header) - generic (see [docs](https:
-//tomasvotava.github.io/fastapi-sso/sso/generic.html)) ### Contributed - Kakao
-(by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
+//tomasvotava.github.io/fastapi-sso/reference/sso.generic/)) ### Contributed -
+Kakao (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92) - Gitlab (by
 Alessandro Pischedda) - [Cereal84](https://github.com/Cereal84) See
 [Contributing](#contributing) for a guide on how to contribute your own login
 provider. ## Installation ### Install using `pip` ```console pip install
 fastapi-sso ``` ### Install using `poetry` ```console poetry add fastapi-sso
 ``` ## Contributing If you'd like to contribute and add your specific login
 provider, please see [Contributing](https://tomasvotava.github.io/fastapi-sso/
```

