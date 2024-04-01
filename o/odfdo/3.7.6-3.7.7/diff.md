# Comparing `tmp/odfdo-3.7.6.tar.gz` & `tmp/odfdo-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odfdo-3.7.6.tar", max compression
+gzip compressed data, was "odfdo-3.7.7.tar", max compression
```

## Comparing `odfdo-3.7.6.tar` & `odfdo-3.7.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.6/LICENSE
--rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.6/NOTICE.txt
--rw-r--r--   0        0        0     3277 2024-03-23 22:16:21.018339 odfdo-3.7.6/README.md
--rw-r--r--   0        0        0     5254 2024-03-23 16:14:57.880774 odfdo-3.7.6/odfdo/__init__.py
--rw-r--r--   0        0        0     2361 2024-03-23 09:53:15.692288 odfdo-3.7.6/odfdo/bookmark.py
--rw-r--r--   0        0        0    13076 2024-03-23 22:16:21.030948 odfdo-3.7.6/odfdo/cell.py
--rw-r--r--   0        0        0    21620 2024-03-23 22:16:21.031098 odfdo-3.7.6/odfdo/const.py
--rw-r--r--   0        0        0    16027 2024-03-23 22:16:21.031267 odfdo-3.7.6/odfdo/container.py
--rw-r--r--   0        0        0     3463 2024-03-23 09:53:15.692544 odfdo-3.7.6/odfdo/content.py
--rw-r--r--   0        0        0     6668 2024-03-23 09:53:15.693983 odfdo-3.7.6/odfdo/datatype.py
--rw-r--r--   0        0        0    41960 2024-03-23 22:16:21.031457 odfdo-3.7.6/odfdo/document.py
--rw-r--r--   0        0        0     4192 2024-03-23 09:53:15.690173 odfdo-3.7.6/odfdo/draw_page.py
--rw-r--r--   0        0        0   107514 2024-03-23 16:14:57.881654 odfdo-3.7.6/odfdo/element.py
--rw-r--r--   0        0        0     7976 2024-03-23 09:53:15.688916 odfdo-3.7.6/odfdo/element_typed.py
--rw-r--r--   0        0        0    15586 2024-03-23 09:53:15.692790 odfdo-3.7.6/odfdo/frame.py
--rw-r--r--   0        0        0     3665 2024-03-23 09:53:15.690454 odfdo-3.7.6/odfdo/header.py
--rw-r--r--   0        0        0     1270 2024-03-23 09:53:15.694433 odfdo-3.7.6/odfdo/header_rows.py
--rw-r--r--   0        0        0     3524 2024-03-23 09:53:15.694687 odfdo-3.7.6/odfdo/image.py
--rw-r--r--   0        0        0     3206 2024-03-23 09:53:15.688794 odfdo-3.7.6/odfdo/link.py
--rw-r--r--   0        0        0     7129 2024-03-23 09:53:15.689684 odfdo-3.7.6/odfdo/list.py
--rw-r--r--   0        0        0     3812 2024-03-23 09:53:15.690547 odfdo-3.7.6/odfdo/manifest.py
--rw-r--r--   0        0        0    18936 2024-03-23 09:53:15.694948 odfdo-3.7.6/odfdo/meta.py
--rw-r--r--   0        0        0    11191 2024-03-23 09:53:15.694558 odfdo-3.7.6/odfdo/note.py
--rw-r--r--   0        0        0    28204 2024-03-23 09:53:15.693394 odfdo-3.7.6/odfdo/paragraph.py
--rw-r--r--   0        0        0     9443 2024-03-23 09:53:15.692654 odfdo-3.7.6/odfdo/paragraph_base.py
--rw-r--r--   0        0        0    14661 2024-03-23 09:53:15.693515 odfdo-3.7.6/odfdo/reference.py
--rw-r--r--   0        0        0    25859 2024-03-23 22:16:21.031623 odfdo-3.7.6/odfdo/row.py
--rw-r--r--   0        0        0        1 2024-03-23 09:53:15.696759 odfdo-3.7.6/odfdo/scripts/__init__.py
--rwxr-xr-x   0        0        0     3280 2024-03-23 16:14:57.881968 odfdo-3.7.6/odfdo/scripts/diff.py
--rwxr-xr-x   0        0        0     2186 2024-03-23 16:14:57.882092 odfdo-3.7.6/odfdo/scripts/folder.py
--rwxr-xr-x   0        0        0     3803 2024-03-23 09:53:15.697520 odfdo-3.7.6/odfdo/scripts/headers.py
--rwxr-xr-x   0        0        0     5832 2024-03-23 16:14:57.882234 odfdo-3.7.6/odfdo/scripts/highlight.py
--rwxr-xr-x   0        0        0     3603 2024-03-23 16:14:57.882360 odfdo-3.7.6/odfdo/scripts/replace.py
--rwxr-xr-x   0        0        0     5752 2024-03-23 16:14:57.882501 odfdo-3.7.6/odfdo/scripts/show.py
--rwxr-xr-x   0        0        0     7576 2024-03-23 16:14:57.882651 odfdo-3.7.6/odfdo/scripts/styles.py
--rwxr-xr-x   0        0        0     3442 2024-03-23 22:16:21.031744 odfdo-3.7.6/odfdo/scripts/table_shrink.py
--rw-r--r--   0        0        0     1936 2024-03-23 09:53:15.690947 odfdo-3.7.6/odfdo/scriptutils.py
--rw-r--r--   0        0        0     1939 2024-03-23 09:53:15.691464 odfdo-3.7.6/odfdo/section.py
--rw-r--r--   0        0        0    11548 2024-03-23 09:53:15.689442 odfdo-3.7.6/odfdo/shapes.py
--rw-r--r--   0        0        0     4691 2024-03-23 09:53:15.691557 odfdo-3.7.6/odfdo/smil.py
--rw-r--r--   0        0        0    38072 2024-03-23 16:14:57.882919 odfdo-3.7.6/odfdo/style.py
--rw-r--r--   0        0        0     5244 2024-03-23 09:53:15.693078 odfdo-3.7.6/odfdo/styles.py
--rw-r--r--   0        0        0   104120 2024-03-23 22:16:21.032049 odfdo-3.7.6/odfdo/table.py
--rw-r--r--   0        0        0        1 2024-03-23 09:53:15.697675 odfdo-3.7.6/odfdo/templates/__init__.py
--rw-r--r--   0        0        0     8291 2024-03-09 17:25:46.512497 odfdo-3.7.6/odfdo/templates/drawing.otg
--rw-r--r--   0        0        0    11017 2024-03-09 17:25:46.513270 odfdo-3.7.6/odfdo/templates/lpod_styles.odt
--rw-r--r--   0        0        0    16065 2024-03-09 17:25:46.513697 odfdo-3.7.6/odfdo/templates/presentation.otp
--rw-r--r--   0        0        0     7432 2024-03-09 17:25:46.514222 odfdo-3.7.6/odfdo/templates/spreadsheet.ots
--rw-r--r--   0        0        0     9620 2024-03-09 17:25:46.514778 odfdo-3.7.6/odfdo/templates/text.ott
--rw-r--r--   0        0        0    17070 2024-03-23 09:53:15.689286 odfdo-3.7.6/odfdo/toc.py
--rw-r--r--   0        0        0    24638 2024-03-23 09:53:15.691372 odfdo-3.7.6/odfdo/tracked_changes.py
--rw-r--r--   0        0        0     1318 2024-03-23 16:14:57.883335 odfdo-3.7.6/odfdo/utils/__init__.py
--rw-r--r--   0        0        0     9339 2024-03-23 09:53:15.696258 odfdo-3.7.6/odfdo/utils/cache_map.py
--rw-r--r--   0        0        0      926 2024-03-23 09:53:15.695794 odfdo-3.7.6/odfdo/utils/cached_element.py
--rw-r--r--   0        0        0     3035 2024-03-23 16:14:57.883429 odfdo-3.7.6/odfdo/utils/color.py
--rw-r--r--   0        0        0     4533 2024-03-23 09:53:15.695970 odfdo-3.7.6/odfdo/utils/coordinates.py
--rw-r--r--   0        0        0     1476 2024-03-23 09:53:15.695219 odfdo-3.7.6/odfdo/utils/formula.py
--rw-r--r--   0        0        0     1314 2024-03-23 09:53:15.695133 odfdo-3.7.6/odfdo/utils/isiterable.py
--rw-r--r--   0        0        0     1429 2024-03-23 09:53:15.695688 odfdo-3.7.6/odfdo/utils/str_convert.py
--rw-r--r--   0        0        0     2503 2024-03-23 09:53:15.695883 odfdo-3.7.6/odfdo/utils/style_constants.py
--rw-r--r--   0        0        0     4272 2024-03-23 09:53:15.695404 odfdo-3.7.6/odfdo/utils/xpath_query.py
--rw-r--r--   0        0        0    14844 2024-03-23 09:53:15.692407 odfdo-3.7.6/odfdo/variable.py
--rw-r--r--   0        0        0     1165 2024-03-23 09:53:15.689580 odfdo-3.7.6/odfdo/version.py
--rw-r--r--   0        0        0     3688 2024-03-23 09:53:15.690853 odfdo-3.7.6/odfdo/xmlpart.py
--rw-r--r--   0        0        0     3878 2024-03-30 10:58:34.883213 odfdo-3.7.6/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 odfdo-3.7.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.7/LICENSE
+-rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.7/NOTICE.txt
+-rw-r--r--   0        0        0     3308 2024-04-01 16:01:23.803500 odfdo-3.7.7/README.md
+-rw-r--r--   0        0        0     5254 2024-04-01 10:08:15.947787 odfdo-3.7.7/odfdo/__init__.py
+-rw-r--r--   0        0        0     2361 2024-04-01 10:08:15.948752 odfdo-3.7.7/odfdo/bookmark.py
+-rw-r--r--   0        0        0    13076 2024-04-01 10:08:15.949530 odfdo-3.7.7/odfdo/cell.py
+-rw-r--r--   0        0        0    21620 2024-04-01 10:08:15.951225 odfdo-3.7.7/odfdo/const.py
+-rw-r--r--   0        0        0    16027 2024-04-01 10:08:15.952036 odfdo-3.7.7/odfdo/container.py
+-rw-r--r--   0        0        0     3463 2024-04-01 10:08:15.952350 odfdo-3.7.7/odfdo/content.py
+-rw-r--r--   0        0        0     6668 2024-04-01 10:08:15.952639 odfdo-3.7.7/odfdo/datatype.py
+-rw-r--r--   0        0        0    41960 2024-04-01 10:08:15.953310 odfdo-3.7.7/odfdo/document.py
+-rw-r--r--   0        0        0     4192 2024-04-01 10:08:15.953626 odfdo-3.7.7/odfdo/draw_page.py
+-rw-r--r--   0        0        0   107411 2024-04-01 10:08:15.954747 odfdo-3.7.7/odfdo/element.py
+-rw-r--r--   0        0        0     7976 2024-04-01 10:08:15.955617 odfdo-3.7.7/odfdo/element_typed.py
+-rw-r--r--   0        0        0    15586 2024-04-01 10:08:15.956248 odfdo-3.7.7/odfdo/frame.py
+-rw-r--r--   0        0        0     3665 2024-04-01 10:08:15.956563 odfdo-3.7.7/odfdo/header.py
+-rw-r--r--   0        0        0     1270 2024-04-01 10:08:15.957382 odfdo-3.7.7/odfdo/header_rows.py
+-rw-r--r--   0        0        0     3524 2024-04-01 10:08:15.957701 odfdo-3.7.7/odfdo/image.py
+-rw-r--r--   0        0        0     3206 2024-04-01 10:08:15.957997 odfdo-3.7.7/odfdo/link.py
+-rw-r--r--   0        0        0     7129 2024-04-01 10:08:15.958225 odfdo-3.7.7/odfdo/list.py
+-rw-r--r--   0        0        0     3812 2024-04-01 10:08:15.958534 odfdo-3.7.7/odfdo/manifest.py
+-rw-r--r--   0        0        0    18936 2024-04-01 10:08:15.958713 odfdo-3.7.7/odfdo/meta.py
+-rw-r--r--   0        0        0    11191 2024-04-01 10:08:15.958954 odfdo-3.7.7/odfdo/note.py
+-rw-r--r--   0        0        0    28204 2024-04-01 10:08:15.959276 odfdo-3.7.7/odfdo/paragraph.py
+-rw-r--r--   0        0        0     9443 2024-04-01 10:08:15.960044 odfdo-3.7.7/odfdo/paragraph_base.py
+-rw-r--r--   0        0        0    14661 2024-04-01 10:08:15.960585 odfdo-3.7.7/odfdo/reference.py
+-rw-r--r--   0        0        0    25859 2024-04-01 10:08:15.961041 odfdo-3.7.7/odfdo/row.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.961512 odfdo-3.7.7/odfdo/scripts/__init__.py
+-rwxr-xr-x   0        0        0     3280 2024-04-01 10:08:15.962026 odfdo-3.7.7/odfdo/scripts/diff.py
+-rwxr-xr-x   0        0        0     2186 2024-04-01 10:08:15.962447 odfdo-3.7.7/odfdo/scripts/folder.py
+-rwxr-xr-x   0        0        0     3803 2024-04-01 10:08:15.963301 odfdo-3.7.7/odfdo/scripts/headers.py
+-rwxr-xr-x   0        0        0     5832 2024-04-01 10:08:15.963611 odfdo-3.7.7/odfdo/scripts/highlight.py
+-rwxr-xr-x   0        0        0     3603 2024-04-01 10:08:15.963998 odfdo-3.7.7/odfdo/scripts/replace.py
+-rwxr-xr-x   0        0        0     5752 2024-04-01 10:08:15.964706 odfdo-3.7.7/odfdo/scripts/show.py
+-rwxr-xr-x   0        0        0     7576 2024-04-01 10:08:15.965411 odfdo-3.7.7/odfdo/scripts/styles.py
+-rwxr-xr-x   0        0        0     3442 2024-04-01 10:08:15.966077 odfdo-3.7.7/odfdo/scripts/table_shrink.py
+-rw-r--r--   0        0        0     1936 2024-04-01 10:08:15.967048 odfdo-3.7.7/odfdo/scriptutils.py
+-rw-r--r--   0        0        0     1939 2024-04-01 10:08:15.967336 odfdo-3.7.7/odfdo/section.py
+-rw-r--r--   0        0        0    11548 2024-04-01 10:08:15.967836 odfdo-3.7.7/odfdo/shapes.py
+-rw-r--r--   0        0        0     4691 2024-04-01 10:08:15.968192 odfdo-3.7.7/odfdo/smil.py
+-rw-r--r--   0        0        0    38072 2024-04-01 10:08:15.968702 odfdo-3.7.7/odfdo/style.py
+-rw-r--r--   0        0        0     5244 2024-04-01 10:08:15.969088 odfdo-3.7.7/odfdo/styles.py
+-rw-r--r--   0        0        0   104120 2024-04-01 10:08:15.969691 odfdo-3.7.7/odfdo/table.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.970133 odfdo-3.7.7/odfdo/templates/__init__.py
+-rw-r--r--   0        0        0     8291 2024-04-01 10:08:15.970835 odfdo-3.7.7/odfdo/templates/drawing.otg
+-rw-r--r--   0        0        0    11017 2024-04-01 10:08:15.971235 odfdo-3.7.7/odfdo/templates/lpod_styles.odt
+-rw-r--r--   0        0        0    16065 2024-04-01 10:08:15.971582 odfdo-3.7.7/odfdo/templates/presentation.otp
+-rw-r--r--   0        0        0     7432 2024-04-01 10:08:15.972020 odfdo-3.7.7/odfdo/templates/spreadsheet.ots
+-rw-r--r--   0        0        0     9620 2024-04-01 10:08:15.972500 odfdo-3.7.7/odfdo/templates/text.ott
+-rw-r--r--   0        0        0    17070 2024-04-01 10:08:15.973345 odfdo-3.7.7/odfdo/toc.py
+-rw-r--r--   0        0        0    24638 2024-04-01 10:08:15.973733 odfdo-3.7.7/odfdo/tracked_changes.py
+-rw-r--r--   0        0        0     1318 2024-04-01 10:08:15.973907 odfdo-3.7.7/odfdo/utils/__init__.py
+-rw-r--r--   0        0        0     9339 2024-04-01 10:08:15.974689 odfdo-3.7.7/odfdo/utils/cache_map.py
+-rw-r--r--   0        0        0      926 2024-04-01 10:08:15.975005 odfdo-3.7.7/odfdo/utils/cached_element.py
+-rw-r--r--   0        0        0     3035 2024-04-01 10:08:15.975436 odfdo-3.7.7/odfdo/utils/color.py
+-rw-r--r--   0        0        0     4533 2024-04-01 10:08:15.975823 odfdo-3.7.7/odfdo/utils/coordinates.py
+-rw-r--r--   0        0        0     1476 2024-04-01 10:08:15.976142 odfdo-3.7.7/odfdo/utils/formula.py
+-rw-r--r--   0        0        0     1314 2024-04-01 10:08:15.976364 odfdo-3.7.7/odfdo/utils/isiterable.py
+-rw-r--r--   0        0        0     1429 2024-04-01 10:08:15.976629 odfdo-3.7.7/odfdo/utils/str_convert.py
+-rw-r--r--   0        0        0     2503 2024-04-01 10:08:15.976906 odfdo-3.7.7/odfdo/utils/style_constants.py
+-rw-r--r--   0        0        0     4272 2024-04-01 10:08:15.977335 odfdo-3.7.7/odfdo/utils/xpath_query.py
+-rw-r--r--   0        0        0    14844 2024-04-01 10:08:15.977547 odfdo-3.7.7/odfdo/variable.py
+-rw-r--r--   0        0        0     1165 2024-04-01 10:08:15.977698 odfdo-3.7.7/odfdo/version.py
+-rw-r--r--   0        0        0     3688 2024-04-01 10:08:15.978014 odfdo-3.7.7/odfdo/xmlpart.py
+-rw-r--r--   0        0        0     3844 2024-04-01 16:01:23.830660 odfdo-3.7.7/pyproject.toml
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 odfdo-3.7.7/PKG-INFO
```

### Comparing `odfdo-3.7.6/LICENSE` & `odfdo-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/README.md` & `odfdo-3.7.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # odfdo
-Python library for OpenDocument format (ODF)
 
+Python library for OpenDocument format (ODF)
 
 ![logo](https://raw.githubusercontent.com/jdum/odfdo/master/odfdo.png)
 
 `odfdo` is a Python3 library implementing the ISO/IEC 26300 OpenDocument Format
 standard.
 
 Project:
-    https://github.com/jdum/odfdo
+https://github.com/jdum/odfdo
 
 Author:
-    jerome.dumonteil@gmail.com
+jerome.dumonteil@gmail.com
 
 License:
-    Apache License, Version 2.0
+Apache License, Version 2.0
 
 `odfdo` is a derivative work of the former `lpod-python` project.
 
-
-Installation
-============
+# Installation
 
 Installation from Pypi (recommended):
 
 ```python
 pip install odfdo
 ```
 
@@ -38,81 +36,72 @@
 
 ```python
 pytest
 ```
 
 The tests should run for a few seconds or minutes and issue no error.
 
-
-Usage
-=====
-
+# Usage
 
     from odfdo import Document, Paragraph
 
     doc = Document('text')
     doc.body.append(Paragraph("Hello world!"))
     doc.save("hello.odt")
 
-
-tl;dr
-=====
+# tl;dr
 
 'Intended Audience :: Developers'
 
-
-Documentation
-=============
+# Documentation
 
 There is no detailed documentation or tutorial, but:
 
- - the `recipes` folder contains more than 50 working sample scripts,
- - the `doc` folder contains an auto generated documentation.
+-   the `recipes` folder contains more than 50 working sample scripts,
+-   the `doc` folder contains an auto generated documentation.
 
 When installing odfdo, a few scripts are installed:
 
- - `odfdo-diff`: show a *diff* between two .odt document.
- - `odfdo-folder`: convert standard ODF file to folder and files, and reverse.
- - `odfdo-show`: dump text from an ODF file to the standard output, and optionally styles and meta informations.
- - `odfdo-styles`: command line interface tool to manipulate styles of ODF files.
- - `odfdo-replace`: find a pattern (regex) in an ODF file and replace by some string.
- - `odfdo-highlight`: highlight the text matching a pattern (regex) in an ODF file.
- - `odfdo-headers`: print the headers of an ODF file.
- - `odfdo-table-shrink`: shrink tables to optimize width and height (experimental).
+-   `odfdo-diff`: show a _diff_ between two .odt document.
+-   `odfdo-folder`: convert standard ODF file to folder and files, and reverse.
+-   `odfdo-show`: dump text from an ODF file to the standard output, and optionally styles and meta informations.
+-   `odfdo-styles`: command line interface tool to manipulate styles of ODF files.
+-   `odfdo-replace`: find a pattern (regex) in an ODF file and replace by some string.
+-   `odfdo-highlight`: highlight the text matching a pattern (regex) in an ODF file.
+-   `odfdo-headers`: print the headers of an ODF file.
+-   `odfdo-table-shrink`: shrink tables to optimize width and height.
 
 About styles: the best way to apply style is by merging styles from a template
 document into your generated document (See `odfdo-styles` script).
 Styles are a complex matter in ODF, so trying to generate styles programmatically
 is not recommended.
 
-
-Limitations
-===========
+# Limitations
 
 `odfdo` is intended to facilitate the generation of ODF documents,
 nevertheless a basic knowledge of the ODF format is necessary.
 
 ODF document rendering can vary greatly from software to software. Especially the
 "styles" of the document allow an adaptation of the rendering for a particular
 software.
 
 The best (only ?) way to apply style is by merging styles from a template
-document into your generated document.
+document into your generated document. However a few recipes show how to make
+programmatically some basic styles: `create_basic_text_styles`, `add_text_span_styles`).
+
+# Related project
 
-Related project
-===============
+I you work on `.ods` files (spreadsheet), you may be interested by these scripts using
+this library to parse/generate `.ods` files:
+`https://github.com/jdum/odsgenerator` and `https://github.com/jdum/odsparsator`
 
-I you work on .ods files (spreadsheet), you may be interested by these scripts that
-use this library to parse/generate .ods files:
-https://github.com/jdum/odsgenerator and https://github.com/jdum/odsparsator
+# Changes from former lpod library
 
-Changes from former lpod library
-================================
 `lpod-python` was written in 2009-2010 as a Python 2.x library,
-see: https://github.com/lpod/lpod-python
+see: `https://github.com/lpod/lpod-python`
 
 `odfdo` is an adaptation of this former project. `odfdo` main changes from `lpod`:
 
- - `odfdo` requires Python version 3.9 to 3.12. For Python 3.6 to 3.8 see previous releases.
- - API change: more pythonic.
- - include recipes.
- - use Apache 2.0 license.
+-   `odfdo` requires Python version 3.9 to 3.12. For Python 3.6 to 3.8 see previous releases.
+-   API change: more pythonic.
+-   include recipes.
+-   use Apache 2.0 license.
```

### Comparing `odfdo-3.7.6/odfdo/__init__.py` & `odfdo-3.7.7/odfdo/__init__.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/bookmark.py` & `odfdo-3.7.7/odfdo/bookmark.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/cell.py` & `odfdo-3.7.7/odfdo/cell.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/const.py` & `odfdo-3.7.7/odfdo/const.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/container.py` & `odfdo-3.7.7/odfdo/container.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/content.py` & `odfdo-3.7.7/odfdo/content.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/datatype.py` & `odfdo-3.7.7/odfdo/datatype.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/document.py` & `odfdo-3.7.7/odfdo/document.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/draw_page.py` & `odfdo-3.7.7/odfdo/draw_page.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/element.py` & `odfdo-3.7.7/odfdo/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 from re import search
 from typing import Any, NamedTuple
 
 from lxml.etree import Element as lxml_Element
 from lxml.etree import (
     XPath,
     _Element,
-    _ElementStringResult,
-    _ElementUnicodeResult,
     fromstring,
     tostring,
 )
 
 from .const import ODF_COLOR_PROPERTY
 from .datatype import Boolean, DateTime
 from .utils import (
@@ -277,17 +275,17 @@
 
     Constructed like any str object but only accepts lxml text objects.
     """
 
     # There's some black magic in inheriting from str
     def __init__(
         self,
-        text_result: _ElementUnicodeResult | _ElementStringResult,
+        text_result: str | bytes,
     ) -> None:
-        self.__parent = text_result.getparent()
+        self.__parent = text_result.getparent()  # type: ignore
         self.__is_text = text_result.is_text
         self.__is_tail = text_result.is_tail
 
     @property
     def parent(self) -> Element | None:
         parent = self.__parent
         # XXX happens just because of the unit test
@@ -1585,15 +1583,15 @@
         """
         element = self.__element
         xpath_instance = xpath_compile(xpath_query)
         elements = xpath_instance(element)
         result: list[Element | Text] = []
         if hasattr(elements, "__iter__"):
             for obj in elements:  # type: ignore
-                if isinstance(obj, (_ElementStringResult, _ElementUnicodeResult)):
+                if isinstance(obj, (str, bytes)):
                     result.append(Text(obj))
                 elif isinstance(obj, _Element):
                     result.append(Element.from_tag(obj))
                 # else:
                 #     result.append(obj)
         return result
```

### Comparing `odfdo-3.7.6/odfdo/element_typed.py` & `odfdo-3.7.7/odfdo/element_typed.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/frame.py` & `odfdo-3.7.7/odfdo/frame.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/header.py` & `odfdo-3.7.7/odfdo/header.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/header_rows.py` & `odfdo-3.7.7/odfdo/header_rows.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/image.py` & `odfdo-3.7.7/odfdo/image.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/link.py` & `odfdo-3.7.7/odfdo/link.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/list.py` & `odfdo-3.7.7/odfdo/list.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/manifest.py` & `odfdo-3.7.7/odfdo/manifest.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/meta.py` & `odfdo-3.7.7/odfdo/meta.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/note.py` & `odfdo-3.7.7/odfdo/note.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/paragraph.py` & `odfdo-3.7.7/odfdo/paragraph.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/paragraph_base.py` & `odfdo-3.7.7/odfdo/paragraph_base.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/reference.py` & `odfdo-3.7.7/odfdo/reference.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/row.py` & `odfdo-3.7.7/odfdo/row.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/diff.py` & `odfdo-3.7.7/odfdo/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/folder.py` & `odfdo-3.7.7/odfdo/scripts/folder.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/headers.py` & `odfdo-3.7.7/odfdo/scripts/headers.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/highlight.py` & `odfdo-3.7.7/odfdo/scripts/highlight.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/replace.py` & `odfdo-3.7.7/odfdo/scripts/replace.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/show.py` & `odfdo-3.7.7/odfdo/scripts/show.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/styles.py` & `odfdo-3.7.7/odfdo/scripts/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scripts/table_shrink.py` & `odfdo-3.7.7/odfdo/scripts/table_shrink.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/scriptutils.py` & `odfdo-3.7.7/odfdo/scriptutils.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/section.py` & `odfdo-3.7.7/odfdo/section.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/shapes.py` & `odfdo-3.7.7/odfdo/shapes.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/smil.py` & `odfdo-3.7.7/odfdo/smil.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/style.py` & `odfdo-3.7.7/odfdo/style.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/styles.py` & `odfdo-3.7.7/odfdo/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/table.py` & `odfdo-3.7.7/odfdo/table.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/templates/drawing.otg` & `odfdo-3.7.7/odfdo/templates/drawing.otg`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/templates/lpod_styles.odt` & `odfdo-3.7.7/odfdo/templates/lpod_styles.odt`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/templates/presentation.otp` & `odfdo-3.7.7/odfdo/templates/presentation.otp`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/templates/spreadsheet.ots` & `odfdo-3.7.7/odfdo/templates/spreadsheet.ots`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/templates/text.ott` & `odfdo-3.7.7/odfdo/templates/text.ott`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/toc.py` & `odfdo-3.7.7/odfdo/toc.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/tracked_changes.py` & `odfdo-3.7.7/odfdo/tracked_changes.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/__init__.py` & `odfdo-3.7.7/odfdo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/cache_map.py` & `odfdo-3.7.7/odfdo/utils/cache_map.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/cached_element.py` & `odfdo-3.7.7/odfdo/utils/cached_element.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/color.py` & `odfdo-3.7.7/odfdo/utils/color.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/coordinates.py` & `odfdo-3.7.7/odfdo/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/formula.py` & `odfdo-3.7.7/odfdo/utils/formula.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/isiterable.py` & `odfdo-3.7.7/odfdo/utils/isiterable.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/str_convert.py` & `odfdo-3.7.7/odfdo/utils/str_convert.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/style_constants.py` & `odfdo-3.7.7/odfdo/utils/style_constants.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/utils/xpath_query.py` & `odfdo-3.7.7/odfdo/utils/xpath_query.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/variable.py` & `odfdo-3.7.7/odfdo/variable.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/version.py` & `odfdo-3.7.7/odfdo/version.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/odfdo/xmlpart.py` & `odfdo-3.7.7/odfdo/xmlpart.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.6/pyproject.toml` & `odfdo-3.7.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 [tool.poetry]
 name = "odfdo"
-version = "3.7.6"
+version = "3.7.7"
 description = "Python library for OpenDocument Format"
 license = "Apache-2.0"
 keywords = ["python", "library", "ODF", "OpenDocument"]
 classifiers = [
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Libraries :: Python Modules",
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 homepage = "https://github.com/jdum/odfdo"
 repository = "https://github.com/jdum/odfdo"
 authors = ["Jérôme Dumonteil <jerome.dumonteil@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "odfdo" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
-lxml = "5.1.0"
-
+lxml = [
+    { version = ">=4.8.0,<5", python = ">=3.9,<3.10" },
+    { version = ">=4.8.0,<5.1.1", python = ">=3.10,<3.11" },
+    { version = ">=4.9.4,<6", python = ">=3.11,<3.12" },
+    { version = ">=4.9.4,<6", python = ">=3.12" },
+]
 [tool.poetry.group.docs.dependencies]
 pdoc = ">=14.4.0"
 
 [tool.poetry.group.dev.dependencies]
 poetry = "~1.8"
 pytest = ">=7.0"
 tox = ">=4"
@@ -62,74 +66,74 @@
 profile = "black"
 
 [tool.ruff]
 target-version = "py312"
 line-length = 88
 fix = false
 lint.select = [
-        # flake8-2020
-        "YTT",
-        # flake8-bandit
-        "S",
-        # flake8-bugbear
-        "B",
-        # flake8-builtins
-        "A",
-        # flake8-comprehensions
-        "C4",
-        # flake8-debugger
-        "T10",
-        # flake8-simplify
-        "SIM",
-        # isort
-        "I",
-        # mccabe
-        "C90",
-        # pycodestyle
-        "E",
-        "W",
-        # pyflakes
-        "F",
-        # pygrep-hooks
-        "PGH",
-        # pyupgrade
-        "UP",
-        # ruff
-        "RUF",
-        # tryceratops
-        "TRY",
+    # flake8-2020
+    "YTT",
+    # flake8-bandit
+    "S",
+    # flake8-bugbear
+    "B",
+    # flake8-builtins
+    "A",
+    # flake8-comprehensions
+    "C4",
+    # flake8-debugger
+    "T10",
+    # flake8-simplify
+    "SIM",
+    # isort
+    "I",
+    # mccabe
+    "C90",
+    # pycodestyle
+    "E",
+    "W",
+    # pyflakes
+    "F",
+    # pygrep-hooks
+    "PGH",
+    # pyupgrade
+    "UP",
+    # ruff
+    "RUF",
+    # tryceratops
+    "TRY",
 ]
 lint.ignore = [
-        # LineTooLong
-        "E501",
-        # DoNotAssignLambda
-        "E731",
-        # Use specific rule codes when ignoring type issues
-        "PGH003",
-        # check for execution of untrusted input
-        "S603",
-        # Class attribute `open` is shadowing a Python builtin
-        "A003",
-        # Use `X | Y` in `isinstance` call instead of `(X, Y)`
-        "UP038",
-        # Avoid specifying long messages outside the exception class
-        "TRY003",
-        # Use ternary operator
-        "SIM108",
-        # Standard pseudo-random generators are not suitable for cryptographic purposes
-        "S311",
-        # Using `lxml` to parse untrusted data is known to be vulnerable to XML attacks
-        "S320",
-        # Use `X | Y` for type annotations
-        "UP007",
+    # LineTooLong
+    "E501",
+    # DoNotAssignLambda
+    "E731",
+    # Use specific rule codes when ignoring type issues
+    "PGH003",
+    # check for execution of untrusted input
+    "S603",
+    # Class attribute `open` is shadowing a Python builtin
+    "A003",
+    # Use `X | Y` in `isinstance` call instead of `(X, Y)`
+    "UP038",
+    # Avoid specifying long messages outside the exception class
+    "TRY003",
+    # Use ternary operator
+    "SIM108",
+    # Standard pseudo-random generators are not suitable for cryptographic purposes
+    "S311",
+    # Using `lxml` to parse untrusted data is known to be vulnerable to XML attacks
+    "S320",
+    # Use `X | Y` for type annotations
+    "UP007",
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "recipes/accessing_a_single_element.py" = ["RUF001"]
-"tests/test_*" = ["S101"]
+"tests/test_*" = ["S101", "RUF005"]
 "recipes/*" = ["S101"]
 
 [tool.mypy]
 check_untyped_defs = "True"
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
```

### Comparing `odfdo-3.7.6/PKG-INFO` & `odfdo-3.7.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odfdo
-Version: 3.7.6
+Version: 3.7.7
 Summary: Python library for OpenDocument Format
 Home-page: https://github.com/jdum/odfdo
 License: Apache-2.0
 Keywords: python,library,ODF,OpenDocument
 Author: Jérôme Dumonteil
 Author-email: jerome.dumonteil@gmail.com
 Requires-Python: >=3.9,<4
@@ -17,41 +17,42 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: lxml (==5.1.0)
+Requires-Dist: lxml (>=4.8.0,<5) ; python_version >= "3.9" and python_version < "3.10"
+Requires-Dist: lxml (>=4.8.0,<5.1.1) ; python_version >= "3.10" and python_version < "3.11"
+Requires-Dist: lxml (>=4.9.4,<6) ; python_version >= "3.11" and python_version < "3.12"
+Requires-Dist: lxml (>=4.9.4,<6) ; python_version >= "3.12"
 Project-URL: Repository, https://github.com/jdum/odfdo
 Description-Content-Type: text/markdown
 
 # odfdo
-Python library for OpenDocument format (ODF)
 
+Python library for OpenDocument format (ODF)
 
 ![logo](https://raw.githubusercontent.com/jdum/odfdo/master/odfdo.png)
 
 `odfdo` is a Python3 library implementing the ISO/IEC 26300 OpenDocument Format
 standard.
 
 Project:
-    https://github.com/jdum/odfdo
+https://github.com/jdum/odfdo
 
 Author:
-    jerome.dumonteil@gmail.com
+jerome.dumonteil@gmail.com
 
 License:
-    Apache License, Version 2.0
+Apache License, Version 2.0
 
 `odfdo` is a derivative work of the former `lpod-python` project.
 
-
-Installation
-============
+# Installation
 
 Installation from Pypi (recommended):
 
 ```python
 pip install odfdo
 ```
 
@@ -65,82 +66,73 @@
 
 ```python
 pytest
 ```
 
 The tests should run for a few seconds or minutes and issue no error.
 
-
-Usage
-=====
-
+# Usage
 
     from odfdo import Document, Paragraph
 
     doc = Document('text')
     doc.body.append(Paragraph("Hello world!"))
     doc.save("hello.odt")
 
-
-tl;dr
-=====
+# tl;dr
 
 'Intended Audience :: Developers'
 
-
-Documentation
-=============
+# Documentation
 
 There is no detailed documentation or tutorial, but:
 
- - the `recipes` folder contains more than 50 working sample scripts,
- - the `doc` folder contains an auto generated documentation.
+-   the `recipes` folder contains more than 50 working sample scripts,
+-   the `doc` folder contains an auto generated documentation.
 
 When installing odfdo, a few scripts are installed:
 
- - `odfdo-diff`: show a *diff* between two .odt document.
- - `odfdo-folder`: convert standard ODF file to folder and files, and reverse.
- - `odfdo-show`: dump text from an ODF file to the standard output, and optionally styles and meta informations.
- - `odfdo-styles`: command line interface tool to manipulate styles of ODF files.
- - `odfdo-replace`: find a pattern (regex) in an ODF file and replace by some string.
- - `odfdo-highlight`: highlight the text matching a pattern (regex) in an ODF file.
- - `odfdo-headers`: print the headers of an ODF file.
- - `odfdo-table-shrink`: shrink tables to optimize width and height (experimental).
+-   `odfdo-diff`: show a _diff_ between two .odt document.
+-   `odfdo-folder`: convert standard ODF file to folder and files, and reverse.
+-   `odfdo-show`: dump text from an ODF file to the standard output, and optionally styles and meta informations.
+-   `odfdo-styles`: command line interface tool to manipulate styles of ODF files.
+-   `odfdo-replace`: find a pattern (regex) in an ODF file and replace by some string.
+-   `odfdo-highlight`: highlight the text matching a pattern (regex) in an ODF file.
+-   `odfdo-headers`: print the headers of an ODF file.
+-   `odfdo-table-shrink`: shrink tables to optimize width and height.
 
 About styles: the best way to apply style is by merging styles from a template
 document into your generated document (See `odfdo-styles` script).
 Styles are a complex matter in ODF, so trying to generate styles programmatically
 is not recommended.
 
-
-Limitations
-===========
+# Limitations
 
 `odfdo` is intended to facilitate the generation of ODF documents,
 nevertheless a basic knowledge of the ODF format is necessary.
 
 ODF document rendering can vary greatly from software to software. Especially the
 "styles" of the document allow an adaptation of the rendering for a particular
 software.
 
 The best (only ?) way to apply style is by merging styles from a template
-document into your generated document.
+document into your generated document. However a few recipes show how to make
+programmatically some basic styles: `create_basic_text_styles`, `add_text_span_styles`).
+
+# Related project
 
-Related project
-===============
+I you work on `.ods` files (spreadsheet), you may be interested by these scripts using
+this library to parse/generate `.ods` files:
+`https://github.com/jdum/odsgenerator` and `https://github.com/jdum/odsparsator`
 
-I you work on .ods files (spreadsheet), you may be interested by these scripts that
-use this library to parse/generate .ods files:
-https://github.com/jdum/odsgenerator and https://github.com/jdum/odsparsator
+# Changes from former lpod library
 
-Changes from former lpod library
-================================
 `lpod-python` was written in 2009-2010 as a Python 2.x library,
-see: https://github.com/lpod/lpod-python
+see: `https://github.com/lpod/lpod-python`
 
 `odfdo` is an adaptation of this former project. `odfdo` main changes from `lpod`:
 
- - `odfdo` requires Python version 3.9 to 3.12. For Python 3.6 to 3.8 see previous releases.
- - API change: more pythonic.
- - include recipes.
- - use Apache 2.0 license.
+-   `odfdo` requires Python version 3.9 to 3.12. For Python 3.6 to 3.8 see previous releases.
+-   API change: more pythonic.
+-   include recipes.
+-   use Apache 2.0 license.
```

