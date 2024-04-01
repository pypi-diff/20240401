# Comparing `tmp/d_fake_seeder-0.0.8.tar.gz` & `tmp/d_fake_seeder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_fake_seeder-0.0.8.tar", max compression
+gzip compressed data, was "d_fake_seeder-0.0.9.tar", max compression
```

## Comparing `d_fake_seeder-0.0.8.tar` & `d_fake_seeder-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11357 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/LICENSE
--rw-r--r--   0        0        0     3008 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/README.md
--rw-r--r--   0        0        0     2080 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/config/default.json
--rwxr-xr-x   0        0        0      231 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/dfakeseeder.desktop
--rwxr-xr-x   0        0        0     1754 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/dfakeseeder.py
--rw-r--r--   0        0        0      462 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/images/alert16.png
--rw-r--r--   0        0        0    14625 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/images/dfakeseeder.png
--rw-r--r--   0        0        0      465 2024-03-31 11:05:29.161349 d_fake_seeder-0.0.8/d_fake_seeder/images/downloading16.png
--rw-r--r--   0        0        0    85775 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/images/screenshot.png
--rw-r--r--   0        0        0      505 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/images/seeding16.png
--rw-r--r--   0        0        0      394 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/images/traffic16.png
--rw-r--r--   0        0        0        0 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/__init__.py
--rw-r--r--   0        0        0     1224 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/controller.py
--rw-r--r--   0        0        0      326 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/handlers/FileModifiedEventHandler.py
--rw-r--r--   0        0        0        0 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/handlers/__init__.py
--rw-r--r--   0        0        0     1007 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/logger.py
--rw-r--r--   0        0        0     7535 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/model.py
--rw-r--r--   0        0        0     5117 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/settings.py
--rw-r--r--   0        0        0      557 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/attributes.py
--rw-r--r--   0        0        0     2354 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/bencoding.py
--rw-r--r--   0        0        0     3740 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/file.py
--rw-r--r--   0        0        0     8874 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/seeder.py
--rw-r--r--   0        0        0    10399 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/torrent.py
--rw-r--r--   0        0        0        0 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/util/__init__.py
--rw-r--r--   0        0        0     2497 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/util/helpers.py
--rw-r--r--   0        0        0    10132 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/view.py
--rw-r--r--   0        0        0        0 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/__init__.py
--rw-r--r--   0        0        0    10158 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/notebook.py
--rw-r--r--   0        0        0     1640 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/states.py
--rw-r--r--   0        0        0     4130 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/statusbar.py
--rw-r--r--   0        0        0     9275 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/toolbar.py
--rw-r--r--   0        0        0    13960 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/lib/views/torrents.py
--rw-r--r--   0        0        0     1731 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/misc/preferences.py
--rw-r--r--   0        0        0     2828 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/misc/udptest.py
--rw-r--r--   0        0        0    24797 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/generated.xml
--rw-r--r--   0        0        0      562 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/menu.xml
--rw-r--r--   0        0        0      445 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/notebook/options.xml
--rw-r--r--   0        0        0     4225 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/notebook/peers.xml
--rw-r--r--   0        0        0     5370 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/notebook.xml
--rw-r--r--   0        0        0     1776 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/preferences.xml
--rw-r--r--   0        0        0     6303 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/statusbar.xml
--rw-r--r--   0        0        0       51 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/styles.css
--rw-r--r--   0        0        0     5702 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/toolbar.xml
--rw-r--r--   0        0        0      643 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/treeview-main.xml
--rw-r--r--   0        0        0      286 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/treeview-stats.xml
--rw-r--r--   0        0        0     2722 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/d_fake_seeder/ui/ui.xml
--rw-r--r--   0        0        0      483 2024-03-31 11:05:29.165349 d_fake_seeder-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 d_fake_seeder-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3008 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/README.md
+-rw-r--r--   0        0        0     2080 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/config/default.json
+-rwxr-xr-x   0        0        0      231 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/dfakeseeder.desktop
+-rwxr-xr-x   0        0        0     1999 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/dfakeseeder.py
+-rw-r--r--   0        0        0      462 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/images/alert16.png
+-rw-r--r--   0        0        0    14625 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/images/dfakeseeder.png
+-rw-r--r--   0        0        0      465 2024-03-31 17:11:09.194482 d_fake_seeder-0.0.9/d_fake_seeder/images/downloading16.png
+-rw-r--r--   0        0        0    85775 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/images/screenshot.png
+-rw-r--r--   0        0        0      505 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/images/seeding16.png
+-rw-r--r--   0        0        0      394 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/images/traffic16.png
+-rw-r--r--   0        0        0        0 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/__init__.py
+-rw-r--r--   0        0        0     1224 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/controller.py
+-rw-r--r--   0        0        0      326 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/handlers/FileModifiedEventHandler.py
+-rw-r--r--   0        0        0        0 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/handlers/__init__.py
+-rw-r--r--   0        0        0     1007 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/logger.py
+-rw-r--r--   0        0        0     7535 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/model.py
+-rw-r--r--   0        0        0     5117 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/settings.py
+-rw-r--r--   0        0        0      557 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/attributes.py
+-rw-r--r--   0        0        0     2354 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/bencoding.py
+-rw-r--r--   0        0        0     3740 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/file.py
+-rw-r--r--   0        0        0     8874 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/seeder.py
+-rw-r--r--   0        0        0    10399 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/torrent.py
+-rw-r--r--   0        0        0        0 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/util/__init__.py
+-rw-r--r--   0        0        0     2497 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/util/helpers.py
+-rw-r--r--   0        0        0    10132 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/view.py
+-rw-r--r--   0        0        0        0 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/__init__.py
+-rw-r--r--   0        0        0    10158 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/notebook.py
+-rw-r--r--   0        0        0     1640 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/states.py
+-rw-r--r--   0        0        0     4130 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/statusbar.py
+-rw-r--r--   0        0        0     9275 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/toolbar.py
+-rw-r--r--   0        0        0    13960 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/lib/views/torrents.py
+-rw-r--r--   0        0        0     1731 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/misc/preferences.py
+-rw-r--r--   0        0        0     2828 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/misc/udptest.py
+-rw-r--r--   0        0        0    24797 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/generated.xml
+-rw-r--r--   0        0        0      562 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/menu.xml
+-rw-r--r--   0        0        0      445 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/notebook/options.xml
+-rw-r--r--   0        0        0     4225 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/notebook/peers.xml
+-rw-r--r--   0        0        0     5370 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/notebook.xml
+-rw-r--r--   0        0        0     1776 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/preferences.xml
+-rw-r--r--   0        0        0     6303 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/statusbar.xml
+-rw-r--r--   0        0        0       51 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/styles.css
+-rw-r--r--   0        0        0     5702 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/toolbar.xml
+-rw-r--r--   0        0        0      643 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/treeview-main.xml
+-rw-r--r--   0        0        0      286 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/treeview-stats.xml
+-rw-r--r--   0        0        0     2722 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/d_fake_seeder/ui/ui.xml
+-rw-r--r--   0        0        0      483 2024-03-31 17:11:09.198482 d_fake_seeder-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 d_fake_seeder-0.0.9/PKG-INFO
```

### Comparing `d_fake_seeder-0.0.8/LICENSE` & `d_fake_seeder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/README.md` & `d_fake_seeder-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,11 +86,11 @@
         "total_uploaded": "Gtk.SpinButton",
         "upload_speed": "Gtk.SpinButton"
     },
     "issues_page": "https://github.com/dmzoneill/DFakeSeeder/issues",
     "website": "https://github.com/dmzoneill/DFakeSeeder/",
     "author": "David O Neill",
     "copyright": "Copyright {year}",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "logo": "images/dfakeseeder.png"
 }
 ```
```

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/config/default.json` & `d_fake_seeder-0.0.9/d_fake_seeder/config/default.json`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/dfakeseeder.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/controller.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,35 @@
-# import gettext
-import gi
-import typer
-from lib.controller import Controller
+import os
+
 from lib.logger import logger
-from lib.model import Model
 from lib.settings import Settings
-from lib.view import View
-
-# Ensure the correct version of Gtk is used
-gi.require_version("Gtk", "4.0")
-
-from gi.repository import Gio, Gtk  # noqa
-
-# Import the Model, View, and Controller classes from their respective modules
 
 
-class DFakeSeeder(Gtk.Application):
-    def __init__(self):
-        super().__init__(
-            application_id="ie.fio.dfakeseeder",
-            flags=Gio.ApplicationFlags.FLAGS_NONE,
-        )
-        logger.info("Startup", extra={"class_name": self.__class__.__name__})
+# Cont roller
+class Controller:
+    def __init__(self, view, model):
+        logger.info("Controller Startup", extra={"class_name": self.__class__.__name__})
         # subscribe to settings changed
         self.settings = Settings.get_instance()
         self.settings.connect("attribute-changed", self.handle_settings_changed)
 
-    def do_activate(self):
-        logger.info("Run Controller", extra={"class_name": self.__class__.__name__})
-
-        # The Model manages the data and logic
-        self.model = Model()
-        # The View manages the user interface
-        self.view = View(self)
-        # The Controller manages the interactions between the Model and View
-        self.controller = Controller(self.view, self.model)
-
-        # Start the controller
-        self.controller.run()
-
-        self.view.window.show()
+        self.view = view
+        self.model = model
+        self.view.set_model(self.model)
+        self.view.connect_signals()
+
+    def run(self):
+        logger.info("Controller Run", extra={"class_name": self.__class__.__name__})
+        for filename in os.listdir(os.path.expanduser("~/.config/dfakeseeder/torrents")):
+            if filename.endswith(".torrent"):
+                torrent_file = os.path.join(
+                    os.path.expanduser("~/.config/dfakeseeder/torrents"),
+                    filename,
+                )
+                self.model.add_torrent(torrent_file)
 
     def handle_settings_changed(self, source, key, value):
-        logger.info("Settings changed", extra={"class_name": self.__class__.__name__})
+        logger.info(
+            "Controller settings changed",
+            extra={"class_name": self.__class__.__name__},
+        )
         # print(key + " = " + value)
-
-
-app = typer.Typer()
-
-
-@app.command()
-def run():
-    d = DFakeSeeder()
-    d.run()
-
-
-# If the script is run directly (rather than imported as a module), create
-# an instance of the UI class
-if __name__ == "__main__":
-    app()
```

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/images/dfakeseeder.png` & `d_fake_seeder-0.0.9/d_fake_seeder/images/dfakeseeder.png`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/images/screenshot.png` & `d_fake_seeder-0.0.9/d_fake_seeder/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/logger.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/logger.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/model.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/model.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/settings.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/settings.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/attributes.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/attributes.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/bencoding.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/bencoding.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/file.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/file.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/seeder.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/seeder.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/torrent/torrent.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/torrent/torrent.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/util/helpers.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/view.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/view.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/views/notebook.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/views/notebook.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/views/states.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/views/states.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/views/statusbar.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/views/statusbar.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/views/toolbar.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/views/toolbar.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/lib/views/torrents.py` & `d_fake_seeder-0.0.9/d_fake_seeder/lib/views/torrents.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/misc/preferences.py` & `d_fake_seeder-0.0.9/d_fake_seeder/misc/preferences.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/misc/udptest.py` & `d_fake_seeder-0.0.9/d_fake_seeder/misc/udptest.py`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/generated.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/generated.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/menu.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/notebook/peers.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/notebook/peers.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/notebook.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/notebook.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/preferences.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/preferences.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/statusbar.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/statusbar.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/toolbar.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/toolbar.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/treeview-main.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/treeview-main.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/d_fake_seeder/ui/ui.xml` & `d_fake_seeder-0.0.9/d_fake_seeder/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `d_fake_seeder-0.0.8/PKG-INFO` & `d_fake_seeder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d_fake_seeder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python gtk fake seeder
 Home-page: https://github.com/dmzoneill/DFakeSeeder
 Author: David O Neill
 Author-email: dmz.oneill@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -101,11 +101,11 @@
         "total_uploaded": "Gtk.SpinButton",
         "upload_speed": "Gtk.SpinButton"
     },
     "issues_page": "https://github.com/dmzoneill/DFakeSeeder/issues",
     "website": "https://github.com/dmzoneill/DFakeSeeder/",
     "author": "David O Neill",
     "copyright": "Copyright {year}",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "logo": "images/dfakeseeder.png"
 }
 ```
```

