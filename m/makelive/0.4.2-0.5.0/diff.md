# Comparing `tmp/makelive-0.4.2.tar.gz` & `tmp/makelive-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makelive-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "makelive-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `makelive-0.4.2.tar` & `makelive-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0      210 2024-01-27 08:25:30.852437 makelive-0.4.2/.gitignore
--rw-r--r--   0        0        0       45 2024-01-27 08:26:04.032800 makelive-0.4.2/.isort.cfg
--rw-r--r--   0        0        0     1070 2024-01-27 08:25:00.677693 makelive-0.4.2/LICENSE
--rw-r--r--   0        0        0     3155 2024-01-27 18:16:48.000650 makelive-0.4.2/README.md
--rw-r--r--   0        0        0      776 2024-01-27 17:47:34.865926 makelive-0.4.2/README_DEV.md
--rw-r--r--   0        0        0      228 2024-01-28 04:36:00.283116 makelive-0.4.2/makelive/__init__.py
--rw-r--r--   0        0        0     3792 2024-01-28 16:49:44.779241 makelive-0.4.2/makelive/__main__.py
--rw-r--r--   0        0        0    10264 2024-01-28 04:36:00.290861 makelive-0.4.2/makelive/makelive.py
--rw-r--r--   0        0        0       22 2024-01-28 16:48:43.335233 makelive-0.4.2/makelive/version.py
--rw-r--r--   0        0        0     1252 2024-01-27 23:01:40.159377 makelive-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      233 2024-01-27 16:47:55.517068 makelive-0.4.2/requirements.txt
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 makelive-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-01-27 08:25:30.852437 makelive-0.5.0/.gitignore
+-rw-r--r--   0        0        0       45 2024-01-27 08:26:04.032800 makelive-0.5.0/.isort.cfg
+-rw-r--r--   0        0        0     1070 2024-01-27 08:25:00.677693 makelive-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3541 2024-04-01 15:35:46.322700 makelive-0.5.0/README.md
+-rw-r--r--   0        0        0      776 2024-01-27 17:47:34.865926 makelive-0.5.0/README_DEV.md
+-rwxr-xr-x   0        0        0     1160 2024-04-01 16:29:45.045140 makelive-0.5.0/build.sh
+-rw-r--r--   0        0        0      290 2024-04-01 15:46:18.251300 makelive-0.5.0/makelive/__init__.py
+-rw-r--r--   0        0        0     4365 2024-04-01 16:23:00.528262 makelive-0.5.0/makelive/__main__.py
+-rw-r--r--   0        0        0    13323 2024-04-01 15:47:55.218199 makelive-0.5.0/makelive/makelive.py
+-rw-r--r--   0        0        0       22 2024-04-01 16:31:18.232439 makelive-0.5.0/makelive/version.py
+-rw-r--r--   0        0        0     1277 2024-04-01 15:29:34.043291 makelive-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      251 2024-04-01 15:30:13.285146 makelive-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     1075 2024-04-01 16:26:18.895822 makelive-0.5.0/scripts/get_latest_pypi_version.py
+-rwxr-xr-x   0        0        0      741 2024-04-01 16:28:22.109190 makelive-0.5.0/scripts/postinstall.sh
+-rwxr-xr-x   0        0        0      159 2024-04-01 16:27:39.271663 makelive-0.5.0/scripts/preinstall.sh
+-rwxr-xr-x   0        0        0     5044 2024-04-01 16:26:18.903159 makelive-0.5.0/scripts/pyapp-runner.sh
+-rwxr-xr-x   0        0        0     2457 2024-04-01 16:28:19.202576 makelive-0.5.0/scripts/uninstall.sh
+-rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 makelive-0.5.0/PKG-INFO
```

### Comparing `makelive-0.4.2/LICENSE` & `makelive-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makelive-0.4.2/README.md` & `makelive-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,23 +26,35 @@
 * `git clone git@github.com:RhetTbull/makelive.git`
 * `cd makelive`
 * `pip install flit`
 * `flit install`
 
 ## API
 
+You can use makelive to programmatically create Live Photo pairs:
+
 ```python
 from makelive import make_live_photo
 
 photo_path = "test.jpg"
 video_path = "test.mov"
 asset_id = make_live_photo(photo_path, video_path)
 print(f"Wrote Asset ID: {asset_id} to {photo_path} and {video_path}")
 ```
 
+You can also check if a photo and video pair are a Live Photo pair and get the asset ID:
+
+```python
+from makelive import live_id, is_live_photo_pair
+photo_path = "test.jpg"
+video_path = "test.mov"
+print(f"Is Live Photo Pair: {is_live_photo_pair(photo_path, video_path)}")
+print(f"Asset ID: {live_id(photo_path)}")
+```
+
 **Note:** XMP metadata in the QuickTime movie file is not preserved by this function which may result in metadata loss.
 
 Metadata including EXIF, IPTC, and XMP are preserved in the image file but will be rewritten and the Core Graphics API may change the order of the metadata and normalize the values. For example, the tag XMP:TagsList will be rewritten as XMP:Subject and the value will be normalized to a list of title case strings.
 
 If you must preserve the original metadata completely, it is recommended to make a copy of the metadata using a tool like [exiftool](https://exiftool.org) before calling this function and then restore the metadata after calling this function. (But take care not to delete the ContentIdentifier metadata.)
 
 ## How it works
```

### Comparing `makelive-0.4.2/README_DEV.md` & `makelive-0.5.0/README_DEV.md`

 * *Files identical despite different names*

### Comparing `makelive-0.4.2/makelive/__main__.py` & `makelive-0.5.0/makelive/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 """Command line interface for makelive."""
 
-
 from __future__ import annotations
 
+import os
 import pathlib
+from collections.abc import Iterable
 
 import click
 
-from .makelive import make_live_photo
+from .makelive import is_image_file, is_live_photo_pair, is_video_file, make_live_photo
 from .version import __version__
 
-IMAGE_EXTENSIONS = [".jpeg", ".jpg", ".heic", ".heif"]
-VIDEO_EXTENSIONS = [".mov", ".mp4"]
-
 
 def find_photo_video_pairs(
-    file_paths: list[str],
-) -> tuple[list[tuple[str, str]], list[str]]:  # noqa: E501 (line too long
+    file_paths: Iterable[str | os.PathLike],
+) -> tuple[list[tuple[pathlib.Path, pathlib.Path]], list[pathlib.Path]]:  # noqa: E501 (line too long
     """Find photo and video pairs in a list of file paths."""
     matched_files, unmatched_files, image_files, video_files = [], [], {}, {}
 
-    for file_path in file_paths:
-        file_path = pathlib.Path(file_path)
+    for fp in file_paths:
+        file_path = pathlib.Path(fp)
         file_stem = file_path.stem
-        if file_path.suffix.lower() in IMAGE_EXTENSIONS:
-            image_files[file_stem] = str(file_path.resolve())
-        elif file_path.suffix.lower() in VIDEO_EXTENSIONS:
-            video_files[file_stem] = str(file_path.resolve())
+        if is_image_file(file_path):
+            image_files[file_stem] = file_path.resolve()
+        elif is_video_file(file_path):
+            video_files[file_stem] = file_path.resolve()
 
     for key, image_file in image_files.items():
         if key in video_files:
             matched_files.append((image_file, video_files[key]))
             del video_files[key]
         else:
             unmatched_files.append(image_file)
 
     unmatched_files.extend(video_files.values())
 
     return matched_files, unmatched_files
 
 
+def check_pair(image: pathlib.Path, video: pathlib.Path):
+    """Check if a photo and video pair is a Live Photo."""
+    if check_id := is_live_photo_pair(image, video):
+        click.echo(f"{image} and {video} are Live Photos: {check_id}")
+    else:
+        click.echo(f"{image} and {video} are not Live Photos")
+
+
 @click.command()
 @click.version_option(version=__version__)
 @click.option(
+    "-c",
+    "--check",
+    is_flag=True,
+    help="Check if file pair is a Live Photo but do not modify it",
+)
+@click.option(
     "-v",
     "--verbose",
     is_flag=True,
     help="Print verbose output",
 )
 @click.option(
     "--manual",
@@ -59,17 +71,18 @@
 )
 @click.argument(
     "files",
     nargs=-1,
     type=click.Path(exists=True, path_type=pathlib.Path),
 )
 def main(
+    check: bool,
     verbose: bool,
     manual: tuple[tuple[pathlib.Path, pathlib.Path]],
-    files: tuple[pathlib.Path],
+    files: tuple[pathlib.Path, ...],
 ):
     """MakeLive: convert a photo (JPEG or HEIC) and video (MOV or MP4) pair to a Live Photo.
 
     This will add the necessary metadata for Apple Photos to recognize the
     photo and video pair as a Live Photo when imported to Photos.
 
     Note: This will modify the image and video files in place and will result in
@@ -87,30 +100,36 @@
     if not manual and not files:
         click.echo("No files specified", err=True)
         click.echo(main.get_help(click.Context(main)))
         raise click.Abort()
 
     # process manual files first
     for image, video in manual:
-        if image.suffix.lower() not in IMAGE_EXTENSIONS:
+        if not is_image_file(image):
             click.echo(f"{image} is not a JPEG or HEIC image", err=True)
             raise click.Abort()
-        if video.suffix.lower() not in VIDEO_EXTENSIONS:
+        if not is_video_file(video):
             click.echo(f"{video} is not a QuickTime movie file", err=True)
             raise click.Abort()
-        asset_id = make_live_photo(image, video)
-        if verbose:
-            click.echo(f"Wrote asset ID: {asset_id} to {image} and {video}")
+        if check:
+            check_pair(image, video)
+        else:
+            asset_id = make_live_photo(image, video)
+            if verbose:
+                click.echo(f"Wrote asset ID: {asset_id} to {image} and {video}")
 
     # process any files passed via FILES argument
     matched_files, unmatched_files = find_photo_video_pairs(files)
 
     for image, video in matched_files:
-        asset_id = make_live_photo(image, video)
-        if verbose:
-            click.echo(f"Wrote asset ID: {asset_id} to {image} and {video}")
+        if check:
+            check_pair(image, video)
+        else:
+            asset_id = make_live_photo(image, video)
+            if verbose:
+                click.echo(f"Wrote asset ID: {asset_id} to {image} and {video}")
     for file in unmatched_files:
         click.echo(f"No matching file pair found for {file}", err=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `makelive-0.4.2/makelive/makelive.py` & `makelive-0.5.0/makelive/makelive.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import os
 import pathlib
 import threading
 import uuid
 
 import AVFoundation
+import cgmetadata
 import objc
 import Quartz
 from Foundation import (
     NSURL,
     CFDictionaryRef,
     NSData,
     NSMutableData,
@@ -199,14 +200,26 @@
             os.rename(temp_filepath, filepath)
         else:
             os.unlink(temp_filepath)
 
         return error or None
 
 
+def is_image_file(filepath: str | os.PathLike):
+    """Return True if the file is a JPEG or HEIC image file"""
+    filepath = pathlib.Path(filepath)
+    return filepath.suffix.lower() in [".jpg", ".jpeg", ".heic", ".heif"]
+
+
+def is_video_file(filepath: str | os.PathLike):
+    """Return True if the file is a MOV or MP4 video file"""
+    filepath = pathlib.Path(filepath)
+    return filepath.suffix.lower() in [".mov", ".mp4"]
+
+
 ### Public API ###
 
 
 def make_live_photo(
     image_path: str | os.PathLike,
     video_path: str | os.PathLike,
     asset_id: str | None = None,
@@ -244,15 +257,84 @@
     """
     image_path = pathlib.Path(image_path)
     video_path = pathlib.Path(video_path)
     if not image_path.exists():
         raise FileNotFoundError(f"{image_path} does not exist")
     if not video_path.exists():
         raise FileNotFoundError(f"{video_path} does not exist")
-    if image_path.suffix.lower() not in [".jpg", ".jpeg", ".heic", ".heif"]:
+    if not is_image_file(image_path):
         raise ValueError(f"{image_path} is not a JPEG or HEIC image")
-    if video_path.suffix.lower() not in [".mov", ".mp4"]:
+    if not is_video_file(video_path):
         raise ValueError(f"{video_path} is not a QuickTime movie file")
     asset_id = asset_id or str(uuid.uuid4()).upper()
     add_asset_id_to_image_file(image_path, asset_id)
     add_asset_id_to_quicktime_file(video_path, asset_id)
     return asset_id
+
+
+def live_id(filepath: str | os.PathLike) -> str | None:
+    """Returns the Live Photo Content Identifier for the file or None
+
+    Args:
+        filepath: Path to the image or video file.
+
+    Returns: The content identifier for the Live Photo or None if not found.
+
+    Note: The content identifier (stored in Maker Notes with key "17" for images and
+        in QuickTime metadata for videos) is used by Photos to link the image and video files
+        together as a Live Photo.
+
+    Raises:
+        FileNotFoundError: If the file does not exist.
+        ValueError: If the file is not a JPEG/HEIC image or MOV/MP4 video file.
+    """
+    filepath = pathlib.Path(filepath)
+    if not filepath.exists():
+        raise FileNotFoundError(f"{filepath} does not exist")
+
+    if is_image_file(filepath):
+        md = cgmetadata.ImageMetadata(filepath)
+        try:
+            return md.asdict()["MakerApple"]["17"]
+        except KeyError:
+            return None
+    elif is_video_file(filepath):
+        with objc.autorelease_pool():
+            url = NSURL.fileURLWithPath_(str(filepath))
+            asset = AVFoundation.AVAsset.assetWithURL_(url)
+            for item in asset.metadata():
+                if item.key() == kKeyContentIdentifier and item.keySpace() == kKeySpaceQuickTimeMetadata:
+                    return str(item.value())
+        return None
+    else:
+        raise ValueError(f"{filepath} is not a JPEG/HEIC image or MOV/MP4 video file")
+
+
+def is_live_photo_pair(image_path: str | os.PathLike, video_path: str | os.PathLike) -> str | bool:
+    """Check if the image and video pair are a Live Photo
+
+    Args:
+        image_path: Path to the image file.
+        video_path: Path to the QuickTime movie file.
+
+    Returns: Asset ID if the file pair is a Live Photo (truthy value), False otherwise.
+
+    Raises:
+        FileNotFoundError: If image_path or video_path does not exist.
+        ValueError: If image_path is not a JPEG or HEIC image or video_path is not a QuickTime movie file.
+    """
+    image_path = pathlib.Path(image_path)
+    video_path = pathlib.Path(video_path)
+    if not image_path.exists():
+        raise FileNotFoundError(f"{image_path} does not exist")
+    if not video_path.exists():
+        raise FileNotFoundError(f"{video_path} does not exist")
+
+    if not is_image_file(image_path):
+        raise ValueError("Image file is not a JPEG or HEIC image")
+    if not is_video_file(video_path):
+        raise ValueError("Video file is not a QuickTime movie file")
+
+    if image_id := live_id(image_path):
+        if video_id := live_id(video_path):
+            return image_id if image_id == video_id else False
+    return False
```

### Comparing `makelive-0.4.2/pyproject.toml` & `makelive-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 authors = [{ name = "Rhet Turnbull", email = "rturnbull+git@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 requires-python = ">3.9"
 dependencies = [
+    "cgmetadata>=0.1.6",
     "click>=8.0.0",
     "pyobjc-core>=9.2",
     "pyobjc-framework-AVFoundation>=9.2",
     "pyobjc-framework-Contacts>=9.2",
     "pyobjc-framework-CoreLocation>=9.2",
     "pyobjc-framework-Quartz>=9.2",
     "pyobjc-framework-UniformTypeIdentifiers>=9.2",
```

### Comparing `makelive-0.4.2/PKG-INFO` & `makelive-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: makelive
-Version: 0.4.2
+Version: 0.5.0
 Summary: Add the necessary metadata to photo + video pair so Photos recognizes them as Live Photos when imported
 Author-email: Rhet Turnbull <rturnbull+git@gmail.com>
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: cgmetadata>=0.1.6
 Requires-Dist: click>=8.0.0
 Requires-Dist: pyobjc-core>=9.2
 Requires-Dist: pyobjc-framework-AVFoundation>=9.2
 Requires-Dist: pyobjc-framework-Contacts>=9.2
 Requires-Dist: pyobjc-framework-CoreLocation>=9.2
 Requires-Dist: pyobjc-framework-Quartz>=9.2
 Requires-Dist: pyobjc-framework-UniformTypeIdentifiers>=9.2
@@ -53,23 +54,35 @@
 * `git clone git@github.com:RhetTbull/makelive.git`
 * `cd makelive`
 * `pip install flit`
 * `flit install`
 
 ## API
 
+You can use makelive to programmatically create Live Photo pairs:
+
 ```python
 from makelive import make_live_photo
 
 photo_path = "test.jpg"
 video_path = "test.mov"
 asset_id = make_live_photo(photo_path, video_path)
 print(f"Wrote Asset ID: {asset_id} to {photo_path} and {video_path}")
 ```
 
+You can also check if a photo and video pair are a Live Photo pair and get the asset ID:
+
+```python
+from makelive import live_id, is_live_photo_pair
+photo_path = "test.jpg"
+video_path = "test.mov"
+print(f"Is Live Photo Pair: {is_live_photo_pair(photo_path, video_path)}")
+print(f"Asset ID: {live_id(photo_path)}")
+```
+
 **Note:** XMP metadata in the QuickTime movie file is not preserved by this function which may result in metadata loss.
 
 Metadata including EXIF, IPTC, and XMP are preserved in the image file but will be rewritten and the Core Graphics API may change the order of the metadata and normalize the values. For example, the tag XMP:TagsList will be rewritten as XMP:Subject and the value will be normalized to a list of title case strings.
 
 If you must preserve the original metadata completely, it is recommended to make a copy of the metadata using a tool like [exiftool](https://exiftool.org) before calling this function and then restore the metadata after calling this function. (But take care not to delete the ContentIdentifier metadata.)
 
 ## How it works
```

