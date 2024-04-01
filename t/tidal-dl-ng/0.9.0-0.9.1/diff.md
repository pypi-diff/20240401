# Comparing `tmp/tidal_dl_ng-0.9.0.tar.gz` & `tmp/tidal_dl_ng-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_dl_ng-0.9.0.tar", max compression
+gzip compressed data, was "tidal_dl_ng-0.9.1.tar", max compression
```

## Comparing `tidal_dl_ng-0.9.0.tar` & `tidal_dl_ng-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    34523 2024-03-22 06:50:42.748877 tidal_dl_ng-0.9.0/LICENSE
--rw-r--r--   0        0        0     6092 2024-03-22 06:50:42.748877 tidal_dl_ng-0.9.0/README.md
--rw-r--r--   0        0        0     4462 2024-03-22 06:51:12.749189 tidal_dl_ng-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      401 2024-03-22 06:50:42.748877 tidal_dl_ng-0.9.0/tidal_dl_ng/__init__.py
--rw-r--r--   0        0        0     3580 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/api.py
--rw-r--r--   0        0        0     6642 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/cli.py
--rw-r--r--   0        0        0     5649 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/config.py
--rw-r--r--   0        0        0     1109 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/constants.py
--rw-r--r--   0        0        0     7299 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/dialog.py
--rw-r--r--   0        0        0    20351 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/download.py
--rw-r--r--   0        0        0    24774 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/gui.py
--rw-r--r--   0        0        0        0 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/__init__.py
--rw-r--r--   0        0        0      674 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/decorator.py
--rw-r--r--   0        0        0     1618 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/decryption.py
--rw-r--r--   0        0        0      173 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/exceptions.py
--rw-r--r--   0        0        0     9804 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/path.py
--rw-r--r--   0        0        0     4345 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/tidal.py
--rw-r--r--   0        0        0      462 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/helper/wrapper.py
--rw-r--r--   0        0        0     1679 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/logger.py
--rw-r--r--   0        0        0     5595 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/metadata.py
--rw-r--r--   0        0        0        0 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/model/__init__.py
--rw-r--r--   0        0        0     3631 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/model/cfg.py
--rw-r--r--   0        0        0      512 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/model/gui_data.py
--rw-r--r--   0        0        0      221 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/model/tidal.py
--rw-r--r--   0        0        0        0 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/__init__.py
--rw-r--r--   0        0        0     4742 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_login.py
--rw-r--r--   0        0        0     4453 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_login.ui
--rw-r--r--   0        0        0    24218 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_settings.py
--rw-r--r--   0        0        0    21205 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_settings.ui
--rw-r--r--   0        0        0     1966 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_version.py
--rw-r--r--   0        0        0     1426 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_version.ui
--rw-r--r--   0        0        0      927 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dummy_register.py
--rw-r--r--   0        0        0     2106 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dummy_wiggly.py
--rw-r--r--   0        0        0    91254 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.icns
--rw-r--r--   0        0        0   220222 2024-03-22 06:50:42.752878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.ico
--rw-r--r--   0        0        0    54166 2024-03-22 06:50:42.756878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.png
--rw-r--r--   0        0        0    20690 2024-03-22 06:50:42.756878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/main.py
--rw-r--r--   0        0        0    18915 2024-03-22 06:50:42.756878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/main.ui
--rw-r--r--   0        0        0     7690 2024-03-22 06:50:42.756878 tidal_dl_ng-0.9.0/tidal_dl_ng/ui/spinner.py
--rw-r--r--   0        0        0      982 2024-03-22 06:50:42.756878 tidal_dl_ng-0.9.0/tidal_dl_ng/worker.py
--rw-r--r--   0        0        0     7446 1970-01-01 00:00:00.000000 tidal_dl_ng-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-22 15:32:28.367964 tidal_dl_ng-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6092 2024-03-22 15:32:28.367964 tidal_dl_ng-0.9.1/README.md
+-rw-r--r--   0        0        0     4512 2024-03-22 15:32:49.124046 tidal_dl_ng-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/__init__.py
+-rw-r--r--   0        0        0     3580 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/api.py
+-rw-r--r--   0        0        0     6634 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/cli.py
+-rw-r--r--   0        0        0     5649 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/config.py
+-rw-r--r--   0        0        0     1109 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/constants.py
+-rw-r--r--   0        0        0     8436 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/dialog.py
+-rw-r--r--   0        0        0    20791 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/download.py
+-rw-r--r--   0        0        0    24962 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/gui.py
+-rw-r--r--   0        0        0        0 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/__init__.py
+-rw-r--r--   0        0        0      674 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/decorator.py
+-rw-r--r--   0        0        0     1618 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/decryption.py
+-rw-r--r--   0        0        0      173 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/exceptions.py
+-rw-r--r--   0        0        0     9963 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/path.py
+-rw-r--r--   0        0        0     4345 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/tidal.py
+-rw-r--r--   0        0        0      462 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/helper/wrapper.py
+-rw-r--r--   0        0        0     1679 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/logger.py
+-rw-r--r--   0        0        0     5595 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/metadata.py
+-rw-r--r--   0        0        0        0 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/model/__init__.py
+-rw-r--r--   0        0        0     3631 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/model/cfg.py
+-rw-r--r--   0        0        0      512 2024-03-22 15:32:28.371964 tidal_dl_ng-0.9.1/tidal_dl_ng/model/gui_data.py
+-rw-r--r--   0        0        0      221 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/model/tidal.py
+-rw-r--r--   0        0        0        0 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/__init__.py
+-rw-r--r--   0        0        0     4742 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_login.py
+-rw-r--r--   0        0        0     4453 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_login.ui
+-rw-r--r--   0        0        0    24218 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_settings.py
+-rw-r--r--   0        0        0    21205 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_settings.ui
+-rw-r--r--   0        0        0     1966 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_version.py
+-rw-r--r--   0        0        0     1426 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_version.ui
+-rw-r--r--   0        0        0      927 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dummy_register.py
+-rw-r--r--   0        0        0     2106 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dummy_wiggly.py
+-rw-r--r--   0        0        0    91254 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.icns
+-rw-r--r--   0        0        0   220222 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.ico
+-rw-r--r--   0        0        0    54166 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.png
+-rw-r--r--   0        0        0    20711 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/main.py
+-rw-r--r--   0        0        0    18917 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/main.ui
+-rw-r--r--   0        0        0     7690 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/ui/spinner.py
+-rw-r--r--   0        0        0      982 2024-03-22 15:32:28.375964 tidal_dl_ng-0.9.1/tidal_dl_ng/worker.py
+-rw-r--r--   0        0        0     7491 1970-01-01 00:00:00.000000 tidal_dl_ng-0.9.1/PKG-INFO
```

### Comparing `tidal_dl_ng-0.9.0/LICENSE` & `tidal_dl_ng-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/README.md` & `tidal_dl_ng-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/pyproject.toml` & `tidal_dl_ng-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tidal-dl-ng"
 authors = ["Robert Honz <cen.sored@gmail.com>"]
-version = "v0.9.0"
+version = "v0.9.1"
 description = "TIDAL Medial Downloader Next Generation!"
 repository = "https://github.com/exislow/tidal-dl-ng"
 documentation = "https://exislow.github.io/tidal-dl-ng/"
 readme = "README.md"
 packages = [
   { include = "tidal_dl_ng" }
 ]
@@ -36,14 +36,15 @@
 m3u8 = "^4.0.0"
 ffmpeg-python = "^0.2.0"
 coloredlogs = "^15.0.1"
 pyside6 = {version = "^6.6.2", optional = true}
 pyqtdarktheme = {version = "^2.1.0", optional = true}
 mpegdash = "^0.4.0"
 rich = "^13.7.1"
+usingversion = "^0.1.2"
 
 [tool.poetry.extras]
 gui = ["pyside6", "pyqtdarktheme"]
 
 [tool.poetry.group.dev]
 optional = true
 
@@ -166,15 +167,15 @@
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
 sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 include_trailing_comma = true
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
-known_third_party = ["Crypto", "PySide6", "coloredlogs", "dataclasses_json", "ffmpeg", "m3u8", "mpegdash", "mutagen", "pathvalidate", "requests", "rich", "tidalapi", "typer"]
+known_third_party = ["Crypto", "PySide6", "coloredlogs", "dataclasses_json", "ffmpeg", "helper", "m3u8", "mpegdash", "mutagen", "pathvalidate", "requests", "rich", "tidalapi", "typer", "usingversion"]
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
 files = ["tidal_dl_ng"]
 python_version = "3.11"
 pretty = true
 show_traceback = true
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/api.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/api.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/cli.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 import typer
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import BarColumn, Console, Progress, SpinnerColumn, TextColumn
 from rich.table import Table
 
-from tidal_dl_ng import __version__
+from tidal_dl_ng import version
 from tidal_dl_ng.config import Settings, Tidal
 from tidal_dl_ng.constants import CTX_TIDAL, MediaType
 from tidal_dl_ng.download import Download
 from tidal_dl_ng.helper.path import get_format_template, path_file_settings
 from tidal_dl_ng.helper.tidal import get_tidal_media_id, get_tidal_media_type
 from tidal_dl_ng.helper.wrapper import LoggerWrapped
 from tidal_dl_ng.model.cfg import HelpSettings
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]}, add_completion=False)
 
 
 def version_callback(value: bool):
     if value:
-        print(f"{__version__}")
+        print(f"{version}")
         raise typer.Exit()
 
 
 @app.callback()
 def callback_app(
     ctx: typer.Context,
     version: Annotated[
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/config.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/config.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/constants.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/constants.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/dialog.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/dialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os.path
 from enum import Enum
 from pathlib import Path
 
+from helper.path import is_installed_ffmpeg
 from PySide6 import QtCore, QtGui, QtWidgets
 from tidalapi import Quality as QualityAudio
 
-from tidal_dl_ng import __version__
+from tidal_dl_ng import version
 from tidal_dl_ng.config import Settings
 from tidal_dl_ng.constants import CoverDimensions, QualityVideo, SkipExisting
 from tidal_dl_ng.model.cfg import HelpSettings
 from tidal_dl_ng.model.cfg import Settings as ModelSettings
 from tidal_dl_ng.ui.dialog_login import Ui_DialogLogin
 from tidal_dl_ng.ui.dialog_settings import Ui_DialogSettings
 from tidal_dl_ng.ui.dialog_version import Ui_DialogVersion
@@ -25,15 +26,15 @@
 
         # Create an instance of the GUI
         self.ui = Ui_DialogVersion()
 
         # Run the .setupUi() method to show the GUI
         self.ui.setupUi(self)
         # Set the version.
-        self.ui.l_version.setText("v" + __version__)
+        self.ui.l_version.setText("v" + version)
         # Show
         self.exec()
 
 
 class DialogLogin(QtWidgets.QDialog):
     """Version dialog."""
 
@@ -82,46 +83,73 @@
         self.settings = settings
         self.data = settings.data
         self.s_settings_save = settings_save
         self.help_settings = HelpSettings()
         pixmapi: QtWidgets.QStyle.StandardPixmap = QtWidgets.QStyle.SP_MessageBoxQuestion
         self.icon = self.style().standardIcon(pixmapi)
 
-        self.parameters_checkboxes = [
-            "lyrics_embed",
-            "lyrics_file",
-            "video_download",
-            "download_delay",
-            "video_convert_mp4",
-        ]
-        self.parameters_combo = [
-            ("skip_existing", SkipExisting),
-            ("quality_audio", QualityAudio),
-            ("quality_video", QualityVideo),
-            ("metadata_cover_dimension", CoverDimensions),
-        ]
-        self.parameters_line_edit = [
-            "download_base_path",
-            "format_album",
-            "format_playlist",
-            "format_mix",
-            "format_track",
-            "format_video",
-        ]
+        self._init_checkboxes()
+        self._init_comboboxes()
+        self._init_line_edit()
 
         # Create an instance of the GUI
         self.ui = Ui_DialogSettings()
 
         # Run the .setupUi() method to show the GUI
         self.ui.setupUi(self)
         # Set data.
         self.gui_populate()
+        self._init_signals()
 
         self.exec()
 
+    def _init_signals(self):
+        self.ui.cb_video_convert_mp4.stateChanged.connect(self.on_cb_video_convert_mp4)
+
+    def on_cb_video_convert_mp4(self, int):
+        if self.ui.cb_video_convert_mp4.isChecked():
+            # Check if ffmpeg is in PATH otherwise show error message.
+            if not is_installed_ffmpeg():
+                self.ui.cb_video_convert_mp4.setChecked(False)
+                self.ui.cb_video_convert_mp4.setCheckState(QtCore.Qt.CheckState.Unchecked)
+                QtWidgets.QMessageBox.critical(
+                    self,
+                    "FFmpeg not found!",
+                    "Either FFmpeg is not installed on your computer or not set within "
+                    "your PATH variable. You cannot activate this option until FFmpeg "
+                    "is correctly installed and set to your environmental PATH variable.",
+                )
+
+    def _init_line_edit(self):
+        self.parameters_line_edit = [
+            "download_base_path",
+            "format_album",
+            "format_playlist",
+            "format_mix",
+            "format_track",
+            "format_video",
+        ]
+
+    def _init_comboboxes(self):
+        self.parameters_combo = [
+            ("skip_existing", SkipExisting),
+            ("quality_audio", QualityAudio),
+            ("quality_video", QualityVideo),
+            ("metadata_cover_dimension", CoverDimensions),
+        ]
+
+    def _init_checkboxes(self):
+        self.parameters_checkboxes = [
+            "lyrics_embed",
+            "lyrics_file",
+            "video_download",
+            "download_delay",
+            "video_convert_mp4",
+        ]
+
     def gui_populate(self):
         self.populate_checkboxes()
         self.populate_combo()
         self.populate_line_edit()
 
     def dialog_dir_open(self, obj_line_edit):
         # If a path is set, use it otherwise the users home directory.
@@ -186,15 +214,15 @@
 
             checkbox.setText(pn)
             checkbox.setToolTip(getattr(self.help_settings, pn))
             checkbox.setIcon(self.icon)
             checkbox.setChecked(getattr(self.data, pn))
 
     def accept(self):
-        # Get settings. TODO
+        # Get settings.
         self.to_settings()
         self.done(1)
 
     def to_settings(self):
         for item in self.parameters_checkboxes:
             setattr(self.settings.data, item, getattr(self.ui, self.prefix_checkbox + item).isChecked())
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/download.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     MediaType,
     SkipExisting,
     StreamManifestMimeType,
     VideoExtensions,
 )
 from tidal_dl_ng.helper.decryption import decrypt_file, decrypt_security_token
 from tidal_dl_ng.helper.exceptions import MediaMissing, UnknownManifestFormat
-from tidal_dl_ng.helper.path import check_file_exists, format_path_media, path_file_sanitize
+from tidal_dl_ng.helper.path import check_file_exists, format_path_media, is_installed_ffmpeg, path_file_sanitize
 from tidal_dl_ng.helper.tidal import (
     instantiate_media,
     items_results_all,
     name_builder_album_artist,
     name_builder_artist,
     name_builder_item,
     name_builder_title,
@@ -78,14 +78,21 @@
         self.session = session
         self.skip_existing = skip_existing
         self.fn_logger = fn_logger
         self.progress_gui = progress_gui
         self.progress = progress
         self.path_base = path_base
 
+        if not is_installed_ffmpeg() and self.settings.data.video_convert_mp4:
+            self.settings.data.video_convert_mp4 = False
+            self.fn_logger.error(
+                "Cannot find FFmpeg in PATH. Videos can be downloaded but will not be processed. "
+                "Make sure FFmpeg is installed correctly and present within your environmental PATH variable."
+            )
+
     def _download(
         self,
         media: Track | Video,
         stream_manifest: StreamManifest,
         path_file: str,
     ) -> str:
         media_name: str = name_builder_item(media)
@@ -280,15 +287,17 @@
             result = ""
 
         return result
 
     def metadata_write(self, track: Track, path_file: str):
         result: bool = False
         release_date: str = (
-            track.album.available_release_date.strftime("%Y-%m-%d") if track.album.available_release_date else track.album.release_date.strftime("%Y-%m-%d") if track.album.release_date else ""
+            track.album.available_release_date.strftime("%Y-%m-%d")
+            if track.album.available_release_date
+            else track.album.release_date.strftime("%Y-%m-%d") if track.album.release_date else ""
         )
         copy_right: str = track.copyright if hasattr(track, "copyright") and track.copyright else ""
         isrc: str = track.isrc if hasattr(track, "isrc") and track.isrc else ""
         lyrics: str = ""
 
         if self.settings.data.lyrics_embed or self.settings.data.lyrics_file:
             # Try to retrieve lyrics.
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/gui.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import sys
 from collections.abc import Callable
 
 from requests.exceptions import HTTPError
 
-from tidal_dl_ng import __version__
+from tidal_dl_ng import version
 from tidal_dl_ng.dialog import DialogLogin, DialogPreferences, DialogVersion
 from tidal_dl_ng.helper.exceptions import MediaUnknown
 from tidal_dl_ng.helper.path import get_format_template
 from tidal_dl_ng.helper.tidal import (
     get_tidal_media_id,
     get_tidal_media_type,
     instantiate_media,
@@ -283,24 +283,24 @@
         menu.exec(self.tr_lists_user.mapToGlobal(point))
 
     def thread_download_list_media(self, point):
         self.thread_it(self.on_download_list_media, point)
         self.thread_it(self.list_items_show_result, point=point)
 
     def on_download_list_media(self, point: QtCore.QPoint):
-        self.b_download.setEnabled(False)
-        self.b_download.setText("Downloading...")
+        self.pb_download.setEnabled(False)
+        self.pb_download.setText("Downloading...")
 
         item = self.tr_lists_user.itemAt(point)
         media = item.data(3, QtCore.Qt.ItemDataRole.UserRole)
 
         self.download(media, self.dl)
 
-        self.b_download.setText("Download")
-        self.b_download.setEnabled(True)
+        self.pb_download.setText("Download")
+        self.pb_download.setEnabled(True)
 
     def search_populate_results(self, query: str, type_media: SearchTypes):
         self.tr_results.clear()
 
         results: [ResultItem] = self.search(query, [type_media])
 
         self.populate_tree_results(results)
@@ -443,19 +443,19 @@
                 )
 
                 result.append(result_item)
 
         return result
 
     def _init_signals(self):
-        self.b_download.clicked.connect(lambda: self.thread_it(self.on_download_results))
+        self.pb_download.clicked.connect(lambda: self.thread_it(self.on_download_results))
         self.l_search.returnPressed.connect(
             lambda: self.search_populate_results(self.l_search.text(), self.cb_search_type.currentData())
         )
-        self.b_search.clicked.connect(
+        self.pb_search.clicked.connect(
             lambda: self.search_populate_results(self.l_search.text(), self.cb_search_type.currentData())
         )
         self.cb_quality_audio.currentIndexChanged.connect(self.on_quality_set_audio)
         self.cb_quality_video.currentIndexChanged.connect(self.on_quality_set_video)
         self.tr_lists_user.itemClicked.connect(self.on_list_items_show)
         self.s_spinner_start[QtWidgets.QWidget].connect(self.on_spinner_start)
         self.s_spinner_stop.connect(self.on_spinner_stop)
@@ -539,16 +539,16 @@
         # Any other args, kwargs are passed to the run function
         worker = Worker(fn, *args, **kwargs)
 
         # Execute
         self.threadpool.start(worker)
 
     def on_download_results(self):
-        self.b_download.setEnabled(False)
-        self.b_download.setText("Downloading...")
+        self.pb_download.setEnabled(False)
+        self.pb_download.setText("Downloading...")
 
         items: [QtWidgets.QTreeWidgetItem] = self.tr_results.selectedItems()
 
         if len(items) == 0:
             logger_gui.error("Please select a row first.")
         else:
             items_pos_last = len(items) - 1
@@ -560,16 +560,16 @@
                     isinstance(media, Track | Video)
                     and self.settings.data.download_delay
                     and items.index(item) < items_pos_last
                 )
 
                 self.download(media, self.dl, delay_track=download_delay)
 
-        self.b_download.setText("Download")
-        self.b_download.setEnabled(True)
+        self.pb_download.setText("Download")
+        self.pb_download.setEnabled(True)
 
     def download(self, media: Track | Album | Playlist | Video | Mix, dl: Download, delay_track: bool = False) -> None:
         self.s_pb_reset.emit()
         self.s_statusbar_message.emit(StatusbarMessage(message="Download started..."))
 
         file_template = get_format_template(media, self.settings)
 
@@ -611,29 +611,32 @@
 
 
 # TODO: Comment with Google Docstrings.
 def gui_activate(tidal: Tidal | None = None):
     # Set dark theme and create QT app.
     qdarktheme.enable_hi_dpi()
     app = QtWidgets.QApplication(sys.argv)
-    qdarktheme.setup_theme()
+    # Fix for Windows: Tooltips have bright font color
+    # https://github.com/5yutan5/PyQtDarkTheme/issues/239
+    # qdarktheme.setup_theme()
+    qdarktheme.setup_theme(additional_qss="QToolTip { border: 0px; }")
 
     # Create icon object and apply it to app window.
     pixmap: QtGui.QPixmap = QtGui.QPixmap("tidal_dl_ng/ui/icon.png")
     icon: QtGui.QIcon = QtGui.QIcon(pixmap)
     app.setWindowIcon(icon)
 
     # This bit gets the taskbar icon working properly in Windows
     if sys.platform.startswith("win"):
         import ctypes
 
         # Make sure Pyinstaller icons are still grouped
         if not sys.argv[0].endswith(".exe"):
             # Arbitrary string
-            my_app_id: str = "exislow.tidal.dl-ng." + __version__
+            my_app_id: str = "exislow.tidal.dl-ng." + version
             ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(my_app_id)
 
     window = MainWindow(tidal=tidal)
     window.show()
 
     sys.exit(app.exec())
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/helper/decorator.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/helper/decorator.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/helper/decryption.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/helper/decryption.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/helper/path.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/helper/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import glob
 import math
 import os
 import re
+import shutil
 from pathlib import Path, PosixPath
 
 from pathvalidate import sanitize_filename, sanitize_filepath
 from pathvalidate.error import ValidationError
 from tidalapi import Album, Mix, Playlist, Track, UserPlaylist, Video
 
 from tidal_dl_ng import __name_display__
 from tidal_dl_ng.constants import FILENAME_SANITIZE_PLACEHOLDER, UNIQUIFY_THRESHOLD, AudioExtensions, MediaType
-from tidal_dl_ng.helper.tidal import name_builder_artist, name_builder_title, name_builder_album_artist
+from tidal_dl_ng.helper.tidal import name_builder_album_artist, name_builder_artist, name_builder_title
 
 
 def path_home() -> str:
     if "XDG_CONFIG_HOME" in os.environ:
         return os.environ["XDG_CONFIG_HOME"]
     elif "HOME" in os.environ:
         return os.environ["HOME"]
@@ -257,7 +258,14 @@
             path_files.append(str(path_parent.joinpath(path_file_stem + extension.value)))
     else:
         path_files: [str] = [path_file]
 
     result = bool(sum([glob.glob(_file) for _file in path_files], []))
 
     return result
+
+
+def is_installed_ffmpeg() -> bool:
+    # Checks if ffmpeg is found in PATH.
+    result: bool = bool(shutil.which("ffmpeg"))
+
+    return result
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/helper/tidal.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/helper/tidal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from tidalapi import Album, Mix, Playlist, Session, Track, UserPlaylist, Video
-from tidalapi.artist import Role, Artist
+from tidalapi.artist import Artist, Role
 from tidalapi.session import SearchTypes
 
 from tidal_dl_ng.constants import MediaType
 from tidal_dl_ng.helper.exceptions import MediaUnknown
 
 
 def name_builder_artist(media: Track | Video | Album) -> str:
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/logger.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/logger.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/metadata.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/metadata.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/model/cfg.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/model/cfg.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/model/gui_data.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/model/gui_data.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_login.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_login.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_login.ui` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_login.ui`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_settings.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_settings.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_settings.ui` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_settings.ui`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_version.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_version.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dialog_version.ui` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dialog_version.ui`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dummy_register.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dummy_register.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/dummy_wiggly.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/dummy_wiggly.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.icns` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.icns`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.ico` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.ico`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/icon.png` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/icon.png`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/main.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,34 +183,34 @@
         self.cb_search_type.setAccessibleDescription("")
         # endif // QT_CONFIG(accessibility)
         self.cb_search_type.setCurrentText("")
         self.cb_search_type.setPlaceholderText("")
 
         self.lh_search.addWidget(self.cb_search_type)
 
-        self.b_search = QPushButton(self.w_central)
-        self.b_search.setObjectName("b_search")
+        self.pb_search = QPushButton(self.w_central)
+        self.pb_search.setObjectName("pb_search")
         # if QT_CONFIG(statustip)
-        self.b_search.setStatusTip("")
+        self.pb_search.setStatusTip("")
         # endif // QT_CONFIG(statustip)
         # if QT_CONFIG(whatsthis)
-        self.b_search.setWhatsThis("")
+        self.pb_search.setWhatsThis("")
         # endif // QT_CONFIG(whatsthis)
         # if QT_CONFIG(accessibility)
-        self.b_search.setAccessibleName("")
+        self.pb_search.setAccessibleName("")
         # endif // QT_CONFIG(accessibility)
         # if QT_CONFIG(accessibility)
-        self.b_search.setAccessibleDescription("")
+        self.pb_search.setAccessibleDescription("")
         # endif // QT_CONFIG(accessibility)
-        self.b_search.setText("Search")
+        self.pb_search.setText("Search")
         # if QT_CONFIG(shortcut)
-        self.b_search.setShortcut("")
+        self.pb_search.setShortcut("")
         # endif // QT_CONFIG(shortcut)
 
-        self.lh_search.addWidget(self.b_search)
+        self.lh_search.addWidget(self.pb_search)
 
         self.lv_search_result.addLayout(self.lh_search)
 
         self.tr_results = QTreeWidget(self.w_central)
         self.tr_results.setObjectName("tr_results")
         self.tr_results.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.tr_results.setProperty("showDropIndicator", False)
@@ -311,37 +311,37 @@
         self.cb_quality_video.setAccessibleDescription("")
         # endif // QT_CONFIG(accessibility)
         self.cb_quality_video.setCurrentText("")
         self.cb_quality_video.setPlaceholderText("")
 
         self.lh_download.addWidget(self.cb_quality_video)
 
-        self.b_download = QPushButton(self.w_central)
-        self.b_download.setObjectName("b_download")
+        self.pb_download = QPushButton(self.w_central)
+        self.pb_download.setObjectName("pb_download")
         # if QT_CONFIG(tooltip)
-        self.b_download.setToolTip("")
+        self.pb_download.setToolTip("")
         # endif // QT_CONFIG(tooltip)
         # if QT_CONFIG(statustip)
-        self.b_download.setStatusTip("")
+        self.pb_download.setStatusTip("")
         # endif // QT_CONFIG(statustip)
         # if QT_CONFIG(whatsthis)
-        self.b_download.setWhatsThis("")
+        self.pb_download.setWhatsThis("")
         # endif // QT_CONFIG(whatsthis)
         # if QT_CONFIG(accessibility)
-        self.b_download.setAccessibleName("")
+        self.pb_download.setAccessibleName("")
         # endif // QT_CONFIG(accessibility)
         # if QT_CONFIG(accessibility)
-        self.b_download.setAccessibleDescription("")
+        self.pb_download.setAccessibleDescription("")
         # endif // QT_CONFIG(accessibility)
-        self.b_download.setText("Download")
+        self.pb_download.setText("Download")
         # if QT_CONFIG(shortcut)
-        self.b_download.setShortcut("")
+        self.pb_download.setShortcut("")
         # endif // QT_CONFIG(shortcut)
 
-        self.lh_download.addWidget(self.b_download)
+        self.lh_download.addWidget(self.pb_download)
 
         self.lh_download.setStretch(0, 5)
         self.lh_download.setStretch(2, 5)
         self.lh_download.setStretch(4, 15)
 
         self.lv_search_result.addLayout(self.lh_download)
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/main.ui` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/main.ui`

 * *Files 0% similar despite different names*

#### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/main.ui` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/main.ui`

```diff
@@ -242,15 +242,15 @@
                         </property>
                         <property name="placeholderText">
                           <string notr="true"/>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="QPushButton" name="b_search">
+                      <widget class="QPushButton" name="pb_search">
                         <property name="statusTip">
                           <string notr="true"/>
                         </property>
                         <property name="whatsThis">
                           <string notr="true"/>
                         </property>
                         <property name="accessibleName">
@@ -432,15 +432,15 @@
                         </property>
                         <property name="placeholderText">
                           <string notr="true"/>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="QPushButton" name="b_download">
+                      <widget class="QPushButton" name="pb_download">
                         <property name="toolTip">
                           <string notr="true"/>
                         </property>
                         <property name="statusTip">
                           <string notr="true"/>
                         </property>
                         <property name="whatsThis">
```

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/ui/spinner.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/ui/spinner.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/tidal_dl_ng/worker.py` & `tidal_dl_ng-0.9.1/tidal_dl_ng/worker.py`

 * *Files identical despite different names*

### Comparing `tidal_dl_ng-0.9.0/PKG-INFO` & `tidal_dl_ng-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-dl-ng
-Version: 0.9.0
+Version: 0.9.1
 Summary: TIDAL Medial Downloader Next Generation!
 Home-page: https://github.com/exislow/tidal-dl-ng
 Author: Robert Honz
 Author-email: cen.sored@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 Requires-Dist: pycryptodome (==3.20.0)
 Requires-Dist: pyqtdarktheme (>=2.1.0,<3.0.0) ; extra == "gui"
 Requires-Dist: pyside6 (>=6.6.2,<7.0.0) ; extra == "gui"
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tidalapi (==0.7.4)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: usingversion (>=0.1.2,<0.2.0)
 Project-URL: Documentation, https://exislow.github.io/tidal-dl-ng/
 Project-URL: Repository, https://github.com/exislow/tidal-dl-ng
 Description-Content-Type: text/markdown
 
 # 🔰 TIDAL Downloader Next Generation! (tidal-dl-ng)
 
 [![Release](https://img.shields.io/github/v/release/exislow/tidal-dl-ng)](https://img.shields.io/github/v/release/exislow/tidal-dl-ng)
```

