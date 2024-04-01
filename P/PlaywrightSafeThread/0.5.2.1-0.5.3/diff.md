# Comparing `tmp/PlaywrightSafeThread-0.5.2.1.tar.gz` & `tmp/PlaywrightSafeThread-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlaywrightSafeThread-0.5.2.1.tar", last modified: Mon Mar 25 08:54:30 2024, max compression
+gzip compressed data, was "PlaywrightSafeThread-0.5.3.tar", last modified: Mon Apr  1 15:54:11 2024, max compression
```

## Comparing `PlaywrightSafeThread-0.5.2.1.tar` & `PlaywrightSafeThread-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/threadsafe_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-25 08:54:30.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-25 08:54:30.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:54:30.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-25 08:54:30.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 08:54:30.000000 PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:54:30.339776 PlaywrightSafeThread-0.5.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-25 08:54:26.000000 PlaywrightSafeThread-0.5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26422 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/threadsafe_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/setup.py
```

### Comparing `PlaywrightSafeThread-0.5.2.1/LICENSE` & `PlaywrightSafeThread-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.2.1/PKG-INFO` & `PlaywrightSafeThread-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.2.1
+Version: 0.5.3
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/plawright_shim.py` & `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread/browser/threadsafe_browser.py` & `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 import asyncio
 import platform
 from threading import Thread, Event
 
 from playwright._impl._driver import compute_driver_executable, get_driver_env
 from playwright.async_api import async_playwright, Page, Browser, BrowserType
 
-UNIX = "windows" not in platform.system().lower()
+sys_os = platform.system()
+
+UNIX = "windows" not in sys_os.lower()
 LTE_PY37 = platform.python_version_tuple()[:2] <= ("3", "7")
 
 SUPPORTED_BROWSERS = ("chromium", "firefox", "webkit")
 BrowserName = Literal["chromium", "firefox", "webkit"]
 # T = TypeVar("T")
 # P = ParamSpec("P")
 PageCallable = Callable  # [Concatenate[Page, P], Awaitable[T]]
@@ -404,20 +406,19 @@
         return self
 
     def __exit__(self, *args):
         self.stop()
 
     def check_is_install(self, browser):
         env = self.get_driver_env()
-        k = {}
-        if "win" in sys.platform:
-            k["creationflags"] = subprocess.CREATE_NO_WINDOW
-
         driver_executable = compute_driver_executable()
-        completed_process = subprocess.check_output(f"{driver_executable} install {browser}  --dry-run", env=env, **k, )
+
+        completed_process = subprocess.check_output(f"{driver_executable} install {browser}  --dry-run", env=env,
+                                                    **creation_flags_dict())
+
         locale_ = ":".join(next(filter(lambda x: "Install location" in x,
                                        completed_process.decode().split("\n")), "").split(":")[1:]).strip()
 
         return locale_ and os.path.exists(locale_)
 
     @staticmethod
     def get_driver_env():
@@ -427,70 +428,85 @@
         # NOTE: we do this to deal with pyinstaller
         if getattr(sys, "frozen", False):
             env.setdefault("PLAYWRIGHT_BROWSERS_PATH", "0")
         return env
 
     def run_playwright(self, *args: str):
         env = self.get_driver_env()
-        k = {}
-        if "win" in sys.platform:
-            k["creationflags"] = subprocess.CREATE_NO_WINDOW
-
         driver_executable = compute_driver_executable()
 
         with subprocess.Popen([str(driver_executable), *args], env=env, stdout=subprocess.PIPE,
-                              stderr=subprocess.STDOUT, **k) as process:
+                              stderr=subprocess.STDOUT, **creation_flags_dict()) as process:
             for line in process.stdout:
-                print(line.decode('utf-8'))
+                Logger.info(line.decode('utf-8'))
 
     ####################################################################################################################
     async def first_page(self) -> "Page":
         page = self.context.pages[0] if self.context.pages else await self.context.new_page()
 
         if self._stealthy:
             from playwright_stealth import stealth_async
             await stealth_async(page)
         return page
 
     async def close(self):
         await self.create_task(self.__stop_playwright())
         self.stop()
 
-    async def goto(self, url, *args, **kwargs):
-        return await self.create_task(self.page.goto(url, *args, **kwargs))
-
-    async def add_script_tag(self, *args, **kwargs):
-        return await self.create_task(self.page.add_script_tag(*args, **kwargs))
-
-    async def expose_function(self, *args, **kwargs):
-        return await self.create_task(self.page.expose_function(*args, **kwargs))
-
-    async def page_wait_for_function(self, *args, **kwargs):
-        return await self.create_task(self.page.wait_for_function(*args, **kwargs))
-
-    async def page_evaluate(self, *args, **kwargs):
-        return await self.create_task(self.page.evaluate(*args, **kwargs))
+    async def goto(self, url, *args, page=None, **kwargs):
+        page = page or self.page
+        return await self.create_task(page.goto(url, *args, **kwargs))
+
+    async def add_script_tag(self, *args, page=None, **kwargs):
+        page = page or self.page
+        return await self.create_task(page.add_script_tag(*args, **kwargs))
+
+    async def expose_function(self, *args, page=None, **kwargs):
+        page = page or self.page
+        return await self.create_task(page.expose_function(*args, **kwargs))
+
+    async def page_wait_for_function(self, *args, page=None, **kwargs):
+        page = page or self.page
+        return await self.create_task(page.wait_for_function(*args, **kwargs))
+
+    async def page_evaluate(self, *args, page=None, **kwargs):
+        page = page or self.page
+        return await self.create_task(page.evaluate(*args, **kwargs))
 
     ####################################################################################################################
     def sleep(self, val, timeout_=None):
         if timeout_ is None:
             timeout_ = val if val > 5 else 5
         self.run_threadsafe(asyncio.sleep(val), timeout_=timeout_)
 
-    def goto_sync(self, url, *args, timeout_=60, **kwargs):
-        return self.run_threadsafe(self.page.goto(url, *args, **kwargs), timeout_=timeout_)
-
-    def add_script_tag_sync(self, *args, timeout_=60, **kwargs):
-        return self.run_threadsafe(self.page.add_script_tag(*args, **kwargs), timeout_=timeout_)
-
-    def expose_function_sync(self, *args, timeout_=60, **kwargs):
-        return self.run_threadsafe(self.page.expose_function(*args, **kwargs), timeout_=timeout_)
-
-    def page_wait_for_function_sync(self, *args, timeout_=60, **kwargs):
-        return self.run_threadsafe(self.page.wait_for_function(*args, **kwargs), timeout_=timeout_)
-
-    def page_evaluate_sync(self, *args, timeout_=60, **kwargs, ):
-        return self.run_threadsafe(self.page.evaluate(*args, **kwargs), timeout_=timeout_)
+    def goto_sync(self, url, *args, page=None, timeout_=60, **kwargs):
+        page = page or self.page
+        return self.run_threadsafe(page.goto(url, *args, **kwargs), timeout_=timeout_)
+
+    def add_script_tag_sync(self, *args, page=None, timeout_=60, **kwargs):
+        page = page or self.page
+        return self.run_threadsafe(page.add_script_tag(*args, **kwargs), timeout_=timeout_)
+
+    def expose_function_sync(self, *args, page=None, timeout_=60, **kwargs):
+        page = page or self.page
+        return self.run_threadsafe(page.expose_function(*args, **kwargs), timeout_=timeout_)
+
+    def page_wait_for_function_sync(self, *args, page=None, timeout_=60, **kwargs):
+        page = page or self.page
+        return self.run_threadsafe(page.wait_for_function(*args, **kwargs), timeout_=timeout_)
+
+    def page_evaluate_sync(self, *args, page=None, timeout_=60, **kwargs, ):
+        page = page or self.page
+        return self.run_threadsafe(page.evaluate(*args, **kwargs), timeout_=timeout_)
 
     def sync_close(self, timeout_=60):
         self.run_threadsafe(self.__stop_playwright(), timeout_=timeout_)
         self.stop()
+
+
+def creation_flags_dict():
+    try:
+        if sys_os == 'Windows':
+            return {"creationflags": subprocess.CREATE_NO_WINDOW}
+    except:
+        Logger.exception("creation_flags_dict")
+    return {}
```

### Comparing `PlaywrightSafeThread-0.5.2.1/PlaywrightSafeThread.egg-info/PKG-INFO` & `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.2.1
+Version: 0.5.3
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.2.1/README.md` & `PlaywrightSafeThread-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.2.1/setup.py` & `PlaywrightSafeThread-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "PlaywrightSafeThread"
 
-version = "0.5.2.1"
+version = "0.5.3"
 
 setup(
     name="PlaywrightSafeThread",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

