# Comparing `tmp/ebookmaker-0.9.6.tar.gz` & `tmp/ebookmaker-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ebookmaker-0.9.6.tar", last modified: Tue Sep  8 18:32:10 2020, max compression
+gzip compressed data, was "dist/ebookmaker-0.9.7.tar", last modified: Mon Sep 14 19:54:31 2020, max compression
```

## Comparing `ebookmaker-0.9.6.tar` & `ebookmaker-0.9.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/
--rw-r--r--   0 eric       (501) staff       (20)     8071 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/PKG-INFO
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     8071 2020-09-08 18:32:09.000000 ebookmaker-0.9.6/ebookmaker.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2293 2020-09-08 18:32:09.000000 ebookmaker-0.9.6/ebookmaker.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)      107 2020-09-08 18:32:09.000000 ebookmaker-0.9.6/ebookmaker.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       11 2020-09-08 18:32:09.000000 ebookmaker-0.9.6/ebookmaker.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2020-09-08 18:32:09.000000 ebookmaker-0.9.6/ebookmaker.egg-info/dependency_links.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/parsers/
--rw-r--r--   0 eric       (501) staff       (20)    15255 2020-06-12 00:05:26.000000 ebookmaker-0.9.6/ebookmaker/parsers/HTMLParser.py
--rw-r--r--   0 eric       (501) staff       (20)     2056 2020-07-06 17:03:13.000000 ebookmaker-0.9.6/ebookmaker/parsers/WrapperParser.py
--rw-r--r--   0 eric       (501) staff       (20)    21357 2020-02-06 17:42:35.000000 ebookmaker-0.9.6/ebookmaker/parsers/GutenbergTextParser.py
--rw-r--r--   0 eric       (501) staff       (20)     4896 2020-06-28 21:36:42.000000 ebookmaker-0.9.6/ebookmaker/parsers/ImageParser.py
--rw-r--r--   0 eric       (501) staff       (20)    16466 2020-06-30 16:35:09.000000 ebookmaker-0.9.6/ebookmaker/parsers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      699 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/parsers/AuxParser.py
--rw-r--r--   0 eric       (501) staff       (20)      320 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/parsers/broken.png
--rw-r--r--   0 eric       (501) staff       (20)    12092 2019-12-18 22:22:25.000000 ebookmaker-0.9.6/ebookmaker/parsers/RSTParser.py
--rw-r--r--   0 eric       (501) staff       (20)     4306 2020-01-09 19:48:59.000000 ebookmaker-0.9.6/ebookmaker/parsers/CSSParser.py
--rw-r--r--   0 eric       (501) staff       (20)       67 2020-09-08 18:03:05.000000 ebookmaker-0.9.6/ebookmaker/Version.py
--rw-r--r--   0 eric       (501) staff       (20)     2581 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/CommonCode.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/writers/
--rw-r--r--   0 eric       (501) staff       (20)     3318 2020-09-08 17:56:47.000000 ebookmaker-0.9.6/ebookmaker/writers/HTMLWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3683 2020-04-20 21:59:23.000000 ebookmaker-0.9.6/ebookmaker/writers/TxtWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3875 2020-09-08 16:13:22.000000 ebookmaker-0.9.6/ebookmaker/writers/KindleWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3981 2020-09-08 17:41:13.000000 ebookmaker-0.9.6/ebookmaker/writers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     3058 2020-04-20 21:58:28.000000 ebookmaker-0.9.6/ebookmaker/writers/PDFWriter.py
--rw-r--r--   0 eric       (501) staff       (20)    19263 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/writers/cover.jpg
--rw-r--r--   0 eric       (501) staff       (20)    46410 2020-09-08 17:51:52.000000 ebookmaker-0.9.6/ebookmaker/writers/EpubWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     2052 2020-06-12 00:05:26.000000 ebookmaker-0.9.6/ebookmaker/writers/PicsDirWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1134 2020-04-20 21:59:03.000000 ebookmaker-0.9.6/ebookmaker/writers/RSTWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1778 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/WriterFactory.py
--rw-r--r--   0 eric       (501) staff       (20)     9065 2020-05-21 17:19:04.000000 ebookmaker-0.9.6/ebookmaker/HTMLChunker.py
--rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     6115 2020-06-12 00:05:26.000000 ebookmaker-0.9.6/ebookmaker/ParserFactory.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/packagers/
--rw-r--r--   0 eric       (501) staff       (20)      472 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/packagers/GzipPackager.py
--rw-r--r--   0 eric       (501) staff       (20)      470 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/packagers/TxtPackager.py
--rw-r--r--   0 eric       (501) staff       (20)      426 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/packagers/PDFPackager.py
--rw-r--r--   0 eric       (501) staff       (20)     5312 2020-04-20 21:48:09.000000 ebookmaker-0.9.6/ebookmaker/packagers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      436 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/packagers/RSTPackager.py
--rw-r--r--   0 eric       (501) staff       (20)     2154 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/packagers/PushPackager.py
--rw-r--r--   0 eric       (501) staff       (20)      443 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/packagers/HTMLPackager.py
--rw-r--r--   0 eric       (501) staff       (20)     8216 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/UnitameData.py
--rw-r--r--   0 eric       (501) staff       (20)    17246 2020-06-30 18:05:06.000000 ebookmaker-0.9.6/ebookmaker/EbookMaker.py
--rw-r--r--   0 eric       (501) staff       (20)     5006 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/Unitame.py
--rw-r--r--   0 eric       (501) staff       (20)     9449 2020-06-29 18:47:29.000000 ebookmaker-0.9.6/ebookmaker/Spider.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/parsers/
--rw-r--r--   0 eric       (501) staff       (20)     1306 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/parsers/default_style.rst
--rw-r--r--   0 eric       (501) staff       (20)    30638 2019-12-18 22:21:23.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/parsers/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/
--rw-r--r--   0 eric       (501) staff       (20)     2134 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2html.css
--rw-r--r--   0 eric       (501) staff       (20)    30528 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/nroff.py
--rw-r--r--   0 eric       (501) staff       (20)    15825 2018-07-13 20:48:42.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/xhtml1.py
--rw-r--r--   0 eric       (501) staff       (20)    15355 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     1053 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2epub.css
--rw-r--r--   0 eric       (501) staff       (20)     8443 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2all.css
--rw-r--r--   0 eric       (501) staff       (20)     2442 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/epub2.py
--rw-r--r--   0 eric       (501) staff       (20)    53385 2020-01-28 00:07:21.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/writers/xetex.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/
--rw-r--r--   0 eric       (501) staff       (20)     1747 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    20583 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/pg-footer.rst
--rw-r--r--   0 eric       (501) staff       (20)     1042 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/pg-header.rst
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/writers/
--rw-r--r--   0 eric       (501) staff       (20)     6294 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/writers/nroff.py
--rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/writers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/transforms/
--rw-r--r--   0 eric       (501) staff       (20)     5794 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/transforms/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)       26 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/transforms/
--rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/transforms/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    36668 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/transforms/parts.py
--rw-r--r--   0 eric       (501) staff       (20)     1819 2016-07-11 15:14:38.000000 ebookmaker-0.9.6/ebookmaker/mydocutils/nodes.py
--rw-r--r--   0 eric       (501) staff       (20)    13984 2020-09-08 18:19:01.000000 ebookmaker-0.9.6/CHANGES
--rw-r--r--   0 eric       (501) staff       (20)     6248 2020-09-08 16:09:45.000000 ebookmaker-0.9.6/README.md
--rw-r--r--   0 eric       (501) staff       (20)     2300 2020-09-08 18:03:21.000000 ebookmaker-0.9.6/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/scripts/
--rwxr-xr-x   0 eric       (501) staff       (20)     1384 2019-10-22 02:03:55.000000 ebookmaker-0.9.6/scripts/rhyme_compiler
--rwxr-xr-x   0 eric       (501) staff       (20)      319 2014-04-29 14:59:44.000000 ebookmaker-0.9.6/scripts/ebookmaker
--rwxr-xr-x   0 eric       (501) staff       (20)     2094 2014-04-15 21:51:03.000000 ebookmaker-0.9.6/scripts/convert_unitame
--rw-r--r--   0 eric       (501) staff       (20)       73 2020-09-08 18:32:10.000000 ebookmaker-0.9.6/setup.cfg
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/
+-rw-r--r--   0 eric       (501) staff       (20)     8504 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/PKG-INFO
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     8504 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2293 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)      107 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       11 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker.egg-info/dependency_links.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/parsers/
+-rw-r--r--   0 eric       (501) staff       (20)    15255 2020-06-12 00:05:26.000000 ebookmaker-0.9.7/ebookmaker/parsers/HTMLParser.py
+-rw-r--r--   0 eric       (501) staff       (20)     2056 2020-07-06 17:03:13.000000 ebookmaker-0.9.7/ebookmaker/parsers/WrapperParser.py
+-rw-r--r--   0 eric       (501) staff       (20)    21357 2020-02-06 17:42:35.000000 ebookmaker-0.9.7/ebookmaker/parsers/GutenbergTextParser.py
+-rw-r--r--   0 eric       (501) staff       (20)     4896 2020-06-28 21:36:42.000000 ebookmaker-0.9.7/ebookmaker/parsers/ImageParser.py
+-rw-r--r--   0 eric       (501) staff       (20)    16466 2020-06-30 16:35:09.000000 ebookmaker-0.9.7/ebookmaker/parsers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      699 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/parsers/AuxParser.py
+-rw-r--r--   0 eric       (501) staff       (20)      320 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/parsers/broken.png
+-rw-r--r--   0 eric       (501) staff       (20)    12092 2019-12-18 22:22:25.000000 ebookmaker-0.9.7/ebookmaker/parsers/RSTParser.py
+-rw-r--r--   0 eric       (501) staff       (20)     4306 2020-01-09 19:48:59.000000 ebookmaker-0.9.7/ebookmaker/parsers/CSSParser.py
+-rw-r--r--   0 eric       (501) staff       (20)       67 2020-09-14 19:20:30.000000 ebookmaker-0.9.7/ebookmaker/Version.py
+-rw-r--r--   0 eric       (501) staff       (20)     2581 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/CommonCode.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/writers/
+-rw-r--r--   0 eric       (501) staff       (20)     3260 2020-09-09 19:50:30.000000 ebookmaker-0.9.7/ebookmaker/writers/HTMLWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3683 2020-04-20 21:59:23.000000 ebookmaker-0.9.7/ebookmaker/writers/TxtWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3842 2020-09-09 19:52:56.000000 ebookmaker-0.9.7/ebookmaker/writers/KindleWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3916 2020-09-09 19:44:41.000000 ebookmaker-0.9.7/ebookmaker/writers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3058 2020-04-20 21:58:28.000000 ebookmaker-0.9.7/ebookmaker/writers/PDFWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)    19263 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/writers/cover.jpg
+-rw-r--r--   0 eric       (501) staff       (20)    46551 2020-09-10 16:03:57.000000 ebookmaker-0.9.7/ebookmaker/writers/EpubWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     2052 2020-06-12 00:05:26.000000 ebookmaker-0.9.7/ebookmaker/writers/PicsDirWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1134 2020-04-20 21:59:03.000000 ebookmaker-0.9.7/ebookmaker/writers/RSTWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1778 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/WriterFactory.py
+-rw-r--r--   0 eric       (501) staff       (20)     9065 2020-05-21 17:19:04.000000 ebookmaker-0.9.7/ebookmaker/HTMLChunker.py
+-rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     6115 2020-06-12 00:05:26.000000 ebookmaker-0.9.7/ebookmaker/ParserFactory.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/packagers/
+-rw-r--r--   0 eric       (501) staff       (20)      472 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/packagers/GzipPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)      470 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/packagers/TxtPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)      426 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/packagers/PDFPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)     5312 2020-04-20 21:48:09.000000 ebookmaker-0.9.7/ebookmaker/packagers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      436 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/packagers/RSTPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)     2154 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/packagers/PushPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)      443 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/packagers/HTMLPackager.py
+-rw-r--r--   0 eric       (501) staff       (20)     8216 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/UnitameData.py
+-rw-r--r--   0 eric       (501) staff       (20)    17246 2020-06-30 18:05:06.000000 ebookmaker-0.9.7/ebookmaker/EbookMaker.py
+-rw-r--r--   0 eric       (501) staff       (20)     5006 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/Unitame.py
+-rw-r--r--   0 eric       (501) staff       (20)     9449 2020-06-29 18:47:29.000000 ebookmaker-0.9.7/ebookmaker/Spider.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/parsers/
+-rw-r--r--   0 eric       (501) staff       (20)     1306 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/parsers/default_style.rst
+-rw-r--r--   0 eric       (501) staff       (20)    30638 2019-12-18 22:21:23.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/parsers/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/
+-rw-r--r--   0 eric       (501) staff       (20)     2134 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2html.css
+-rw-r--r--   0 eric       (501) staff       (20)    30528 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/nroff.py
+-rw-r--r--   0 eric       (501) staff       (20)    15825 2018-07-13 20:48:42.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/xhtml1.py
+-rw-r--r--   0 eric       (501) staff       (20)    15355 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     1053 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2epub.css
+-rw-r--r--   0 eric       (501) staff       (20)     8443 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2all.css
+-rw-r--r--   0 eric       (501) staff       (20)     2442 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/epub2.py
+-rw-r--r--   0 eric       (501) staff       (20)    53365 2020-09-14 18:53:21.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/writers/xetex.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/
+-rw-r--r--   0 eric       (501) staff       (20)     1747 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    20583 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/pg-footer.rst
+-rw-r--r--   0 eric       (501) staff       (20)     1042 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/pg-header.rst
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/writers/
+-rw-r--r--   0 eric       (501) staff       (20)     6294 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/writers/nroff.py
+-rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/writers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/transforms/
+-rw-r--r--   0 eric       (501) staff       (20)     5794 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/transforms/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)       26 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/transforms/
+-rw-r--r--   0 eric       (501) staff       (20)       27 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/transforms/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    36668 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/transforms/parts.py
+-rw-r--r--   0 eric       (501) staff       (20)     1819 2016-07-11 15:14:38.000000 ebookmaker-0.9.7/ebookmaker/mydocutils/nodes.py
+-rw-r--r--   0 eric       (501) staff       (20)    14774 2020-09-14 19:17:25.000000 ebookmaker-0.9.7/CHANGES
+-rw-r--r--   0 eric       (501) staff       (20)     6609 2020-09-14 19:07:57.000000 ebookmaker-0.9.7/README.md
+-rw-r--r--   0 eric       (501) staff       (20)     2300 2020-09-14 19:20:55.000000 ebookmaker-0.9.7/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/scripts/
+-rwxr-xr-x   0 eric       (501) staff       (20)     1384 2019-10-22 02:03:55.000000 ebookmaker-0.9.7/scripts/rhyme_compiler
+-rwxr-xr-x   0 eric       (501) staff       (20)      319 2014-04-29 14:59:44.000000 ebookmaker-0.9.7/scripts/ebookmaker
+-rwxr-xr-x   0 eric       (501) staff       (20)     2094 2014-04-15 21:51:03.000000 ebookmaker-0.9.7/scripts/convert_unitame
+-rw-r--r--   0 eric       (501) staff       (20)       73 2020-09-14 19:54:31.000000 ebookmaker-0.9.7/setup.cfg
```

### Comparing `ebookmaker-0.9.6/PKG-INFO` & `ebookmaker-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookmaker
-Version: 0.9.6
+Version: 0.9.7
 Summary: The Project Gutenberg tool to generate EPUBs and other ebook formats.
 Home-page: https://github.com/gutenbergtools/ebookmaker/
 Author: Marcello Perathoner
 Maintainer: Eric Hellman
 Maintainer-email: eric@hellman.net
 License: GPL v3
 Description: # EbookMaker
@@ -16,24 +16,33 @@
         
         
         ## Prerequisites
         
         * Python3 >= 3.6
         * HTMLTidy (http://binaries.html-tidy.org/),
         * Kindlegen (https://www.amazon.com/gp/feature.html/?docId=1000765211) or Calibre (https://calibre-ebook.com/)
-        * TexLive (to build from TeX), and
+        * TexLive (to build from TeX and rst), and
         * groff (not sure when this is needed).
         
         For cover generation
         
         * Cairo https://www.cairographics.org/download/
         * Noto Sans and Noto Sans CJK:
             * CentOS or RedHat: `yum install google-noto-sans-cjk-fonts; yum install google-noto-sans-fonts`
             * Ubuntu: `apt-get install fonts-noto-cjk fonts-noto`
         
+        For RST conversion
+        
+        * Libertinus Serif and Libertinus Sans https://github.com/alerque/libertinus
+            * For Linux, 
+                * Download the latest release https://github.com/alerque/libertinus/releases/latest
+                * unzip, put .otf files into ~/.fonts 
+                * update font catalog `fc-cache -f -v`
+        * DejaVu Sans Mono https://dejavu-fonts.github.io/
+        
         Tested with Python 3.6
         
         ## Install
         
         (master branch, editable install)
         `pipenv install ebookmaker`
```

### Comparing `ebookmaker-0.9.6/ebookmaker.egg-info/PKG-INFO` & `ebookmaker-0.9.7/ebookmaker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookmaker
-Version: 0.9.6
+Version: 0.9.7
 Summary: The Project Gutenberg tool to generate EPUBs and other ebook formats.
 Home-page: https://github.com/gutenbergtools/ebookmaker/
 Author: Marcello Perathoner
 Maintainer: Eric Hellman
 Maintainer-email: eric@hellman.net
 License: GPL v3
 Description: # EbookMaker
@@ -16,24 +16,33 @@
         
         
         ## Prerequisites
         
         * Python3 >= 3.6
         * HTMLTidy (http://binaries.html-tidy.org/),
         * Kindlegen (https://www.amazon.com/gp/feature.html/?docId=1000765211) or Calibre (https://calibre-ebook.com/)
-        * TexLive (to build from TeX), and
+        * TexLive (to build from TeX and rst), and
         * groff (not sure when this is needed).
         
         For cover generation
         
         * Cairo https://www.cairographics.org/download/
         * Noto Sans and Noto Sans CJK:
             * CentOS or RedHat: `yum install google-noto-sans-cjk-fonts; yum install google-noto-sans-fonts`
             * Ubuntu: `apt-get install fonts-noto-cjk fonts-noto`
         
+        For RST conversion
+        
+        * Libertinus Serif and Libertinus Sans https://github.com/alerque/libertinus
+            * For Linux, 
+                * Download the latest release https://github.com/alerque/libertinus/releases/latest
+                * unzip, put .otf files into ~/.fonts 
+                * update font catalog `fc-cache -f -v`
+        * DejaVu Sans Mono https://dejavu-fonts.github.io/
+        
         Tested with Python 3.6
         
         ## Install
         
         (master branch, editable install)
         `pipenv install ebookmaker`
```

### Comparing `ebookmaker-0.9.6/ebookmaker.egg-info/SOURCES.txt` & `ebookmaker-0.9.7/ebookmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/HTMLParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/WrapperParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/WrapperParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/GutenbergTextParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/GutenbergTextParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/ImageParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/ImageParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/AuxParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/AuxParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/RSTParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/RSTParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/parsers/CSSParser.py` & `ebookmaker-0.9.7/ebookmaker/parsers/CSSParser.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/CommonCode.py` & `ebookmaker-0.9.7/ebookmaker/CommonCode.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/HTMLWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/HTMLWriter.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,98 +5,98 @@
 
 HTMLWriter.py
 
 Copyright 2009 by Marcello Perathoner
 
 Distributable under the GNU General Public License Version 3 or newer.
 
-Writes one HTML file. Currently used only for RST input. 
+Writes one HTML file. Currently used only for RST input.
 Needs revision to use with multi-file books and HTML input.
 
 """
 
 
 import os
 import copy
 
 from lxml import etree
 
 import libgutenberg.GutenbergGlobals as gg
 from libgutenberg.GutenbergGlobals import xpath
-from libgutenberg.Logger import info, debug, error, exception
+from libgutenberg.Logger import info, exception
 
 from ebookmaker import writers
 from ebookmaker.CommonCode import Options
 
 options = Options()
 
-class Writer (writers.HTMLishWriter):
+class Writer(writers.HTMLishWriter):
     """ Class for writing HTML files. """
 
 
-    def add_dublincore (self, job, tree):
+    def add_dublincore(self, job, tree):
         """ Add dublin core metadata to <head>. """
-        source = gg.archive2files (
+        source = gg.archive2files(
             options.ebook, job.url)
 
-        if hasattr (options.config, 'FILESDIR'):
-            job.dc.source = source.replace (options.config.FILESDIR, options.config.PGURL)
+        if hasattr(options.config, 'FILESDIR'):
+            job.dc.source = source.replace(options.config.FILESDIR, options.config.PGURL)
 
-        for head in xpath (tree, '//xhtml:head'):
-            for e in job.dc.to_html ():
+        for head in xpath(tree, '//xhtml:head'):
+            for e in job.dc.to_html():
                 e.tail = '\n'
-                head.append (e)
+                head.append(e)
 
 
-    def build (self, job):
+    def build(self, job):
         """ Build HTML file. """
 
-        htmlfilename = os.path.join (os.path.abspath(job.outputdir),
-                                     job.outputfile)
+        htmlfilename = os.path.join(os.path.abspath(job.outputdir),
+                                    job.outputfile)
         try:
-            os.remove (htmlfilename)
+            os.remove(htmlfilename)
         except OSError:
             pass
 
         try:
-            info ("Creating HTML file: %s" % htmlfilename)
+            info("Creating HTML file: %s" % htmlfilename)
 
             for p in job.spider.parsers:
                 # Do html only. The images were copied earlier by PicsDirWriter.
 
                 xhtml = None
-                if hasattr (p, 'rst2html'):
-                    xhtml = p.rst2html (job)
-                elif hasattr (p, 'xhtml'):
-                    p.parse ()
-                    xhtml = copy.deepcopy (p.xhtml)
+                if hasattr(p, 'rst2html'):
+                    xhtml = p.rst2html(job)
+                elif hasattr(p, 'xhtml'):
+                    p.parse()
+                    xhtml = copy.deepcopy(p.xhtml)
 
                 if xhtml is not None:
-                    self.make_links_relative (xhtml, p.attribs.url)
+                    self.make_links_relative(xhtml, p.attribs.url)
 
-                    self.add_dublincore (job, xhtml)
+                    self.add_dublincore(job, xhtml)
 
                     # makes iphones zoom in
-                    self.add_meta (xhtml, 'viewport', 'width=device-width')
-                    self.add_meta_generator (xhtml)
+                    self.add_meta(xhtml, 'viewport', 'width=device-width')
+                    self.add_meta_generator(xhtml)
 
                     # This writer has currently to deal only with RST
                     # input.  The RST writer has a workaround that
                     # avoids writing empty elements.  So we don't need
                     # the same ugly workaround as the EPUB writer,
                     # that has to deal with HTML input too.
-                    html = etree.tostring (xhtml,
-                                           method = 'xml',
-                                           doctype = gg.XHTML_DOCTYPE,
-                                           encoding = 'utf-8',
-                                           pretty_print = True,
-                                           xml_declaration = True)
+                    html = etree.tostring(xhtml,
+                                          method='xml',
+                                          doctype=gg.XHTML_DOCTYPE,
+                                          encoding='utf-8',
+                                          pretty_print=True,
+                                          xml_declaration=True)
 
-                    self.write_with_crlf (htmlfilename, html)
+                    self.write_with_crlf(htmlfilename, html)
                     break
-            info ("Done HTML file: %s" % htmlfilename)
+            info("Done HTML file: %s" % htmlfilename)
 
         except Exception as what:
-            exception ("Error building HTML %s: %s" % (htmlfilename, what))
-            if os.access (htmlfilename, os.W_OK):
-                os.remove (htmlfilename)
+            exception("Error building HTML %s: %s" % (htmlfilename, what))
+            if os.access(htmlfilename, os.W_OK):
+                os.remove(htmlfilename)
             raise what
```

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/TxtWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/TxtWriter.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/KindleWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/KindleWriter.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,97 +21,97 @@
 from ebookmaker.writers import BaseWriter
 from ebookmaker.CommonCode import Options
 
 options = Options()
 no_kindlegen_langs = ['ceb', 'eo', 'fur', 'ia', 'ilo', 'iu', 'mi',
                       'myn', 'nah', 'nap', 'oc', 'oji', 'tl']
 
-class Writer (BaseWriter):
+class Writer(BaseWriter):
     """ Class for writing kindle files. """
 
 
-    def build (self, job):
+    def build(self, job):
         """ Build kindle file from epub using amazon kindlegen or calibre. """
 
         if job.dc.languages:
             if job.dc.languages[0].id in no_kindlegen_langs:
                 mobimaker = options.config.MOBILANG
             else:
                 mobimaker = options.config.MOBIGEN
         if not mobimaker:
             info('no mobimaker available')
             return
 
         # kindlegen needs localized paths
         outputdir = os.path.abspath(job.outputdir)
 
-        info ("Creating Kindle file: %s" % os.path.join (outputdir, job.outputfile))
-        info ("            ... from: %s" % job.url)
+        info("Creating Kindle file: %s" % os.path.join(outputdir, job.outputfile))
+        info("            ... from: %s" % job.url)
 
         try:
-            cwd = os.getcwd ()
-            os.chdir (outputdir)
+            cwd = os.getcwd()
+            os.chdir(outputdir)
             if 'ebook-convert' in mobimaker:
-                kindlegen = subprocess.Popen (
+                kindlegen = subprocess.Popen(
                     [
                         mobimaker,
                         job.url,
-                        os.path.basename (job.outputfile),
+                        os.path.basename(job.outputfile),
                         '--personal-doc="[EBOK]"',
                     ],
                     stdin=subprocess.PIPE,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE
                 )
             else:
-                kindlegen = subprocess.Popen (
+                kindlegen = subprocess.Popen(
                     [
                         mobimaker,
-                        '-o', os.path.basename (job.outputfile),
+                        '-o', os.path.basename(job.outputfile),
                         job.url
                     ],
                     stdin=subprocess.PIPE,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE
                 )
 
         except OSError as what:
-            os.chdir (cwd)
-            error ("KindleWriter: %s %s" % (mobimaker, what))
+            os.chdir(cwd)
+            error("KindleWriter: %s %s" % (mobimaker, what))
             raise SkipOutputFormat
 
-        (stdout, stderr) = kindlegen.communicate ()
+        (stdout, stderr) = kindlegen.communicate()
 
-        os.chdir (cwd)
+        os.chdir(cwd)
 
         if kindlegen.returncode > 0:
-            regex = re.compile (r'^(\w+)\(prcgen\):')
+            regex = re.compile(r'^(\w+)\(prcgen\):')
 
             # pylint: disable=E1103
-            msg = stderr.rstrip ()
+            msg = stderr.rstrip()
             if msg:
-                msg = msg.decode (sys.stderr.encoding)
-                error (msg)
-            msg = stdout.rstrip ()
-            msg = msg.decode (sys.stdout.encoding)
-            for line in msg.splitlines ():
-                match = regex.match (line)
+                msg = msg.decode(sys.stderr.encoding)
+                error(msg)
+            msg = stdout.rstrip()
+            msg = msg.decode(sys.stdout.encoding)
+            for line in msg.splitlines():
+                match = regex.match(line)
                 if match:
-                    sline = regex.sub ("", line)
-                    g = match.group (1).lower ()
+                    sline = regex.sub("", line)
+                    g = match.group(1).lower()
                     if g == 'info':
                         if sline == 'MOBI File generated with WARNINGS!':
                             # we knew that already
                             continue
-                        # info ("kindlegen: %s" % sline)
+                        # info("kindlegen: %s" % sline)
                     elif g == 'warning':
-                        if sline.startswith ('Cover is too small'):
+                        if sline.startswith('Cover is too small'):
                             continue
                         if sline == 'Cover not specified':
                             continue
-                        warning ("kindlegen: %s" % sline)
+                        warning("kindlegen: %s" % sline)
                     elif g == 'error':
-                        error ("kindlegen: %s" % sline)
+                        error("kindlegen: %s" % sline)
                     else:
-                        error (line)
+                        error(line)
 
-        info ("Done Kindle file: %s" % os.path.join (outputdir, job.outputfile))
+        info("Done Kindle file: %s" % os.path.join(outputdir, job.outputfile))
```

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/writers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,121 +25,121 @@
 from libgutenberg import MediaTypes
 
 from ebookmaker import parsers
 from ebookmaker import ParserFactory
 from ebookmaker.Version import VERSION, GENERATOR
 
 
-class BaseWriter (object):
+class BaseWriter(object):
     """
     Base class for EpubWriter, PluckerWriter, ...
 
     also used as /dev/null writer for debugging
 
     """
 
-    def build (self, job):
+    def build(self, job):
         """ override this in a real writer """
         pass
 
 
     @staticmethod
-    def write_with_crlf (filename, bytes_):
+    def write_with_crlf(filename, bytes_):
         # \r\n is PG standard
-        bytes_ = b'\r\n'.join (bytes_.splitlines ()) + b'\r\n'
+        bytes_ = b'\r\n'.join(bytes_.splitlines()) + b'\r\n'
 
         # open binary so windows doesn't add another \r
-        with open (filename, 'wb') as fp:
-            fp.write (bytes_)
+        with open(filename, 'wb') as fp:
+            fp.write(bytes_)
 
 
-    def validate (self): # pylint: disable=R0201
+    def validate(self): # pylint: disable=R0201
         """ Validate the output with some (external) tool.
 
         Override this in a real writer.
 
         """
         return 0
 
 
-    def sync (self):
+    def sync(self):
         """  Override this if you need to sync before program exit. """
         pass
 
 
-    def make_links_relative (self, xhtml, base_url):
+    def make_links_relative(self, xhtml, base_url):
         """ Make absolute links in xhtml relative to base_url. """
 
-        debug ("Making links relative to: %s" % base_url)
-        xhtml.rewrite_links (partial (gg.make_url_relative, base_url))
+        debug("Making links relative to: %s" % base_url)
+        xhtml.rewrite_links(partial(gg.make_url_relative, base_url))
 
 
 
-em = ElementMaker (namespace = str (gg.NS.xhtml),
-                   nsmap = { None: str (gg.NS.xhtml) })
+em = ElementMaker(namespace=str(gg.NS.xhtml),
+                  nsmap={None: str(gg.NS.xhtml)})
 
 
-class HTMLishWriter (BaseWriter):
+class HTMLishWriter(BaseWriter):
     """ Base class for writers with HTMLish contents. """
 
     @staticmethod
-    def add_class (elem, class_):
+    def add_class(elem, class_):
         """ Add a class to html element. """
 
-        classes = elem.get ('class', '').split ()
-        classes.append (class_)
-        elem.set ('class', ' '.join (classes))
+        classes = elem.get('class', '').split()
+        classes.append(class_)
+        elem.set('class', ' '.join(classes))
 
 
     @staticmethod
-    def add_meta (xhtml, name, content):
+    def add_meta(xhtml, name, content):
         """ Add a meta tag. """
 
-        for head in gg.xpath (xhtml, '//xhtml:head'):
-            meta = em.meta (name = name, content = content)
+        for head in gg.xpath(xhtml, '//xhtml:head'):
+            meta = em.meta(name=name, content=content)
             meta.tail = '\n'
-            head.append (meta)
+            head.append(meta)
 
 
     @staticmethod
-    def add_meta_generator (xhtml):
+    def add_meta_generator(xhtml):
         """ Add our piss mark. """
 
-        HTMLishWriter.add_meta (xhtml, 'generator', GENERATOR % VERSION)
+        HTMLishWriter.add_meta(xhtml, 'generator', GENERATOR % VERSION)
 
 
     @staticmethod
-    def add_internal_css (xhtml, css_as_string):
+    def add_internal_css(xhtml, css_as_string):
         """ Add internal stylesheet to html. """
 
         if css_as_string and xhtml is not None:
-            css_as_string = '\n' + css_as_string.strip (' \n') + '\n'
-            for head in gg.xpath (xhtml, '//xhtml:head'):
-                style = em.style (css_as_string, type = 'text/css')
+            css_as_string = '\n' + css_as_string.strip(' \n') + '\n'
+            for head in gg.xpath(xhtml, '//xhtml:head'):
+                style = em.style(css_as_string, type='text/css')
                 style.tail = '\n'
-                head.append (style)
+                head.append(style)
 
     @staticmethod
-    def add_body_class (xhtml, classname):
+    def add_body_class(xhtml, classname):
         """ Add a class to the body element. """
 
         if classname and xhtml is not None:
-            for body in gg.xpath (xhtml, '//xhtml:body'):
-                HTMLishWriter.add_class (body, classname)
+            for body in gg.xpath(xhtml, '//xhtml:body'):
+                HTMLishWriter.add_class(body, classname)
 
 
-    def add_external_css (self, spider, xhtml, css_as_string, url):
+    def add_external_css(self, spider, xhtml, css_as_string, url):
         """ Add external stylesheet to html. """
 
         if css_as_string:
-            attribs = parsers.ParserAttributes ()
-            attribs.orig_mediatype = attribs.HeaderElement ('text/css')
+            attribs = parsers.ParserAttributes()
+            attribs.orig_mediatype = attribs.HeaderElement('text/css')
             attribs.url = attribs.orig_url = url
-            p = ParserFactory.ParserFactory.get (attribs)
-            p.parse_string (css_as_string)
-            spider.parsers.append (p)
+            p = ParserFactory.ParserFactory.get(attribs)
+            p.parse_string(css_as_string)
+            spider.parsers.append(p)
 
         if xhtml is not None:
-            for head in gg.xpath (xhtml, '//xhtml:head'):
-                link = em.link (href = url, rel = 'stylesheet', type = 'text/css')
+            for head in gg.xpath(xhtml, '//xhtml:head'):
+                link = em.link(href=url, rel='stylesheet', type='text/css')
                 link.tail = '\n'
-                head.append (link)
+                head.append(link)
```

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/PDFWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/PDFWriter.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/cover.jpg` & `ebookmaker-0.9.7/ebookmaker/writers/cover.jpg`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/EpubWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/EpubWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         return page_map
 
 
 class OutlineFixer(object):
     """ Class that fixes outline levels. """
 
     def __init__(self):
-        self.stack = [(0,0),]
+        self.stack = [(0, 0),]
         self.last = 0
 
     def level(self, in_level):
         if in_level < 1:
             return in_level
         (promotion, from_level) = self.stack[-1]
         if in_level > self.last + 1:
@@ -333,15 +333,15 @@
 
     def __unicode__(self):
         """ Serialize toc.ncx as unicode string. """
         ncx = self.ncx
         tocdepth = 1
 
         if self.toc:
-            # normalize toc so that it starts with an h1 and doesn't jump down more than one 
+            # normalize toc so that it starts with an h1 and doesn't jump down more than one
             # level at a time
             fixer = OutlineFixer()
             for t in self.toc:
                 t[2] = fixer.level(t[2])
 
             # flatten toc if it contains only one top-level entry
             top_level_entries = sum(t[2] == 1 for t in self.toc)
@@ -845,20 +845,21 @@
                 node.tail = six.text_type(node.tail).translate(Writer.translate_map)
 
 
     @staticmethod
     def fix_incompatible_css(sheet):
         """ Strip CSS properties and values that are not EPUB compatible. """
 
-        # debug("enter fix_incompatible_css")
+        cssclass = re.compile(r'\.(-?[_a-zA-Z]+[_a-zA-Z0-9-]*)')
 
         for rule in sheet:
             if rule.type == rule.STYLE_RULE:
+                ruleclasses = list(cssclass.findall(rule.selectorList.selectorText))
                 for p in list(rule.style):
-                    if p.name == 'float':
+                    if p.name == 'float' and "x-ebookmaker" not in ruleclasses:
                         debug("Dropping property %s" % p.name)
                         rule.style.removeProperty('float')
                         rule.style.removeProperty('width')
                         rule.style.removeProperty('height')
                     elif p.name == 'position':
                         debug("Dropping property %s" % p.name)
                         rule.style.removeProperty('position')
@@ -1276,15 +1277,15 @@
                             self.strip_pagenumbers(xhtml, strip_classes)
 
                         # build up TOC
                         # has side effects on xhtml
                         ncx.toc += p.make_toc(xhtml)
 
                         # allows authors to customize css for epub
-                        self.add_body_class (xhtml, 'x-ebookmaker')
+                        self.add_body_class(xhtml, 'x-ebookmaker')
 
                         self.insert_root_div(xhtml)
                         self.fix_charset(xhtml)
                         self.fix_style_elements(xhtml)
                         self.reflow_pre(xhtml)
 
                         # strip all links to items not in manifest
```

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/PicsDirWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/PicsDirWriter.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/writers/RSTWriter.py` & `ebookmaker-0.9.7/ebookmaker/writers/RSTWriter.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/WriterFactory.py` & `ebookmaker-0.9.7/ebookmaker/WriterFactory.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/HTMLChunker.py` & `ebookmaker-0.9.7/ebookmaker/HTMLChunker.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/ParserFactory.py` & `ebookmaker-0.9.7/ebookmaker/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/packagers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/packagers/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/packagers/PushPackager.py` & `ebookmaker-0.9.7/ebookmaker/packagers/PushPackager.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/UnitameData.py` & `ebookmaker-0.9.7/ebookmaker/UnitameData.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/EbookMaker.py` & `ebookmaker-0.9.7/ebookmaker/EbookMaker.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/Unitame.py` & `ebookmaker-0.9.7/ebookmaker/Unitame.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/Spider.py` & `ebookmaker-0.9.7/ebookmaker/Spider.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/parsers/default_style.rst` & `ebookmaker-0.9.7/ebookmaker/mydocutils/parsers/default_style.rst`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/parsers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2html.css` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2html.css`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/nroff.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/nroff.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/xhtml1.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/xhtml1.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2epub.css` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2epub.css`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/rst2all.css` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/rst2all.css`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/epub2.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/epub2.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/writers/xetex.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/writers/xetex.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
 \usepackage{polyglossia}
 \setotherlanguages{<otherlanguages>}
 
 \usepackage{xltxtra}
 
 \defaultfontfeatures{Scale=MatchLowercase}
-\setmainfont[Numbers=OldStyle]{Linux Libertine O}
-\setsansfont{Linux Biolinum O}
+\setmainfont{Libertinus Serif}
+\setsansfont{Libertinus Sans}
 \setmonofont[HyphenChar=None]{DejaVu Sans Mono}
 
 \usepackage{calc}
 \usepackage{graphicx}
 \usepackage{alltt}
 \usepackage{float}
```

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/__init__.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/pg-footer.rst` & `ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/pg-footer.rst`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/parsers/pg-header.rst` & `ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/parsers/pg-header.rst`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/writers/nroff.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/writers/nroff.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/gutenberg/transforms/__init__.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/gutenberg/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/transforms/parts.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/transforms/parts.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/ebookmaker/mydocutils/nodes.py` & `ebookmaker-0.9.7/ebookmaker/mydocutils/nodes.py`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/CHANGES` & `ebookmaker-0.9.7/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+0.9.7 September 14, 2020
+- changed font for rst conversion. Linux Libertine was unmaintained since 2012 and no package was available for CENTOS8. We switched to the closest replacement, Libertinus https://github.com/alerque/libertinus
+- added documentation about configuration for rst conversion
+- the deprecated 'handheld' @media query was being used to prevent ebookmaker from stripping floats. to preserve this feature, ebookmaker no longer strips floats when the css selector contains the x-ebookmaker class. Most likely, float stripping was originally needed because html pages were designed before the advent of EPUB. Today, we can assume that if the html designer uses the x-ebookmaker class, they've considered the impact of the float on the generated EPUB.
+- assorted delinting
+
 0.9.6 September 8, 2020
 - added 'x-ebookmaker' class to epub body elements. There are now 4 "x-ebookmaker" classes
-    - css can now apply styles that are triggered by being a descendent of .x-ebookmaker. This addition is meant to replace the 'mobile' @media query that is deprecated in HTML 5
+    - css can now apply styles that are triggered by being a descendent of .x-ebookmaker. This addition is meant to replace the 'handheld' @media query that is deprecated in HTML 5
     - the 'x-ebookmaker-important' class on on image element tells ebookmaker not to remove the image, even in no-images builds.
     - the 'x-ebookmaker-drop' class tells ebookmaker to remove an element and its descendents from ebook builds.
     - the 'x-ebookmaker-pageno' class is applied to some span elements whose content has been stripped because they use a class that indicates they represent page numbers: pagenum pageno page pb folionum foliono
 - added mayan as a language not supported by kindlegen
 - typos fixed in README - thanks Joseph Koshy
 
 0.9.5 July 6, 2020
```

### Comparing `ebookmaker-0.9.6/README.md` & `ebookmaker-0.9.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,33 @@
 
 
 ## Prerequisites
 
 * Python3 >= 3.6
 * HTMLTidy (http://binaries.html-tidy.org/),
 * Kindlegen (https://www.amazon.com/gp/feature.html/?docId=1000765211) or Calibre (https://calibre-ebook.com/)
-* TexLive (to build from TeX), and
+* TexLive (to build from TeX and rst), and
 * groff (not sure when this is needed).
 
 For cover generation
 
 * Cairo https://www.cairographics.org/download/
 * Noto Sans and Noto Sans CJK:
     * CentOS or RedHat: `yum install google-noto-sans-cjk-fonts; yum install google-noto-sans-fonts`
     * Ubuntu: `apt-get install fonts-noto-cjk fonts-noto`
 
+For RST conversion
+
+* Libertinus Serif and Libertinus Sans https://github.com/alerque/libertinus
+    * For Linux, 
+        * Download the latest release https://github.com/alerque/libertinus/releases/latest
+        * unzip, put .otf files into ~/.fonts 
+        * update font catalog `fc-cache -f -v`
+* DejaVu Sans Mono https://dejavu-fonts.github.io/
+
 Tested with Python 3.6
 
 ## Install
 
 (master branch, editable install)
 `pipenv install ebookmaker`
```

### Comparing `ebookmaker-0.9.6/setup.py` & `ebookmaker-0.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # ebookmaker distribution
 #
 
 from setuptools import setup
 
-VERSION = '0.9.6'
+VERSION = '0.9.7'
 
 setup (
     name = 'ebookmaker',
     version = VERSION,
 
     packages = [
         'ebookmaker',
```

### Comparing `ebookmaker-0.9.6/scripts/rhyme_compiler` & `ebookmaker-0.9.7/scripts/rhyme_compiler`

 * *Files identical despite different names*

### Comparing `ebookmaker-0.9.6/scripts/convert_unitame` & `ebookmaker-0.9.7/scripts/convert_unitame`

 * *Files identical despite different names*

